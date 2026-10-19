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



0.00%,yespowerurx,CPU
0.65%,"ethash, etchash",AMD / NVIDIA / Intel GPU
0.85%,"kawpow, fishhash, randomx, verushash, autolykos2",CPU / GPU
1.00%,"blake3_decred, sha256d_csd, rinhash, randomalpha",CPU / GPU
1.50%,"xelishashv3, qhash",CPU / GPU
2.00%,"flex, noid, pearlhash, quantus",CPU / GPU
3.00%,"argon2id_exfer, xhash",CPU / GPU
