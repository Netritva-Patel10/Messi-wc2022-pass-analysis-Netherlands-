# Lionel Messi: Open-Play Progressive Pass & Tactical Analysis
### FIFA World Cup 2022 Quarter-Final: Argentina vs. Netherlands

A multi-modal sports performance analysis combining Python event-data processing with Dartfish video telestration to analyze Lionel Messi's playmaking against the Netherlands' 5-3-2 mid-block.

---

## 📌 Project Overview
- **Match:** Argentina vs. Netherlands (FIFA World Cup 2022 QF)
- **Subject:** Lionel Messi's open-play progressive pass selection
- **Key Highlight:** Tactical breakdown of the 34th-minute line-breaking assist to Nahuel Molina
- **Data Source:** StatsBomb Open Data

---

## 🛠️ Data Methodology & Filtering Criteria
Using Python (`Pandas`), the StatsBomb match dataset was filtered using the following parameters:
- **Player Selection:** Filtered strictly for `Lionel Messi`.
- **Progressive Pass Definition:** Open-play passes with a minimum 10-yard forward distance gain toward the opponent's goal or any completed pass into the penalty box.
- **Exclusions:** All set pieces (corners, throw-ins, indirect free kicks) were excluded to focus purely on open-play tactical creation.

---

## 💻 Tech Stack & Workflow
- **Python (`Pandas`, `mplsoccer`):**
  - Spatial distance and metric calculations (x, y coordinates to goal Euclidean distance).
  - Dark-mode pitch map visualization illustrating pass origin and destination vectors.
- **Dartfish:**
  - Broadcast footage synchronization with event data.
  - Video telestration: Freeze-frame player spotlights, space overlays, and movement annotations.

---

## 📁 Repository Structure
- `Messi_progressive_passes.csv`: Filtered dataset containing Messi's open-play progressive passes and spatial metrics.
- `Argentina_Messi_analysis.ipynb`: Jupyter Notebook containing data cleaning, progressive pass logic, and pitch map code.
- `argentina_progressive_passes.png`: High-resolution dark-mode pitch map visualization.
- `README.md`: Project documentation and methodology overview.

---

## ⚽ Key Tactical Finding
- **34th-Minute Assist:** Messi's pass to Molina originated at (85.6, 44.9) and terminated inside the box at (103.4, 50.6).
- **Distance Impact:** Reduced goal distance from 34.75 yards to 19.70 yards—a 15.05-yard line-breaking progression that bypassed 5 Dutch central defenders.
