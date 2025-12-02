# Project Overview

This is a homelab project focused on building a secure, efficient, and well-managed personal server environment. The immediate goal is to consolidate services, improve security, and establish a solid foundation for future projects.

The primary services currently in scope are:
- Jellyfin (chosen as the primary media server)
- Minecraft Server
- A future landing page and DNS service.

This project is being developed within the IDX environment, with progress and action items tracked in the `todo.md` file.

# Current Status and Immediate Priorities

The project is undergoing a foundational review and rebuild. The current homelab server is running on Ubuntu Desktop, which is not ideal. The access is secured with a password, which is a major security risk.

The following are the highest priorities:

1.  **Secure SSH Access:** The immediate and most critical task is to switch from password-based SSH authentication to SSH key-based authentication. This is a non-negotiable step to secure the server.
2.  **OS Migration:** The long-term plan is to migrate the server from Ubuntu Desktop to Ubuntu Server. This will provide a more stable, secure, and efficient base for the homelab. A detailed plan for this migration is outlined in the `todo.md` file.
3.  **Service Consolidation:** Plex will be decommissioned in favor of Jellyfin to reduce redundancy and simplify the setup.

# Development Plan

All development tasks and action items are tracked in the `todo.md` file. This file serves as the single source of truth for the project's direction and progress.

# Building and Running

There are currently no build or run commands defined for the landing page project. The `.idx/dev.nix` file is set up for a development environment, but the specific packages for languages and frameworks (e.g., Node.js, Python) are not yet enabled.

**TODO:** To start development on the landing page, you will need to:

1.  Uncomment and add the necessary packages in `.idx/dev.nix`.
2.  Define a `start` command in the `idx.workspace.onStart` or `idx.previews` section of `.idx/dev.nix`.
3.  Create the necessary source code files.

# Development Conventions

There are no established development conventions at this time. As the project evolves, it will be important to establish a consistent coding style, testing strategy, and contribution process. The `Guidelines.md` file can be used to document these conventions.
