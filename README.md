# TMFG Simulator: Topological Mean Field Games for Social Exclusion and Hysteresis

## 🌍 Social Problem Awareness & Project Purpose
In the contemporary **attention economy**, the rapid proliferation of fake news, algorithmic sorting, and echo chambers has fundamentally fractured human communication. However, marginalized minorities and victims of collective ostracism are often dismissed by platform administrators and traditional statistics as mere "random noise" or "acceptable outliers."

The primary objective of this project is to **computationally expose and mathematically prove the structural violence inherent in modern digital ecosystems**. 
By running massive-scale simulations (up to $N=10^8$), this project reveals a disturbing truth:
1. **The Tyranny of the Law of Large Numbers (LLN):** In environments warped by social conformity (sontaku) and fake expected payoffs, scaling up data does not reveal the truth. Instead, it causes a "Variance Collapse," forcing the system into a deterministic, biased limit where minority distress signals are systematically and mathematically oppressed.
2. **Scapegoating as a Topological Defect:** Excluded minorities are not statistical errors; they are permanent "topological voids" (Betti 1) punched into the social fabric by the asymmetric gravity of majority illusion.
3. **The Cruelty of Hysteresis:** Once a community is divided by fake news and scapegoating, merely debunking the fake news post-hoc does not heal the divide. The capacity for relationship repair suffers an exponential death, making the social exclusion **structurally irreversible**.

This codebase provides the rigorous numerical evidence needed to argue for proactive, algorithmic interventions (such as protecting "weak ties") to restore informational hygiene in our digital society.

---

## 🔬 Theoretical Framework: The TMFG Model
This simulator integrates **Mean Field Games (MFG)** with **Topological Data Analysis (TDA)** concepts to model boundedly rational agents under incomplete information.
* **Conformity as a Metric Tensor:** Peer pressure acts as a gravitational field, warping the social space and forcing agents to deterministically fall into polarized echo chambers.
* **Topological Penalty ($e^{-\gamma D_t}$):** As the magnitude of fragmentation ($D$) increases, the network's ability to repair itself decays exponentially, creating a "Point of No Return."

---

## 📂 Repository Structure

### 1. `mainA.py` - Macroscopic Illusion and Irreversible Fragmentation
* **Goal:** Simulates the explosive dynamics of public illusion driven by fake expected payoffs and validates the "Variance Collapse."
* **Features:** Expands the sample size from $N=10^3$ to $N=10^8$. Demonstrates that even after fake news is exposed (payoff drops to 0), the fragmentation level remains permanently high (Hysteresis). It proves that massive datasets converge to a biased deterministic limit, silencing minority variance.

### 2. `mainB.py` - Dynamics of Pseudo-Scapegoating and Exploitation Gaps
* **Goal:** Models the asymmetric attack vectors targeting a specific minority (5% of the population) under fake victimhood claims.
* **Features:** Introduces a targeting coefficient ($v_i$) to simulate scapegoating. It explicitly visualizes the "Exploitation Gap" between the majority and the minority, and plots the exact "Death of the Repair Function" (Topological Penalty). It proves that the societal divide is irreversible even after the fake narrative is debunked.

---

## 🚀 Usage / How to Run

### Prerequisites
Make sure you have Python 3.8+ installed. Install the required dependencies using the provided `request.txt` (or `requirements.txt`) file.

```bash
pip install -r request.txt

Running the SimulationsBoth scripts are highly optimized to process up to 100,000,000 agents using batch processing to prevent memory crashes. The initial states are completely randomized to eliminate initial-value dependency.Bash# Run Experiment A
python mainA.py

# Run Experiment B
python mainB.py
OutputsUpon completion, the scripts will generate:summary_results.csv / summary_expB_comprehensive.csv: Contains the final fragmentation metrics and standard errors across all $N$ scales.history_N_*.csv: Time-series data of conformity and defect states for each scale.simulation_plots.png / comprehensive_pseudo_scapegoat_plots.png: High-resolution visualizations of the hysteresis, topological penalty, and LLN convergence.A compressed .zip file containing all outputs for easy downloading.📜 LicenseThis project is open-source. Researchers, data scientists, and policy-makers are encouraged to use these algorithms to audit platforms and advocate for better informational health diagnostics.
