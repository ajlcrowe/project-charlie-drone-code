# Project Charlie: Drone Code
- **Purpose**: Final puzzle in a group "Find Maple" game (Maple, a dog, is lost in the Amazon). School / group project.
- **Concept** (one line): Five hours after Maple went missing, players crack the drone's code to open its live camera feed and finally see Maple.
- **Core loop**:
  1. *Radio channel (cipher)*: a decoder key maps 6 jungle pictures to numbers; decode a 3-picture signal and type the numbers. Wrong numbers turn red and clear; correct ones lock.
  2. *Camera lock (code breaker)*: guess a 4-picture code (no repeats) from 6 pictures. Each tile shows ✓ right spot, ↔ in the code but wrong spot, ✕ not in the code. "Get a clue" reveals one picture in place for 1 battery bar (max 2).
  3. *Reveal*: live drone feed of Maple with howler monkeys, then a group-decision screen (stay with the monkeys vs come home) with vote counters.
- **Win / lose**: Win by cracking the 4-picture code. Lose when the drone battery (8 tries) runs out; the code is shown and a new one is generated. Step 1 has unlimited tries.
- **Controls**: Mouse / touch. Keyboard: step 1 digits 1–9 + Backspace; step 2 keys 1–6 pick pictures, Backspace undoes, Enter sends.
- **Design source**: Freeform (vibe-coded). Dusk-rainforest palette, chunky "field tablet" panels, all art drawn as inline SVG in code. Fonts: Lilita One, Nunito, Chakra Petch (Google Fonts, OFL).
- **Figma link or references**: none
- **Target**: both (phone and laptop)
- **Live URL / repo**: https://ajlcrowe.github.io/project-charlie-drone-code/ · https://github.com/ajlcrowe/project-charlie-drone-code (Pages from `main`, root). Single self-contained `index.html`.
- **Status**: Built and playtested headlessly (every path: cipher wrong/right, guesses, clue, win, lose/retry, feed, votes, play again). No console errors at 360px, 390px and 1280px widths. Tuning values are in the `CONFIG` block at the top of the script (battery, clue cost/limit, code length, timings).
