# Main Features

- All content is file-based
- Search file names and contents
- Markdown editor in the browser
- Login system for edit protection
- Simple and Lightweight


# Environment Variables

Environment variables take the highest priority and override values set in `config/config.js`.

| Variable              | Config Key            | Type    | Description                                                                 |
| --------------------- | --------------------- | ------- | --------------------------------------------------------------------------- |
| `SESSION_SECRET`      | `session_secret`      | String  | Session signing secret. Min 32 chars. Generate: `openssl rand -base64 32`   |
| `ADMIN_USERNAME`      | `credentials[0]`      | String  | Admin username (must be set together with `ADMIN_PASSWORD`)                 |
| `ADMIN_PASSWORD`      | `credentials[0]`      | String  | Admin password (must be set together with `ADMIN_USERNAME`)                 |
| `CONTENT_DIR`         | `content_dir`         | String  | Path to content directory containing `.md` files (default: `content/pages`) |
| `BASE_URL`            | `base_url`            | String  | Base URL of the site (e.g. `https://docs.example.com`)                      |
| `SITE_TITLE`          | `site_title`          | String  | Site title shown in the browser and header                                  |
| `GOOGLE_ANALYTICS_ID` | `google_analytics_id` | String  | Google Analytics 4 measurement ID (e.g. `G-XXXXXXXXXX`)                     |
| `LOCALE`              | `locale`              | String  | Locale code for UI translations (e.g. `en`, `fr`)                           |
| `AUTHENTICATION`      | `authentication`      | Boolean | Set to `true` to enable authentication                                      |
| `ALLOW_EDITING`       | `allow_editing`       | Boolean | Set to `true` to enable the web editor                                      |
| `ADDRESS`             | _(server)_            | String  | IP address to listen on (default: `127.0.0.1`)                              |
| `PORT`                | _(server)_            | Number  | Port to listen on (default: `8080`)                                         |
| `HOST`                | _(server)_            | String  | Deprecated — use `ADDRESS` instead                                          |

