# TQK Local Server

A free, portable local development server for Windows — PHP, Laravel and
WordPress, running as a proper desktop app instead of a browser tab full of
config files.

Think Laragon/XAMPP, but with multiple PHP *and* MySQL/MariaDB versions
side by side, one-click WordPress installs, a disposable local SSH box for
testing, and a database/backup workflow that doesn't require phpMyAdmin for
every little thing.

## Download

Grab the latest `TQKServer.zip` from the [Releases](../../releases) page
(~1.6 GB — it ships with PHP, MySQL, Apache, Nginx, phpMyAdmin and Memcached
already inside, so it works the moment you extract it, no extra downloads).

No installer, no setup wizard.

## Getting started

1. Extract the zip anywhere (an external drive works fine — the app is
   fully portable). Keep `TQKServer.exe` and the `bin/` folder next to each
   other; they need to stay together.
2. Run `TQKServer.exe`.
3. That's it — PHP, MySQL/MariaDB, Apache/Nginx and phpMyAdmin are already
   there. The app only reaches out to the internet for things that aren't
   bundled: extra PHP/MySQL versions, Xdebug, Redis, Composer packages,
   the WSL SSH test box, and so on — all optional, all on demand.

Everything the app writes — sites, databases, SQL dumps and backups, logs,
local SSL certs — stays inside that same folder. Nothing touches your user
profile or the Windows registry. Delete the folder and it's gone.

## Features

### Projects
One-click create or import PHP, Laravel and WordPress projects. Each one
gets its own domain, database and PHP version automatically — no manual
vhost editing.

### Multiple PHP versions, side by side
Install as many PHP versions as you need and pick one per project — no
more "switch PHP globally and hope nothing else breaks." Per version: turn
extensions on/off, toggle OPcache, and enable Xdebug with one click (it's
downloaded and matched to that exact PHP build automatically, since a
wrong Xdebug DLL just silently fails to load).

### Multiple MySQL/MariaDB versions, side by side
Same idea as PHP: install several database server versions and switch
which one is active — each version keeps its own data folder, so nothing
gets mixed up or lost when you switch back and forth.

### SQL Dumps, backup & restore
- **SQL Dumps** — dump any database to a plain, portable `.sql.gz` with
  the real `mysqldump`, right from the Overview page (not TQK Server's own
  format) — hand it to any DBA or MySQL tool.
- **App backups** — back up a whole project (code + database) to one zip
  in a single click.
- **Restore & import** — restore any backup with one click, or import any
  `.sql`/`.sql.gz` file already on your disk into a chosen database.
- Everything runs as a background job with live byte-level progress, so
  large databases don't leave you guessing whether it's stuck.
- phpMyAdmin is one click away too (installed on demand).

### Local SSH test box
Spin up a disposable Ubuntu server inside WSL, purely on your own machine,
to test anything that needs a real SSH target — deploy scripts, remote
backup/pull tooling, whatever you're building. Fully isolated from your
real machine; regenerate its key any time.

### Domains & SSL that just work
Local `.test` domains (or your own TLD) with a trusted local CA installed
automatically, so every project gets working HTTPS with no browser
warnings — no more clicking through "Not Secure" on localhost.

### Web server & mail, your choice
Switch between Apache (full `.htaccess` support) and Nginx (fastest for
WordPress) — only one runs at a time, and there's a one-click config test
before you commit to it. A built-in mail catcher grabs everything sent by
WordPress, Laravel or plain PHP `mail()` so you can read it in the app —
nothing ever actually leaves your computer.

### Extras
Optional Redis, Memcached and a portable Git, installed on demand when a
project needs them.

### Bilingual
English and Vietnamese UI, switchable instantly, no reload.

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
