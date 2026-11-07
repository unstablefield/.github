# Support

Read the wiki in the engine repository first. It covers installation, the
hardware each tier needs, the Create, Chat and Models pages, the API, and
every measurement behind the minimum-spec table.

Questions go to the
[discussions](https://github.com/unstablefield/.github/discussions) on this
repository.

Bugs go to the issues on the engine repository. While that repository is
private, open them [here](https://github.com/unstablefield/.github/issues)
instead. The bug template asks for the hardware, the backend, the model and
tier, and the tail of `logs/run_and_install.log` from the data directory
(`~/.local/share/unstablefield/` unless `UNSTABLEFIELD_DATA_DIR` moved it).
That file has ids and timings and no prompts, so it is safe to paste.

Reports of a tier working or failing on hardware that has not been measured
(ROCm, XPU, Apple, 6 GB and 4 GB cards, Windows) are wanted. There is a
template for them. A calibration or parity report that moves a tier from
`estimated` to `calibrated` is sent as a pull request; the wiki page on
calibration says how.

Security problems are not raised in issues. See [SECURITY.md](SECURITY.md).
