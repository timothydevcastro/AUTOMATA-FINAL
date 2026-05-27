# ATMTA - Interactive Tracing System: Professional Screen Recording & Voiceover Script

This document serves as your master guide for recording an engaging, premium screen demo of the ATMTA interactive workspace. It is structured into distinct chapters matching the natural flow of the application. 

Use this script as a dual-monitor or split-screen companion while recording. It contains **Visual Actions** (exactly what to do with your mouse and keyboard) alongside a fully written, natural **Voiceover Narration** (what you will say).

---

## 🛠️ Recording Preparation Checklist

1. **Browser State**: Clean browser window (no bookmarks toolbar, no tabs showing if possible, or in full-screen F11 mode).
2. **Audio Setup**: A high-quality microphone with proper pop filtering. Speak in a steady, enthusiastic, and professional tone.
3. **Screen Resolution**: Standard 1080p (1920x1080) works best for displaying both the sidebar and the main graph view without excessive panning.
4. **Theme Initial State**: Start with the **Light Theme** active on the Landing Page.
5. **Mouse Movements**: Keep mouse movements smooth and deliberate. When the script says "hover" or "click", do so cleanly and hold for a split second to let the viewer's eye trace your path.

---

## 🎬 Master Demo Script

### Chapter 1: The High-Aesthetic Landing Page
*Focus: First impressions, minimalist styling, dynamic grid, and visual polish.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[0:00 - Start on the Landing Page]**<br>Display the main landing page. Slowly scroll down slightly to show the layout, then scroll back up. Keep the mouse pointer steady near the center. | "Hello, and welcome to ATMTA—a premium, interactive tracing system designed to make Automata and Formal Languages visual, intuitive, and highly interactive. At first glance, you are greeted by an elegant, modern workspace." |
| **[0:15 - Point out the background details]**<br>Gently circle the mouse over the background, indicating the faint lines and the color glows. | "Notice the soft, minimalist grid lines, set to a subtle point-zero-six opacity for a premium aesthetic, and the slow, radial glow blobs drifting gracefully in the background. It feels alive, modern, and highly polished." |
| **[0:30 - Hover and launch]**<br>Hover over the **Launch App** CTA button in the navbar (watch it lift and glow). Click the button to launch the workspace. | "Let's click 'Launch App' to step inside the interactive tracing environment where logic meets design." |

---

### Chapter 2: The Core Workspace & Interactive Navigation
*Focus: Sidebar organization, branding, active meta, problem presets, theme toggling, and regex formatting.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[0:42 - Show the general workspace layout]**<br>Slowly hover the mouse from the left sidebar to the top bar and then the main central panel. | "Welcome to the workspace. The UI is split into a premium sidebar on the left and a scrollable content area on the right, keeping your focus where it matters." |
| **[0:55 - Show the Sidebar details]**<br>Hover over the custom integrated **logo_atmt.png** in the top left, then hover over the **Active Definition Card** (navy background, emerald green text). | "At the top of the sidebar is our custom ATMTA branding. Below it, the navy-and-emerald Active Definition Card dynamically details the active machine parameters: the Start State, the Accepting Set, and the Alphabet Rules Set currently loaded." |
| **[1:10 - Switch between the 2 active Regex Problems]**<br>Move your cursor to the top header. Click on the **Regex {0, 1}** preset button. Watch the whole workspace rebuild instantly, then click back on **Regex {a, b}** to return. | "One of ATMTA's defining features is its multi-preset architecture. Right in the header, you can switch between our two active regex problems. Clicking 'Regex 0-1' instantly rebuilds the entire workspace—the DFA graph, CFG rules, PDA mappings, start states, and accept sets. Let's return to 'Regex a-b' for our first trace walkthrough." |
| **[1:25 - Toggle theme twice]**<br>Move the cursor to the top header and click the **Dark** theme button. Let the UI transition, wait a second, then click the **Light** theme button to return. | "Atmosphere is everything. With a single click of our theme selector, you can instantly toggle between an ultra-clean Light Mode and a deep, immersive Dark Mode. Notice how all graph lines, texts, and panels transition instantly." |
| **[1:40 - Toggle regex formatting]**<br>Hover over the **Regular Expression Rule Set** card. Click the **Format: USE \|** button in the card's header, let it change to **USE +**, then click it again. | "In our Regular Expression panel, we display the exact rule set governing our active DFA. You can click the 'Format' toggle to seamlessly swap the union operator between JFLAP's mathematical plus sign and computer science's pipe operator." |

