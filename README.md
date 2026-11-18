# SE3-AUV

**SE(3)-Intrinsic Model Predictive Control and Disturbance Observer for AUV 6-DoF Pose Tracking**

![status](https://img.shields.io/badge/status-under%20review-yellow)
![code](https://img.shields.io/badge/code-coming%20soon-lightgrey)

> **Code release.** The manuscript is currently under review. The full implementation, simulator, configuration files, and figure-generation scripts will be released in this repository **upon acceptance of the paper**.

## Overview

The code is intended to support reproduction of the paper's simulations, ablations, and water-tank analyses, and to provide a baseline for further work on geometric predictive control for marine vehicles.

## Release plan

- [ ] C++ implementation
- [ ] 6-DoF Fossen simulator with scenario configurations
- [ ] Controller and observer parameters, and the experiment settings used in the paper
- [ ] Python scripts for analysis and figure generation
- [ ] Processed water-tank logs and plotting data, where permitted
- [ ] Build, usage, and reproduction documentation

Watch this repository to be notified when the code is released.

## Planned repository layout

```text
SE3-AUV/
├── src/                 # C++ core
├── include/             # public headers
├── sim/                 # 6-DoF plant, sensors, thrusters, scenarios
├── configs/             # controller, observer, and experiment parameters
├── scripts/             # Python analysis and figure generation
├── data/                # processed tank logs and plotting data
├── docs/                # build, usage, and reproduction notes
├── CMakeLists.txt
└── README.md
```

The layout is indicative and may change at release.

## Requirements (planned)

| Component | Requirement |
|---|---|
| C++ | C++17 compiler |
| Build | CMake ≥ 3.16 |
| Linear algebra | Eigen ≥ 3.3 |
| QP solver | OSQP ≥ 0.6 |
| Scripts | Python ≥ 3.9, NumPy, pandas, matplotlib |
| Platform | Linux preferred; Windows via WSL intended |

Experiment configurations will be selected through files under `configs/`; entry points and output formats will be documented in `docs/`.

## Contact

Linghao Yang (corresponding author)

Email: linghao_yangneu@163.com

GitHub: [@Linghao-Yang](https://github.com/Linghao-Yang)

## Contributing

Issues and pull requests will be welcome once the code is released.

## License

The code will be released under an open-source license; the exact license will be stated at release. Until then, please contact the authors before reusing any material.

## Disclaimer

This is research code. It is not certified for navigation, control, or operation of physical vehicles in the field, and it must not be used in safety-critical applications without independent verification.
