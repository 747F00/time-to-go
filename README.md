# time-to-go

Answers one question: **"When should I leave?"**

Give it a start place, an end place, and the time you need to arrive — it works
backward to tell you the latest departure time and the public-transit route to
take.

## How it works

No database — every answer is computed live from two APIs:

- **[Kakao Local](https://developers.kakao.com/docs/latest/en/local/dev-guide)** — place name → coordinates
- **[ODsay](https://lab.odsay.com/guide/releaseReference)** — public-transit routing

Only public transit (`PUBTRANS`) is supported today; other transportation
modes exist in the API for request compatibility only.

## Repositories

This is the umbrella repo for the time-to-go project. Code lives in sibling repos:

| Repo | Stack | Status |
|---|---|---|
| [time-to-go-api](https://github.com/747F00/time-to-go-api) | Kotlin / Spring Boot | live |
| [time-to-go-web](https://github.com/747F00/time-to-go-web) | Next.js / React | live — https://time-to-go.seheon.kr |
| [time-to-go-ios](https://github.com/747F00/time-to-go-ios) | Swift | scaffold only |

## Docs

- [Personas](docs/personas.md)

## License

[MIT](LICENSE)
