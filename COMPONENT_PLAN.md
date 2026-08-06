# Component Plan — atc-social

This document details the components, primary data structures, and core functions implemented in `atc-social`.

## Core Component Specification

### 1. P2P Chat (`chat/chat_system.atc`)
- **Module**: `chat_system`
- **ATC Standard**: `ATC-45`
- **Description**: Direct messages, group chat, encrypted channels
- **Key Data Structure**: `ChatMessage`
- **Key Function**: `send_message()` — Routes end-to-end encrypted message through P2P network overlay

### 1. Social Feed (`feed/social_feed.atc`)
- **Module**: `social_feed`
- **ATC Standard**: `ATC-45`
- **Description**: Posts, likes, comments, follows, curation
- **Key Data Structure**: `FeedPost`
- **Key Function**: `publish_post()` — Broadcasts social post content hash to network feed index

### 1. Social Identity (`identity/social_identity.atc`)
- **Module**: `social_identity`
- **ATC Standard**: `ATC-45`
- **Description**: Profile, avatar, bio, on-chain identity
- **Key Data Structure**: `UserProfile`
- **Key Function**: `update_profile()` — Updates decentralised social profile metadata and handle bindings

### 1. Reputation System (`reputation/reputation_system.atc`)
- **Module**: `reputation_system`
- **ATC Standard**: `ATC-45`
- **Description**: Score, badges, endorsements
- **Key Data Structure**: `ReputationScore`
- **Key Function**: `calculate_reputation()` — Computes peer-weighted social reputation score

### 1. Messaging (`messaging/messaging.atc`)
- **Module**: `messaging`
- **ATC Standard**: `ATC-45`
- **Description**: Notifications, announcements, DM routing
- **Key Data Structure**: `Notification`
- **Key Function**: `push_notification()` — Dispatches system or social notification to target account

### 1. Moderation (`moderation/moderation.atc`)
- **Module**: `moderation`
- **ATC Standard**: `ATC-45`
- **Description**: Content policies, reports, appeals, bans
- **Key Data Structure**: `ModerationReport`
- **Key Function**: `review_report()` — Evaluates community content reports and updates moderation status

