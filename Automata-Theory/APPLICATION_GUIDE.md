# 3.2 APPLICATION STEP-BY-STEP GUIDE

This section outlines the complete user flow of the ATMTA Interactive Tracing System, demonstrating how users can seamlessly navigate the application, configure their desired regular expression, simulate state machines, and perform in-depth computational analysis. 

---

### Step 1: Accessing the Application Workspace

**[ INSERT SCREENSHOT HERE: The full landing page of the application ]**  
*Figure 3.2.1 Landing Page*

Upon launching the application, the user is greeted by the ATMTA landing page. Clicking the **"Enter Dashboard"** button transitions the user from the introductory screen directly into the main interactive workspace.

---

### Step 2: Selecting the Target Language (Regex)

**[ INSERT SCREENSHOT HERE: A cropped view of the top-right corner showing the {a, b} and {0, 1} toggle buttons ]**  
*Figure 3.2.2 Selecting the Regular Expression*

The first action within the dashboard is selecting the target language. At the top right corner, users can toggle between the **Regex {a, b}** and **Regex {0, 1}** rule sets. Selecting a regex instantly updates the active definitions, transitions, and structural graphs across the entire system to match the chosen language logic.

---

### Step 3: Navigating the Automata Models

**[ INSERT SCREENSHOT HERE: The Left Sidebar highlighting the DFA, CFG, and PDA tabs along with the Active Definition box ]**  
*Figure 3.2.3 Automata Navigation and Active Definitions*

Using the left sidebar navigation, users can seamlessly switch between three different formal language models: **Deterministic Finite Automata (DFA)**, **Context-Free Grammar (CFG)**, and **Pushdown Automata (PDA)**. The Active Definition panel below dynamically displays the corresponding start states, accepting sets, and alphabet rules for whichever tab is currently selected.

---

### Step 4: Manually Inputting Test Strings

**[ INSERT SCREENSHOT HERE: The Sequence Tester panel focusing on the "+ Add Test Case" button and the input box ]**  
*Figure 3.2.4 Adding Strings to the Queue*

To interact with the system, users start at the **Sequence Tester** panel located below the main graph. By typing a sequence of characters and clicking the **"+ Add Test Case"** button, the user can manually stage specific strings. These strings are queued up, preparing them to be tested against the active automata.

---

### Step 5: Bulk Generation via Auto-Generator

**[ INSERT SCREENSHOT HERE: The Auto-Generator pop-up panel showing the min/max length inputs and the Generate Cases button ]**  
*Figure 3.2.5 The Auto-Generator Module*

Instead of manually typing individual strings, users can utilize the built-in **Auto-Generator** feature. By specifying a minimum length, maximum length, and the total number of desired cases, the system will algorithmically generate a bulk list containing a mix of valid (accepted) and invalid (rejected) test strings. These are automatically populated into the test queue alongside any manually added strings.

---

### Step 6: Executing the Validation

**[ INSERT SCREENSHOT HERE: The Sequence Tester panel focusing on the "Validate" button inside a test case, and the "Validate All Cases" button ]**  
*Figure 3.2.6 Initiating the Validation Process*

Once the queue is populated with test strings, the user can initiate the simulation. The user can either click the individual blue **"VALIDATE"** button next to a specific string to run it, or click the **"Validate All Cases"** button to batch process the entire queue. Once validation is initiated, the tested strings are recorded into the Test History for future reference.

---

### Step 7: Live Path Tracing and Simulation

**[ INSERT SCREENSHOT HERE: The main DFA or PDA Graph actively simulating, with a specific node highlighted in orange ]**  
*Figure 3.2.7 Live Graph Tracing and Visualization*

Immediately after clicking validate, the Live Transition Graph Viewer executes a real-time animated trace. The interactive canvas visually highlights the active state (in amber) and draws out the transition paths (in yellow) in real-time, providing immediate and intuitive visual feedback on exactly how the machine processes each character. Users can also pan and zoom the canvas using their mouse to focus on specific complex path routes.

---

### Step 8: Analyzing the Computation Results

**[ INSERT SCREENSHOT HERE: The Computation Panel slide-out drawer showing the step-by-step table ]**  
*Figure 3.2.8 Computation Table and Verdict*

Alongside the visual graph animation, the **Computation Panel** provides a detailed, step-by-step tabular breakdown of the machine's state transitions. This allows users to deeply analyze the trace history of the input string—showing the current state, the read input, and the resulting next state—culminating in a definitive, color-coded **ACCEPTED** or **REJECTED** verdict.

---

### Step 9: Persistent Analysis via Docking

**[ INSERT SCREENSHOT HERE: The Sequence Tester panel showing the green "Dock to Side" button at the top right ]**  
*Figure 3.2.9 Docking the Interface*

For continuous and persistent analysis, users can click the green **"Dock to Side"** button located at the top right of the Sequence Tester panel. This action locks the test history and computation layout to the right side of the screen and dynamically resizes the main graph canvas. This smart layout adjustment ensures the user can comfortably view both the real-time graph animation and their sequenced tests simultaneously without having to scroll.
