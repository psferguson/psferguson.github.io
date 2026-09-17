---
layout: page
title: Instrumentation & Data
permalink: /instrumentation/
nav_order: 2
redirect_from:
  - /infrastructures
---

![Peter at the Rubin Observatory summit]({{site.baseurl}}/public/images/peter_w_rubin.jpg){: width="250" style="float: right; margin: 0 0 1rem 1rem"}

Science with wide-field surveys is only as good as the instruments, calibrations,
and validation behind the catalogs. I have worked at every stage of that chain, from
building a calibration instrument in a lab, to verifying telescope hardware on the
summit, to writing the software that decides whether a survey's data products are
ready for cosmology. Most recently that has meant the Vera C. Rubin Observatory,
where I was on the core commissioning analysis team and now contribute in-kind as
LSST operations ramp up.

## Instruments and telescope integration

- **Rubin Observatory system integration (2023).** Spent six months on the summit in
  Chile as a core member of the system-performance analysis team and as a volunteer
  observing specialist. Designed and ran tests of the primary/tertiary mirror cell
  (M1M3) and the Telescope Mount Assembly, built the software to run those analyses
  automatically, and documented the results. Co-author on the SPIE 2024 papers on the
  [M1M3 support system](https://ui.adsabs.harvard.edu/abs/2024SPIE13094E..29Q),
  [M1M3 cell integration](https://ui.adsabs.harvard.edu/abs/2024SPIE13094E..51D),
  [M2 integration](https://ui.adsabs.harvard.edu/abs/2024SPIE13094E..2DR), and
  [integrated mount performance](https://ui.adsabs.harvard.edu/abs/2024SPIE13094E..09S).
- **TCal.** Lead developer of a mobile spectrophotometric calibration instrument
  built at Texas A&M to measure the throughput of any imaging system as a function of
  wavelength, so that follow-up telescopes can be placed on a common photometric
  system with LSST ([SPIE 2018](https://ui.adsabs.harvard.edu/abs/2018SPIE10702E..3AF),
  [SPIE 2020](https://ui.adsabs.harvard.edu/abs/2020SPIE11447E..5UF);
  [more details]({{site.baseurl}}/2021/02/28/TCal.html)).
- **FLAMINGOS-2 filters.** Commissioned two new medium-band K filters on
  FLAMINGOS-2 at Gemini South.

## Photometric calibration

![View from the Rubin Observatory summit]({{site.baseurl}}/public/images/rubin_view.jpg){: width="250" style="float: right; margin: 0 0 1rem 1rem"}

- **The Monster.** Led the creation of
  [`the_monster`](https://github.com/lsst/the_monster), an all-sky *ugrizy* reference
  catalog with synthetic fluxes that bootstraps Rubin's photometric calibration during
  commissioning and early operations
  ([Ferguson et al. 2025, DMTN-277](https://doi.org/10.71929/rubin/2583688)).
- **DELVE.** Implemented and characterized the photometric calibration and validation
  for the DECam Local Volume Exploration Survey, a ~2.5-billion-source *griz* catalog
  over 20,000 deg² built from archival DECam data and 130 nights of dedicated observing
  ([DR1](https://ui.adsabs.harvard.edu/abs/2021ApJS..256....2D),
  [DR2](https://ui.adsabs.harvard.edu/abs/2022ApJS..261...38D)). Those calibrations
  now underpin cosmology results, including the
  [DECADE cosmic shear analysis of 270 million galaxies](https://ui.adsabs.harvard.edu/abs/2026PhRvD.114d3527A)
  and the [first weak-lensing detection around low-mass galaxies](https://ui.adsabs.harvard.edu/abs/2026PhRvD.114b3040T),
  as well as the satellite and stream discoveries on my [research page]({{site.baseurl}}/research/).
- **Cross-calibration for transient follow-up.** Contributor to the Dark Energy
  Bedrock All-sky Supernova program's
  [cross-calibration and simulations](https://ui.adsabs.harvard.edu/abs/2026ApJ...996....7A).

## Data systems, validation, and science verification

- **Rubin Science Pipelines.** Developer of
  [`faro`](https://ui.adsabs.harvard.edu/abs/2022SPIE12189E..0MG) and its successor
  [`analysis_tools`](https://github.com/lsst/analysis_tools), the metric frameworks
  that automatically verify and validate data processed with the Rubin Science
  Pipelines.
- **Commissioning science verification.** Led ad hoc validation studies of AuxTel and
  precursor data, helped design the science validation surveys for commissioning, and
  served as science lead for the sample-production science unit (object detection,
  quality flags, verification and validation samples, survey property maps). This
  work fed into [Data Preview 1](https://ui.adsabs.harvard.edu/abs/2026AJ....171..360V).
- **Selection functions with synthetic source injection.** Use injected sources to
  measure survey completeness and contamination as a function of position, and to
  build training sets for machine-learning classifiers
  (e.g. [Boone, Ferguson et al. 2026](https://ui.adsabs.harvard.edu/abs/2026ApJ..1001..208B)).
- **Survey property maps.** Compute and visualize depth, seeing, and other survey
  properties with `decasu` and `healsparse` for DELVE and DES analyses.
- **DESC.** Bridge between the Rubin project and the Dark Energy Science
  Collaboration's Photometric Corrections, Science Release and Validation, and
  Commissioning working groups.
