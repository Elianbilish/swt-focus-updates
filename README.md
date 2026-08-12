# SWT Focus Updates

This public repository stores the current macOS update archive and its signed `appcast.xml` feed for SWT Focus.

- It contains no student profile, API key, transcript, or practice record.
- SWT Focus verifies every downloaded archive with its embedded EdDSA public key before installation.
- Keep `appcast.xml` and the matching update archive together. Do not edit the feed by hand after it has been signed.
- After uploading a release, run `scripts/verify_cloud_release.sh` in the SWT Focus project. It checks the live feed version, signed archive URL, and byte-for-byte equality with the local release archive before the release is marked complete.
