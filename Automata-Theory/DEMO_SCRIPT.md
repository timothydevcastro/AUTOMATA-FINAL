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

### Chapter 4: Sequence Tester & Auto-Generator
*Focus: Add rows, validate single/all, validation spinners, BFS/DFS auto-generator.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[2:32 - Click Add Test Case]**<br>Scroll down to the **Sequence Tester**. Click **+ Add Test Case** to create a new row. | "Below the graph is the Sequence Tester. You can add custom test cases with a click of a button to validate multiple strings." |
| **[2:40 - Input a custom string and validate]**<br>In the newly added row, type `aababaa` and press **Enter** (or click the **Validate** button). Watch the spinner and the final green badge. | "Let's type in `aababaa` and hit Enter. Watch how the row lights up with an amber glow, displays a dynamic validation spinner, and then reveals a green checkmark indicating the string is accepted, along with its full state-transition path." |
| **[3:00 - Show an invalid validation]**<br>In the next row, type `aabac` and click **Validate**. Watch the red badge. | "What about invalid input? Typing a string with an invalid character like `c` instantly flags it, highlighting where the transition broke." |
| **[3:15 - Show row controls]**<br>Hover over the individual clear button `↺` and click it, showing the field emptying. Then click the `×` button to delete the row. | "Each row is fully controlled, featuring an individual clear button to wipe the text field and a delete button to keep your workspace clean." |
| **[3:25 - Open Auto-Generator Panel]**<br>Click the purple **Auto-Generate** button. The generator panel slides open. | "To speed up testing, we've built a robust, algorithmic Auto-Generator." |
| **[3:35 - Run Auto-Generator]**<br>Select **6 strings** count, leave Min/Max as is, and click **Generate**. Watch the rows populate and the status message appear. | "By defining a minimum and maximum length, our system performs an optimized BFS and DFS search through the active DFA. It generates a balanced, shuffled mix of exactly half accepted and half rejected test strings. Let's click Generate." |
| **[3:50 - Click Validate All Cases]**<br>Click the blue **Validate All Cases** button. Watch each row validate sequentially with the spinner and turn into red/green badges. | "Now, click 'Validate All Cases'. The simulator runs through each generated test string one by one, animating the active row in amber before showing the final result." |

---

### Chapter 5: Step-by-Step Tracing & Synchronized Highlights
*Focus: Trace replay, play/pause animation, character bar highlights, autoscrolling table.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[4:10 - Load a string for Replay]**<br>In the sidebar, point to the **Test History** list (showing the records of validated strings). In the graph header, select one of the accepted strings (like `aababaa`) from the **Replay** dropdown. | "Every test string is recorded in the Sidebar's Test History. To analyze a specific run, simply pick it from the Replay dropdown to load the active trace." |
| **[4:25 - Pause the animation and point to components]**<br>The animation will automatically start playing. Click the **⏸ Pause** button in the trace controls. | "When loaded, a dedicated trace playback controller appears. I'll pause it here so we can look at the fine details." |
| **[4:38 - Point out active badges]**<br>Point to the amber **Validating: [string]** badge that popped up above the SVG canvas. | "First, notice the pulsing amber validation badge. It clearly displays the active string being evaluated." |
| **[4:48 - Highlight the Synchronized Character Bar]**<br>Point to the **Computation Breakdown** panel (which automatically opened). Hover over the character bar where past letters are faded, the current is amber, and future are dark. | "At the same time, the Computation Breakdown panel reveals a synchronized character bar. As the machine processes the string, past characters fade out, the currently active character glows in amber, and future characters wait in queue." |
| **[5:05 - Step through manually]**<br>Click the **Next →** button twice, then the **← Prev** button once. Observe the node highlighting (amber fill/stroke) on the SVG canvas. | "We can step through the trace manually. Watch the SVG canvas: the active state and active transition edge light up in high-contrast amber, matching our exact position in the string." |
| **[5:20 - Highlight the Autoscrolling Delta Table]**<br>Scroll down slightly so the **Computation Table** is fully visible. Step forward and watch the table row auto-scroll and highlight. | "Below the character bar, the formal Delta transition table shows every evaluation step. The active step highlights and automatically scrolls smoothly into view, ensuring perfect visibility for long strings." |
| **[5:35 - Hit Play to finish]**<br>Click **▶ Play** again and watch the animation play to the end, showing the final state turning green (Accept) and the sidebar updating. | "Let's resume the playback. As it reaches the end, the graph displays the final verdict—routing us smoothly to an accepting state." |

