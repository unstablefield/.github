# Contributing

Most contributions to UnstableField are one of three things: a measurement
from a GPU that has not been calibrated, a model for the catalogue, or a code
change. The engine repository's wiki page on calibration and parity says
exactly how each one is done; what follows is the short version.

Measurements. Every tier on ROCm, XPU and Apple hardware is labelled
`estimated` until a calibration report from matching hardware is reviewed. Run
the calibrate or parity command from the wiki on your card, then open a pull
request that adds the JSON under `benchmarks/` and gives your driver version
in the description.

Models. The default catalogue takes Apache-2.0, ungated models only.
Everything else goes in the Extended list with its license fields filled in.
A model with no license is not listed anywhere. Open an issue with the model
request template before writing a catalogue entry, so the license is checked
first.

Code. Run the tests before pushing, bump the version in `manifest.json`,
`engine/pyproject.toml` and `ui/package.json` together for any code change,
and add one plain-words line to `CHANGELOG.md` for anything a user would
notice. Documentation changes bump nothing. Keep pull requests to one change;
a refactor and a feature are two pull requests.

The code is GPL-3.0. By sending a pull request you agree that your change is
licensed the same way.

Please read the [code of conduct](CODE_OF_CONDUCT.md) too.
