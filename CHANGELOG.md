# Changelog

All notable changes to AmpereBuddy will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2025-12-22

### Added
- Initial release of AmpereBuddy
- Real-time battery monitoring with charge percentage and health status
- Time remaining display for discharge and charge
- Current, maximum, and design capacity tracking (mAh)
- Battery cycle count with design cycle comparison
- Temperature, voltage, and amperage readings
- Individual cell voltage monitoring
- Charger/adapter details (wattage, type, wireless detection)
- Battery controller chip information
- Lifetime statistics (operating hours, temperature records)
- Mac model and processor identification
- CPU cores breakdown (performance/efficiency)
- GPU and Neural Engine core count
- RAM and storage information with SMART status
- Display information and Metal support status
- System security settings overview
- CPU and memory usage monitoring
- Weekly battery health snapshots with historical tracking
- Event log with 13 event types (charger events, temperature warnings, etc.)
- Low battery notifications and sounds (20% threshold)
- Fully charged notifications and sounds
- Critical battery status alerts
- Charger connection notifications
- High temperature warnings
- 4 built-in color themes + custom color picker
- 3 status bar display modes (icon only, icon+%, icon+%+time)
- Launch at login option
- Secure update checking with Ed25519 signature verification
- Certificate pinning for update server connections
- Desktop Mac detection with friendly "No Battery" message

### Security
- Ed25519 cryptographic signature verification for all updates
- TLS certificate pinning for macfoundry.it
- SHA-256 hash verification for downloaded files
- No telemetry or analytics - complete privacy

---

## Version History Format

Each release will document:
- **Added** - New features
- **Changed** - Changes to existing functionality
- **Deprecated** - Features to be removed in future versions
- **Removed** - Removed features
- **Fixed** - Bug fixes
- **Security** - Security improvements and vulnerability fixes
