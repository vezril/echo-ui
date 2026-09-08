# echo-ui — Echo's console (subscription management)

The console for **Echo** (the anonymous YouTube follower). It manages **subscriptions + the download
queue/status/errors** and the channel-follow config. **Viewing happens in Artemis, not here** — Echo
posts videos into the gallery.

**Status:** SEED (2026-09-08). Not built. Design: `codex/docs/echo.md`.

## Conventions

`UX-STANDARDS.md` + `UI-PLAYBOOK.md` in this folder are the **copied-in binding standards** (dark-
only, per-god accent; same build/deploy conventions as the sibling consoles). **Accent: TBD** — Echo
has no mark yet; assign one in `codex/docs/ux-standards.md` and generate art via the
constellation-logo pipeline. Deploys are the Codex session's. Owner/coordination per
`codex/docs/session-coordination.md`.

## Stack (when built)

Next.js 16 + React 19 + Tailwind v4, same as the sibling consoles (Node 22+). A BFF fronts
echo-service; the browser talks same-origin only.

## Scope (v1)

Add channels (by handle / URL / channel_id), edit per-channel config (the schema in
`codex/docs/echo.md`), watch the download queue + errors, pause/enable channels. **Not** a video
player — that's Artemis.

## License

MIT — see [LICENSE.md](LICENSE.md).
