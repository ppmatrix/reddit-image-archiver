# Reddit Image Archiver

A local, non-commercial Python application for organizing and
archiving publicly accessible images from selected Reddit communities.

## Project status

Early development (F0 — project setup).

Reddit API access has not yet been approved.
No Reddit data collection functionality is currently implemented.

## Objectives

- Support multiple user-selected subreddits.
- Discover accessible image posts and Reddit galleries.
- Download images where authorized and permitted.
- Organize images by subreddit and publication year.
- Store post metadata in a local SQLite database.
- Detect duplicate images using SHA-256.
- Support interrupted download recovery.
- Generate archive and download reports.
- Retrieve historical posts within authorized API limits.

## Initial target

r/FoundPhotos

Additional subreddits may be configured in future versions.

## Technology

- Python 3.12+
- PRAW (Reddit API)
- requests
- Pillow
- SQLite
- python-dotenv
- Ubuntu 24.04 / WSL

## Planned architecture

- Reddit API client
- Post discovery
- Image and gallery downloader
- Metadata persistence
- Duplicate detection
- Logging and reporting

## API access and compliance

This project requires authorized Reddit API access.

The application is intended for personal, non-commercial use.
It will operate in read-only mode and respect applicable API
rate limits, content restrictions, deletion requirements,
and Reddit's Developer Terms and Data API Terms.

Historical retrieval is limited to content available through
authorized interfaces. Complete subreddit coverage is not guaranteed.

Images and metadata are stored locally and are not included
in this source repository.

## Security

Credentials are stored locally in a .env file.
Secrets, downloaded media, databases, and logs are excluded
from version control.

## License

No software license has been selected yet.
Third-party content remains subject to its respective rights.
