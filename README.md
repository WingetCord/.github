# WingetCord

**WingetCord** is a modern, TypeScript-first Discord bot framework designed for developers who want **speed, organization, and extensibility**. Unlike large frameworks like `discord.js`, WingetCord focuses on **lightweight architecture, modular design, and a developer-friendly experience**. It’s a **new and emerging library**, aiming to simplify Discord bot development while keeping performance and maintainability at the core.

> ⚠️ WingetCord is **Closed Source**. Developers can use it via the official documentation and examples only.

---

## **Key Features**

### REST API
- Full Async/Await implementation for requests.
- Route-specific queuing to handle rate limits internally.
- Exponential backoff retry mechanism for network and server errors.
- Comprehensive caching: Guilds, Members, Channels, Roles, Emojis.
- Support for all major endpoints (Users, Guilds, Channels, Webhooks, Roles, Commands).
- Modular handlers for each entity type (UserHandler, GuildHandler, ChannelHandler, etc.).

### Gateway & Sharding
- Robust Gateway connection with heartbeat management.
- Auto-reconnect and session resume for stability.
- Internal rate limit handling for high-frequency events.
- Sharding support for large servers.
- Optimized, asynchronous Event Dispatcher to avoid blocking.

### Interactions & Slash Commands
- Slash command registration and syncing with Discord.
- Collector system for Buttons, Select Menus, and Modals with automatic timeout.
- Fast acknowledge (<3s) to prevent interaction timeouts.
- Permission checks before executing commands.
- Automatic cleanup of collectors to prevent memory leaks.
- Comprehensive error handling with logs and user-friendly responses.

### Voice & Audio
- Resilient voice connection management.
- Modular Audio Player with async queue system.
- Atomic operations for skip, pause, resume, and volume adjustments.
- Garbage collection for voice channels.
- No WebSocket leaks, fully decoupled from core system.

### Security & Validation
- Payload validation for all requests and events.
- Input sanitation for all user-generated content.
- Robust permission system respecting role hierarchy.
- Logging for any unauthorized or suspicious actions.

### Developer Experience
- Full TypeScript strict mode.
- Modular architecture: REST, RateLimit, Queue, Gateway, Voice.
- Detailed logging for retries, rate limits, and collector timeouts.
- Hot-reloading support for commands and events.
- Practical, working examples included.
- Unit-test ready handlers and commands for reliability.

---

## **Getting Started**

### Installation
> WingetCord is a **private library** hosted in a GitHub Organization. Access is required to install via npm or yarn.

```bash
npm install @your-org/wingetcord
# or with yarn
yarn add @your-org/wingetcord