---

### Chapter 6: The Split-Screen "Dock to Side" Layout
*Focus: Responsive design, workspace flexibility, side-by-side mode.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[5:50 - Click Dock to Side]**<br>Click the green **Dock to Side** button in the Sequence Tester header. Watch the layout smoothly transition side-by-side. | "If you are on a wider screen and want to test while keeping an eye on the graph, simply click 'Dock to Side'. The workspace instantly splits into a highly efficient side-by-side layout." |
| **[6:05 - Scroll and show usability]**<br>Briefly scroll the sequence tester list on the right, showing that the graph on the left stays locked in view. | "Now you can run validations, step through traces, and analyze delta tables without ever losing sight of the transition graph. It's the ultimate productivity layout." |
| **[6:18 - Undock the view]**<br>Click the orange **Undock** button. The screen snaps back to the stacked layout. | "Clicking 'Undock' snaps everything back into a clean, focused, stacked view." |

---

### Chapter 7: Context-Free Grammar (CFG) & Pushdown Automata (PDA) Layouts
*Focus: CFG representation, PDA 2 preset, specialized curves, clean reject blocks, layered text.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[6:28 - Switch to CFG Tab]**<br>In the sidebar navigation, click on the **Context-Free Grammar (CFG)** button. | "Beyond DFAs, ATMTA fully supports CFGs and Pushdown Automata. Let's switch to the CFG tab to view the clean, formal production rules generated dynamically." |
| **[6:40 - Switch to {0, 1} Preset]**<br>Go to the top bar and click the **Regex {0, 1}** preset button. | "Now, let's select the Regex zero-one preset in the header once again to load our second problem. This will allow us to showcase our most detailed workspace feature: Pushdown Automata." |
| **[6:52 - Switch to PDA Tab]**<br>In the sidebar navigation, click on the **Pushdown Automata (PDA)** button. | "Now, click on the Pushdown Automaton tab. This loads the beautiful, custom-designed PDA transition graph." |
| **[7:05 - Demonstrate the PDA layout details]**<br>Drag and zoom inside the PDA canvas. Point to the diamond-shaped READ blocks, the clean curved transition lines, stack operations `0, Z / 0Z`, and the aligned Reject blocks. | "Take a look at the level of detail here. This is a complex, multi-state PDA. The graph uses diamond-shaped READ blocks, square START and ACCEPT blocks, and custom, curved transition lines that prevent overlapping. Stack operations are clearly formatted as input, pop, slash, push." |
| **[7:25 - Highlight the layered details and Reject alignment]**<br>Move the mouse to the REJECT blocks on the outer edges and highlight the layered label text. | "Notice how the REJECT blocks are perfectly aligned along the margins to keep the workspace organized, and all labels are layered cleanly so they are readable even in complex segments." |
| **[7:38 - Point to the PDA Delta Matrix]**<br>Scroll down to show the **Formal Delta Transition Matrix**. | "Below the graph, the complete Formal Delta Transition Matrix is displayed, mapping out the machine's exact state behavior for academic rigor." |

---

### Chapter 8: Conclusion
*Focus: Wrap-up, final visual high-point.*

| Visual Action (What to show) | Voiceover Narration (What to say) |
| :--- | :--- |
| **[7:50 - Return to DFA Tab]**<br>Switch back to the **DFA** tab, click **⟲ Reset View** on the graph, and hover the mouse over the brand logo in the sidebar. | "ATMTA brings theoretical computer science to life through advanced simulation, responsive controls, and high-fidelity visuals. It is the ultimate sandbox for learning, testing, and visualizing formal languages. Thank you for watching!" |

---

## 💡 Pro-Tips for the Best Recording

*   **Pace Yourself**: Do not rush. Let the voiceover lead, and match your mouse actions to your speech.
*   **Mouse Path**: Move in straight lines or gentle curves. Avoid quick, jerky movements or shaking the cursor when talking about a feature.
*   **Audio Editing**: After recording, apply a slight "noise reduction" and "limiter" filter to your voice audio in your editing software (like Audacity or Premiere) to give the voiceover that professional studio feel.
