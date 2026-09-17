# TQK Local Server

**A local PHP/Laravel/WordPress server that actually gets out of your way.**

Extract, double-click, start building. PHP, MySQL, Apache and Nginx are
already inside the download — no installer, no "please restart your
computer," no fighting with `php.ini` in Notepad at midnight.

Free. Portable. Nothing installed outside its own folder — delete the
folder and your machine is exactly like it never existed.

## Why people switch to it

- **Multiple PHP versions, side by side** — pick one per project instead
  of switching PHP globally and hoping nothing else on your machine
  breaks.
- **Multiple MySQL/MariaDB versions, side by side** — same idea, each
  version keeps its own data, switch freely.
- **One-click WordPress, Laravel and plain PHP projects** — domain,
  database and PHP version wired up automatically, no manual vhost
  editing.
- **Real SSL on localhost** — a trusted local CA gets installed for you,
  so every project gets working HTTPS instead of a red "Not Secure"
  warning.
- **A database workflow that doesn't route through phpMyAdmin for
  everything** — dump any database to a plain, portable `.sql.gz` with
  the real `mysqldump`, restore or import with one click, watch live
  progress on large files instead of wondering if it's frozen.
- **Xdebug that just works** — installed and matched to the exact PHP
  build running, because a mismatched Xdebug DLL fails silently and
  wastes an afternoon.
- **A disposable local SSH box** — spin up an isolated Ubuntu server
  inside WSL whenever something you're building needs a real SSH target,
  gone when you don't.
- **Mail that never leaves your machine** — everything sent by
  WordPress, Laravel or PHP's `mail()` lands in a built-in inbox you can
  actually read.
- English and Vietnamese UI, switchable instantly.

## Download

**[Get the latest release →](../../releases/latest)**

`TQKServer.zip` — about 360 MB. Already contains PHP, MySQL, Apache,
Nginx, phpMyAdmin and Memcached. Nothing else to install first.

## Getting started

1. Extract the zip anywhere — an external drive works fine, the app is
   fully portable. Keep `TQKServer.exe` and the `bin/` folder next to each
   other.
2. Run `TQKServer.exe`.
3. Create your first project from the Overview page.

That's the whole setup. The app only reaches out to the internet for
things it doesn't already ship with — extra PHP/MySQL versions, Xdebug,
Redis, Composer packages, the WSL SSH box — and only when you actually ask
for them.

Everything the app writes — projects, databases, SQL dumps and backups,
logs, local SSL certs — stays inside that same folder. Nothing touches
your user profile or the Windows registry. Delete the folder and it's
gone, no trace.

## What's next

See [ROADMAP.md](ROADMAP.md) — pushing projects straight to a real server
over SSH or a hosting panel's API, no manual SFTP required.

## TQK Multisite

Outgrown a single local server? If you're operating many independent
WordPress sites for real customers — separate databases, staff accounts,
backups, plugin/theme governance, one dashboard for all of it — the
companion paid product **TQK Multisite** is built exactly for that, and
TQK Local Server can optionally host it. Separate product, separate
license, nothing bundled here.

## Support this project

TQK Local Server is free, and stays free. If it saved you real time and
you'd like to say thanks:

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
