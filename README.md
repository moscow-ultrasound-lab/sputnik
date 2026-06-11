# SPUTNIK Phantom

**S**tandardized **P**hantom for **U**ltrasound **T**esting and **N**umerical **I**maging **K**it

<!--[![Paper](https://img.shields.io/badge/paper-Medical_Physics-0077B5)](ссылка на DOI статьи 1 после публикации)-->
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

Low‑cost, reproducible, open‑source wire phantom for automated quality control (QC) of ultrasound scanners: spatial resolution (FWHM) and signal‑to‑noise ratio (SNR).

![SPUTNIK phantom](./docs/sputnik_header.png) <!-- добавите фото фантома -->

## 🚀 Quick links

- [📄 Paper (Medical Physics, 202X)](ссылка)
- [📦 Zenodo archive (all datasets & CAD)](ссылка)
- [🔬 MUSL Open Phantoms](https://drleonov.github.io/phantoms/)

## 🧩 Versions

| Version | Focus | Status | Folder |
|---------|-------|--------|--------|
| **v1.0** | Wire phantom + automated FWHM/SNR | ✅ Published | [`/v1.0-wire`](./v1.0-wire) |
| v2.0 | Contrast resolution | 🔜 Under review | `/v2.0-contrast` (soon) |
| v3.0 | 3D + elastography | 🔜 In preparation | `/v3.0-3d-elasto` (soon) |
| v4.0 | Modular kit | 🔜 Planned | `/v4.0-kit` (planned) |

## 📦 v1.0 – Wire QC phantom

### What's included

- `cad/` – laser‑cut DXF and STEP models
- `software/` – Python scripts for FWHM/SNR calculation from DICOM
- `protocol/` – step‑by‑step fabrication protocol (PDF)
- `validation/` – example output and sample DICOM

### Quick start

1. Clone this repository
2. Install dependencies: `pip install -r v1.0-wire/software/requirements.txt`
3. Run analysis: `python v1.0-wire/software/calc_fwhm_snr.py --input sample.dcm`
4. See `validation/example_output.csv` for expected results

### Hardware requirements

- Laser cutter (e.g., Wattsan 0503) for acrylic housing
- Steel wire (0.22 mm)
- PVC plastisol
- Ultrasound scanner (any B‑mode system)

## 📖 How to cite

If you use SPUTNIK v1.0 in your research, please cite:

> Chistova A., Leonov D. The SPUTNIK phantom: A low‑cost PVC‑based wire phantom for automated quality control of ultrasound spatial resolution and SNR. *Medical Physics*, 202X; XX(X):XXXX–XXXX. DOI: XXXX

For the software and hardware design, please also cite this GitHub repository:

> Moscow Ultrasound Lab. SPUTNIK phantom: Standardized Phantom for Ultrasound Testing and Numerical Imaging Kit. GitHub. https://github.com/moscow-ultrasound-lab/sputnik

## 📜 License

Hardware designs: CC BY‑NC 4.0  
Software: MIT  
Data: CC0 (public domain)

## 🙏 Acknowledgements

Developed at Moscow Ultrasound Lab.

## 🔗 Related projects

- [RUFUS](https://github.com/moscow-ultrasound-lab/rufus) – RF ultrasound simulation
- [PhantomAR](https://github.com/moscow-ultrasound-lab/PhantomAR) – Augmented reality for ultrasound phantoms
- [MUSL Open Phantoms](https://drleonov.github.io/phantoms/) – Main portal
