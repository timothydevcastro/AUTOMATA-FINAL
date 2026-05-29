# CFG vs Regex Analysis

This document contains a detailed structural analysis comparing the hardcoded Regular Expressions against their corresponding Context-Free Grammars (CFGs).

---

## 1. Regex {a, b} — 100% Correct 🎯

**Regex:**
`(aa+bb)(a+b)*(a+b+ab+ba)(a+b+ab+ba)*(aa+bab)*(a+b+aa)(a+b+bb+aa)`

**CFG:**
```text
S -> A B C D E F G
A -> aa | bb                 (Perfectly matches aa+bb)
B -> aB | bB | λ             (Perfectly matches (a+b)*)
C -> a | b | ab | ba         (Perfectly matches a+b+ab+ba)
D -> aD | bD | abD | baD | λ (Perfectly matches (a+b+ab+ba)*)
E -> aaE | babE | λ          (Perfectly matches (aa+bab)*)
F -> a | b | aa              (Perfectly matches a+b+aa)
G -> a | b | bb | aa         (Perfectly matches a+b+bb+aa)
```

**Conclusion:**
This CFG is structurally flawless. Every single non-terminal maps directly to a specific block in the regex.

---

## 2. Regex {0, 1} — 95% Correct (One minor structural detail)

**Regex:**
`(((101)+(111)*+(100))+(1+0+11)*)(1+0+01)*(111+000+101)(1+0)*`

**Current CFG Implementation:**
```text
S → X Y Z W
X → 101 | 100 | 111X | U
U → 1U | 0U | 11U | λ 
Y → 1Y | 0Y | 01Y | λ      (Perfectly matches (1+0+01)*)
Z → 111 | 000 | 101        (Perfectly matches 111+000+101)
W → 1W | 0W | λ            (Perfectly matches (1+0)*)
```

**Proposed CFG Implementation:**
```text
S → X Y Z W
X → 101 | 100 | V | U
V → 111V | λ
U → 1U | 0U | 11U | λ
Y → 1Y | 0Y | 01Y | λ      (Perfectly matches (1+0+01)*)
Z → 111 | 000 | 101        (Perfectly matches 111+000+101)
W → 1W | 0W | λ            (Perfectly matches (1+0)*)
```

---

### The Structural Difference in Variable `X`
The first block of the regex is a pure **Union (OR)** of four options:
$$\underbrace{((101) + (111)^* + (100)) + (1+0+11)^*}_{\text{Variable } X}$$

* **In the Current CFG:** The rule `X → 111X` loops back to `X` itself. This behaves like a **concatenation** of `(111)*` with any other option in `X` (e.g., we can generate `111` followed by `101`, which is not allowed by a pure OR in that specific block).
* **In the Proposed CFG:** The rule `X → 101 | 100 | V | U` with `V → 111V | λ` isolates the `(111)*` part into variable `V`. Once you choose `V`, you can only generate multiples of `111` and cannot loop back to pick `101` or `100`, perfectly matching the regex's Union structure.

### Mathematical Equivalence
Because the rule `U` generates all combinations of `0`s and `1`s anyway, both versions are mathematically equivalent and accept the exact same set of strings. 

However, the **Proposed CFG** is 100% structurally accurate to the layout of the regex.
