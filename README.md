# PkgDashboards

<!-- [![Build Status](https://travis-ci.com/baggepinnen/PkgDashboards.jl.svg?branch=master)](https://travis-ci.com/baggepinnen/PkgDashboards.jl) -->
<!-- [![Codecov](https://codecov.io/gh/baggepinnen/PkgDashboards.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/PkgDashboards.jl) -->

Create a dashboard with all your badges!

The exported functions are
- `dashboard(target_users; output=:markdown, autoopen=true, stargazers=false, githubci=false, stars=true)`
- `pkgdashboard(packagenames; kwargs...)`
- `uberdashboard(; kwargs...)` Generate dashboard for the entire General registry.

### Arguments:
- `target_users`: a string or a vector of strings with github usernames or org names
- `output`: `:markdown` or `:html`
- `autoopen`: indicate whether or not the result is opened in editor or browser
- `githubci`: Also add a Badge for github CI
- `stars`: Add github stars badge
- `stargazers`: include a plot with github stars over time

## Usage:
The following are some things you can do
```julia
dashboard("github_username")
dashboard(["username1", "username2"])
dashboard("github_username", output=:html, stargazers=true, stars=false, autoopen=true)
pkgdashboard(["PackageName1","PackageName2"])
```

## Result
`dashboard("baggepinnen")`:

|                                                                                                                URL |                                                                                                                                                                  Build status |                                                                                                                                                                                 PkgEval |                                                                                                                                                                              CodeCov |                                                                                                                                                                   Github stars |
|--------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|                               [baggepinnen/AdaptiveFilters](https://github.com/baggepinnen/AdaptiveFilters.jl.git) |                               [![Build Status](https://travis-ci.org/baggepinnen/AdaptiveFilters.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/AdaptiveFilters.jl) |                [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/A/AdaptiveFilters.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                               [![codecov](https://codecov.io/gh/baggepinnen/AdaptiveFilters.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/AdaptiveFilters.jl) |                               [![Stars](https://img.shields.io/github/stars/baggepinnen/AdaptiveFilters.jl.svg)](https://github.com/baggepinnen/AdaptiveFilters.jl/stargazers) |
|                       [baggepinnen/AutomaticDocstrings](https://github.com/baggepinnen/AutomaticDocstrings.jl.git) |                       [![Build Status](https://travis-ci.org/baggepinnen/AutomaticDocstrings.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/AutomaticDocstrings.jl) |            [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/A/AutomaticDocstrings.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                       [![codecov](https://codecov.io/gh/baggepinnen/AutomaticDocstrings.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/AutomaticDocstrings.jl) |                       [![Stars](https://img.shields.io/github/stars/baggepinnen/AutomaticDocstrings.jl.svg)](https://github.com/baggepinnen/AutomaticDocstrings.jl/stargazers) |
|               [baggepinnen/BasisFunctionExpansions](https://github.com/baggepinnen/BasisFunctionExpansions.jl.git) |               [![Build Status](https://travis-ci.org/baggepinnen/BasisFunctionExpansions.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/BasisFunctionExpansions.jl) |        [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/B/BasisFunctionExpansions.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |               [![codecov](https://codecov.io/gh/baggepinnen/BasisFunctionExpansions.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/BasisFunctionExpansions.jl) |               [![Stars](https://img.shields.io/github/stars/baggepinnen/BasisFunctionExpansions.jl.svg)](https://github.com/baggepinnen/BasisFunctionExpansions.jl/stargazers) |
|                                     [baggepinnen/BlobTracking](https://github.com/baggepinnen/BlobTracking.jl.git) |                                     [![Build Status](https://travis-ci.org/baggepinnen/BlobTracking.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/BlobTracking.jl) |                   [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/B/BlobTracking.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                                     [![codecov](https://codecov.io/gh/baggepinnen/BlobTracking.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/BlobTracking.jl) |                                     [![Stars](https://img.shields.io/github/stars/baggepinnen/BlobTracking.jl.svg)](https://github.com/baggepinnen/BlobTracking.jl/stargazers) |
|       [baggepinnen/ControlSystemIdentification](https://github.com/baggepinnen/ControlSystemIdentification.jl.git) |       [![Build Status](https://travis-ci.org/baggepinnen/ControlSystemIdentification.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/ControlSystemIdentification.jl) |    [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/C/ControlSystemIdentification.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |       [![codecov](https://codecov.io/gh/baggepinnen/ControlSystemIdentification.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/ControlSystemIdentification.jl) |       [![Stars](https://img.shields.io/github/stars/baggepinnen/ControlSystemIdentification.jl.svg)](https://github.com/baggepinnen/ControlSystemIdentification.jl/stargazers) |
| [baggepinnen/DifferentialDynamicProgramming](https://github.com/baggepinnen/DifferentialDynamicProgramming.jl.git) | [![Build Status](https://travis-ci.org/baggepinnen/DifferentialDynamicProgramming.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/DifferentialDynamicProgramming.jl) | [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/D/DifferentialDynamicProgramming.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) | [![codecov](https://codecov.io/gh/baggepinnen/DifferentialDynamicProgramming.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/DifferentialDynamicProgramming.jl) | [![Stars](https://img.shields.io/github/stars/baggepinnen/DifferentialDynamicProgramming.jl.svg)](https://github.com/baggepinnen/DifferentialDynamicProgramming.jl/stargazers) |
|                           [baggepinnen/DiskDataProviders](https://github.com/baggepinnen/DiskDataProviders.jl.git) |                           [![Build Status](https://travis-ci.org/baggepinnen/DiskDataProviders.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/DiskDataProviders.jl) |              [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/D/DiskDataProviders.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                           [![codecov](https://codecov.io/gh/baggepinnen/DiskDataProviders.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/DiskDataProviders.jl) |                           [![Stars](https://img.shields.io/github/stars/baggepinnen/DiskDataProviders.jl.svg)](https://github.com/baggepinnen/DiskDataProviders.jl/stargazers) |
|           [baggepinnen/DynamicMovementPrimitives](https://github.com/baggepinnen/DynamicMovementPrimitives.jl.git) |           [![Build Status](https://travis-ci.org/baggepinnen/DynamicMovementPrimitives.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/DynamicMovementPrimitives.jl) |      [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/D/DynamicMovementPrimitives.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |           [![codecov](https://codecov.io/gh/baggepinnen/DynamicMovementPrimitives.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/DynamicMovementPrimitives.jl) |           [![Stars](https://img.shields.io/github/stars/baggepinnen/DynamicMovementPrimitives.jl.svg)](https://github.com/baggepinnen/DynamicMovementPrimitives.jl/stargazers) |
|                                             [baggepinnen/Hyperopt](https://github.com/baggepinnen/Hyperopt.jl.git) |                                             [![Build Status](https://travis-ci.org/baggepinnen/Hyperopt.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/Hyperopt.jl) |                       [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/H/Hyperopt.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                                             [![codecov](https://codecov.io/gh/baggepinnen/Hyperopt.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/Hyperopt.jl) |                                             [![Stars](https://img.shields.io/github/stars/baggepinnen/Hyperopt.jl.svg)](https://github.com/baggepinnen/Hyperopt.jl/stargazers) |
|                                       [baggepinnen/LPVSpectral](https://github.com/baggepinnen/LPVSpectral.jl.git) |                                       [![Build Status](https://travis-ci.org/baggepinnen/LPVSpectral.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/LPVSpectral.jl) |                    [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/L/LPVSpectral.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                                       [![codecov](https://codecov.io/gh/baggepinnen/LPVSpectral.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/LPVSpectral.jl) |                                       [![Stars](https://img.shields.io/github/stars/baggepinnen/LPVSpectral.jl.svg)](https://github.com/baggepinnen/LPVSpectral.jl/stargazers) |
|                                     [baggepinnen/LazyWAVFiles](https://github.com/baggepinnen/LazyWAVFiles.jl.git) |                                     [![Build Status](https://travis-ci.org/baggepinnen/LazyWAVFiles.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/LazyWAVFiles.jl) |                   [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/L/LazyWAVFiles.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                                     [![codecov](https://codecov.io/gh/baggepinnen/LazyWAVFiles.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/LazyWAVFiles.jl) |                                     [![Stars](https://img.shields.io/github/stars/baggepinnen/LazyWAVFiles.jl.svg)](https://github.com/baggepinnen/LazyWAVFiles.jl/stargazers) |
|                                 [baggepinnen/LengthChannels](https://github.com/baggepinnen/LengthChannels.jl.git) |                                 [![Build Status](https://travis-ci.org/baggepinnen/LengthChannels.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/LengthChannels.jl) |                 [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/L/LengthChannels.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                                 [![codecov](https://codecov.io/gh/baggepinnen/LengthChannels.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/LengthChannels.jl) |                                 [![Stars](https://img.shields.io/github/stars/baggepinnen/LengthChannels.jl.svg)](https://github.com/baggepinnen/LengthChannels.jl/stargazers) |
|       [baggepinnen/LinearTimeVaryingModelsBase](https://github.com/baggepinnen/LinearTimeVaryingModelsBase.jl.git) |       [![Build Status](https://travis-ci.org/baggepinnen/LinearTimeVaryingModelsBase.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/LinearTimeVaryingModelsBase.jl) |    [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/L/LinearTimeVaryingModelsBase.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |       [![codecov](https://codecov.io/gh/baggepinnen/LinearTimeVaryingModelsBase.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/LinearTimeVaryingModelsBase.jl) |       [![Stars](https://img.shields.io/github/stars/baggepinnen/LinearTimeVaryingModelsBase.jl.svg)](https://github.com/baggepinnen/LinearTimeVaryingModelsBase.jl/stargazers) |
|               [baggepinnen/LowLevelParticleFilters](https://github.com/baggepinnen/LowLevelParticleFilters.jl.git) |               [![Build Status](https://travis-ci.org/baggepinnen/LowLevelParticleFilters.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/LowLevelParticleFilters.jl) |        [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/L/LowLevelParticleFilters.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |               [![codecov](https://codecov.io/gh/baggepinnen/LowLevelParticleFilters.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/LowLevelParticleFilters.jl) |               [![Stars](https://img.shields.io/github/stars/baggepinnen/LowLevelParticleFilters.jl.svg)](https://github.com/baggepinnen/LowLevelParticleFilters.jl/stargazers) |
|                 [baggepinnen/MonteCarloMeasurements](https://github.com/baggepinnen/MonteCarloMeasurements.jl.git) |                 [![Build Status](https://travis-ci.org/baggepinnen/MonteCarloMeasurements.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/MonteCarloMeasurements.jl) |         [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/M/MonteCarloMeasurements.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                 [![codecov](https://codecov.io/gh/baggepinnen/MonteCarloMeasurements.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/MonteCarloMeasurements.jl) |                 [![Stars](https://img.shields.io/github/stars/baggepinnen/MonteCarloMeasurements.jl.svg)](https://github.com/baggepinnen/MonteCarloMeasurements.jl/stargazers) |
|                             [baggepinnen/PriorityChannels](https://github.com/baggepinnen/PriorityChannels.jl.git) |                             [![Build Status](https://travis-ci.org/baggepinnen/PriorityChannels.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/PriorityChannels.jl) |               [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/P/PriorityChannels.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                             [![codecov](https://codecov.io/gh/baggepinnen/PriorityChannels.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/PriorityChannels.jl) |                             [![Stars](https://img.shields.io/github/stars/baggepinnen/PriorityChannels.jl.svg)](https://github.com/baggepinnen/PriorityChannels.jl/stargazers) |
|                                             [baggepinnen/Robotlib](https://github.com/baggepinnen/Robotlib.jl.git) |                                             [![Build Status](https://travis-ci.org/baggepinnen/Robotlib.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/Robotlib.jl) |                       [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/R/Robotlib.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                                             [![codecov](https://codecov.io/gh/baggepinnen/Robotlib.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/Robotlib.jl) |                                             [![Stars](https://img.shields.io/github/stars/baggepinnen/Robotlib.jl.svg)](https://github.com/baggepinnen/Robotlib.jl/stargazers) |
|             [baggepinnen/SingularSpectrumAnalysis](https://github.com/baggepinnen/SingularSpectrumAnalysis.jl.git) |             [![Build Status](https://travis-ci.org/baggepinnen/SingularSpectrumAnalysis.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/SingularSpectrumAnalysis.jl) |       [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/S/SingularSpectrumAnalysis.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |             [![codecov](https://codecov.io/gh/baggepinnen/SingularSpectrumAnalysis.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/SingularSpectrumAnalysis.jl) |             [![Stars](https://img.shields.io/github/stars/baggepinnen/SingularSpectrumAnalysis.jl.svg)](https://github.com/baggepinnen/SingularSpectrumAnalysis.jl/stargazers) |
|                                       [baggepinnen/ThreadTools](https://github.com/baggepinnen/ThreadTools.jl.git) |                                       [![Build Status](https://travis-ci.org/baggepinnen/ThreadTools.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/ThreadTools.jl) |                    [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/T/ThreadTools.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                                       [![codecov](https://codecov.io/gh/baggepinnen/ThreadTools.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/ThreadTools.jl) |                                       [![Stars](https://img.shields.io/github/stars/baggepinnen/ThreadTools.jl.svg)](https://github.com/baggepinnen/ThreadTools.jl/stargazers) |
|                           [baggepinnen/TotalLeastSquares](https://github.com/baggepinnen/TotalLeastSquares.jl.git) |                           [![Build Status](https://travis-ci.org/baggepinnen/TotalLeastSquares.jl.svg?branch=master)](https://travis-ci.org/baggepinnen/TotalLeastSquares.jl) |              [![PkgEval](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/T/TotalLeastSquares.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) |                           [![codecov](https://codecov.io/gh/baggepinnen/TotalLeastSquares.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/baggepinnen/TotalLeastSquares.jl) |                           [![Stars](https://img.shields.io/github/stars/baggepinnen/TotalLeastSquares.jl.svg)](https://github.com/baggepinnen/TotalLeastSquares.jl/stargazers) |
