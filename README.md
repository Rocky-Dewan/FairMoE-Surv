# FairMoE-Surv: A Fairness-Gated Neuro-Symbolic Mixture-of-Experts for Equitable Clinical Risk Prediction with Cross-Cohort Validation

**Md Rocky Dewan**<sup>1</sup> [![ORCID](https://img.shields.io/badge/ORCID-0009--0007--1477--4022-A6CE39?logo=orcid&logoColor=white)](https://orcid.org/0009-0007-1477-4022), **Rownuk Ara Rumy**<sup>2</sup>, and **Md. Saddam Hossain**<sup>3</sup>

<sup>1,3</sup>Department of Computer Science and Engineering, Bangladesh University of Business and Technology (BUBT), Dhaka, Bangladesh  
<sup>2</sup>Department of Computer Science and Engineering, Stamford University Bangladesh, Dhaka, Bangladesh

[![Conference](https://img.shields.io/badge/Accepted-IEEE%20CSDE%202026-blue)](https://www.ieee-csde.org/)
[![Status](https://img.shields.io/badge/Proceedings-Coming%20Soon-orange)](#citation)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Official repository for the paper **"FairMoE-Surv: A Fairness-Gated Neuro-Symbolic Mixture-of-Experts for Equitable Clinical Risk Prediction with Cross-Cohort Validation"**, accepted at the **11th IEEE Asia-Pacific Conference on Computer Science and Data Engineering (IEEE CSDE 2026)**.

---

## Publication Details

- **Title:** FairMoE-Surv: A Fairness-Gated Neuro-Symbolic Mixture-of-Experts for Equitable Clinical Risk Prediction with Cross-Cohort Validation
- **Conference:** 11th IEEE Asia-Pacific Conference on Computer Science and Data Engineering ([IEEE CSDE 2026](https://www.ieee-csde.org/))
- **Date:** 1–3 November 2026
- **Location:** Cox’s Bazar, Bangladesh
- **Status:** Accepted (Online IEEE Xplore proceedings coming soon)


---

## Abstract

Fairness-aware clinical risk models are often evaluated using aggregate metrics that may obscure disparities across protected groups and provide limited evidence of generalizability. We address both issues with **FairMoE-Surv**, a neuro-symbolic, fairness-gated mixture-of-experts (MoE) architecture that combines:
- A hybrid learned/symbolic router
- Clinically grouped mechanism tokens
- Momentum-updated population-prototype attention
- A top-2-of-6 MoE layer
- Demographic-parity and proxy-feature consistency regularizers
- A calibration module

On $N = 28,800$ real, de-identified CIBMTR allogeneic hematopoietic-cell-transplantation records spanning six self-reported race groups, FairMoE-Surv achieves:
- **89.2% AUROC**, **88.9% accuracy**, **88.4% F1**, **89.1% precision**, **87.8% recall**, and **88.7% concordance index**, outperforming CoxPH (83.8%), Random Survival Forest (85.2%), DeepSurv (86.1%), DeepHit (84.8%), and MTLR (86.9%).
- Lowest **demographic-parity gap (9.6% vs. 14.1–20.1%)**, **equal-opportunity gap (9.1% vs. 15.3–23.6%)**, and **expected calibration error (2.8% vs. 4.1–6.7%)** across all six race groups.

Retraining on a disease-mismatched SEER breast-cancer cohort ($N = 4,024$, three race groups) preserves FairMoE-Surv’s superiority while revealing fairness gap adjustments, demonstrating the necessity of cross-cohort retraining for validating fairness generalization.
---

## Key Features & Contributions

- **Neuro-Symbolic Architecture:** Combines symbolic domain knowledge and logical rules with deep survival analysis networks.
- **Fairness-Gated MoE:** Integrates a fairness-aware gating mechanism to ensure equitable risk predictions across diverse demographic groups.
- **Cross-Cohort Validation:** Evaluated across multi-center clinical cohorts to demonstrate generalizability, robustness, and demographic fairness.

---


### 2. Running the Notebooks

Launch Jupyter Notebook or JupyterLab or colab or kaggle to execute the experiments:


## Citation

If you find this work useful in your research, please consider citing our paper (IEEE Xplore citation link will be updated upon publication):

```bibtex
@inproceedings{fairmoesurv2026,
  title     = {FairMoE-Surv: A Fairness-Gated Neuro-Symbolic Mixture-of-Experts for Equitable Clinical Risk Prediction with Cross-Cohort Validation},
  author    = {Md Rocky Dewan , Rownuk Ara Rumy and Md. Saddam Hossain},
  booktitle = {Proceedings of the 11th IEEE Asia-Pacific Conference on Computer Science and Data Engineering (IEEE CSDE 2026)},
  location  = {Cox's Bazar, Bangladesh},
  pages     = {1--6},
  year      = {2026},
  month     = {November},
  publisher = {IEEE},
  doi       = {10.1109/CSDE59999.2026.XXXXXXX}  /* Update once available on IEEE Xplore */
}
```

---

## ✉️ Contact & Feedback

For questions, issues, or collaboration inquiries regarding **FairMoE-Surv**, please open an issue in this repository or contact the authors.
