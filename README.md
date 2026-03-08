# Unraid Templates

Unraid Docker templates for [DPB (Debrid Plex Bridge)](https://github.com/roandegraaf/DPB).

## Installation

1. In Unraid, go to **Docker** tab
2. Scroll down to **Template Repositories**
3. Add this URL: `https://github.com/roandegraaf/unraid-templates`
4. Click **Save**
5. Click **Add Container** and select **DPB** from the template dropdown

## Templates

### DPB

A single Docker container for managing Plex with Real-Debrid. Bundles Zurg, rclone, Zilean, PostgreSQL, and a web UI.

**Requirements:**
- [Real-Debrid API key](https://real-debrid.com/apitoken)
- [TMDB API key](https://www.themoviedb.org/settings/api)

**Required settings:**
| Setting | Description |
|---------|-------------|
| Config Path | App config, database, and logs (`/mnt/user/appdata/dpb`) |
| Library Path | Your Plex media library directory |
| Zurg Mount | FUSE mount point for Real-Debrid content |
| Real-Debrid API Key | Your RD API token |
| TMDB API Key | For movie/show metadata |
| NextAuth Secret | Generate with `openssl rand -base64 32` |
