<div align="center">

# Discord.JS Template Handler Bot

**A modular Discord.js bot starter with process-based sharding**

[![Discord.js](https://img.shields.io/badge/discord.js-v14-5865F2?logo=discord&logoColor=white)](https://discord.js.org/)
[![Node.js](https://img.shields.io/badge/Node.js-16.x-339933?logo=node.js&logoColor=white)](https://nodejs.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

</div>

---

## Overview

A starter project for building a Discord bot with **discord.js v14**. The launcher creates a `ShardingManager`, reads its token and shard configuration from the project config, and starts one or more bot processes.

## Stack

| Technology | Role |
|---|---|
| Node.js | JavaScript runtime |
| discord.js 14 | Discord API client and sharding |
| Chalk | Colored terminal output |
| MySQL2 / Sequelize | Database tooling included in the dependencies |
| node-cron | Scheduled task support |

## Getting started

### Requirements

- Node.js **16.x** (as declared in `package.json`)
- npm
- A Discord application and bot token

### Install

```bash
git clone https://github.com/sor1209/Discord.JS-TemplateHandler-Bot.git
cd Discord.JS-TemplateHandler-Bot
npm install
```

### Configure

Set the bot token and shard configuration in the project's config file:

```
core/manager/config.js
```

Keep the token private. Do not commit credentials or paste them into public issues.

### Run

```bash
npm start
```

For development with automatic restart:

```bash
npm run dev
```

Register or deploy application commands with:

```bash
npm run deploy
```

## Project scripts

| Command | Description |
|---|---|
| `npm start` | Start the bot launcher |
| `npm run dev` | Run with nodemon |
| `npm run deploy` | Run the command deployment script |

## Notes

- The launcher uses process-based sharding.
- When more than one shard is configured, shards are spawned with a 5-second interval.
- Review the configuration and bot entry point before deploying to a production server.

---

<div align="center">

**Built with Node.js and discord.js**

</div>
