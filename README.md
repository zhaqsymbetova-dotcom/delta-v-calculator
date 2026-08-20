# Delta-V Calculator for Spacecraft Missions

## Project Overview

This tool calculates the characteristic velocity (delta-V) and required propellant mass for spacecraft maneuvers using the Tsiolkovsky rocket equation. It compares chemical and electric propulsion systems for a reference transfer mission.

## Methodology

The core equation used is:

**ΔV = Isp × g₀ × ln(m₀ / mₖ)**

Where:
- **ΔV** — delta-V, characteristic velocity change (m/s)
- **Isp** — specific impulse (seconds)
- **g₀** — standard gravity, 9.81 m/s²
- **m₀** — initial spacecraft mass (kg)
- **mₖ** — final spacecraft mass (kg)

Two engine types are compared:
- **Chemical propulsion** (Isp = 300 s)
- **Electric propulsion** (Isp = 2500 s)

## Key Results

For a reference mission with ΔV = 4200 m/s (LEO to GTO transfer) and initial mass m₀ = 1000 kg:

| Propulsion Type | Isp (s) | Fuel Required (kg) |
|-----------------|---------|-------------------|
| Chemical        | 300     |     3185.7        |
| Electric        | 2500    |     157.3         |

**Conclusion:** Electric propulsion provides significant fuel savings for this mission, making it preferable for long-duration transfers despite lower thrust levels.

## Tools Used

- Python
- NumPy
- Matplotlib
- Google Colab

## Files

- `delta_v_calculator.ipynb` — Jupyter notebook containing the full calculation and visualizations.

## Author

Aigerim Zhaksymbet
