# GovTrack

GovTrack is a free, open-access platform for tracking the United States Congress. It has provided legislative transparency data since 2004, serving millions of users including journalists, legislative professionals, educators, and the general public. GovTrack is operated by Civic Impulse, LLC and maintained by Joshua Tauberer.

## API

GovTrack exposes a read-only REST API at `https://www.govtrack.us/api/v2/` powered by django-simplegetapi. No authentication or API key is required.

**Base URL:** `https://www.govtrack.us/api/v2/`

**Available Endpoints:**

| Endpoint | Description |
|---|---|
| `/api/v2/bill` | Bills and resolutions |
| `/api/v2/vote` | Roll call votes |
| `/api/v2/vote_voter` | Individual voting records |
| `/api/v2/person` | Members of Congress |
| `/api/v2/role` | Congressional roles (senator, representative) |
| `/api/v2/committee` | Congressional committees |
| `/api/v2/committee_member` | Committee membership |
| `/api/v2/cosponsorship` | Bill cosponsorship records |

**Response Formats:** JSON, JSONP, CSV, XML

**Example:**
```
GET https://www.govtrack.us/api/v2/bill?congress=119&limit=20
GET https://www.govtrack.us/api/v2/person?lastname=Smith
GET https://www.govtrack.us/api/v2/vote?congress=119&limit=20
```

## Data

GovTrack data covers U.S. Congress legislative activities from 1789 to the present, including:

- Bill and resolution status and full text
- Roll call votes on legislation and procedural motions
- Member of Congress profiles, voting records, and attendance
- Congressional committee membership
- Cosponsorship relationships between legislators

For bulk data needs, GovTrack recommends using the [unitedstates/congress](https://github.com/unitedstates/congress) open-source scrapers.

## Links

- **Website:** https://www.govtrack.us
- **API Docs:** https://www.govtrack.us/developers/api
- **Blog:** https://www.govtrack.us/blog/
- **GitHub:** https://github.com/govtrack
- **LinkedIn:** https://www.linkedin.com/company/govtrack
- **X (Twitter):** https://x.com/govtrack
- **Contact:** hello@govtrack.us

## APIs.json

This repository contains an [APIs.json 0.19](https://apisjson.org/) profile for GovTrack maintained by the [API Evangelist](https://apievangelist.com) project.
