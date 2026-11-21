# Side-Channel Attacks — Training Labs

Hands-on lab materials for a training on **microarchitectural** and **acoustic** side-channel
attacks. For authorized security education only.

## Contents

| File | What it is |
|---|---|
| `microarch_lab_students.zip` | **Part A — Microarchitectural.** Jupyter notebooks (with TODO stubs) to build Flush+Reload, Spectre v1 and Meltdown against a deterministic model, plus a real-hardware Flush+Reload bonus in C (Linux/x86). Runs on any OS. |
| `acoustic_lab_students.zip` | **Part B — Acoustic.** Jupyter notebooks (with TODO stubs) to recover keypad numbers, typed words and sentences from sound, judge whether a result is real, and test defences. Includes the recordings. |
| `microarch_lab_solutions.zip` | **Part A — instructor package.** The full `microarch_lab/` folder: `student/` stubs plus fully worked `solutions/` notebooks (every self-check prints PASS), the deterministic model, the instructor guide and the native C sources. |
| `acoustic_lab_solutions.zip` | **Part B — instructor package.** The acoustic `lab/` folder (library, recordings, student stubs) with the fully worked notebooks in `lab/solutions/`, including the merged all-labs notebook and a version with saved outputs. Run the solutions from inside `lab/solutions/`. |
| `Acoustic_All_Demos.zip` | **Instructor demo pack (acoustic).** Ready-to-run, fully worked demos shown live in class: keypad-tone (DTMF) decoding, app-usage classification, a CPU-instruction "doctor", and typed-sentence recovery. MATLAB + Python/Jupyter, with the recordings and expected outputs included. These are demonstrations, not the student exercises. |
| `flush-reload-demo_i9.zip` | A self-contained demo that reproduces the Yarom & Falkner (USENIX 2014) Flush+Reload cache attack and recovers an RSA private key from a locally-built, deliberately-vulnerable GnuPG 1.4.13. Uses a throwaway key in a sandbox; the host's real keyring is never touched. Needs Intel + Hyper-Threading on bare-metal Linux. |

Each zip contains its own `README.md` with setup and instructions.

## Responsible use

These materials are for learning how the attacks work and how to defend against them. Only run
them against systems and data you are authorized to test. The Flush+Reload demo attacks a
throwaway key it generates for itself — do not point it at anyone else's key.
