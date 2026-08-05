# UniFi Network App Categories

Searchable reference of every application and category recognized by UniFi Network for traffic identification and traffic rules.

**[View the live reference &#8594;](https://ozark-connect.github.io/unifi-network-app-categories/)**

## What is this?

When you create Traffic Rules in UniFi Network to block, allow, or rate-limit traffic by category (like "Online Games" or "Social Networking"), these are the specific apps included. Data is extracted from the UniFi Network web app code and updates with new releases.

## Current Data

- **UniFi Network**: 10.6.88
- **DPI Signatures**: v2.128
- **Categories**: 35
- **Applications**: 2109
- **Last Updated**: 2026-08-05

## One App, One Category

Each application is mapped to exactly one category. Some apps may appear in broader categories than you'd expect - for example, several well-known adult sites are under "Media streaming services" rather than "Adult", and AI chatbots like ChatGPT appear under "TopSites-Adult". Review the specific apps in each category before creating traffic rules.

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

## A Note on App IDs

UniFi uses compound IDs that encode the category: `compound_id = (category_id << 16) + app_id`. This site maps apps to categories using the explicit `category_id` declared in the web app code, not the encoded ID. In practice they almost always agree - we found one exception out of 2109 apps.

## Contributing

Found an issue? [Open an issue](https://github.com/Ozark-Connect/unifi-network-app-categories/issues) or submit a pull request.
