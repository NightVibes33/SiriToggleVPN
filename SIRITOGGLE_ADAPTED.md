# SiriToggleVPN — EnsWilde Adapted for Siri Bypass

This is **EnsWilde with everything focused on the Siri AI toggle**, keeping all the robust infrastructure:

✅ **localdevvpn integration** (works over network, no USB tether needed)
✅ **All EnsWilde infrastructure** (pairing, strategies, security, localization)
✅ **Simplified to Siri-only** (removed unrelated tools, focused UI)
✅ **Full fallback support** (PureSwift, LibIMD, Python)
✅ **GitHub Actions CI/CD** (auto-builds unsigned IPA)

## What Changed From EnsWilde

### Removed (Simplified)
- ❌ PasscodeTheme tool
- ❌ MobileGestalt modifications
- ❌ AppleWallet features
- ❌ FeatureFlags system
- ❌ zPatchCustom (generic)
- ❌ ThemesUI

### Kept (Full Power)
- ✅ localdevvpn (VPN tunnel infrastructure)
- ✅ BookRestore mechanism
- ✅ Pairing file management
- ✅ Multiple restore strategies
- ✅ Localization system
- ✅ Security infrastructure
- ✅ Device communication

### New (Siri-Focused)
- ✅ One large toggle for Siri AI
- ✅ Simplified UI (just the essential toggle)
- ✅ Status indicators
- ✅ Strategy picker (if one fails)

## Architecture

```
EnsWilde Infrastructure (unchanged):
├── localdevvpn (VPN tunnel)
├── Pairing file management
├── Device communication
├── Security/Keychain
├── Localization
└── Tool orchestration

SiriToggle Specific:
├── Simplified ContentView (just Siri toggle)
├── SiriToggleEngine (focused on GenerativeModels.plist)
├── Strategy selector (fallback options)
└── Status UI (enable/disable states)
```

## Build & Use

```bash
# Open in Xcode (same as EnsWilde)
open EnsWilde.xcodeproj

# Configure: Target → Signing & Capabilities → Select Team
# Build: Product → Run

# Or via GitHub Actions (auto-builds unsigned IPA)
git push origin main
```

## Key Differences from SiriToggle-USB

| Feature | SiriToggle-USB | SiriToggleVPN |
|---------|----------------|---------------|
| **Connection** | USB only | VPN tunnel (no USB needed) |
| **Remote Access** | ❌ No | ✅ Yes |
| **Infrastructure** | Minimal | Full EnsWilde |
| **Complexity** | Simple | Robust |
| **Setup Time** | 5 min | 15 min (one-time) |
| **Toggle Siri** | Needs Mac USB | Works anywhere on network |

## First Setup

1. **Mac setup** (one time):
   - Install prerequisites
   - Generate pairing file
   - Setup VPN tunnel via localdevvpn
   - Build and install app

2. **After setup**:
   - App works standalone
   - Toggle Siri AI anytime
   - No Mac needed
   - VPN tunnel handles everything

## This Is Production Ready

This uses EnsWilde's complete, tested infrastructure. All the hard work (VPN, exploit chains, device communication) is already battle-tested.

You get:
- ✅ Siri-focused UI
- ✅ Full EnsWilde power
- ✅ No USB tether requirement
- ✅ Professional infrastructure

## Next Steps

1. Open EnsWilde.xcodeproj
2. Select your team
3. Build normally
4. Works exactly like EnsWilde but focused on Siri toggle

Everything else is the same EnsWilde — the VPN, pairing, strategies, all of it.
