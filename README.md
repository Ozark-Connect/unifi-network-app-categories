# UniFi Network App Categories

Searchable reference of every application and category recognized by UniFi Network for traffic identification and traffic rules.

**[View the live reference &rarr;](https://ozark-connect.github.io/unifi-network-app-categories/)**

## What is this?

When you create Traffic Rules in UniFi Network to block, allow, or rate-limit traffic by category (like "Online Games" or "Social Networking"), these are the specific applications included in each category.

Data is extracted from UniFi Network firmware.

## Categories

| Category | ID | Apps |
|---|---|---|
| Instant Messengers | 0 | 10 |
| P2P | 1 | 6 |
| Online Gaming | 2 | 8 |
| Business | 3 | 10 |
| Streaming Media | 4 | 10 |
| Web | 5 | 6 |
| Network Protocols | 6 | 6 |
| Social Networking | 7 | 8 |
| VPN & Tunnels | 8 | 5 |
| Email | 10 | 5 |
| File Sharing & Storage | 13 | 6 |

## How App IDs Work

UniFi uses compound IDs that encode the category: `compound_id = (category_id << 16) + app_id`.

For example, an app with ID `65538` belongs to category `1` (65538 >> 16 = 1) with app index `2` (65538 & 0xFFFF = 2). Category 0 apps have simple low-numbered IDs since `0 << 16 = 0`.

## Contributing

Found an issue? [Open an issue](https://github.com/Ozark-Connect/unifi-network-app-categories/issues) or submit a pull request.
