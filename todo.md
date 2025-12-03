# Homelab Project TODO

This file tracks the foundational rebuild of the homelab environment. The current setup is insecure and inefficient. All items on this list are mandatory before proceeding to new projects.

## Phase 1: Secure the Foundation

- [ ] **Secure SSH Access:**
  - [ ] Generate a new SSH key pair on your client machine.
  - [ ] Add the public key to the `authorized_keys` file on your server.
  - [ ] **Crucially:** Disable password-based SSH authentication entirely.
- [ ] **Plan OS Migration:**
  - [ ] Formulate a detailed plan to migrate from Ubuntu Desktop to Ubuntu Server.
  - [ ] This plan must include data backup strategies for your existing services (Minecraft world, Jellyfin metadata, etc.).
- [ ] **Decommission Plex:**
  - [ ] Shut down the Plex service.
  - [ ] Uninstall the Plex package.
  - [ ] Remove all associated Plex data and configuration files.

## Phase 2: Rebuild and Redeploy (Future)

- [ ] Execute the OS migration to Ubuntu Server.
- [ ] Re-install and configure services (Jellyfin, Minecraft) on the new server OS.
- [ ] Implement a proper DNS solution.
- [ ] Begin development on the landing page.