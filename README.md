# AniMappings

A project to scrape anime meta from lots of websites using anilist id's

## Technologies Used

- Node.js
- TypeScript
- Prisma

## Getting Started

### Prerequisites

A **Postgresql** database needs to already be setup. You can use [Neon.tech](https://neon.tech/) and [Planetscale](https://planetscale.com/) offer amazing free tiers that you can utilize

### Installation

1. Clone the repository: `git clone https://github.com/illusionTBA/AniMappings.git`
2. Install dependencies: `npm install`
3. crawl anilist to populate DB: `npm run crawl`
4. Start the server: `npm start`

## Usage

- You can export all of the DB into a json file using the `npm run export` command
- Using the webserver (`npm start`) you can request the `/anilist/id` to recieve the meta for that anime (replacing `id` with the anilist id)
- Crawling is how the database populates itself. You can use `npm run crawl` to start crawling anilist and other providers. If it crashes it will start off where it left off.

## Acknowledgements

- [Mr Ethical](https://github.com/MrEthical06) Integrated the lastId feature.
- [Eltik](https://github.com/eltik) Inspired me to do this project with his [AniSync](https://github.com/Eltik/AniSync) Project.
