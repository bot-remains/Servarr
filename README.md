# Servarr

This Docker Compose configuration sets up a comprehensive media management system. Below is an overview of each service included in the configuration along with the ports they use and a brief description.

## Services

| Service      | Ports                | Description                                                  |
|--------------|----------------------|--------------------------------------------------------------|
| qbittorrent  | 8080, 6881 (TCP/UDP) | A powerful, open-source BitTorrent client.                   |
| radarr       | 7878                 | A movie collection manager for Usenet and BitTorrent users.  |
| sonarr       | 8989                 | A TV series collection manager for Usenet and BitTorrent users. |
| lidarr       | 8686                 | A music collection manager for Usenet and BitTorrent users.  |
| readarr      | 8787                 | A book collection manager for Usenet and BitTorrent users.   |
| whisparr     | 6969                 | A software solution for managing adult content.              |
| bazarr       | 6767                 | A companion app to Sonarr and Radarr to manage subtitles.    |
| prowlarr     | 9696                 | An indexer manager/proxy for *arr apps.                      |
| overseerr    | 5055                 | A request management and media discovery tool for Plex.      |
| notifiarr    | 5454                 | A notification tool that integrates with *arr apps and Plex. |
| flaresolverr | 8191                 | A proxy server to bypass Cloudflare protection.              |
| tor-privoxy  | 9050, 9051, 8118     | Tor and Privoxy to enable anonymous browsing and connections.|

## Getting Started

### Prerequisites

- Docker installed on your machine.
- Docker Compose installed on your machine.

### Setup

1. **Clone the repository** (if applicable) or create a `docker-compose.yml` file with the provided configuration.

2. **Adjust file paths**: Update the volume paths to your preferred directories. Replace `Path/for/config`, `Path/for/completed/downloads`, etc., with actual paths on your machine.

3. **Run Docker Compose**: Navigate to the directory containing your `docker-compose.yml` file and run the following command:

   ```bash
   docker-compose up -d
