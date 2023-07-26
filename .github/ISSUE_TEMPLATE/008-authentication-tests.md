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
