# MatchWire 🎴🎙️

### Arena pairs the match. MatchWire opens the table.

Magic has always been more than cards and rules. It is the greeting before the
first draw, the reaction to an impossible topdeck, the conversation between
plays, and the final *good game* when the dust settles.

MatchWire brings that table feeling to MTG Arena.

## ✨ The vision

You queue for an ordinary Arena match. Your opponent does the same. If you both
use MatchWire, the match becomes your table:

- 💬 Chat without exchanging usernames or room codes
- 🎙️ Talk like you would across a real table
- 📹 Turn on video when both players want the full face-to-face game
- 🔒 Connect directly, with no permanent public room
- 👋 Stay for the post-match conversation, then leave the table naturally

No Discord detour. No friend request. No invitation link pasted into chat. The
match already knows who belongs at the table, so the match itself is the room.

MatchWire is for the games where seeing the player across from you makes every
bluff, comeback, misplay, and ridiculous win more memorable.

The table belongs over the game itself, so conversation does not require leaving
Arena for a separate chat application.

---

## 🚧 CURRENT BUILD // v0.1.9

> [!IMPORTANT]
> MatchWire is currently a **pre-alpha voice test build**. When both players run
> this version, it can open temporary peer-to-peer text chat and explicit
> opt-in voice over Arena. Text has passed a live in-game test. Voice and
> result-screen overlay behavior still need live validation; video is not
> implemented.

### Shipped ✅

- [x] Installable Windows desktop app
- [x] MatchWire interface and status screen
- [x] Public downloads and automatic update channel
- [x] Repeatable Windows release pipeline
- [x] First end-to-end update-path release
- [x] Consecutive updater release validation
- [x] Unattended, match-safe desktop updates
- [x] Automatic Arena match lifecycle detection
- [x] Reciprocal match rendezvous and WebRTC verification probe
- [x] Hosted ephemeral signaling endpoint
- [x] Arena-attached overlay and ephemeral peer-to-peer text
- [x] Automatic chat opening without dashboard focus or taskbar interference
- [x] Reliable dashboard, shortcut, and overlay recovery around Arena focus
- [x] Automatic same-match connection and in-memory chat recovery
- [x] Explicit microphone setup, input selection, mute, and peer-to-peer voice

### Next up 🧭

- [x] Confirm that both players see the same Arena match identity
- [x] Detect match start, completion, and leaving automatically
- [x] Prove reciprocal pairing and a direct data channel with saved match logs
- [x] Bring the temporary rendezvous endpoint online
- [x] Introduce two live desktop clients through a temporary connection
- [x] Bring text chat online for testing
- [x] Validate in-game overlay chat between two live desktop clients
- [ ] Validate overlay chat on the result screen and at scene exit
- [x] Add opt-in voice controls and microphone selection
- [ ] Validate voice between two live Arena clients
- [ ] Add opt-in video

Both sides of one real Arena match confirm the same match and reciprocal player
identities. MatchWire now follows that live lifecycle, reports reciprocal
identities through the temporary hosted rendezvous, and attempts a direct WebRTC
data-channel probe. Saved match perspectives verify that the channel survives
the match result and closes when either player leaves the Arena scene. Two live
`v0.1.3` clients completed that full path during a Direct Challenge, including
result-screen persistence and scene-exit teardown. The overlay has now carried
text chat during a live two-client Arena game. The overlay now also provides a
non-transmitting microphone setup step, local input selection, mute, and voice
that starts only after both players opt in. If a direct connection is
interrupted, `v0.1.9` keeps the table visible, rebuilds WebRTC while the Arena
match remains active, and synchronizes the last 100 in-memory messages directly
between recovery-capable peers. The next quest is validating voice and the
complete overlay lifecycle between two live clients.

Starting with `v0.1.5`, MatchWire downloads updates in the background and
silently restarts to install them. If an Arena match is active, it waits until
the local player leaves the match scene so the table is not interrupted.
`v0.1.8` also checks the release channel hourly, keeping clients current even
when MatchWire remains open across a later release. `v0.1.9` makes an explicit
second launch surface the existing dashboard and lets the global table shortcut
restore Arena after another window takes focus.

## 🚀 Try the overlay build

[**Download MatchWire for Windows**](https://github.com/sne11ius/matchwire-releases/releases/latest)

The installer is currently unsigned, so Windows SmartScreen may show a warning.
If you downloaded it from this official repository, select **More info** and
then **Run anyway**.

## 📜 Ship log

| Release | Codename | Status |
| --- | --- | --- |
| [`v0.1.9`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.9) | Steady Table | Current |
| [`v0.1.8`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.8) | Update Pulse | Updater reliability |
| [`v0.1.7`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.7) | Table Talk | Voice controls |
| [`v0.1.6`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.6) | Open Table | Overlay behavior |
| [`v0.1.5`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.5) | Silent Switch | Unattended updates |
| [`v0.1.4`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.4) | Table View | Overlay introduction |
| [`v0.1.3`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.3) | Direct Probe | Direct-path validation |
| [`v0.1.2`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.2) | Update Echo | Updater validation |
| [`v0.1.1`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.1) | Update Ping | Updater validation |
| [`v0.1.0`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.0) | Boot Sequence | Foundation online |

## 🧪 Project status

- **Platform:** Windows x64
- **Stage:** Experimental pre-alpha
- **Media access:** Camera stays off; microphone setup and transmission require
  explicit actions, and transmission starts only after both players join voice
- **Data:** No MatchWire accounts, recordings, or persistent match history
- **Development:** Active spare-time project, one verified assumption at a time

Watch this repository for the next drop. The first real milestone is not a
feature count. It is two Arena opponents discovering the same table. ⚡
