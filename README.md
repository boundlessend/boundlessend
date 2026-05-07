# howdy ( ◡̀_◡́)ᕤ

python backend developer

i'm focused on building practical API services with clear business logic, database design, authentication, tests, and documentation

work mostly with **FastAPI**, **PostgreSQL**, **SQLAlchemy**, **Alembic**, **Pydantic**, **JWT auth**, **pytest**, and Docker-based development workflows

## a little about me

- python web services & api architecture
- build REST APIs with validation, persistence, permissions, and predictable error handling
- have experience with both small MVP services and more complex domain logic
- ok working with technical documentation, test scenarios, and clean project structure
- simple, explicit solutions over unnecessary infrastructure

## tech stack

**languages:** Python, SQL  
**backend:** FastAPI, Django, Django REST Framework, Flask  
**databases:** PostgreSQL, SQLite, in-memory storage for MVPs  
**ORM / migrations:** SQLAlchemy, Alembic  
**auth:** JWT, bcrypt, Bearer token flows, owner/admin access rules  
**testing:** pytest, API tests, negative scenarios, WebSocket tests  
**tools:** Git, GitHub, Docker, Docker Compose, Linux, GitHub Actions  
**other:** REST API, WebSocket, Pydantic, MCP tools, fake LLM workflows, report generation

## completed backend projects

### API services

- **URL Shortener API**  
  FastAPI service for creating short links, redirecting by code, expiration handling, and click statistics.

- **Meeting Room Booking API**  
  Booking service with room/date filters, cancellation flow, and interval conflict validation.

- **Habit Tracker API**  
  PostgreSQL-based habit tracker with completion marks, current streaks, best streaks, and statistics.

- **Pastebin API**  
  Text snippet service with public/private snippets, raw output, expiration rules, and language filtering.

- **Polls & Voting API**  
  Poll creation, voting rules, duplicate vote protection, poll closing, and result aggregation.

- **Bookmarks & Article Collections API**  
  Collections, bookmarks, relationship modeling, duplicate protection, and PostgreSQL persistence.

### Auth, roles, and business logic

- **Leave Requests Approval API**  
  JWT authentication, user/admin roles, personal leave requests, approval/rejection flow, and access control.

- **Warehouse Reservations & Shipping API**  
  Product stock management, reservations, cancellation, shipping confirmation, admin-only operations, and stock consistency rules.

- **Support Tickets & Comments API**  
  Ticket categories, comments, event history, status transitions, priority changes, assignment logic, and owner/admin permissions.

### Advanced learning projects

- **Educational Chat Assistant with MCP Tools**  
  Backend chat service with JWT auth, WebSocket events, stored message history, fake LLM agent, mock MCP tools, file artifacts, and suggested actions.

- **Configurable Training Report Generator**  
  Report-agent that loads YAML scenarios, generates markdown reports, exports DOCX, uses fake LLM workflows, and exposes FastMCP tools.

## what i care about

- predictable API contracts
- clear validation and error responses
- reproducible setup through README and migrations
- tests for happy paths and negative scenarios
- explicit business rules instead of hidden assumptions
- clean separation between routers, schemas, services, models, and tests

## currently improving

- production-style FastAPI architecture
- database modeling and transactional logic
- testing strategy for APIs, auth, WebSocket, and service layers
- Docker Compose workflows
- backend agents, MCP tools, and fake LLM pipelines
