# Project
## Data Engineering
### Nov. 14th 2026
I'm building a working **data pipeline for real satellite tracking data**

**The goal** is to build a *real* data pipeline that:
- **pulls** orbital data (TLEs) from Space-Track, using my credentials.
- **stores** raw data downloads
- **cleans and decodes** them into usable form
- **runs on a schedule** on its own, writing a record of each run
- is **tested** so I know it works

Here's what each folder is for:

- `docs/`: Notes, decoded TLE, and project specs
- `orbital/`: TLE parser, Space-Tracker client
- `scripts/`: Runnable scripts, the things I actually launch
- `tests/`: Tests that check my code is working
- `config/`: - Settings and watch lists, such as which satellites to track
- `data/raw,data/processed/`: Downloaded and cleaned data
- `logs/`: Records of each pipeline run

*Where things stand now*
Phase 1: setup complete; pipeline work starts in Phase 2. Must be able to run Phase 1 from memory before proceeding. Setting up my logs will come in Phase 2.