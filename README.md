# 🌌 JWST Spectral Analysis of NGC 7469

> End-to-end analysis of **James Webb Space Telescope (JWST) MIRI IFU data** to study the spectral properties of the galaxy **NGC 7469**.

---

## 📌 Overview

This project performs a detailed analysis of **JWST MIRI spectral cubes** to extract and study the infrared spectrum of **NGC 7469**, a luminous infrared galaxy.

The workflow includes:

* Pixel scale calculation in **parsecs per pixel**
* Spectral extraction from **different galactic regions**
* Visualization of **astrophysical spectral features**

---

## 🌠 Scientific Context

NGC 7469 is a well-known **luminous infrared galaxy** featuring:

* An **Active Galactic Nucleus (AGN)**
* A **star-forming circumnuclear ring**

Infrared spectroscopy helps in:

* Detecting **PAH emission features** (star formation indicators)
* Studying **ionized and molecular gas**
* Understanding **galactic structure and energy processes**

---

## 🎯 Objectives

* 📏 Convert pixel scale from angular units to **physical scale (pc/pixel)**
* 🌍 Compute angular diameter distance using cosmology
* 🧩 Extract spectra from **center and ring regions**
* 📊 Compare spectral properties across regions
* 🌈 Identify key spectral emission features

---

## 🔬 Methodology

1. Load JWST FITS spectral cubes
2. Extract header parameters (`CDELT`, `CRVAL`, etc.)
3. Convert pixel scale:

   * Degrees → Arcseconds → Parsecs
4. Compute angular diameter distance using **Planck18 cosmology**
5. Apply **DS9 region masks**
6. Extract:

   * Intensity
   * Error
   * Wavelength (rest-frame corrected)
7. Combine spectra across channels
8. Visualize results using Matplotlib and Plotly

---

## 📊 Results

* Pixel scale (approx):

  * ~44.53 pc (Channel 1)
  * ~58.23 pc (Channel 2)
  * ~68.51 pc (Channel 3)
  * ~119.89 pc (Channel 4)

* Generated outputs:

  * Combined galaxy spectrum
  * Center vs Ring spectral comparison
  * Feature-annotated spectrum

---

## 📂 Project Structure

```id="ht4p9x"
jwst-ngc7469-analysis/
│── notebooks/
│   └── jwst_analysis.ipynb
│── outputs/
│   ├── spectrum.png
│   ├── comparison.png
│── data/ (not included)
│── README.md
│── requirements.txt
```

---

## 🛠️ Tech Stack

* Python
* Astropy
* NumPy
* Matplotlib
* Plotly
* Pandas
* Regions (DS9)

---

## ⚙️ Setup

Install dependencies:

```bash id="n72yfp"
pip install -r requirements.txt
```

---

## 🚧 Future Work

* Automated detection of spectral lines
* Improved noise filtering
* Multi-object (multi-galaxy) analysis
* Integration with machine learning models

---

## 👩‍💻 Author

**Aaria Joshi**

---
