# 🍃 Synthetic Food Generator

[![CI](https://github.com/GALACTIC-UNION/synthetic-food-generator/actions/workflows/ci.yml/badge.svg)](https://github.com/GALACTIC-UNION/synthetic-food-generator/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python 3.12+](https://img.shields.io/badge/python-3.12%2B-blue)](https://www.python.org/)

**Computational design and bioreactor control platform for cell-cultured and
fermentation-derived food production** — Part of the OCN GAIA-NANO domain.

---

## Overview

Synthetic Food Generator (SFG) bridges metabolic engineering, bioreactor automation,
and nutritional optimisation to streamline the development of cell-cultured meat,
precision-fermented proteins, and microalgae-based food products.

### Key Capabilities

| Capability | Description |
|---|---|
| **Nutritional optimisation** | Linear programming for target macro/micronutrient profiles |
| **Bioreactor control** | PID controller integration for DO, pH, temperature, and agitation |
| **Cell line management** | Tracking and characterisation of cell line passages and performance |
| **Fermentation modelling** | Logistic and Monod kinetic models for growth prediction |
| **Regulatory compliance** | Automated generation of safety dossiers aligned with FDA/EFSA templates |

---

## Quick Start

```bash
git clone https://github.com/GALACTIC-UNION/synthetic-food-generator.git
cd synthetic-food-generator
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
cp config/config.example.yaml config/config.yaml
python src/bioreactor/controller.py --mode simulation
```

## Project Structure

```
synthetic-food-generator/
├── src/
│   ├── bioreactor/       # PID controllers and bioreactor adapters
│   ├── nutrition/        # Nutritional profile optimisation
│   ├── cell_lines/       # Cell line database and passage tracking
│   ├── fermentation/     # Kinetic models and batch prediction
│   └── compliance/       # Regulatory dossier generators
├── docs/
│   ├── bioreactor-setup.md
│   ├── fermentation-models.md
│   └── regulatory-guide.md
├── tests/
├── config/
├── .github/workflows/ci.yml
├── requirements.txt
├── CONTRIBUTING.md
└── README.md
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

MIT — see [LICENSE](LICENSE).
