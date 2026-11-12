# Support

Read the [wiki](https://github.com/unstablefield/unstablefield/tree/main/wiki)
in the engine repository first. It covers installation, the hardware each tier
needs, the Create, Chat and Models pages, the API, and every measurement
behind the minimum-spec table.

Questions go to the
[discussions](https://github.com/unstablefield/unstablefield/discussions) on
the engine repository.

Bugs go to its [issues](https://github.com/unstablefield/unstablefield/issues/new/choose).
The bug template asks for the hardware, the backend, the model and tier, and
the tail of `logs/run_and_install.log` from the data directory
(`~/.unstablefield/` unless `UNSTABLEFIELD_HOME` moved it).
That file has ids and timings and no prompts, so it is safe to paste.

Reports of a tier working or failing on hardware that has not been measured
(ROCm, XPU, Apple, 6 GB and 4 GB cards, Windows) are wanted. There is a
template for them. A calibration or parity report that moves a tier from
`estimated` to `calibrated` is sent as a pull request; the wiki page on
calibration says how.

Security problems are not raised in issues. See [SECURITY.md](SECURITY.md).
