# Knighty

**First jailbreak hider for iOS 18 / Dopamine 3.** Hides the jailbreak from apps without killing tweak injection (unlike Dopamine Hide Jailbreak).

Compiled packages only. Source is not published.

## Install with Sileo

1. Add this source:

```
https://bbpotklo.github.io/knighty/
```

2. Also add **opa334's repo** if you don't have it:

```
https://opa334.github.io
```

Knighty needs **AltList** for the app picker.

3. Search **Knighty**, install, respring.

Keep Dopamine **Hide Jailbreak** off.

## Settings

After install, open the **Settings** app. **Knighty** is in the main list.

- **Enabled** — master switch
- **Knighty Applicationlist** — separate Settings row (same icon), search, switches off by default. InstaPay and Ana Vodafone are always hidden when Knighty is on.
- Hook toggles for files, tweaks, URL schemes, Frida ports, VPN (off by default), debugger flag

Respring from Sileo after changing settings if an app still sees the jailbreak.

## Choicy

Install Knighty **1.1.28+** before Choicy. For InstaPay / Ana Vodafone: leave Knighty on, disable Crane and Ghost. Do not turn off tweaks for SpringBoard.

## What it hides

| Layer | What it covers |
|-------|----------------|
| Filesystem | Jailbreak paths (`/var/jb`, Dopamine / procursus, TweakInject, apt, …) |
| URLs | Cydia / Sileo / Filza URL schemes |
| Loaded tweaks | Injected dylib names |
| VM map | Extra r-x pages / ElleKit trampolines omitted from `vm_region` |
| Network | Frida port probes (`27042` / `27043`); VPN interfaces (`utun`, ipsec) |
| Anti-debug | Debugger attach flag |

arm64 and arm64e. Rootless Dopamine 3.
