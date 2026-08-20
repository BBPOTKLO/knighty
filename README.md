# Knighty

Jailbreak detection bypass for **Dopamine 3 / iOS 18**. Injects like a normal tweak and hooks detection APIs — it does **not** disable injection like Dopamine Hide Jailbreak.

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

After install, open the **Settings** app. You will see **Knighty** and **Knighty Applications** next to each other.

- **Knighty** — master switch, All Applications, hook toggles
- **Knighty Applications** — app picker (turn All Applications off first, then enable apps here)

Respring from Sileo after changing settings if an app still sees the jailbreak.

## Choicy

For apps that still detect you: inject **only Knighty** for that app. Disable Crane, Ghost, and other UI tweaks there.

## What it hides

| Layer | What it covers |
|-------|----------------|
| Filesystem | Jailbreak paths (`/var/jb`, Dopamine / procursus, TweakInject, apt, …) |
| URLs | Cydia / Sileo / Filza URL schemes |
| Loaded tweaks | Injected dylib names |
| Network | Frida port probes (`27042` / `27043`) |
| Anti-debug | Debugger attach flag |

arm64 and arm64e. Rootless Dopamine 3.
