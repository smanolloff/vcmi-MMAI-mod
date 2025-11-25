# Overview

A [VCMI](https://github.com/vcmi/vcmi) mod for distributing pre-trained
[`MMAI`](https://github.com/smanolloff/vcmi-MMAI) models through the VCMI mod
system.

## Publishing new models

When a new model is trained (via the
[`vcmi-gym`](https://github.com/smanolloff/vcmi-gym) project), it can be
published as a new version of the `MMAI` mod through VCMI's modding system:

1. Create a new github release and upload the new models (large onnx binary files)
as release assets.
1. Run the "Upload VCMI mod archive" github workflow and specify the release tag.
The workflow will package the models along with the source code into a
`vcmi-mod.zip` file and upload it as a release asset.
1. TODO - describe steps to update VCMI launcher's download URL to point to
  the new `vcmi-mod.zip`.
