# scfmDataPrep (development version)

- New parameters `fireMultiplier`, `fireMultiplierMethod`, `fireMultiplierWeights` and `scaleMaxFireSize` scale the burn rate estimated from data, e.g. for a scenario with more fire. They are passed to `scfmutils::calcZonalRegimePars()`, which splits the multiplier between the ignition rate, escape probability and mean fire size (see `?scfmutils::partitionBurnRateMultiplier`). A polygon with a `targetBurnRate` ignores `fireMultiplier`. With the defaults (`fireMultiplier = 1`, `scaleMaxFireSize = FALSE`) results are unchanged.
- Requires scfmutils >= 2.0.9.9012.

# scfmDataPrep 2.1.0

- Released with the scfm family at 2.1.0.

- changed `fireEpoch` from 1970-2020 in order to expand input data so that more wildfire is detected on the landscape

# scfmDataPrep 0.0.1 (04 February 2025)

- initial module version
