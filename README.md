<h1 align="center">Dikshant Chandel</h1>

<p align="center">
  Software Engineer and Security Researcher<br>
  I write Rust that holds up, and I break software that doesn't<br>
  Founder of <a href="https://clickswave.org">Clickswave</a>. Web apps, binaries, reverse engineering.
</p>

<p align="center">
  <a href="https://www.rust-lang.org/"><img alt="Rust" src="https://img.shields.io/badge/Rust-DEA584?style=for-the-badge&logo=rust&logoColor=black"></a>
  <a href="https://svelte.dev/docs/kit"><img alt="SvelteKit" src="https://img.shields.io/badge/SvelteKit-FF3E00?style=for-the-badge&logo=svelte&logoColor=white"></a>
  <a href="https://www.postgresql.org/"><img alt="Postgres" src="https://img.shields.io/badge/Postgres-336791?style=for-the-badge&logo=postgresql&logoColor=white"></a>
</p>

---

### Products

**[Crossfyre](https://crossfyre.io)** runs recon and vulnerability workflows across a fleet of nodes in parallel. Pure Rust, no Python glue.

**[SiloCat](https://silo.cat)** encrypts files in the browser. The server only ever holds ciphertext, so there is nothing useful to leak.

### Open source

| | |
|---|---|
| **[crossfyre-toolchain](https://github.com/clickswave/crossfyre-toolchain)** | The scanners on their own, in your terminal. It ate voyage and mach. Apache-2.0. |
| **[silocat](https://github.com/clickswave/silocat)** | silo.cat's source, so you don't have to take my word about the encryption. AGPL-3.0. |
| **[limeyard](https://github.com/clickswave/limeyard)** | Deliberately vulnerable targets with an answer key, for finding out how bad your scanner really is. MIT. |

### Bugs

I find them in other people's software and report them privately. They get listed here once the vendors ship fixes, which takes however long it takes.

| | |
|---|---|
| **[CVE-2026-104626](https://www.cve.org/CVERecord?id=CVE-2026-104626)** | Gitea, Critical 9.0. Cancel your own fork PR run, wait for a maintainer to click Re-run, and the fork's workflow runs on their runners as root without ever being approved. Five of us found it independently. |
| **[CVE-2026-104633](https://www.cve.org/CVERecord?id=CVE-2026-104633)** | Gitea, Medium 6.5. A migration source reporting a page size of zero sent six download loops round forever. One request took a server from 99MiB to 5.7GB in ninety seconds. |
| **[CVE-2026-109310](https://www.cve.org/CVERecord?id=CVE-2026-109310)** | SiYuan, Medium 6.5. One GET to the dynamic icon endpoint ran an uncapped template function until the kernel was OOM-killed. No login needed on a default publish service. |
| **[CVE-2026-117677](https://www.cve.org/CVERecord?id=CVE-2026-117677)** | Gitea, Medium. A Helm chart upload was decompressed and read to the end before the size quota was checked, so a 1MB chart took a server from 105MiB to over 5GB of memory in 17.5 seconds. Shared with two other reporters. |
| **[CVE-2026-105661](https://www.cve.org/CVERecord?id=CVE-2026-105661)** | Gitea, Medium 5.3. Every anonymous request for an ordinary user's organisation repositories page panicked and wrote a stack trace to the log. Shared with two other reporters. |
| **[GHSA-4p83-c4wg-59q4](https://github.com/opf/openproject/security/advisories/GHSA-4p83-c4wg-59q4)** | OpenProject, Medium 4.3. A cache shared between viewers served the first one's permissions to everyone after, so the meeting agenda API leaked private work package subjects. No CVE. |

The ones still with maintainers are counted at [crossfyre.io/disclosures](https://crossfyre.io/disclosures).

---

<p align="center">
  <a href="https://linkedin.com/in/kewmine"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0id2hpdGUiPjxwYXRoIGQ9Ik0yMC40NDcgMjAuNDUyaC0zLjU1NHYtNS41NjljMC0xLjMyOC0uMDI3LTMuMDM3LTEuODUyLTMuMDM3LTEuODUzIDAtMi4xMzYgMS40NDUtMi4xMzYgMi45Mzl2NS42NjdIOS4zNTFWOWgzLjQxNHYxLjU2MWguMDQ2Yy40NzctLjkgMS42MzctMS44NSAzLjM3LTEuODUgMy42MDEgMCA0LjI2NyAyLjM3IDQuMjY3IDUuNDU1djYuMjg2ek01LjMzNyA3LjQzM2MtMS4xNDQgMC0yLjA2My0uOTI2LTIuMDYzLTIuMDY1IDAtMS4xMzguOTItMi4wNjMgMi4wNjMtMi4wNjMgMS4xNCAwIDIuMDY0LjkyNSAyLjA2NCAyLjA2MyAwIDEuMTM5LS45MjUgMi4wNjUtMi4wNjQgMi4wNjV6bTEuNzgyIDEzLjAxOUgzLjU1NVY5aDMuNTY0djExLjQ1MnpNMjIuMjI1IDBIMS43NzFDLjc5MiAwIDAgLjc3NCAwIDEuNzI5djIwLjU0MkMwIDIzLjIyNy43OTIgMjQgMS43NzEgMjRoMjAuNDUxQzIzLjIgMjQgMjQgMjMuMjI3IDI0IDIyLjI3MVYxLjcyOUMyNCAuNzc0IDIzLjIgMCAyMi4yMjUgMHoiLz48L3N2Zz4="></a>
  <a href="https://app.hackthebox.com/public/users/200315"><img alt="Hack The Box" src="https://img.shields.io/badge/Hack%20The%20Box-9FEF00?style=for-the-badge&logo=hackthebox&logoColor=black"></a>
</p>

<p align="center">
  Contract work and collaborations: <a href="mailto:team@clickswave.org">team@clickswave.org</a>
</p>
