# Was the Bus On Time? Statistics

On-time performance statistics for Intercity Transit buses (Olympia, Washington), computed from the agency's public real-time data by [Was the Bus On Time?](https://wasthebusontime.com), an **unofficial**, open-source project.

> **This project is not affiliated with, endorsed by, or associated with Intercity Transit in any way.**

This repository holds the numbers the website publishes. It is updated automatically, so its history is a public record of every published figure, corrections included. The code that collects the data and computes these statistics lives in [wasthebusontime/wasthebusontime](https://github.com/wasthebusontime/wasthebusontime).

## Status
Empty for now. Real-time data has been collected since October 4, 2026. Statistics will appear here once the processing pipeline is running. The file layout below may change before then.

## What's here (planned)
| Path | Contents |
|---|---|
| `site/` | Precomputed JSON files the website loads (system, route, and stop pages) |
| `csv/` | Aggregate statistics as CSV, for anyone to download and reuse |

These are **aggregates**: counts of departures that were early, on time, or late, and how late, by route, stop, time of day, day of week, and date. This repository contains no raw feed data and no per-trip records.

## How "on time" is measured
In brief:
- **On time** follows Intercity Transit's own published standard. A bus is on time if it leaves a timepoint no earlier than scheduled and no more than 5 minutes late.
- A second, clearly labeled figure uses a more common window: up to 1 minute early to 5 minutes late.
- Actual departure times come from the agency's real-time feed, checked against vehicle GPS positions.
- Departures with missing data are excluded, never guessed, and gaps in collection are reported.

The full methodology, including its limitations, will be on the website.

## Updates
Statistics are recomputed every night, after the service day ends. A run may also revise recent days if late data arrives, and a methodology change can revise past figures. Either way the change shows up in this repository's history.

## License
The statistics in this repository are licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). Please credit **"Was the Bus On Time? (wasthebusontime.com)"** and link to the license.

## Data source and attribution
The statistics are derived from schedule and real-time data provided **"AS IS"** by Intercity Transit and used under the [Sound Transit Open Transit Data: Transit Data Terms of Use](https://www.soundtransit.org/help-contacts/business-information/open-transit-data-otd/transit-data-terms-use). Intercity Transit retains all rights to its data and trademarks. The CC BY 4.0 license above covers only the statistics computed by this project, not Intercity Transit's data.

## Corrections and contact
Found a problem? Open an issue in this repository or email contact@wasthebusontime.com.
