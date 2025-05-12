# Compararea Algoritmilor pentru Rezolvarea Problemei Satisfiabilității (SAT)

Acest repository conține materialele pentru lucrarea "Compararea teoretică și experimentală a algoritmilor pentru rezolvarea problemei satisfiabilității în logica propozițională", care evaluează trei algoritmi fundamentali: Rezoluția, Davis-Putnam și DPLL/CDCL.

## Conținut

- `paper/`: Lucrarea în format LaTeX
- `scripts/`: Scripturi Python pentru analiza experimentală și generarea graficelor
- `results/`: Rezultatele experimentelor și figurile generate
- `benchmarks/`: Script pentru descărcarea benchmark-urilor SATLIB

## Structură

Acest proiect **nu reimplementează** algoritmii SAT, ci se bazează pe implementări open source existente pentru evaluarea experimentală:

| Algoritm | Implementare de referință | Repository |
|----------|--------------------------|------------|
| DPLL/CDCL | MiniSat | [https://github.com/niklasso/minisat](https://github.com/niklasso/minisat) |
| Rezoluție | PySAT | [https://github.com/pysathq/pysat](https://github.com/pysathq/pysat) |
| Davis-Putnam | Z3 | [https://github.com/Z3Prover/z3](https://github.com/Z3Prover/z3) |

## Instalare

Pentru a rula scripturile de analiză, aveți nevoie de următoarele dependențe:

```bash
# Instalare dependențe Python
pip install matplotlib numpy pandas pysat z3-solver

# Pentru a utiliza MiniSat
git clone https://github.com/niklasso/minisat.git
cd minisat
make
cd ..
