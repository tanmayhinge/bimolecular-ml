# Bi-molecular machine learning: excitonic coupling

Kernel model predicting the excitonic coupling energy of a molecule pair (A, B) from Coulomb-matrix representations of the two geometries, with a learning curve characterising how the error falls with the number of reference calculations.

## Data

`BiMolData/` (not redistributed here):

| file | contents |
| --- | --- |
| `Coord_A.xyz` | 200 geometries of monomer A |
| `Coord_B.xyz` | 200 geometries of monomer B |
| `CouplingEnergies.csv` | coupling energy for each of the 40,000 (A, B) pairs |
| `Coord_supermol.xyz` | the 40,000 pairs treated as single molecules |

## Running

```sh
python -m venv .venv
.venv/bin/pip install -r requirements.txt
.venv/bin/jupyter lab challenge.ipynb
```

`challenge.ipynb` runs top to bottom from a clean kernel and is self-checking: the correctness conditions are `assert`s, not printed output.
