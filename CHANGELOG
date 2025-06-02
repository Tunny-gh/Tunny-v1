# Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/) and this project adheres to [Semantic Versioning](http://semver.org/).

Please see [here](https://github.com/Tunny-gh/Tunny-v1/releases) for the data released for each version.

---

## [v1.0.5-RC1] -2025-06-02

### Added

- Disable Rhino viewport updates during optimization checkbox in Settings/Misc tab.
  - The drawing to viewport stops, allowing faster optimization to be performed.
- Creating a file named quit.fishing in the .tunny_env folder to stop optimization.
- Optuna pruner support.
- Fully NEW UI
- Variables can now be set to log scale from the UI.
- Checkbox which minimize Rhino Window when start optimization
- Support some optunahub sampler.
  - Auto sampler, MOEA/D sampler, MO-CMA-ES sampler, DifferentialEvolution sampler, c-TPE sampler, HEBO sampler
- ConstructFishEggByCsv component
  - Make it easy to set FishEgg to use csv.
- Other Grasshopper component compatibility check.
- Support NetCore build
  - net7 for Rhino8
  - net9 for Rhino9
- Support mac Rhino8 and Rhino9
  - Both arm64 and x64
  - using eto UI
- Objective input values check
  - if null or list or tree input to objectives, Tunny throw error.
- Added error handling when an unexpected file path is entered in FishPrintByPath
  - support only bitmap type file.
- Tunny environment directory can open from Tunny fishing component menu items.
- Enhance GA base algorithm
  - Add mutation & crossover settings
- Add Command in Rhino
  1. `TunnyGetLicense` command which get Tunny license from cloud zoo.
  2. `TunnyRunDashboard` command which run optuna dashboard.

### Changed

- Default log file is set to "Verbose" with a retention period of 1 day.
- Dashboard & TT-DesignExplorer trial attribute handling.
  - Attribute values are shown in ParallelCoordinate plot in dashboard.
  - Attribute values are shown in graph & trial value table in TT-DesignExplorer.
- Stop log output to console.
- Disable window minimize button.
- No log output to the Rhino console.
- Human in the loop code was moved to the Optuna project to improve maintainability.
- Remove Geometry & Direction input from ConstructFishAttribute component.
  - Study direction can set in new Tunny UI.
  - If you need save geometry, Please use artifact feature.
- Update Grasshopper UI enable/disable timing.
  - Disable when Tunny UI wake up
  - Enable when Tunny UI closed
- For improve visibility, ConstructFishAttribute is colored.
- Improve result log file load speed.
  - Tunny was loading the result file when launching the UI, and when the log file was large, it took a long time to launch.
  - With this update, log files are now about 60 times faster to load.
    - What used to take about 5 minutes to load the results of 30,000 trials can now be loaded in about 5 seconds.
- Add Fish panel output to artifact info.
- Update ConstructFishEgg component
  - Add fill color
  - Add SkipIfExit input
- Update optuna v4.3

### Removed

- Geometry & Direction input in ConstructFisAttr component.
  - If you use Geometry, please use artifact.
  - Direction can set in New Tunny UI.

### Fixed

- Tunny UI wont wake up when rhino7(net4.8) version settings file deserialize.
- FishPrintByPath locks the image.
- Mesh could not be put directly into Artifact.
- Human in the loop exception with stop_flag.
- Even the multi-purpose Human in the loop specifies GP and the optimization does not flow, so TPE is chosen.
- Pareto Front plot with 3 objectives visualize error.
- Delegate initialize error when push run optimize button.
- If there is not examples dir in .tunny_env, tunny throw exception when Loading instruction.
- Use try-catch syntax to avoid LoadingInstruction exception.
- Same capture is saved when using FishPrintByCapture.
- SQLite library conflict to speckle

---

## Template

## [X.Y.Z] -20xx-xx-xx

### Added

for new features.

### Changed

for changes in existing functionality.

### Deprecated

for soon-to-be removed features.

### Removed

for now removed features.

### Fixed

for any bug fixes.

### Security

in case of vulnerabilities.
