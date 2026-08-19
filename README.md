<h1 align="center">( ◡̀_◡́)ᕤ senya</h1>

python backend developer

I build FastAPI services where the business rules are written down instead of implied: transactional consistency, JWT auth, predictable error contracts, and tests that run in CI on every push. Day to day that means PostgreSQL, SQLAlchemy, Alembic, Pydantic, pytest and Docker Compose.

Open to remote backend roles: API services, internal tools, automation, data-heavy workflows. Based in UTC+3, working in Russian and English.

## selected work

### [Configurable Training Report Generator](https://github.com/boundlessend/report_agent_api)

[![tests](https://github.com/boundlessend/report_agent_api/actions/workflows/tests.yml/badge.svg)](https://github.com/boundlessend/report_agent_api/actions/workflows/tests.yml)

Loads report scenarios from YAML, runs them through a fixed workflow, renders Markdown and exports DOCX. The same workflow is reachable two ways: from the CLI and through two FastMCP tools, so an MCP client can generate a report without knowing anything about the internals. 14 tests, SQLite storage, `uv` for dependency locking.

### [Educational Chat Assistant API](https://github.com/boundlessend/chat_assistant_api)

[![tests](https://github.com/boundlessend/chat_assistant_api/actions/workflows/tests.yml/badge.svg)](https://github.com/boundlessend/chat_assistant_api/actions/workflows/tests.yml)

Chat backend over 10 endpoints, one of them a WebSocket. JWT is checked before the socket is accepted, and a connection without a valid token is closed with code 1008 rather than allowed to raise inside the ASGI stack. Agent tool calls are deterministic, so the WebSocket flow is testable end to end: 14 tests, 89% coverage.

### [Promo Codes & Activations API](https://github.com/boundlessend/promos_api)

[![tests](https://github.com/boundlessend/promos_api/actions/workflows/tests.yml/badge.svg)](https://github.com/boundlessend/promos_api/actions/workflows/tests.yml)

15 endpoints for issuing and redeeming promo codes. Per-user and total activation limits, validity windows, and a rule that matters more than it looks: once a code has been activated, its type, target user and campaign stop being editable. Code uniqueness sits on a database constraint with an IntegrityError handler behind it, not on the service-level check alone. 18 tests, 85% coverage.

### [Wavelength Online](https://github.com/boundlessend/wave_site) → [live](https://wavesite-rho.vercel.app)

Board game for a group, one room per link, each player on their own device. No auth server: the room secret lives in the URL fragment and never reaches the backend, and every realtime message is encrypted with a key derived from it. The target zone is committed as a hash before the round and revealed after, so it cannot be swapped once the guessing starts. State authority migrates between clients on presence loss.

## smaller api projects

- [Warehouse Reservations & Shipping API](https://github.com/boundlessend/stock_api): stock reservations, cancellation, shipping confirmation, consistency rules
- [Support Tickets & Comments API](https://github.com/boundlessend/support_api): categories, event history, status transitions, owner/admin permissions
- [Leave Requests Approval API](https://github.com/boundlessend/leave_api): JWT access and refresh tokens in Redis, session-wide logout
- [Polls & Voting API](https://github.com/boundlessend/poll_backend): single-vote enforcement, manual and timer-based closing
- [URL Shortener API](https://github.com/boundlessend/shorto): custom codes, TTL expiry, per-link stats
- [Meeting Room Booking API](https://github.com/boundlessend/book_a_meeting-room): availability slots, filters by room and date

## what I care about

- api contracts that are easy to understand and hard to misuse
- constraints in the database, not just checks in the service layer
- error responses a client can branch on without parsing prose
- tests that cover permissions and failure paths, not only the happy one

## contact

Telegram [@boundlessend](https://t.me/boundlessend) · ohrimmmmm@yahoo.com
