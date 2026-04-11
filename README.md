# Activity System Analyser based on cultural-historical activity theory (CHAT)

An interactive single-page application for analysing human activity with Engeström's Activity System model in cultural-historical activity theory (CHAT).

**Live demo:** [https://jourde.github.io/chat/interface.html](https://jourde.github.io/chat/interface.html)

## Overview

The tool lets you describe an activity system by filling in six connected components:

| Component | Description |
| --- | --- |
| **Mediating artefacts (tools and signs)** | Technologies, symbols, or language used to carry out the activity |
| **Subject** | The person or group whose perspective is being analysed |
| **Object (motive-bearing)** | What the activity is directed at and works to transform; the object embeds the motive |
| **Rules** | Norms, conventions, and regulations that shape the activity |
| **Community** | The collective that shares or co-orients toward the same object |
| **Division of Labour** | How tasks, roles, and power are distributed |

The application also supports contradiction mapping, summary generation, JSON-based data portability, and diagram export.

## Features

- Interactive SVG diagram with guided editing for each node
- Single-system and dual-system analysis modes
- Shared Object and Shared Outcome(s) editing in dual-system mode
- Contradiction mapping with visual overlays:
  - `Primary` contradiction within one component
  - `Secondary` contradiction between two components in the same system
  - `Inter-systemic` contradiction between two systems
- Live summary panel that updates as you type
- Additional notes area
- Summary export as plain text, Markdown, or JSON
- JSON import using the app's export schema
- Diagram export as `SVG` or `PNG`
- Standalone export of interface copy for UI review
- Clipboard copy for summary and notes
- Keyboard-accessible controls, menus, and dialogs

## Interface

The action bar is organised into three groups:

- `View`
  - `Show two systems` toggles between one-system and two-system analysis
- `Contradictions`
  - `⚡ Add a contradiction` switches the diagram into contradiction-selection mode
- `Export`
  - `Export UI Content for Review`
  - `Copy summary and notes`
  - `Export diagram` → `SVG` or `PNG`
  - `Export summary and notes` → `Plain text`, `Markdown`, or `JSON`
  - `Import JSON`

## Usage

No build step or dependency installation is required.

1. Open `Engeström_Activity_System_Analyser.html` in a modern browser.
2. Click a node in the diagram to edit it.
3. Fill in the six components of the activity system.
4. Optionally add notes in the summary panel.
5. Export, copy, or import data as needed.

### Contradictions

To record contradictions:

1. Click `⚡ Add a contradiction`.
2. Choose nodes in the diagram:
   - Click the same node twice for a `Primary` contradiction.
   - Click two different nodes in the same system for a `Secondary` contradiction.
   - In dual-system mode, click one node in each system for an `Inter-systemic` contradiction.
3. Enter the contradiction description and save it.

### Dual-system mode

To analyse two interacting activity systems:

1. Click `Show two systems`.
2. Fill in nodes in `System 1` and `System 2`.
3. Click the central `Shared Object` and `Shared Outcome(s)` controls to describe what connects both systems.
4. Use contradiction mode to capture within-system and across-system tensions.

### Import and export

- Use `Export summary and notes` to download the current analysis as:
  - plain text
  - Markdown
  - JSON
- Use `Import JSON` to restore a previous analysis from the app's JSON export format
- Use `Export diagram` to download the current diagram as:
  - `SVG`
  - `PNG`
- Use `Export UI Content for Review` to export the interface text and prompts used in the application

## Accessibility

The SPA is designed for keyboard and assistive-technology use:

- interactive SVG nodes are keyboard focusable
- controls expose ARIA labels and menu semantics where needed
- live announcements are sent to a polite screen-reader region
- focus is managed for menus and the legal dialog
- visible focus indicators are provided throughout the interface

## Privacy

The application runs entirely client-side in the browser.

- no user data is sent to a server by the application
- no framework or external runtime is required
- exports and imports operate locally on the user's device

## Browser support

Current versions of major modern browsers are supported, including:

- Chrome
- Firefox
- Safari
- Edge

## Theoretical background

This tool is based on Engeström's Activity System framework and third-generation CHAT for analysing complex human activities, shared objects, and systemic tensions.

**Key references**

- Engeström, Y. (1987). *Learning by expanding: An activity-theoretical approach to developmental research.* Orienta-Konsultit.
- Engeström, Y. (2001). Expansive learning at work: Toward an activity theoretical reconceptualization. *Journal of Education and Work, 14*(1), 133–156.

## Licence

MIT Licence — François Jourde (2026)
