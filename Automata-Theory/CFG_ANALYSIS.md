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

**CFG:**
```text
S → X Y Z W
X → 101 | 100 | 111X | U   <-- Let's look at this
U → 1U | 0U | 11U | λ 
Y → 1Y | 0Y | 01Y | λ      (Perfectly matches (1+0+01)*)
Z → 111 | 000 | 101        (Perfectly matches 111+000+101)
W → 1W | 0W | λ            (Perfectly matches (1+0)*)
```

**Conclusion:**
`Y`, `Z`, and `W` are mapped perfectly. 

However, for `X`, the regex block `(((101)+(111)*+(100))+(1+0+11)*)` is a pure **Union (OR)** of four distinct possibilities. 
Your current rule `X → 101 | 100 | 111X | U` uses `111X` which loops back onto `X`. Technically, this means it generates `(111)*` *concatenated* with the other choices (e.g. allowing `111` followed by `101`). 

Because `U` generates all combinations of 0s and 1s anyway, it doesn't break the actual language accepted (it's mathematically equivalent). But if you want to be **academically, structurally perfect** so it exactly mirrors a union, you should separate `(111)*` into its own variable so it stands alone, like this:

```text
X → 101 | 100 | V | U
V → 111V | λ
U → 1U | 0U | 11U | λ
```
