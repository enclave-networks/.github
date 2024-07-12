---
name: Release Checklist
about: Track testing progress against a pre-defined checklist.
title: Release Checklist
labels: 
assignees: ''

---

# Release Checklist

- [ ] Completed Pulumi end-to-end tests successfully
- [ ] Peer-to-peer connections are established
- [ ] Relay connections are established
- [ ] Policy changes are propagated to the endpoint
- [ ] Systems can be disabled and re-enabled
- [ ] Systems can be revoked sucessfully
- [ ] Successful enrolment with general use keys
- [ ] Successful enrolment with ephemeral keys
- [ ] DNS stub resolver works

## Windows

- [ ] Responds to start, stop and run operations
- [ ] Can successfully switch between profiles
- [ ] Can be successfully upgraded from an earlier enrolled version
- [ ] Sucessfully runs the unattended installer
- [ ] Continues to operate following sleep, hibernate and resume operations on physical devices
- [ ] DNS stub resolver works

## Linux tests

- APT 
    - [ ] Runs on Ubuntu 20.04
    - [ ] Runs on Ubuntu 22.04
- RPM
    - [ ] Runs on CentOS (latest)
- [ ] Runs on arm64
- [ ] Runs on Windows ARM64
- [ ] Runs on Windows X64
- [ ] Enclave auth verb works as expected
- [ ] Can be successfully upgraded from an earlier enrolled version
- [ ] DNS stub resolver works

## MacOS

- [ ] Pkg file is successfully installed 
- [ ] Enclave auth verb works as expected
- [ ] Can be successfully upgraded from an earlier enrolled version
- [ ] DNS stub resolver works

## Docker

- [ ] Container runs on Synology NAS
- [ ] Container runs on WSL2
- [ ] Container runs on Ubuntu 22.04
- [ ] Can be successfully upgraded from an earlier enrolled version

# Key Feature Testing

- [ ] Test DNS automatic name registration

- [ ] Test performance to Azure Files and as an Internet Gateway (capture before and after). Benchmark on a `D2_v3`

- [ ] Verify serial number information is stored in the platform database

## Enclave Gateway

- [ ] Test Gateway DNS is forwarding and answering 
- Test Gateway priority
      - [ ] Preferred
      - [ ] Geographic
      - [ ] Ordered
      - [ ] Check that system gateway preferences take effect immediately
      - [ ] Check that policy re-ordering takes effect immediately
      - [ ] Check that gateways are correctly chosen by geography

## Authentication Providers

- [ ] Microsoft
- [ ] OIDC

## Autentication

### Windows

- [ ] Log in button appears when a single trust requirement is added.
- [ ] Log in button disappears when all trust requirements are removed.
- [ ] Log in button works.
- [ ] Log out button works.
- [ ] Scheduler automatically logs in again when restarting the tray after an access token expires
- [ ] Scheduler automatically logs in again after restarting the fabric.
- [ ] Scheduler automatically logs in again after switching profiles.
- [ ] Ending an RDP session automatically logs out.
- [ ] Failing a user authentication trust requirement when the scheduler is "slow-ticking" and the tray is minimised raises a notification immediately
- [ ] Scheduler refreshes when an access token expires.
- [ ] On physical laptop: locking the laptop screen *does not* log you out.
- [ ] On physical laptop: logging out *does* log you out. Note: currently broken in latest GA: #795 
- [ ] On physical laptop, unplugged: after coming out of sleep, laptop refreshes access token (if necessary)
- [ ] Removing a trust requirement should not discard the token.
- [ ] When authority/tenant ID on policy changes, silent login attempted with new authority, followed by presenting login button if necessary.

### iOS

- [ ] Log in button appears when a single trust requirement is added.
- [ ] Log in button disappears when all trust requirements are removed.
- [ ] Log in button works.
- [ ] Log out button works.
- [ ] Scheduler automatically logs in again after starting the app.
- [ ] Scheduler automatically logs in again when starting the VPN extension without the app.
- [ ] Failing a user authentication trust requirement when the scheduler is "slow-ticking" and the app is closed raises a notification immediately
- [ ] Clicking an authentication notification redirects to the app.
- [ ] Scheduler automatically logs in again after restarting the fabric.
- [ ] Scheduler logs in again after access token expires while the internet is disconnected.
- [ ] Scheduler refreshes when an access token expires (with the UI closed).
- [ ] Removing a trust requirement should not discard the token.
- [ ] Permission to display notifications is requested upon enrolment.
- [ ] When authority/tenant ID on policy changes, silent login attempted with new authority, followed by presenting login button if necessary.

### Android

- [ ] Log in button appears when a single trust requirement is added.
- [ ] Log in button disappears when all trust requirements are removed.
- [ ] Log in button works.
- [ ] Log out button works.
- [ ] Scheduler automatically logs in again after starting the app.
- [ ] Failing a user authentication trust requirement when the scheduler is "slow-ticking" and the app is closed raises a notification immediately
- [ ] Clicking an authentication notification redirects to the app.
- [ ] Scheduler automatically logs in again after restarting the fabric.
- [ ] Scheduler logs in again after access token expires while the internet is disconnected.
- [ ] Scheduler refreshes when an access token expires (with the UI closed).
- [ ] Removing a trust requirement should not discard the token.
- [ ] When authority/tenant ID on policy changes, silent login attempted with new authority, followed by presenting login button if necessary.
