# Homelab Setup TODO

This document outlines the critical next steps for your homelab setup. We will mark items as completed as we progress.

## Immediate Security Fixes

- [ ] **Secure SSH Access:** Implement SSH key-based authentication and disable password-based login. This is the highest priority.
    - [ ] Generate SSH key pair on your local machine.
    - [ ] Copy public key to the Ubuntu server.
    - [ ] Disable password authentication in `/etc/ssh/sshd_config`.

## Homelab Optimization

- [x] **Commit to Jellyfin and remove Plex.**
- [ ] **Migrate from Ubuntu Desktop to Ubuntu Server:**
    - [ ] **Inventory and Backup:**
        - [ ] Make a complete list of all running services.
        - [ ] Back up all configuration files (e.g., from `/etc`).
        - [ ] Back up all service data (media, databases, etc.).
        - [ ] Verify backups.
    - [ ] **Wipe and Reinstall:**
        - [ ] Wipe the current OS.
        - [ ] Install a fresh, minimal version of Ubuntu Server.
    - [ ] **Restore and Reconfigure:**
        - [ ] Reinstall services from the command line.
        - [ ] Restore configuration files.
        - [ ] Restore data.

## Future Enhancements

- [ ] **Set up DNS:** Correctly configure your DNS service.
- [ ] **Develop Landing Page:** Implement a landing page for your homelab services.
