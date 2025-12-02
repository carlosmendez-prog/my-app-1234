# Project Overview

This is a homelab dashboard project, intended to provide a central interface for managing and accessing services on a personal server. The project is in its early stages and is configured to be developed within the IDX environment.

The `README.md` file lists the following services to be included in the dashboard:
- Jellyfin
- Plex
- Minecraft Server Status
- Minecraft Server

# Building and Running

There are currently no build or run commands defined for this project. The `.idx/dev.nix` file is set up for a development environment, but the specific packages for languages and frameworks (e.g., Node.js, Python) are not yet enabled.

**TODO:** To start development, you will need to:

1.  Uncomment and add the necessary packages in `.idx/dev.nix`. For example, for a web-based dashboard, you might uncomment `pkgs.nodejs_20`.
2.  Define a `start` command in the `idx.workspace.onStart` or `idx.previews` section of `.idx/dev.nix` to run your application. For example:
    ```nix
    previews = {
      enable = true;
      previews = {
        web = {
          command = ["npm" "run" "dev"];
          manager = "web";
          env = {
            PORT = "$PORT";
          };
        };
      };
    };
    ```
3.  Create the necessary source code files (e.g., `index.html`, `app.js`).

# Development Conventions

There are no established development conventions at this time. As the project evolves, it will be important to establish a consistent coding style, testing strategy, and contribution process. The `Guidelines.md` file can be used to document these conventions.
