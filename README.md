# UniFi Network App Categories

Searchable reference of every application and category recognized by UniFi Network for traffic identification and traffic rules.

**[View the live reference &#8594;](https://ozark-connect.github.io/unifi-network-app-categories/)**

## What is this?

When you create Traffic Rules in UniFi Network to block, allow, or rate-limit traffic by category (like "Online Games" or "Social Networking"), these are the specific applications included in each category.

Data is extracted from UniFi Network firmware.

## Current Data

- **UniFi Network**: 10.1.85
- **DPI Signatures**: v2.128
- **Categories**: 35
- **Applications**: 2109
- **Last Updated**: 2026-02-24

## Categories

| Category | ID | Apps |
|----------|----|------|
| Instant messengers | 0 | 64 |
| Peer-to-peer networks | 1 | 136 |
| File sharing services and tools | 3 | 77 |
| Media streaming services | 4 | 188 |
| Email messaging services | 5 | 67 |
| VoIP services | 6 | 23 |
| Database tools | 7 | 9 |
| Online games | 8 | 202 |
| Management tools and protocols | 9 | 15 |
| Remote access terminals | 10 | 33 |
| Tunneling and proxy services | 11 | 72 |
| Investment platforms | 12 | 16 |
| Web services | 13 | 239 |
| Security update tools | 14 | 38 |
| Web instant messengers | 15 | 3 |
| Business tools | 17 | 55 |
| Network protocols | 18 | 245 |
| Network protocols | 19 | 247 |
| Network protocols | 20 | 184 |
| Adult | 22 | 1 |
| Private protocols | 23 | 2 |
| Social networks | 24 | 88 |
| TopSites-Adult | 28 | 2 |
| TopSites-Arts | 29 | 29 |
| TopSites-Business | 30 | 2 |
| TopSites-Computers | 31 | 3 |
| TopSites-Health | 33 | 13 |
| TopSites-Home | 34 | 9 |
| TopSites-News | 36 | 19 |
| TopSites-Recreation | 37 | 5 |
| TopSites-Science | 40 | 7 |
| TopSites-Shopping | 41 | 11 |
| TopSites-Society | 42 | 1 |
| TopSites-Sports | 43 | 6 |
| Unknown | 255 | 1 |

## How App IDs Work

UniFi uses compound IDs that encode the category: `compound_id = (category_id << 16) + app_id`.

For example, an app with ID `65538` belongs to category `1` (65538 >> 16 = 1) with app index `2` (65538 & 0xFFFF = 2). Category 0 apps have simple low-numbered IDs since `0 << 16 = 0`.

## One App, One Category

Each application is mapped to exactly one category in the UniFi Network web app code. This means some apps may appear in broader categories than you'd expect. For example, several well-known adult sites are categorized under "Media streaming services" rather than "Adult", and AI chatbots like ChatGPT appear under "TopSites-Adult".

These are the mappings as they exist in the UniFi Network web app code — review the specific apps in each category before creating traffic rules.

## Contributing

Found an issue? [Open an issue](https://github.com/Ozark-Connect/unifi-network-app-categories/issues) or submit a pull request.
