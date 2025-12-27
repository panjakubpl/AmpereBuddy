# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 1.0.x   | :white_check_mark: |

## Reporting a Vulnerability

If you discover a security vulnerability in AmpereBuddy, please report it responsibly:

1. **Do NOT** create a public GitHub issue for security vulnerabilities
2. Send details to: **security@macfoundry.it**
3. Include:
   - Description of the vulnerability
   - Steps to reproduce
   - Potential impact
   - Any suggested fixes (optional)

### What to Expect

- **Acknowledgment**: Within 48 hours
- **Initial Assessment**: Within 7 days
- **Resolution Timeline**: Depends on severity
  - Critical: 24-72 hours
  - High: 1-2 weeks
  - Medium/Low: Next scheduled release

### After Reporting

- We will investigate and validate the issue
- We will work on a fix and coordinate disclosure
- You will be credited (unless you prefer anonymity)
- A security advisory will be published after the fix is released

---

## Security Measures in AmpereBuddy

### Update Verification

All updates are protected by multiple security layers:

1. **Ed25519 Digital Signatures**
   - Every update is cryptographically signed
   - Public key is embedded in the app
   - Invalid signatures are rejected

2. **Certificate Pinning**
   - TLS connections pin to specific certificates
   - Prevents man-in-the-middle attacks
   - Backup pins for Let's Encrypt intermediates

3. **SHA-256 Hash Verification**
   - Downloaded files are verified against published hashes
   - Prevents tampering and corruption

### Data Security

- All user data is stored locally on your Mac
- No cloud sync or remote storage
- Protected by macOS file permissions
- Compatible with FileVault encryption

### Network Security

- HTTPS only (HTTP connections rejected)
- No telemetry or analytics transmitted
- Update checks are GET-only (no user data sent)
- Network access can be disabled in Settings

### Permissions

AmpereBuddy requests minimal permissions:
- IOKit access for battery data (no user prompt required)
- Optional notification permissions
- Optional launch-at-login capability

No access to:
- Camera, microphone
- Contacts, calendar, photos
- File system (beyond app data)
- Keychain
- Location services

---

## Best Practices for Users

1. **Download from official sources only**
   - macfoundry.it/amperebuddy
   - Verify the SHA-256 hash if provided

2. **Keep the app updated**
   - Enable automatic update checks in Settings
   - Security fixes are distributed via updates

3. **Verify app signature**
   - Right-click app > Get Info
   - Should show signed by developer

4. **Use FileVault**
   - Encrypts all data on your Mac
   - Protects AmpereBuddy data files

---

## Changelog

Security-related changes are documented in [CHANGELOG.md](CHANGELOG.md) under the "Security" section for each release.
