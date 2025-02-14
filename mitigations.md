# Mitigations

## Proposed Mitigations

We propose the following three mitigations to lower the risk of attacks on vending machines.

### 1. Implement Strong Authentication and Encryption
- Require secure authentication for service techs and administrative users.
- Encrypt communication between the machine and backend servers to prevent interception of payment data.
- **DREAD updates:** **Damage (↓), Exploitability (↓), Affected Users (↓)**

### 2. Harden Physical Security 
- Reinforce locks, sensors, and glass to prevent unauthorized physical access.
- Implement a **safe-fault mechanism** if tampering is detected
- **DREAD updates:** **Damage (↓), Exploitability (↓)**

### 3. Regular Patching and Monitoring
- Update firmware regularly to for vulnerabilities.
- Implement anomaly detection (e.g. suspicious transactions or break in attempts).
- **DREAD updates:** **Reproducibility (↓), Exploitability (↓)**

| Threat | Damage (D) | Reproducibility (R) | Exploitability (E) | Affected Users (A) | Discoverability (D) | Risk Score (Avg) | Updated Factors |
|--------|------------|---------------------|---------------------|---------------------|----------------------|------------------|----------------|
| **Threat #1: Employee steals cash/coins** | **7** (↓) | **8** | **6** (↓) | **7** (↓) | **10** | **7.6** (was **8.4**) | Damage, Exploitability, Affected Users |
| **Threat #2: Employee steals products using duplicate key** | **9** (↓) | **5** | **3** (↓) | **7** | **4** | **5.6** (was **6.0**) | Damage, Exploitability |
| **Threat #3: Skimming device steals credit card data** | **8** (↓) | **5** (↓) | **2** (↓) | **7** (↓) | **4** | **5.2** (was **6.2**) | Damage, Reproducibility, Exploitability, Affected Users |
| **Threat #4: Student tilts machine to steal products** | **6** (↓) | **3** | **2** (↓) | **7** | **10** | **5.6** (unchanged) | Damage, Exploitability |
| **Threat #5: Student pries open door to steal contents** | **8** (↓) | **2** | **2** (↓) | **7** | **8** | **5.4** (was **5.8**) | Damage, Exploitability |
