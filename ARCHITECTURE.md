# Architecture Specification — atc-social

## Overview
`atc-social` is designed as a core module in **L7 — Social** of the A-TownChain architecture.

## Repository Metadata
- **Repository Name**: `atc-social`
- **Title**: Social Layer
- **Layer**: L7 — Social
- **Sprint**: 3.2
- **ATC Standard**: ATC-45
- **Primary Specification**: Social Layer — P2P Chat, Social Feed, Identity, Reputation

## Directory Structure

```text
atc-social/
├── chat/
│   └── chat_system.atc
├── feed/
│   └── social_feed.atc
├── identity/
│   └── social_identity.atc
├── reputation/
│   └── reputation_system.atc
├── messaging/
│   └── messaging.atc
├── moderation/
│   └── moderation.atc
├── README.md
├── ARCHITECTURE.md
├── COMPONENT_PLAN.md
├── FILE_REGISTER.md
├── STATUS.md
├── ROADMAP.md
├── CHANGELOG.md
├── .gitignore
└── LICENSE
```

## Component Architecture Table

| Directory | File | Module Name | Primary Responsibility |
| --- | --- | --- | --- |
| `chat/` | `chat_system.atc` | `chat_system` | P2P Chat — Direct messages, group chat, encrypted channels |
| `feed/` | `social_feed.atc` | `social_feed` | Social Feed — Posts, likes, comments, follows, curation |
| `identity/` | `social_identity.atc` | `social_identity` | Social Identity — Profile, avatar, bio, on-chain identity |
| `reputation/` | `reputation_system.atc` | `reputation_system` | Reputation System — Score, badges, endorsements |
| `messaging/` | `messaging.atc` | `messaging` | Messaging — Notifications, announcements, DM routing |
| `moderation/` | `moderation.atc` | `moderation` | Moderation — Content policies, reports, appeals, bans |
