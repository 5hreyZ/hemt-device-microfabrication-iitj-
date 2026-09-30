# Fabrication and Electrical Characterization of AlGaN/GaN HEMTs

[![Institution - IIT Jodhpur](https://img.shields.io/badge/Institution-IIT_Jodhpur-003366?style=flat&logo=academia)](https://www.iitj.ac.in)
[![Department - Electrical Engineering](https://img.shields.io/badge/Department-Electrical_Engineering-darkblue?style=flat)](https://ee.iitj.ac.in)
![Device - AlGaN/GaN HEMT](https://img.shields.io/badge/Device-AlGaN%2FGaN%20HEMT-orange?style=flat)
![Cleanroom - Class 100/1000](https://img.shields.io/badge/Cleanroom-Class%20100%2F1000-teal?style=flat)
![Instrumentation - Keithley 6430 SMU](https://img.shields.io/badge/Instrumentation-Keithley%206430%20SMU-purple?style=flat)
![Status - Complete](https://img.shields.io/badge/Status-Completed-success?style=flat)

> **Author:** Shrey Painuli (M25EET007)  
> **Course Instructor:** Prof. Mahesh Kumar  
> **Department:** Department of Electrical Engineering, Indian Institute of Technology (IIT) Jodhpur  

---

## ⚡ Project Overview

This repository documents the end-to-end cleanroom microfabrication, selective multi-metal wet etching, and sub-femtoamp electrical characterization of **AlGaN/GaN High Electron Mobility Transistors (HEMTs)**. 

The experimental sequence covers substrate cleaving along crystallographic planes, 4-stage ultrasonic surface degreasing, high-vacuum thermal evaporation of an Al/Cr/Au (180 nm / 30 nm / 200 nm) ohmic stack, photolithographic micro-patterning, selective cyclic wet chemical etching, and rapid thermal annealing (RTA at 850°C). Measurements conducted on a **Keithley 6430 Sub-Femtoamp SMU** demonstrate contact activation from an as-deposited insulating open-circuit (< 0.35 nA) to active conduction (48 µA at 10 V) via quantum mechanical field emission.

<p align="center">
  <img src="assets/hemt_fabrication_workflow.png" alt="AlGaN/GaN HEMT Microfabrication & Characterization Workflow" width="100%"/>
</p>

---

## 🔬 1. Substrate Inspection & Wafer Cleaving

| (a) Side-Profile View | (b) HEMT Wafer Top Reflection | (c) Monocrystalline Si Top Reflection |
| :---: | :---: | :---: |
| <img src="assets/fig1a_wafer_side_comparison.jpg" width="240"/> | <img src="assets/fig1b_hemt_top_reflection.jpg" width="135"/> | <img src="assets/fig1c_si_top_reflection.jpg" width="240"/> |
| *Identical macroscopic wafer thickness* | *Metallic greyish optical reflectance* | *Distinct purple interference tone* |

### Wafer Slicing & Cleaving

<p align="center">
  <img src="assets/fig2_si_wafer_slicing.jpg" width="280" alt="Wafer Slicing via Diamond Scribing & Cantilever Cleavage"/><br/>
  <em>Wafer slicing via diamond scribing & cantilever cleaving along crystallographic planes</em>
</p>

| Parameter | Bulk Silicon Dummy | Epitaxial HEMT Wafer |
| :--- | :--- | :--- |
| **Role** | Cleaving / dicing practice | High-value active substrate |
| **Cleavage Plane** | {111} / {110} natural crystallographic planes | Heteroepitaxial AlGaN/GaN on Si(111) |
| **Fracture Quality** | Atomically flat mirror facet | Preserved from scratching and surface damage |
| **Tooling** | Diamond-tip scriber on glass support | Cleanroom Teflon-tipped tweezers |

---

## 🧪 2. Substrate Degreasing & Ultrasonic Cleaning

| (a) Chemical Solvents | (b) DI Water Cascade Rinse | (c) Thermal Evaporator Chamber |
| :---: | :---: | :---: |
| <img src="assets/fig2a_cleaning_solvents.jpg" width="270"/> | <img src="assets/fig2b_di_water_rinse.jpg" width="270"/> | <img src="assets/fig3c_thermal_evaporator.jpg" width="202"/> |
| *IPA, Acetone & Methanol reagents* | *Cascading deionized water rinse* | *High-vacuum deposition chamber* |

| (d) Ultrasonic Bath Processor | (e) Cleanroom Sample Handling | (f) Inert N₂ Gas Drying |
| :---: | :---: | :---: |
| <img src="assets/fig3a_ultrasonic_processor.jpg" width="180"/> | <img src="assets/fig3b_sample_handling.jpg" width="180"/> | <img src="assets/fig2c_n2_gas_drying.jpg" width="180"/> |
| *Cavitation acoustic processing* | *Teflon tweezer specimen transfer* | *Filtered dry nitrogen purge* |

### 4-Stage Ultrasonic Solvent Protocol (RCA-Style)
| Stage | Chemical Solvent | Bath Temperature | Duration | Physical & Chemical Rationale |
| :---: | :--- | :---: | :---: | :--- |
| **1** | Isopropanol (IPA) | Ambient (25°C) | 10 min | Gross particulate removal and polar trace stripping |
| **2** | Heated Acetone | 70°C – 80°C | 10 min | Dissolution of synthetic oils, waxes, and heavy organic grease |
| **3** | Methanol | Ambient (25°C) | 10 min | Stripping of dried acetone films and lightweight polar residues |
| **4** | DI Water + N₂ | Ambient (25°C) | Cascade + Blow Dry | Complete solvent displacement, ionic rinse, and inert drying |

---

## ⚡ 3. Thermal Evaporation Metallization Stack (PVD)

| Layer | Metal | Thickness | Function | Material Properties |
| :---: | :---: | :---: | :--- | :--- |
| **1 (Bottom)** | **Aluminum (Al)** | 180 nm | Primary Contact Layer | Low work function (4.28 eV); reacts with GaN during RTA to form donor vacancies (V_N⁺⁺) |
| **2 (Middle)** | **Chromium (Cr)** | 30 nm | Sacrificial Diffusion Barrier | High melting point (1907°C); prevents Au spike diffusion into 2DEG; promotes Al-to-Au adhesion |
| **3 (Top)** | **Gold (Au)** | 200 nm | Low-Resistivity Capping | Oxidation protection, bulk current spreading, and ductile pad for tungsten probe landing |

* **Base Chamber Pressure:** < 2.0 × 10⁻⁶ Torr (Turbomolecular high-vacuum pump)
* **Mean Free Path ($\lambda$):** ≈ 50 m >> 30 cm source-to-substrate distance (collision-free molecular trajectory)

---

## 🎯 4. Photolithography & Resist Patterning

| (a) Holmarc Spin Coater Console | (b) Substrate & Mask Fixture Plate | (c) Contact Hard Shadow Masks |
| :---: | :---: | :---: |
| <img src="assets/fig4a_spin_coater_console.jpg" width="112"/> | <img src="assets/fig4b_substrate_holder.jpg" width="266"/> | <img src="assets/fig4c_metal_shadow_masks.jpg" width="356"/> |
| *Digital RPM controller console* | *Substrate positioning vacuum chuck* | *Precision metal shadow / stencil masks* |

### Lithographic Recipe Parameters
| Process Step | Equipment / Reagent | Operating Parameters | Target Specification |
| :--- | :--- | :--- | :--- |
| **Spin Coating** | Holmarc HO-TH-05C | Verified 3915 rpm (4000 rpm nominal), 45 s, 500 rpm/s ramp | ~1.3 µm uniform DNQ-novolac resist |
| **Soft Bake** | Cleanroom Hot Plate | 115°C for 60 s | Solvent evaporation (PGMEA), stress relief |
| **UV Exposure** | Contact Mask Aligner | Broadband UV (365–436 nm), Chrome mask | Insoluble DNQ → Soluble indene carboxylic acid |
| **Development** | Positive Developer | Immersion for ~40 s followed by DI water quench | Clean pattern resolution with vertical resist sidewalls |
| **Hard Bake** | Cleanroom Hot Plate | 90°C for 90 s | Polymer cross-linking for chemical acid etch resistance |

---

## 🧪 5. Selective Tri-Metal Wet Etching & Failure Analysis

| (a) Incomplete Etch / Residue | (b) Severe Over-Etch & Undercut | (c) Optimized Selective Etch |
| :---: | :---: | :---: |
| <img src="assets/fig5a_incomplete_etching.jpg" width="215"/> | <img src="assets/fig5b_severe_overetching.jpg" width="360"/> | <img src="assets/fig5c_optimized_etching.jpg" width="180"/> |
| *Milky resist scumming & incomplete metal clearance* | *Etchant lateral attack eroding contact pad structure* | *Pristine, sharply delineated Au/Cr/Al contact pads* |

### Orthogonal Tri-Metal Wet Etch Chemistry
| Step | Metal Layer | Chemical Reagents | Duration | Governing Chemical Reaction Mechanism |
| :---: | :---: | :--- | :---: | :--- |
| **1** | **Au** (200 nm) | KI : I₂ : H₂O | 10 – 20 s | 2Au + I₃⁻ + I⁻ → 2[AuI₂]⁻ *(stops selectively at Cr)* |
| **2** | **Cr** (30 nm) | (NH₄)₂Ce(NO₃)₆ / HClO₄ (CAN) | 50 – 70 s | Ce⁴⁺ + Cr → Ce³⁺ + Cr⁶⁺ *(stops selectively at Al)* |
| **3** | **Al** (180 nm) | H₃PO₄ : HNO₃ : CH₃COOH : H₂O | 4 × 30 s (120 s) | Al + HNO₃ → Al₂O₃; Al₂O₃ + 6H₃PO₄ → 2Al(H₂PO₄)₃ |
| **4** | **PR Strip** | Acetone → IPA → DI → N₂ | Complete | Strips protective resist mask, exposing intact metallic contacts |

---

## 📊 6. Electrical Characterization (Pre-RTA vs. Post-RTA)

### Instrumentation Setup & Pre-RTA Open-Circuit State
| (a) Probe Station Contacting Pads | (b) Pre-RTA KickStart Sweep (0 to 6 V) | (c) Pre-RTA Secondary Sweep (0 to 5 V) |
| :---: | :---: | :---: |
| <img src="assets/fig6a_probe_station.jpg" width="300"/> | <img src="assets/fig6b_prerta_iv_curve.jpg" width="240"/> | <img src="assets/fig6c_prerta_secondary_sweep.jpg" width="250"/> |
| *Tungsten needle probes landed on pads* | *Current flat along noise floor (-50 to +350 pA)* | *Sub-nA baseline confirms zero carrier transport* |

### Post-RTA Contact Activation (850°C, 45 s)
| (a) Device 1 Post-RTA I–V Characteristic | (b) Device 2 Post-RTA I–V Characteristic |
| :---: | :---: |
| <img src="assets/fig7a_postrta_device1_iv.jpg" width="380"/> | <img src="assets/fig7b_postrta_device2_iv.jpg" width="380"/> |
| *Robust ohmic activation reaching **48 µA at 10 V*** | *Consistent quasi-ohmic conduction reaching **26 µA at 10 V*** |

### Quantitative Performance Comparison
| Parameter / Metric | Pre-RTA (As-Deposited State) | Post-RTA (850°C, 45 s Annealed State) | Change / Significance |
| :--- | :--- | :--- | :--- |
| **Metallurgical Phase** | Unreacted Al/Cr/Au discrete thin films | AlN + dense V_N⁺⁺ donor vacancies + Au-Al phases | Solid-state reaction completed |
| **Conduction State** | Open-circuit / insulating blocking barrier | Active quasi-ohmic / channel conduction | Ohmic contact formed |
| **Drain Current @ 5 V** | < 5 nA (instrument noise floor) | ~18 µA (Device 1) / ~10 µA (Device 2) | > 3 × 10³ current increase |
| **Drain Current @ 10 V**| Non-conductive (~0 µA) | **48 µA (Device 1) / 26 µA (Device 2)** | **> 5 orders of magnitude jump** |
| **Transport Mechanism**| Thermionic emission blocked by Φ_B ≈ 0.8 – 1.0 eV | Field Emission (quantum tunneling) via thin W_D < 2 nm | Low-resistance carrier injection into 2DEG |
