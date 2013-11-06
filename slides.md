# Firefox Accounts
## on FirefoxOS First-Time Use

we've got two things to talk about
firefox accounts on firefoxos NOW
and firefox accounts on the firefox platform in the future

we're trying hard to land for 1.3
we're thinking hard about 1.4 and beyond

## What is Firefox Accounts

Firefox Accounts is a system that gives you a single way to sign into all
Mozilla services on Firefox and FirefoxOS
- marketplace
- wheresmyfox
- sync
- etc

show me?
sign in on device
settings app

## Current Status, Future Plans

now:
very simple - sign-in for 1.3

next:
more awesome: sync

on the horizon:
a way for third-party services to participate (e.g., contacts sync)
a way for third-party non-certified apps to participate (sign-in request)

## Why Are We Doing This?

why build this when we have persona? a sign-in system - not an account system
fxa - a place to persist user data and sign in

is it a silo?  i hate silos!
no.  it provides convenience for firefox users
but user maintains control over own data
this is a way to provide access to services
not to own the user

deeper info

## When Is This Happening
 
- version 1.3 of fxos for accounts sign-in (wmf, mkt)
- version 1.4 for deeper features (sync, keys, etc)

architecture
bugs
roadmap

## What Can I Do With Firefox Accounts?

two parts to this queston
1. what is stored in the fxa database
2. what services can fxa enable?

hwat goes in fxa - not much 
    - some keys
    - an email

in the (near) future -
additional services that need data (contacts, bookmarks, notes, etc)
will run their own services to store and manage that data
we will provide a template for doing this

## How Do I Use It?

The DOM API is the same as for persona

for sign-in, it's the browserid (persona) protocol
with one additon:

    nav.id.watch({wantIssuer: "firefox-accounts"});
    nav.id.request()

? how do i logout?



