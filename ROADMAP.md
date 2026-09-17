# Roadmap

What's planned next for TQK Local Server. Nothing here is built yet — this
is a plan, not a promise of a date.

## Remote server automation

Right now, moving a project from your local machine to a real server is a
manual step: open an SFTP client, drag the files across, done by hand.

The plan is to bring that inside TQK Local Server itself, so "push this up
to the server" becomes one click instead of a separate manual upload:

- **SSH** — connect to any plain Linux server and push files, create the
  remote database, and deploy directly, no control panel required.
- **cPanel** — talk to cPanel's own API to create the database and set up
  the domain (parked/addon domain), then push the files over.
- **OnePanel** — same idea, via OnePanel's API.
- **Cloud storage** — push a zipped export straight to Google Drive or
  Dropbox, and pull one back down the same way, for teams that hand off
  projects that way instead of straight server-to-server.

The underlying zip/export step already exists (Databases → SQL Dumps,
Apps → Backup) — this is about what happens *after* the zip: where it
goes, and how it gets there without you doing it by hand.

Have a specific panel or workflow you'd want supported first? Open an
issue, or reach out directly — see the [README](README.md) for contact
details.
