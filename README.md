# MATCHWIRE

**PRE-ALPHA // TABLE LINK PROTOCOL**

MTG Arena decides the matchup. MatchWire is being built to turn that same
matchup into a temporary player-to-player table for text, voice, and video.

No lobby. No room code. No permanent room. The link should exist for the match
and disappear when the match ends.

[**Download the current Windows build**](https://github.com/sne11ius/matchwire-releases/releases/latest)

## SYSTEM STATUS

```text
WINDOWS CLIENT       ONLINE
LOCAL INSTALLER      ONLINE
SELF-UPDATE CHANNEL  ONLINE
ARENA MATCH DETECTION AWAITING DUAL-LOG CONFIRMATION
PEER RENDEZVOUS      NOT DEPLOYED
TEXT / VOICE / VIDEO NOT DEPLOYED
```

The downloadable application is a working desktop and update foundation. It
does not yet detect matches or connect players. The next checkpoint is proving
that both sides of one real Arena match observe the same match ID and reciprocal
player IDs.

## CURRENT BUILD // v0.1.0 "BOOT SEQUENCE"

- Installable 64-bit Windows desktop client
- Public GitHub release channel
- User-controlled update checks, downloads, and restart
- Secure Electron renderer boundary
- MatchWire visual shell and status display

[Read the v0.1.0 field report](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.0)

## NEXT OBJECTIVE // RECIPROCAL SIGNAL

Two isolated Arena clients will play one Direct Challenge while preserving both
`Player.log` perspectives. That test must confirm:

- Both clients observe the same match identifier.
- Each client identifies itself and its opponent in reciprocal positions.
- A reliable event marks the end of the match.

Only after that signal is confirmed will MatchWire add rendezvous and WebRTC.
The prototype is deliberately advancing one verified assumption at a time.

## INSTALL ADVISORY

The current Windows installer is unsigned. Windows SmartScreen may display a
warning; select **More info** and then **Run anyway** only if you downloaded the
installer from this repository. Code signing is deferred while MatchWire is a
small experimental project.

## TRANSMISSION LOG

| Version | State | Field report |
| --- | --- | --- |
| `v0.1.0` | Current | [Boot Sequence](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.0) |

## OPERATING CONDITIONS

- Windows x64 only
- Experimental pre-alpha software
- No MatchWire account system or persistent match history
- Camera and microphone are not activated by this build
- Installer and update metadata are published here; application development is
  managed in a separate private source repository

This repository is the official public release channel for MatchWire.
