# TQK Local Server

A free, portable local development server for Windows — PHP, Laravel and
WordPress, running as a proper desktop app instead of a browser tab full of
config files.

Think Laragon/XAMPP, but with one-click WordPress installs, multi-PHP
switching, real project management, and a database/backup workflow that
doesn't require phpMyAdmin for every little thing.

## Download

Grab the latest `TQKServer.exe` from the [Releases](../../releases) page.

No installer, no setup wizard — just run it.

## Getting started

1. Put `TQKServer.exe` in its own folder (an external drive works fine —
   the app is fully portable).
2. Run it.
3. The app installs the runtime pieces it needs (PHP, MySQL/MariaDB, a web
   server) on first use, straight from the Overview page.

Everything the app writes — sites, databases, SQL dumps and backups, logs,
local SSL certs — stays inside that same folder. Nothing touches your user
profile or the Windows registry. Delete the folder and it's gone.

## Features

- **Apps** — one-click create/import PHP, Laravel and WordPress projects;
  each gets its own domain, database and PHP version automatically.
- **Databases** — browse every local MySQL/MariaDB database, create/drop
  them, open phpMyAdmin (installed on demand), and:
  - **SQL Dumps** — dump any database to a plain, portable `.sql.gz` with
    the real `mysqldump`, right from the Overview page. Hand it to any DBA
    or MySQL tool — no proprietary format.
  - **Backup & restore** — back up a whole app (code + database) to one
    zip, or just a database; restore either with one click; import any
    `.sql`/`.sql.gz` file already on disk into a chosen database.
- **PHP** — switch PHP version per project, install/enable/disable
  extensions, auto-install Xdebug matched to the running PHP build.
- **Domains & SSL** — local `.test` (or your own TLD) domains with a
  trusted local CA, so every project gets working HTTPS with no browser
  warnings.
- **Web / Server** — start, stop and configure Apache/Nginx, MySQL/MariaDB
  and Mail (Mailpit) as independent services, each with its own status and
  logs.
- **Extras** — optional Redis, Memcached and a portable Git, installed on
  demand.
- English and Vietnamese UI, switchable instantly.

## TQK Multisite

If you outgrow a single local server and need to run and operate many
independent WordPress sites for real customers — separate databases, staff
accounts, backups, package/plugin governance, one dashboard — the companion
paid product **TQK Multisite** is built exactly for that, and TQK Local
Server can optionally host it. It's a separate product with its own
license.

## Support this project

TQK Local Server is free. If it saves you time and you'd like to say
thanks:

**Contact**
Trương Quang Khải
Phone: 0364 999 916
Email: roo.adm@gmail.com

**Donate**
Bank: Vietcombank
SWIFT/BIC: BFTVVNVX
Account holder: Truong Quang Khai
Account number: 0501 000 151853
Branch: Cu Chi

## License

MIT — see [LICENSE](LICENSE).
