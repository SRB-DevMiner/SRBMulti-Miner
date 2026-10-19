# ⚡ SRBMiner-MULTI Setup & Configurations

A high-performance configuration and startup repository for **SRBMiner-MULTI** — supporting multi-algorithm and dual-mining on AMD, NVIDIA, Intel GPUs, and CPUs.

---

## 🚀 Quick Start

1. Download the latest official release from the [SRBMiner-Multi GitHub Repository](https://github.com/doktor83/SRBMiner-Multi) or the [Official Website](https://www.srbminer.com/download.html).
2. Extract the archive into your preferred directory.
3. Place your custom configuration files inside the `configs/` folder and startup scripts inside `scripts/`.

---

## 📊 Supported Hardware & Fee Overview

* **AMD GPUs:** RX 9xxx, 7xxx, 6xxx, 5xxx, VEGA, RX 4xx/5xx series, BC-250.
* **NVIDIA GPUs:** Blackwell, Hopper, Ada Lovelace, Ampere, Turing, Pascal.
* **Intel GPUs:** Battlemage, Alchemist.
* **CPU Mining:** Fully optimized support for RandomX, VerusHash, HeavyHash, and more.

> 💡 **Dev Fee:** Varies between `0.00%` and `3.00%` depending on the algorithm selected (e.g., standard algorithms like `ethash` carry a low `0.65%` fee, while specialized dual-mining or heavy algorithms may vary).

---

## ⚙️ Popular Dual-Mine Combinations

SRBMiner-MULTI allows you to mine up to **4 different algorithms/coins simultaneously**. Some popular configurations include:
* `fishhash` + `qhash`
* `autolykos2` + `heavyhash`
* `etchash` + `blake3_decred`
* `randomepic` / `progpow_epic` + **Any algorithm**

---

## 📄 License & Disclaimer

Copyright © **doktor83**. All rights reserved. 
This repository contains configuration templates and helper scripts only. The proprietary binaries belong to the original author. Use responsibly on hardware you own or are authorized to manage. Provided **"AS IS"** without warranty of any kind.


@echo off
cd /d %~dp0
:: Example startup command for SRBMiner-MULTI
SRBMiner-MULTI.exe --config ..\configs\dual-mine-fishhash.json
pause



# ⚡ Supported Algorithms & Hardware Compatibility

An overview of all algorithms supported by **SRBMiner-MULTI**, including developer fee structures, dual-mining matrix, and device support.

---

## 📊 Overview Matrix

| Device Type | Symbol | Support Status |
| :--- | :---: | :--- |
| **CPU** | `C` | AMD Ryzen, Intel Core, ARM, EPYC, Xeon |
| **AMD GPU** | `A` | RX 9xxx, 7xxx, 6xxx, 5xxx, VEGA, RX 4xx/5xx, BC-250 |
| **NVIDIA GPU** | `N` | Blackwell, Hopper, Ada Lovelace, Ampere, Turing, Pascal |
| **Intel GPU** | `I` | Battlemage, Alchemist |

---

## 💸 DevFee & Algorithm List

> 💡 **DevFee Range:** Fees range from **0.00%** to **3.00%** depending on algorithm complexity and optimization level.

### 🟢 Low Fee (0.00% – 0.85%)

| Fee | Algorithm | CPU | AMD | NVIDIA | Intel |
| :---: | :--- | :---: | :---: | :---: | :---: |
| `0.00%` | **yespowerurx** | 🟢 | 🔴 | 🔴 | 🔴 |
| `0.65%` | **etchash** | 🔴 | 🟢 | 🟢 | 🟢 |
| `0.65%` | **ethash** | 🔴 | 🟢 | 🟢 | 🟢 |
| `0.85%` | **argon2d_16000** | 🟢 | 🟢 | 🔴 | 🔴 |
| `0.85%` | **argon2d_dynamic** | 🟢 | 🟢 | 🔴 | 🔴 |
| `0.85%` | **cpupower** | 🟢 | 🔴 | 🔴 | 🔴 |
| `0.85%` | **cryptonight_gpu** | 🟢 | 🟢 | 🟢 | 🟢 |
| `0.85%` | **cryptonight_turtle** | 🟢 | 🟢 | 🟢 | 🔴 |
| `0.85%` | **curvehash** | 🟢 | 🟢 | 🔴 | 🔴 |
| `0.85%` | **evrprogpow** | 🔴 | 🟢 | 🟢 | 🟢 |
| `0.85%` | **firopow** | 🔴 | 🟢 | 🟢 | 🟢 |
| `0.85%` | **fishhash** | 🔴 | 🟢 | 🟢 | 🟢 |
| `0.85%` | **ghostrider** | 🟢 | 🔴 | 🔴 | 🔴 |
| `0.85%` | **heavyhash** | 🔴 | 🟢 | 🟢 | 🟢 |
| `0.85%` | **kawpow** | 🔴 | 🟢 | 🟢 | 🟢 |
| `0.85%` | **meowpow** | 🔴 | 🟢 | 🟢 | 🟢 |
| `0.85%` | **randomx** | 🟢 | 🔴 | 🔴 | 🔴 |
| `0.85%` | **verushash** | 🟢 | 🔴 | 🔴 | 🔴 |

---

### 🟡 Medium Fee (1.00% – 1.50%)

| Fee | Algorithm | CPU | AMD | NVIDIA | Intel |
| :---: | :--- | :---: | :---: | :---: | :---: |
| `1.00%` | **autolykos2** | 🔴 | 🟢 | 🟢 | 🟢 |
| `1.00%` | **blake3_decred** | 🔴 | 🟢 | 🟢 | 🟢 |
| `1.00%` | **randomalpha** | 🟢 | 🔴 | 🔴 | 🔴 |
| `1.00%` | **randomy** | 🟢 | 🔴 | 🔴 | 🔴 |
| `1.00%` | **rinhash** | 🟢 | 🔴 | 🔴 | 🔴 |
| `1.00%` | **sha256d_csd** | 🔴 | 🟢 | 🟢 | 🟢 |
| `1.00%` | **verthash** | 🔴 | 🟢 | 🟢 | 🟢 |
| `1.50%` | **qhash** | 🔴 | 🟢 | 🟢 | 🟢 |
| `1.50%` | **xelishashv3** | 🟢 | 🟢 | 🟢 | 🟢 |

---

### 🔴 High Fee (2.00% – 3.00%)

| Fee | Algorithm | CPU | AMD | NVIDIA | Intel |
| :---: | :--- | :---: | :---: | :---: | :---: |
| `2.00%` | **blake3_an** | 🔴 | 🟢 | 🟢 | 🟢 |
| `2.00%` | **flex** | 🟢 | 🔴 | 🔴 | 🔴 |
| `2.00%` | **noid** | 🔴 | 🟢 | 🟢 | 🔴 |
| `2.00%` | **pearlhash** | 🔴 | 🟢 | 🟢 | 🔴 |
| `2.00%` | **quantus** | 🔴 | 🟢 | 🟢 | 🟢 |
| `3.00%` | **argon2id_exfer** | 🟢 | 🟢 | 🟢 | 🔴 |
| `3.00%` | **xhash** | 🔴 | 🟢 | 🟢 | 🟢 |

---

## 🔀 Dual Mining Combinations

SRBMiner-MULTI allows simultaneous mining of memory-hard and core-heavy algorithms:

```text
├── Primary: Fishhash      ──►  Secondary: Qhash / Blake3_Decred
├── Primary: Autolykos2    ──►  Secondary: Qhash / Blake3_Decred / Heavyhash
├── Primary: Etchash/Ethash──►  Secondary: Blake3_Decred / Heavyhash
└── Primary: Xhash         ──►  Secondary: Qhash / Blake3_Decred
