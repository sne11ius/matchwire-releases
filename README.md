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

## 🚧 CURRENT BUILD // v0.1.4

> [!IMPORTANT]
> MatchWire is currently a **pre-alpha overlay test build**. When both players
> run this version, it can open temporary peer-to-peer text chat over Arena. The
> overlay still needs live two-client validation, and voice and video are not
> implemented.

### Shipped ✅

- [x] Installable Windows desktop app
- [x] MatchWire interface and status screen
- [x] Public downloads and automatic update channel
- [x] Repeatable Windows release pipeline
- [x] First end-to-end update-path release
- [x] Consecutive updater release validation
- [x] Automatic Arena match lifecycle detection
- [x] Reciprocal match rendezvous and WebRTC verification probe
- [x] Hosted ephemeral signaling endpoint
- [x] Arena-attached overlay and ephemeral peer-to-peer text

### Next up 🧭

- [x] Confirm that both players see the same Arena match identity
- [x] Detect match start, completion, and leaving automatically
- [x] Prove reciprocal pairing and a direct data channel with saved match logs
- [x] Bring the temporary rendezvous endpoint online
- [x] Introduce two live desktop clients through a temporary connection
- [x] Bring text chat online for testing
- [ ] Validate overlay chat between two live desktop clients
- [ ] Add opt-in voice and video

Both sides of one real Arena match confirm the same match and reciprocal player
identities. MatchWire now follows that live lifecycle, reports reciprocal
identities through the temporary hosted rendezvous, and attempts a direct WebRTC
data-channel probe. Saved match perspectives verify that the channel survives
the match result and closes when either player leaves the Arena scene. Two live
`v0.1.3` clients have now completed that full path during a Direct Challenge,
including result-screen persistence and scene-exit teardown. The next quest is
validating the new `v0.1.4` Arena overlay and ephemeral text chat between those
live clients, then using that same surface for opt-in voice and video.

## 🚀 Try the overlay build

[**Download MatchWire for Windows**](https://github.com/sne11ius/matchwire-releases/releases/latest)

The installer is currently unsigned, so Windows SmartScreen may show a warning.
If you downloaded it from this official repository, select **More info** and
then **Run anyway**.

## 📜 Ship log

| Release | Codename | Status |
| --- | --- | --- |
| [`v0.1.4`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.4) | Table View | Current |
| [`v0.1.3`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.3) | Direct Probe | Direct-path validation |
| [`v0.1.2`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.2) | Update Echo | Updater validation |
| [`v0.1.1`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.1) | Update Ping | Updater validation |
| [`v0.1.0`](https://github.com/sne11ius/matchwire-releases/releases/tag/v0.1.0) | Boot Sequence | Foundation online |

## 🧪 Project status

- **Platform:** Windows x64
- **Stage:** Experimental pre-alpha
- **Media access:** Camera and microphone remain off in the current build
- **Data:** No MatchWire accounts, recordings, or persistent match history
- **Development:** Active spare-time project, one verified assumption at a time

Watch this repository for the next drop. The first real milestone is not a
feature count. It is two Arena opponents discovering the same table. ⚡
