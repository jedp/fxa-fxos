# Firefox Accounts
## on FirefoxOS First-Time Use

we've got two things to talk about
firefox accounts on firefoxos NOW
and firefox accounts on the firefox platform in the future

we're trying hard to land for 1.3
we're thinking hard about 1.4 and beyond

## What is Firefox Accounts

Firefox Accounts is a system that gives you a single way to sign into all
Mozilla services on Firefox and FirefoxOS.

- Tracking Bug: 920135 
- For 1.3: Sign-in, sign-out (Marketplace, WheresMyFox)
- For 1.4: Attached services (Sync)

## What Will The User See?

- UX for flows: Bug 897600 (attachment)
- FTE flow: https://www.youtube.com/watch?v=ZjSUN7SAEmw

## Some Questions You Might Have

- Do I have to create a Firefox Account to use Firefox?
- How do I sign up or sign in?
- Why not Persona? What' the difference?
- Can I use Persona to sign in?
- Are we creating another silo?
- What information will it store about the user?
- Can I put my application or service's data in Firefox Accounts?
- Can I use it to sign into non-Mozilla services?
- Does it provide email?
- What services will it enable?

crazy ideas for the future: https://wiki.mozilla.org/User:Dria/PiCL_Future_Ideas

## Current Status, Future Plans

For 1.3, we are targeting:
- DOM API for sign-in

    navigator.id.watch({wantIssuer: "firefox-accounts"});
    navigator.id.request();

- IAC API for certified apps (FTE, Settings)

For 1.4 and beyond:

- a way for third-party services to participate (e.g., contacts sync service)
- a way for third-party non-certified apps to participate (sign-in request)

## When Is This Happening
 
- version 1.3 of fxos for accounts sign-in (wmf, mkt)
- version 1.4 for deeper features (sync, keys, etc)

## Architectural Overview

- Tracking bug: 
- img/architecture.png

## How Do I Use It?

The DOM API is the same as for persona

for sign-in, it's the browserid (persona) protocol
with one additon:

    nav.id.watch({wantIssuer: "firefox-accounts"});
    nav.id.request()

? how do i logout?


## Where Can I Learn More

FAQ
Wiki

