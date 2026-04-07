# Activity System Analyser based on cultural-historical activity theory (CHAT)

An interactive, browser-based tool for analysing human activity using Engeström's Activity System model, grounded in cultural-historical activity theory (CHAT).

**Live demo:** [https://jourde.github.io/chat/interface.html](https://jourde.github.io/chat/interface.html)

--

## What it does

The tool lets you map and analyse an activity system by filling in six interconnected components:

| Component | Description |
|---|---|
| **Mediating artefacts (tools and signs)** | Technologies, symbols or language used to accomplish the activity |
| **Subject** | The person or group whose perspective is being analysed |
| **Object / Motive** | What is being transformed; the immediate goals and underlying motives |
| **Rules** | Norms, conventions and regulations that constrain or guide the activity |
| **Community** | Others who share a stake in the activity |
| **Division of Labour** | How tasks, roles and power are distributed |

You can also identify **contradictions** at three levels — tensions within a component, between components of the same system, or across two systems — and export the full analysis.

---

## Features

- **Interactive SVG diagram** — click any node to open a guided editor with prompts for each component
- **Two-system view** — toggle between a single activity system and a dual-system view showing two systems alongside a Shared Object and Shared Outcome(s), following Engeström's third-generation CHAT framework
- **Three levels of contradiction tracking** — with visual indicators on the diagram:
  - ⚡ **Inner** — a tension within a single component (e.g. a tool that is both required and unusable)
  - ⚡ **Secondary** — a tension between two components within the same system (e.g. Rules clashing with the Object)
  - ↔ **Inter-systemic** — a tension between the two activity systems (dual-system view only)
- **Live summary panel** — real-time display of all component values and contradictions as you type
- **Additional notes** — free-text field for observations and reflections
- **Export** — download the full analysis as plain text, Markdown, or JSON
- **Copy to clipboard** — one-click copy of the summary and notes
- **Accessible** — full keyboard navigation, ARIA labels, screen-reader live announcements, WCAG 2.1 AA focus indicators

---

## Theoretical background

This tool is based on **Engeström's Activity System** (1987, 2001), a model from cultural-historical activity theory (CHAT) for analysing complex human activities as systems. The six components and their relationships make visible the structural tensions — contradictions — that drive development and change within an activity.

The **two-system view** implements the third-generation CHAT framework, which places two activity systems in dialogue around a shared object, enabling analysis of inter-organisational and boundary-crossing activity.

**Contradictions** are central to CHAT analysis. The tool supports three levels:

| Level | Label | Description |
|---|---|---|
| Level 1 | Inner | Tension within a single component |
| Level 2 | Secondary | Tension between two components of the same system |
| Level 4 | Inter-systemic | Tension between two activity systems |

**Key references:**
- Engeström, Y. (1987). *Learning by expanding: An activity-theoretical approach to developmental research.* Orienta-Konsultit.
- Engeström, Y. (2001). Expansive learning at work: Toward an activity theoretical reconceptualization. *Journal of Education and Work, 14*(1), 133–156.

---

## Usage

No installation or build step required. The tool is a single self-contained HTML file.

1. Download `Engeström_Activity_System_Analyser.html`
2. Open it in any modern browser
3. Click a node on the triangle to begin filling in your activity system
4. Use **⚡ Add a contradiction** to mark tensions:
   - Click the **same node twice** for an inner contradiction
   - Click **two different nodes in the same system** for a secondary contradiction
5. Export or copy your analysis when done

To use the two-system view:

1. Click **Show two systems**
2. Click nodes in either triangle to edit System 1 or System 2 independently
3. Click the **Shared Object** box and **Shared Outcome(s)** label in the centre to describe what connects both systems
4. In contradiction mode, click **one node in System 1 and one in System 2** to mark an inter-systemic contradiction

---

## Privacy

All data is processed entirely in your browser. Nothing is transmitted to any server. The tool has no external dependencies and makes no network requests after the initial page load.

---

## Browser support

Any modern browser (Chrome, Firefox, Safari, Edge). No polyfills or transpilation required.

---

## Licence

MIT Licence — François Jourde (2026)