---

### Chapter 3: Deterministic Finite Automata (DFA) Graph & Live Tooltips
*Focus: SVG Graph viewer, pan & zoom, tooltip generation, academic notation.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[1:42 - Zoom and Pan the Graph]**<br>Move your mouse inside the **Live DFA Transition Graph Viewer**. Use the scroll wheel to zoom out and in, click and drag to pan, and then click the reset icon `⟲` to fit it back perfectly. | "Here is the heart of the simulator: the Live DFA Transition Graph Viewer. Rendered in crisp, scalable SVG, you can click and drag to pan, scroll to zoom smoothly, and click the reset button to snap it back into view." |
| **[2:00 - Hover nodes for tooltips]**<br>Hover over node **S0**, then **S1**, then **S3**. Let the tooltip box pop up on screen each time. | "By hovering over any state, the viewer dynamically queries the transition matrix and generates a tooltip showing all outgoing transitions—such as 'on a' to S1 or 'on b' to S2." |
| **[2:15 - Point out the math symbols]**<br>Point the mouse cursor at the small symbols inside the circles: the minus sign in **S0**, and the plus signs in accept states **S8**, **S9**, and **S10**. | "We've integrated standard JFLAP notation: a minus sign indicates the start state, a green ring with a plus sign represents accept states, and a plus-minus symbol is used if a state is both a start and accept state." |

---

### Chapter 4: Manual String Validation & Live Graph Transition
*Focus: Adding test cases, typing a string, manual validation, live transition visualization on the DFA, and detailed path/reject subtext.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[2:32 - Click Add Test Case]**<br>Scroll down to the **Sequence Tester** section. Click the **+ Add Test Case** button. | "Now let's scroll down to the Sequence Tester. I'm going to click '+ Add Test Case' to create a new input field." |
| **[2:42 - Input a custom string]**<br>Type a valid test string, such as `aababaa`, into the input box. | "Let's type in a custom string—like `aababaa`." |
| **[2:50 - Click Validate and watch the Live Transition]**<br>Click **Validate** (or press Enter). Immediately look up at the DFA graph to show the states highlighting in amber as the transition runs, ending with a green success badge. | "Now we'll click Validate. Notice how the DFA graph instantly highlights each active state in amber as it processes the path, ending with a green checkmark indicating the string is accepted." |
| **[3:00 - Point out the transition path details]**<br>Hover over the subtext directly under the green **✓ Accepted** badge showing the state list: `Path: S0 → S1 → S3 → S4 → S6 → S8 → S8`. | "As you can see here, it also says the path it took for it to get accepted." |
| **[3:12 - Input a rejecting string and validate]**<br>Click **+ Add Test Case** again, type an invalid string (like one that triggers a rejection), and click **Validate**. Point to the red **X Rejected** badge and its subtext `Rejected at S3`. | "And when we add and test a rejected string, it also says exactly where it was rejected." |

---

### Chapter 5: Auto-Generator, Batch Validation, & Dock-to-Side
*Focus: Algorithmic string generation, batch testing, and split-screen workflow layout.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[3:05 - Open Auto-Generator]**<br>Click the purple **Auto-Generate** button in the sequence tester header. | "To speed up our testing, we can click the purple 'Auto-Generate' button to open the algorithmic generation panel." |
| **[3:15 - Generate test cases]**<br>Set the string count to **6**, leave length presets as default, and click **Generate**. | "I'll generate six strings. The algorithm quickly creates a clean, balanced mix of accepted and rejected test cases." |
| **[3:25 - Click Dock to Side]**<br>Click the green **Dock to Side** button in the Sequence Tester header. Watch the layout split side-by-side. | "Let's click 'Dock to Side'. The workspace transitions into a side-by-side layout, locking the DFA graph on the left while keeping all of our test cases visible on the right." |
| **[3:35 - Click Validate All Cases]**<br>Click the blue **Validate All Cases** button. Watch each row validate and the DFA graph transitions light up. | "Now let's click 'Validate All Cases'. The simulator runs through all of our inputs sequentially, and we can watch the DFA graph transition and highlight in real-time." |
| **[3:50 - Click Undock]**<br>Click the orange **Undock** button to return the layout to stacked. | "I'll click Undock to bring us back to the standard stacked layout." |

