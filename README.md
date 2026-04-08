# MFEA-EI: A Parameter-Free Multifactorial Evolutionary Algorithm with Electrostatic-Inspired Interactions

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

This repository contains the source code for **MFEA-EI**, a parameter-free Evolutionary Multitasking (EMT) algorithm designed to solve multiple optimization tasks simultaneously via adaptive knowledge transfer.

## Overview

Evolutionary Multitasking (EMT) is a powerful paradigm that accelerates convergence by transferring genetic knowledge across different optimization tasks. However, indiscriminate transfer often leads to **negative transfer**, where information from unrelated tasks degrades performance.

**MFEA-EI** solves this by introducing a novel, **electrostatic-inspired charge mechanism** to intelligently guide inter-task mating. The framework assigns performance-based charges to individuals relative to their peers:
* **Negative Charge:** Assigned to high-performing elite solutions.
* **Positive Charge:** Assigned to under-performing solutions.

By simulating electrostatic principles, the algorithm promotes beneficial knowledge transfer through the attraction of opposite charges and prevents negative transfer by repelling same-charge interactions, all without requiring manual parameter tuning.

## Key Features

* **Parameter-Free:** Eliminates the need to manually tune the random mating probability (`rmp`) parameter, relying entirely on the dynamic state of the population.
* **Adaptive Knowledge Transfer:** Intelligently balances constructive transfer (attraction) and defensive preservation (repulsion).
* **Mathematically Grounded:** Asymptotic stability and convergence of the framework are guaranteed using Lyapunov stability theory.
* **Proven Effectiveness:** Surpasses state-of-the-art methods on standard benchmark suites (**CEC2017-MTSO**, **WCCI2020-MTSO**) and complex real-world engineering problems (Photovoltaic Models parameter extraction).

## Installation

Clone the repository and install the required dependencies:

```bash
git clone [https://github.com/yourusername/MFEA-EI.git](https://github.com/kanchan999/MFEA-EI.git)
cd MFEA-EI
pip install -r requirements.txt
