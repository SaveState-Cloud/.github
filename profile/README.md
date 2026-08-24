<p align="center">
  <a href="https://savestate.dk/" aria-label="SaveState Backup website">
    <img src="https://savestate.dk/favicon-192.png" width="96" height="96" alt="SaveState logo">
  </a>
</p>

# SaveState

[SaveState](https://savestate.dk/) is an automated, encrypted cloud backup service for Windows systems, servers, application data, and important files.

The SaveState Vault desktop agent creates scheduled, versioned backups, encrypts data before upload, and stores the encrypted repository in EU-resident cloud storage. Compression and deduplication reduce the physical storage used, while uploads, restores, and encrypted repository traffic are included without a paid transfer overage.

## Official links

- [SaveState website](https://savestate.dk/)
- [Features and pricing](https://savestate.dk/#pricing)
- [Download SaveState Vault for Windows](https://api.savestate.dk/download/windows)
- [Backup and restore support](https://savestate.dk/support)
- [About SaveState](https://savestate.dk/about)

## Open-source desktop client

The customer-side Windows application is available in [`savestate-desktop`](https://github.com/SaveState-Cloud/savestate-desktop). It contains the Tauri desktop shell, scheduling and profile management, client-side key handling, the Kopia integration, and the authenticated public API client.

The hosted API, operator Engine, storage infrastructure, billing systems, and private partner tooling are maintained separately.

Security issues affecting the public desktop client should be reported through the private process described in its [`SECURITY.md`](https://github.com/SaveState-Cloud/savestate-desktop/blob/main/SECURITY.md), not through a public issue.
