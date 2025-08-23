# Distribution Guide

This repository is used for distributing Magnum desktop application binaries.

## Release Process

1. Build applications for all platforms using the main development repository
2. Test thoroughly on target platforms
3. Create a new GitHub Release with version tag (e.g., `v1.0.0`)
4. Upload platform-specific binaries to the release:
   - `Magnum-v1.0.0-macos.dmg` - macOS installer
   - `Magnum-v1.0.0-windows.msi` - Windows installer  
   - `Magnum-v1.0.0-linux.deb` - Debian/Ubuntu package
   - `Magnum-v1.0.0-linux.rpm` - RedHat/Fedora package
   - `Magnum-v1.0.0-linux.AppImage` - Universal Linux binary

## Binary Naming Convention

Format: `Magnum-v{VERSION}-{PLATFORM}.{EXTENSION}`

Examples:
- `Magnum-v1.0.0-macos.dmg`
- `Magnum-v1.0.0-windows.msi`
- `Magnum-v1.0.0-linux.deb`
- `Magnum-v1.0.0-linux.rpm`
- `Magnum-v1.0.0-linux.AppImage`

## Version History

Versions will be documented in GitHub Releases with detailed changelog.

## Platform Support

- **macOS**: 10.15+ (Intel and Apple Silicon)
- **Windows**: Windows 10/11 (64-bit)
- **Linux**: Modern distributions (glibc 2.17+)

## Notes

- Binaries are stored as GitHub Release attachments, not in git
- This repository contains only documentation and metadata
- Main development happens in the private development repository