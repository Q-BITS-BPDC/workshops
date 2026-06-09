# Q-BITS Workshops

Hands-on quantum computing workshops by the Q-BITS club at BITS Pilani Dubai Campus. All materials are open — slides and Jupyter notebooks for every session.

---

## Getting Started

### Prerequisites

- Python 3.10 or newer
- Jupyter Lab or Jupyter Notebook

### Installation

```bash
git clone https://github.com/Q-BITS-BPDC/workshops
cd workshops
pip install -r requirements.txt
jupyter lab
```

### Core dependencies

```
qiskit >= 1.0
qiskit-aer
pennylane >= 0.35
numpy
matplotlib
jupyter
```

### IBM Quantum access (Track 3 onwards)

Track 3 runs circuits on real IBM hardware. Create a free account at [quantum.ibm.com](https://quantum.ibm.com) and save your token:

```python
from qiskit_ibm_runtime import QiskitRuntimeService
QiskitRuntimeService.save_account(channel="ibm_quantum", token="YOUR_TOKEN")
```

---

## Workshop Tracks

Four tracks covering the full breadth of quantum computing. Start at Track 0 if you're new — or jump in wherever your background fits.

```
Track 0 — Foundations    no prerequisites
Track 1 — Algorithms     linear algebra + Track 0
Track 2 — Applications   Track 1 + basic ML knowledge
Track 3 — Hardware       Track 1 + some physics background
```

---

### Track 0 — Foundations
> No prerequisites. Designed for complete beginners.

| # | Workshop | Topics | Notebook | Slides |
|---|---|---|---|---|
| W01 | What is a Qubit? | Superposition, Bloch sphere, measurement | [📓](track-0/W01/notebook.ipynb) | [📊](track-0/W01/slides.pdf) |
| W02 | Quantum Gates 101 | X, H, CNOT, Toffoli, circuit notation | [📓](track-0/W02/notebook.ipynb) | [📊](track-0/W02/slides.pdf) |
| W03 | Your First Circuit | Qiskit basics, Bell states, entanglement | [📓](track-0/W03/notebook.ipynb) | [📊](track-0/W03/slides.pdf) |
| W04 | Measurement & Probability | Born rule, expectation values, sampling | [📓](track-0/W04/notebook.ipynb) | [📊](track-0/W04/slides.pdf) |

---

### Track 1 — Algorithms
> Prerequisites: linear algebra, Track 0.

| # | Workshop | Topics | Notebook | Slides |
|---|---|---|---|---|
| W05 | Deutsch-Jozsa | Quantum parallelism, oracles, phase kickback | [📓](track-1/W05/notebook.ipynb) | [📊](track-1/W05/slides.pdf) |
| W06 | Grover's Search | Amplitude amplification, oracle construction | [📓](track-1/W06/notebook.ipynb) | [📊](track-1/W06/slides.pdf) |
| W07 | Quantum Fourier Transform | QFT circuit, phase estimation | [📓](track-1/W07/notebook.ipynb) | [📊](track-1/W07/slides.pdf) |
| W08 | Shor's Algorithm | Period finding, classical post-processing, factoring | [📓](track-1/W08/notebook.ipynb) | [📊](track-1/W08/slides.pdf) |

---

### Track 2 — Applications
> Prerequisites: Track 1, basic ML knowledge.

| # | Workshop | Topics | Notebook | Slides |
|---|---|---|---|---|
| W09 | Variational Quantum Circuits | Ansatz design, parameter shift rule, PennyLane | [📓](track-2/W09/notebook.ipynb) | [📊](track-2/W09/slides.pdf) |
| W10 | Quantum Machine Learning | QSVM, hybrid QNN, data encoding | [📓](track-2/W10/notebook.ipynb) | [📊](track-2/W10/slides.pdf) |
| W11 | Post-Quantum Cryptography | Lattice crypto, CRYSTALS-Kyber, NIST PQC standards | [📓](track-2/W11/notebook.ipynb) | [📊](track-2/W11/slides.pdf) |
| W12 | QAOA for Optimisation | Max-Cut, Ising model, portfolio optimisation | [📓](track-2/W12/notebook.ipynb) | [📊](track-2/W12/slides.pdf) |

---

### Track 3 — Hardware
> Prerequisites: Track 1, some physics background helpful. Requires IBM Quantum account.

| # | Workshop | Topics | Notebook | Slides |
|---|---|---|---|---|
| W13 | Noise & Decoherence | T1, T2 times, noise models, Aer simulation | [📓](track-3/W13/notebook.ipynb) | [📊](track-3/W13/slides.pdf) |
| W14 | Quantum Error Correction | Shor code, stabiliser formalism, surface codes | [📓](track-3/W14/notebook.ipynb) | [📊](track-3/W14/slides.pdf) |
| W15 | Running on Real Hardware | IBM Quantum, transpilation, primitive-based execution | [📓](track-3/W15/notebook.ipynb) | [📊](track-3/W15/slides.pdf) |

---

## Repository Structure

```
workshops/
├── track-0/
│   ├── W01/
│   │   ├── notebook.ipynb
│   │   ├── slides.pdf
│   │   └── README.md
│   ├── W02/ ...
│   ├── W03/ ...
│   └── W04/ ...
├── track-1/
│   ├── W05/ ...
│   └── ...
├── track-2/
│   ├── W09/ ...
│   └── ...
├── track-3/
│   ├── W13/ ...
│   └── ...
├── specials/
    ├── sp1/ ...
    └── ...
├── requirements.txt
├── CONTRIBUTING.md
└── README.md
```

Each workshop folder contains:
- `notebook.ipynb` — hands-on Jupyter notebook
- `slides.pdf` — session slides
- `README.md` — topic summary, prerequisites, and further reading

---

## Recordings Archive

Session recordings are linked below as workshops are conducted. Recordings are hosted on Google Drive / YouTube — links will be added after each session.

| # | Workshop | Recording |
|---|---|---|
| W01 | What is a Qubit? | — |
| W02 | Quantum Gates 101 | — |
| W03 | Your First Circuit | — |
| W04 | Measurement & Probability | — |
| W05 | Deutsch-Jozsa | — |
| W06 | Grover's Search | — |
| W07 | Quantum Fourier Transform | — |
| W08 | Shor's Algorithm | — |
| W09 | Variational Quantum Circuits | — |
| W10 | Quantum Machine Learning | — |
| W11 | Post-Quantum Cryptography | — |
| W12 | QAOA for Optimisation | — |
| W13 | Noise & Decoherence | — |
| W14 | Quantum Error Correction | — |
| W15 | Running on Real Hardware | — |

---

## Contributing a Workshop

Want to run a workshop for Q-BITS? Great. Here's how:

1. **Propose it** — open an issue with the title `[Workshop Proposal] Your Topic` and include: topic, target track, prerequisites, and a rough outline
2. **Get it reviewed** — the technical lead will review and assign a slot
3. **Use the template** — copy `_template/` into the right track folder and rename it
4. **Submit a PR** — once your notebook and slides are ready, open a pull request against `main`

### Workshop quality checklist

- [ ] Notebook runs end-to-end without errors
- [ ] All cells have markdown explanations above them
- [ ] Slides are in PDF format
- [ ] `README.md` inside the workshop folder lists prerequisites and further reading
- [ ] No hardcoded file paths or local dependencies

---

*Faculty Advisor: Dr. Tamizharasan Periyasamy, Deputy Head, Department of Computer Science, BITS Pilani Dubai*  
*Maintained by [Q-BITS](https://github.com/Q-BITS-BPDC)*