---

### Chapter 6: Trace Replay, Manual Playback, & Computation Breakdown
*Focus: History dropdown, manual animation controls (play/pause/prev/next), character queue, delta table, and test history.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[4:00 - Replay a specific string]**<br>Select `aababaa` from the **Replay** dropdown in the graph header. | "To inspect a specific run in detail, we can select our string `aababaa` from the Replay dropdown." |
| **[4:10 - Pause and play the animation]**<br>The animation starts playing automatically. Click the **⏸ Pause** button, wait a second, then click **▶ Play**. | "The tracing animation begins on its own. We can hit Pause at any point, and press Play to resume." |
| **[4:22 - Use Next and Previous controls]**<br>Click the **Next →** button a few times to step forward. Then click **← Prev** to step back. | "We can also step through character by character. I'll click 'Next' to move forward, or 'Previous' to go backward, and we can watch the active states shift in the graph above." |
| **[4:35 - Show Computation Breakdown]**<br>Point your mouse to the **Computation Breakdown** panel. Highlight the character queue (past processed letters are faded, current letter is amber, future letters are dark). | "Let's check the Computation Breakdown panel. The character bar shows our string queue: past characters are faded out, the current active character glows in amber, and remaining characters wait in line." |
| **[4:50 - Scroll through the delta transition table]**<br>Scroll down slightly to the **Computation Table**. Step forward again and show the row highlighting and scrolling automatically. | "Below the character bar, the formal Delta transition table maps out every evaluation step. The active step highlights and automatically scrolls into view as the trace progresses." |
| **[5:05 - View Test History]**<br>Move your mouse to the **Test History** section in the left sidebar to show the log of validated runs. Click the trash icon to show the clear history action. | "All of our validated runs are saved right here in the Test History sidebar. If we ever want a clean slate, we can simply click the clear history icon." |

---

### Chapter 7: Context-Free Grammar (CFG) & Pushdown Automata (PDA) Layouts
*Focus: CFG production rules, PDA transition diagrams, stack operations, and delta matrices.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[5:20 - Switch to CFG Tab]**<br>In the left sidebar, click the **Context-Free Grammar (CFG)** button. | "Beyond DFAs, ATMTA fully supports CFGs. Let's switch to the CFG tab to see the clean, dynamically generated production rules." |
| **[5:32 - Load Regex {0, 1} and go to PDA tab]**<br>Click **Regex {0, 1}** preset in the header, then click the **Pushdown Automata (PDA)** tab in the sidebar. | "Now let's select the Regex zero-one preset in the header, and click the Pushdown Automata tab in the sidebar." |
| **[5:45 - Inspect PDA Graph]**<br>Drag and zoom inside the PDA canvas. Point to the diamond-shaped READ blocks, curved transitions, stack operations (`0, Z / 0Z`), and the aligned REJECT blocks on the outer edges. | "This loads our Pushdown Automaton. We can zoom and pan to see the diamond-shaped READ blocks, custom curved transitions that prevent overlap, stack operations, and cleanly aligned REJECT blocks on the margins." |
| **[6:00 - Show PDA Transition Matrix]**<br>Scroll down below the graph to reveal the **Formal Delta Transition Matrix**. | "Right below the graph, the complete Formal Delta Transition Matrix displays the machine's exact state behavior." |

---

### Chapter 8: Conclusion
*Focus: Summary and wrap-up.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[6:15 - Return to DFA Tab]**<br>Switch back to the **DFA** tab, click **⟲ Reset View** on the graph, and hover the mouse over the logo in the sidebar. | "Let's return to the DFA tab, reset our view, and wrap up. ATMTA provides a complete, high-fidelity visualization suite for automata and formal languages. Thank you for watching!" |

---

## 💡 Pro-Tips for the Best Recording

*   **Pace Yourself**: Do not rush. Let the voiceover lead, and match your mouse actions to your speech.
*   **Mouse Path**: Move in straight lines or gentle curves. Avoid quick, jerky movements or shaking the cursor when talking about a feature.
*   **Audio Editing**: After recording, apply a slight "noise reduction" and "limiter" filter to your voice audio in your editing software (like Audacity or Premiere) to give the voiceover that professional studio feel.
