# Homelab Setup TODO

This document outlines the critical next steps for your homelab setup. We will mark items as completed as we progress.

## Immediate Security Fixes

- [ ] **Secure SSH Access:** Implement SSH key-based authentication and disable password-based login. This is the highest priority.
    - [ ] Generate SSH key pair on your local machine.
    - [ ] Copy public key to the Ubuntu server.
    - [ ] Disable password authentication in `/etc/ssh/sshd_config`.

## Homelab Optimization

- [ ] **Review Service Redundancy:** Choose between Jellyfin and Plex, and remove the other.
- [ ] **Consider OS Migration:** Plan for a migration from Ubuntu Desktop to Ubuntu Server for improved efficiency and security.

## Future Enhancements

- [ ] **Set up DNS:** Correctly configure your DNS service.
- [ ] **Develop Landing Page:** Implement a landing page for your homelab services.
