# Clutch Riding Analysis: Fleet Level Summary

**Period:** Current Observation Window (Last 30–32 Days) | **Total Vehicles: 10**
**Analysis done on:** 9 vehicles with recorded telematics events
**Note:** Fuel data unreliable for 5 low-utilisation vehicles (sensor artefact — fuel values disproportionate to distance). Fuel-based metrics marked with `*` use reliable subset only (4 vehicles).

---

## 1. Fleet Utilization Overview

| Metric | Fleet Total |
|---|---|
| Total Distance Covered | 17,516.72 km |
| Total Fuel Consumed | ~6,848 Liters `(reliable vehicles)*` |
| Total Clutch Riding (CR) Distance | 3,233.35 km |
| Total Normal Riding Distance | 14,283.37 km |
| Total Fuel Consumed in CR Events | ~1,127 Liters `(reliable vehicles)*` |
| Fleet Avg Clutch Riding % | ~18% |
| Fleet Avg CR Fuel % | ~16% `(reliable vehicles)*` |

> `*` Reliable fuel data covers vehicles: it_861557068883245, it_861557068884995, it_861557068887675, it_861557068957445

---

## 2. CR-Based Cost Impact

| Metric | Value |
|---|---|
| Total Possible Clutch Cost Savings — Current Period | ₹6,079 |
| Total Possible Clutch Cost Savings if CR Reduced by 50% | ₹3,040 |
| Annualized Opportunity (Projected) | ₹72,948 |

> This is a recoverable cost through **Driver Training**, **Foot-off-Clutch Discipline**, and **Real-Time Telematics CR Alerts**

**How the current period savings are calculated:**

```
Total Extra Effective Wear  = Total CR Distance × (5−1)
                            = 3,233.35 km × 4
                            = 12,933.40 km of excess clutch wear

Savings (Current Period)    = (12,933.40 / 1,00,000) × ₹47,000*
                            = 0.12933 × ₹47,000
                            = ₹6,079

*₹47,000 = ₹35,000 replacement + 1.5 days × ₹8,000 downtime per clutch event

At 50% CR Reduction         = ₹6,079 / 2  = ₹3,040
Annualized Opportunity      = ₹6,079 × 12 = ₹72,948
```

---

## 3. High-Impact Vehicles — Top Optimization Targets

> Ranked by annual clutch cost exposure (projected at 50,000 km/vehicle/year)

| Vehicle Number | Total Possible Savings from CR (₹/yr) | Possible Savings at 50% CR Reduction (₹/yr) | CR% | Effective Clutch Life (km) | Degradation Factor | Clutch Life Lost (km) |
|---|---|---|---|---|---|---|
| it_861557068957445 | **₹55,460** | **₹27,730** | **59%** | 29,762 | 3.35× | 70,238 |
| it_861557068884664 | ₹31,960 | ₹15,980 | 34% | 42,373 | 2.36× | 57,627 |
| it_861557068888210 | ₹30,080 | ₹15,040 | 32% | 43,860 | 2.28× | 56,140 |
| it_861557068887337 | ₹29,140 | ₹14,570 | 31% | 44,643 | 2.24× | 55,357 |
| it_861557068885943 | ₹20,680 | ₹10,340 | 22% | 53,191 | 1.88× | 46,809 |
| it_861557068884995 | ₹8,460 | ₹4,230 | 9% | 73,529 | 1.38× | 26,471 |

> **Fleet-Wide Annual Excess Cost** (if current patterns persist at 50,000 km/vehicle/year): **₹1,79,070 / year**

---

## Annexure — Per-Vehicle Detailed Metrics

| Vehicle Number | Total KM | CR KM | Normal KM | CR% | Effective Wear KM | Clutch Life Used (%) | Current Period CR Cost (₹) |
|---|---|---|---|---|---|---|---|
| it_861557068957445 | 4,028.34 | 2,369.95 | 1,658.39 | 59% | 13,508 | 13.51% | ₹4,455 |
| it_861557068884995 | 8,408.93 | 793.00 | 7,615.93 | 9% | 11,581 | 11.58% | ₹1,491 |
| it_861557068883245 | 2,428.75 | 31.18 | 2,397.57 | 1% | 2,553 | 2.55% | ₹59 |
| it_861557068887675 | 2,541.90 | 8.62 | 2,533.28 | 0% | 2,576 | 2.58% | ₹16 |
| it_861557068887337 | 44.80 | 13.80 | 31.00 | 31% | 100 | 0.10% | ₹26 |
| it_861557068884664 | 14.20 | 4.80 | 9.40 | 34% | 33 | 0.03% | ₹9 |
| it_861557068888210 | 26.50 | 8.60 | 17.90 | 32% | 61 | 0.06% | ₹16 |
| it_861557068885943 | 14.70 | 3.20 | 11.50 | 22% | 28 | 0.03% | ₹6 |
| it_861557068958229 | 8.60 | 0.20 | 8.40 | 2% | 9 | 0.01% | ₹0 |
| **Fleet Total** | **17,516.72** | **3,233.35** | **14,283.37** | **~18%** | **30,449** | — | **₹6,079** |

> **Current Period CR Cost** = (CR_km × 4 / 1,00,000) × ₹47,000 — represents the clutch replacement + downtime cost incurred due to clutch riding during the observation period.

---

*Projections assume ₹35,000/clutch replacement, 1.5 days downtime at ₹8,000/day, and 1,00,000 km normal clutch lifespan. Annualized figures at 50,000 km/vehicle/year. Clutch wear multiplier: 5× per CR km (industry standard for heavy commercial vehicles).*
