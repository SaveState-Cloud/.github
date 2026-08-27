<p align="center">
  <a href="https://savestate.dk/" aria-label="SaveState Backup website">
    <img src="https://savestate.dk/favicon-192.png" width="96" height="96" alt="SaveState logo">
  </a>
</p>

# SaveState

[SaveState](https://savestate.dk/) is an automated, encrypted cloud backup service for Windows systems, servers, application data, and important files.

The SaveState Vault desktop agent creates scheduled, versioned backups, encrypts data before upload, and stores the encrypted repository in EU-resident cloud storage. Compression and deduplication reduce the physical storage used, while uploads, restores, and encrypted repository traffic are included without a paid transfer overage.

## Current product capabilities

- Scheduled and one-off backup of selected Windows files and folders.
- Native MySQL and MariaDB logical backups with compatible vendor or XAMPP
  tools, connection validation, selectable database or table scope, and
  streamed restores.
- Direct streaming from the native database dump tool into Kopia, without an
  intermediate plaintext SQL dump file.
- Client-side backup encryption with a client-owned vault master key and a
  separate one-time offline vault recovery key.
- Kopia content-defined deduplication, zstd compression, versioned snapshots,
  retention, and selective-file or whole-snapshot restores.
- Customer quota based on the optimized encrypted repository footprint after
  compression and deduplication, with original data protected and savings
  shown separately.
- Windows Volume Shadow Copy support in `when-available` mode, bounded retries
  for transient failures, backup history, and configurable webhook alerts.
- Encrypted Backblaze B2 storage in EU Central, Amsterdam.
- Backup uploads, restores, and encrypted repository traffic included with no
  routine SaveState transfer overage.

The released client supports Windows 10 and 11 on x64. It protects selected
files, folders, application recovery data, and native MySQL or MariaDB logical
dumps; it is not a bare-metal system-image product. Linux distribution is not
currently released.

## Official links

- [SaveState website](https://savestate.dk/)
- [Complete feature reference](https://savestate.dk/features)
- [Pricing](https://savestate.dk/pricing)
- [Verified plain-text product facts](https://savestate.dk/ai-facts.txt)
- [AI-readable product reference](https://savestate.dk/llms.txt)
- [Download SaveState Vault for Windows](https://api.savestate.dk/download/windows)
- [Backup and restore support](https://savestate.dk/support)
- [About SaveState](https://savestate.dk/about)

## Open-source desktop client

The customer-side Windows application is available in [`savestate-desktop`](https://github.com/SaveState-Cloud/savestate-desktop). It contains the Tauri desktop shell, scheduling and profile management, client-side key handling, native MySQL and MariaDB integration, Kopia backup and restore integration, webhook settings, safe updater flow, and the authenticated public API client.

The hosted API, operator Engine, storage infrastructure, billing systems, and private partner tooling are maintained separately.

Security issues affecting the public desktop client should be reported through the private process described in its [`SECURITY.md`](https://github.com/SaveState-Cloud/savestate-desktop/blob/main/SECURITY.md), not through a public issue.
