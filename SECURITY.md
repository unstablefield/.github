# Security

UnstableField runs on one machine. It uploads nothing unless the user turns on
anonymous usage data or presses Send on a report, and then only to
unstablefield.com. The server binds
to 127.0.0.1 unless started with `--host`, and there is no authentication:
remote access is out of scope, so a server opened to a network is open to
everyone on it. That is documented behaviour, not a vulnerability.

What counts as a vulnerability:

- A model file, LoRA, image, prompt or chat message that makes the engine run
  code or read or write files outside its data directory.
- A request to the local API that does the same.
- A download the engine or the installer performs (model files from Hugging
  Face, `uv`, the chat runtime's libraries) that could be swapped or
  tampered with on the way, where the engine does not notice.
- Anything that sends data off the machine while usage data is off, or sends
  more than the [documented fields](https://github.com/unstablefield/unstablefield/blob/main/wiki/architecture.md#telemetry)
  while it is on. Prompts, paths, file names and error text never leave.

Report it privately through GitHub's
[vulnerability reporting](https://github.com/unstablefield/unstablefield/security/advisories/new)
on the engine repository. Do not open a public issue. Say which version (the `version` in `manifest.json`),
which backend, and how to reproduce it. You will get a reply from the
maintainer, and a fix lands in the engine repository with a changelog entry
that credits you unless you ask otherwise.

Nothing has been released yet, so there is no list of supported versions. The
newest commit on `main` is what gets fixed.
