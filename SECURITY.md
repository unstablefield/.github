# Security

UnstableField runs on one machine and sends nothing anywhere. The server binds
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
- Anything that sends data off the machine.

Report it privately through GitHub's vulnerability reporting on this
repository: open the Security tab and choose "Report a vulnerability". Do not
open a public issue. Say which version (the `version` in `manifest.json`),
which backend, and how to reproduce it. You will get a reply from the
maintainer, and a fix lands in the engine repository with a changelog entry
that credits you unless you ask otherwise.

Nothing has been released yet, so there is no list of supported versions. The
newest commit on `main` is what gets fixed.
