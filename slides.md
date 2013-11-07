# Firefox Accounts and FirefoxOS

## Topics

- What Firefox Accounts is (and isn't)
- What we are working on for 1.3
- What we plan for the future

## What is Firefox Accounts

Firefox Accounts is a system that gives you a single way to sign into all
Mozilla services on Firefox and FirefoxOS.

- Tracking Bug: 920135 
- For 1.3: DOM API for Sign-in, sign-out (Marketplace, WheresMyFox)
- For 1.4: Attached services (Sync)

## What Will The User See?

- UX for flows: Bug 897600 (attachment)
- FTE flow: [https://www.youtube.com/watch?v=ZjSUN7SAEmw](https://www.youtube.com/watch?v=ZjSUN7SAEmw)
- More flows: [https://www.dropbox.com/s/9tfzlxpg2khgr4q/FxA%20Animation.m4v](https://www.dropbox.com/s/9tfzlxpg2khgr4q/FxA%20Animation.m4v)

## Some Questions You Might Have

- Do I have to create a Firefox Account to use Firefox?
- How do I sign up or sign in?
- Why not Persona? What's the difference?
- Can I use Persona to sign in?
- Are we creating another silo?
- What information will it store about the user?
- Can I put my application or service's data in Firefox Accounts?
- Can I use it to sign into non-Mozilla services?
- Does it provide email?
- What services will it enable?

crazy ideas for the future: https://wiki.mozilla.org/User:Dria/PiCL_Future_Ideas

## Implementation Timeline

For 1.3, we are targeting:

- DOM API for sign-in

    navigator.id.watch({wantIssuer: "firefox-accounts"});
    navigator.id.request();

- IAC API for certified apps (FTE, Settings)

For 1.4 and beyond:

- a way for third-party services to participate (e.g., contacts sync service)
- a way for third-party non-certified apps to participate (sign-in request)

## Architectural Overview

![Architecture](/Users/zeus/code/fxa-fxos/img/architecture.png "FirefoxOS Architecture")

## Where Can I Learn More

- [https://wiki.mozilla.org/Identity/Firefox-Accounts](https://wiki.mozilla.org/Identity/Firefox-Accounts)
- [https://mail.mozilla.org/listinfo/dev-fxacct](https://mail.mozilla.org/listinfo/dev-fxacct)

## People

In addition to everyone on in Identity and FirefoxOS who have helped out:

- Borja Salguero (dev)
- Fernando Moreno (dev)
- Francisco Jordano (dev)
- Jed Parsons (dev)
- John Gruen (UX)
- Olav Nymoen (dev)
- Ryan Feeley (UX)
- Sam Penrose (dev)
- Sergi Mansilla (dev)
- Shane Tomlinson (dev)
- Zach Carter (dev)

