<img src="UnstableField GitHub Banner.png" width="100%" height="auto" alt="">

# Welcome to UnstableField

Local image, video and chat generation on your own GPU. It runs entirely on
your machine with its own engine built on torch and diffusers. A planner fits
each model to the hardware it finds, picking the weights' precision, offloading
and attention for the VRAM and RAM you actually have, so the same catalogue
runs on a 12 GB desktop and an 8 GB laptop. You pick Image or Video, a quality
and an aspect; it picks everything else. Chat runs on a local text model that
can start those jobs for you.

By default nothing is uploaded. The engine downloads a model's files when you
install it, the chat runtime's libraries on the first chat, and twice a day a
version file from GitHub to tell you when an update is out. Anonymous usage
data (timings, memory, GPU, error categories and ratings, never prompts or
file names) is off until you turn it on, and every batch sent is written to a
local log. There are no content filters. The code is GPL-3.0.

The engine and the web UI live in
[unstablefield/unstablefield](https://github.com/unstablefield/unstablefield).
Questions go to its
[discussions](https://github.com/unstablefield/unstablefield/discussions),
bugs and requests to its
[issues](https://github.com/unstablefield/unstablefield/issues), and pull
requests are welcome there; its
[CONTRIBUTING.md](https://github.com/unstablefield/unstablefield/blob/main/CONTRIBUTING.md)
says how. The website is at [unstablefield.com](https://unstablefield.com).
