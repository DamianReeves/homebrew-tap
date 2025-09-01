# DamianReeves Homebrew Tap

Official Homebrew tap for DamianReeves projects.

## Quick Start

```bash
# Add the tap
brew tap DamianReeves/tap

# Install sync-tools
brew install sync-tools

# Verify installation
sync-tools --version
```

## Available Packages

### sync-tools
Go CLI wrapper around rsync with advanced filtering and SyncFile post-sync actions.

**Features:**
- Advanced directory synchronization with conflict resolution
- .syncignore files and gitignore integration  
- Whitelist mode with sophisticated pattern matching
- SyncFile format with APPEND/PREPEND post-sync actions
- Git patch generation and application
- Interactive two-phased sync with plan editing
- Comprehensive BDD test coverage (57/57 scenarios passing)

**Installation:**
```bash
brew install DamianReeves/tap/sync-tools
```

**Project:** https://github.com/DamianReeves/sync-tools

## Automated Updates

This tap is automatically maintained by GoReleaser. When new releases are created in source projects, the corresponding Homebrew formulas are updated automatically.

## Manual Updates

If you need to manually update a formula:

1. Check the source project's latest release
2. Update the formula file in `Formula/`
3. Test the formula: `brew audit --strict Formula/package-name.rb`
4. Install test: `brew install --build-from-source ./Formula/package-name.rb`
5. Commit and push changes

## Support

For issues with packages, please report them in the respective source repositories:
- sync-tools issues: https://github.com/DamianReeves/sync-tools/issues

For tap-specific issues, create an issue in this repository.
