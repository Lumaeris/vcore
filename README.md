# vcore

Just a simple image for my old laptop that I will use to selfhost my stuff, I have no other use for it. I did this majorly because I can utilize [`build-chunked-oci`](https://coreos.github.io/rpm-ostree/build-chunked-oci/) to reduce update sizes (it's not fun to download 3 very large layers everyday...) and include small changes so I don't have to do it manually on live system.

This image probably won't stick for a long time, not sure yet.

## Why "vcore"?

"v" as in [VedaOS](https://github.com/Lumaeris/vedaos) and "core" as in [ucore](https://github.com/ublue-os/ucore) project I'm using here or [Fedora CoreOS](https://fedoraproject.org/coreos/), the base of it all. I couldn't think of a better name so there's that :slightly_smiling_face:

## Verification

These images are signed with [Sigstore](https://www.sigstore.dev/)'s [cosign](https://github.com/sigstore/cosign). You can verify the signature by downloading the `cosign.pub` file from this repo and running the following command:

```bash
cosign verify --key cosign.pub ghcr.io/lumaeris/vcore
```
