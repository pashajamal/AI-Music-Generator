# JS Bach Chorales Music Analysis & Processing

This repository contains tools for loading, analyzing, and processing the JS Bach Chorales dataset using Python. It structures polyphonic 4-part harmony midi/note sequences from tabular data formats into structured lists ready for machine learning models (e.g., LSTMs, Transformers) or algorithmic music analysis, complete with interactive musical playback.

## Features
- **Data Loading & Organization:** Automatically walks through and sorts train, validation, and test splits from CSV files.
- **Polyphonic Note Parsing:** Extracts 4-part harmonies (`note0`, `note1`, `note2`, `note3`) corresponding to Soprano, Alto, Tenor, and Bass lines.
- **Musical Attribute Extraction:** Analyzes data parameters like pitch ranges (e.g., Lowest note: 36 / C1, Highest note: 81 / A5) and rests/silence indicators (0).
- **Interactive Music Playback:** Utilizes `music21j` inside Jupyter Notebooks to embed audio/midi playbacks of parsed data.

## Project Structure
```text
├── chorales/
│   ├── train/          # CSV files for training chorales
│   ├── valid/          # CSV files for validation chorales
│   └── test/           # CSV files for testing chorales
├── Main.ipynb          # Core notebook containing processing and analysis logic
└── README.md           # Repository documentation