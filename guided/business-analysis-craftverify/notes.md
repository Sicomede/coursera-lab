# Notes: Business Analysis and Process Management (CraftVerify)

## Where the guided path felt limiting

- The Mahi format is a useful starting brief but does not enforce stakeholder analysis, RACI, or data flow diagrams. I extended beyond the guided template to produce all six artifacts because a real BA capstone would require them.
- The course did not explicitly cover BPMN gateway types. I used exclusive gateways (XOR) for the tier decision but a real submission might also need parallel gateways or event-based gateways to model concurrent paths.

## What I extended on my own

- Added a BPMN swimlane diagram. The Mahi example doesn't include one.
- Added a data flywheel feedback loop visible in both the swimlane phase 2 diagram and the DFD, since CraftVerify's core moat is the network effect on the training data.
- Added the RACI matrix to surface accountability gaps, which the guided template left implicit.
- Built a power and interest grid rather than just a flat stakeholder list.

## What broke

- Initial swimlane attempt put all phases on one horizontal canvas. At 680px wide that was unreadable. Split into two phases with prose between, which is the recommended approach for complex BPMN flows.
- First DFD draft mixed process flow and data flow notation. Had to redo it with cleaner DFD conventions: external entities as squares, processes as rounded rectangles, data stores as open-ended rectangles, all arrows labeled with the data being passed, not the action being performed.

## Random observations

- The data flywheel pattern (sample feeds the training dataset which improves the model which scores the next sample better) is the same structural pattern as Tesla's autopilot data collection. Worth flagging as a general business analysis pattern.
- A second accountability person on any RACI row is a smell. I had to revise three rows where I'd accidentally put two As.
- BPMN swimlanes make handoffs visible as arrow crossings between lanes. A process with many lane crossings is a process with many integration risks. This was the most useful diagnostic insight from the project.

## Project metadata

- Started: 05/17/2026
- Finished: 05/17/2026
- Time spent: roughly 4 hours
- Difficulty: 1 out of 5
- Tools: draw.io
- Notation: BPMN 2.0 (informal), Yourdon DFD notation, standard RACI
- Reference framework: PMBOK stakeholder management techniques
