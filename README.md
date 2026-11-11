# NroChill iOS

Unity iOS export. Codemagic workflow: `ios-unsigned`.

## Codemagic

1. Add this GitHub repository in Codemagic as an iOS app.
2. Select configuration from `codemagic.yaml` and branch `main`.
3. Start workflow **NroChill unsigned IPA**.
4. Download `NroChill-unsigned.ipa` from build artifacts.

Native static libraries use Git LFS; the workflow downloads them before building.
No Apple certificate or provisioning profile is required for this unsigned build.
The IPA must be signed before installation on a normal iOS device.
