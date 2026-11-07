<img src="UnstableField GitHub Banner.png" width="100%" height="auto" alt="">

# Welcome to UnstableField

Local image, video and chat generation on your own GPU. It runs entirely on
your machine with its own engine built on torch and diffusers. A planner fits
each model to the hardware it finds, picking the weights' precision, offloading
and attention for the VRAM and RAM you actually have, so the same catalogue
runs on a 12 GB desktop and an 8 GB laptop. You pick Image or Video, a quality
and an aspect; it picks everything else. Chat runs on a local text model that
can start those jobs for you.

Nothing leaves the machine. The only network use is downloading a model's
files when you install it and the chat runtime's libraries on the first chat.
There are no content filters and no telemetry. The code is GPL-3.0.

The engine repository is not public yet. Until it is, questions and reports go
to the [discussions](https://github.com/unstablefield/.github/discussions) and
[issues](https://github.com/unstablefield/.github/issues) on this repository.
The website is at [unstablefield.com](https://unstablefield.com).
