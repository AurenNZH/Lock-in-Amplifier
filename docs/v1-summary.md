# Version 1 Summary

Version 1 was an exploratory lock-in amplifier prototype. It combined an analogue signal path with digital reference generation and readout, aiming to recover a signal component coherent with a known reference.

## Architecture

The prototype used a device-under-test signal path followed by pre-amplification and filtering. A NUCLEO-F446RE generated reference timing signals for in-phase and quadrature demodulation. Switch-based multiplier stages performed phase-sensitive detection, and the resulting I/Q channels were sampled by the microcontroller ADC for PC readout.

The useful circuit references for this stage are kept as LTspice schematic files in `LIA_SPICE_SIM/` and the root-level `.asc` files.

## What Worked

- The project established a complete signal-chain concept from sensor input to PC readout.
- The I/Q demodulation architecture was captured clearly enough to guide the redesign.
- PCB assembly and bench testing exposed practical implementation constraints.
- The LTspice schematics remain useful as references for analogue front-end and demodulator decisions.

## Limitations

- The firmware and MATLAB processing work were rudimentary and are not being treated as reusable development foundations.
- Generated simulation outputs and logs are too bulky and noisy for the repository.
- The PCB Gerbers and BOM are v1 manufacturing artifacts rather than useful v2 source material.
- The full design reports are kept local; this repository carries only a concise summary.

## V2 Motivation

Version 2 should focus on the lessons from v1 rather than preserving every implementation detail. The redesign should revisit the analogue front end, phase-sensitive detector implementation, filtering strategy, digital acquisition path, and test methodology with a cleaner repository structure from the start.
