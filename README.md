# Experimental Modal Analysis — Impact Hammer

Identifying natural frequencies and mode shapes of a 3-storey steel frame structure using impact hammer excitation.

For full methodology, results, and discussion see [`report.pdf`](./report.pdf).

---

## Repository Structure

```
├── data/               # Raw accelerometer and force time-series
├── scripts/
│   ├── calibration.py
│   ├── frf.py
│   └── modal_id.py
├── matlab/             # Equivalent MATLAB scripts
├── report.pdf
└── README.md
```

---

## Dependencies

```bash
pip install numpy scipy pandas matplotlib
```

MATLAB Signal Processing Toolbox required for the stabilisation diagram script.

---

## Usage

```bash
python scripts/calibration.py
python scripts/frf.py --data data/
python scripts/modal_id.py --plot
```
