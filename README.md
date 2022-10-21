# Habitica Self-Hosted Fork

Host a custom Habitica instance on your home network!

Inspired by <https://github.com/headcounter/shabitica>

## Main features

### Host your own Habitica instance on your own network

### Provide custom content (items/armor/pets/etc.) to your users

To keep my kids excited about this long-term, I need to be able to add new content frequently that they will be excited about. The content itself may end up being copyrighted so it won't be part of this fork's open-source offering, but you can imagine any number of ways you could incorporate your users' favorite fandoms in motivating ways.

### Multi-User Kiosk Mode

The ability to use a shared device as a Habitica kiosk, and users are able to quickly sign in and check off items. Also auto log-off users after a short timeout.

## Why not just use [shabitica](https://github.com/headcounter/shabitica)?

A few things about that project turned me off:

* Not regularly maintained
* Departed from the upstream technology stack
* Only runs on a specific operating system

However, the goals of this project are mostly aligned with [shabitica's fundamental differences](https://github.com/headcounter/shabitica#differences-from-the-upstream-project):

### Initial alignment

I feel like these are critical to a viable self-hosted instance:

* Invite-only by default
* Free subscriptions for all users
* Use a custom mailer daemon
* No support for the mobile apps

### Eventual alignment

These are features that will eventually get to if I can:

* Do not use any 3rd-party services
* Sandboxing by default whenever possible: I'd like to harden the docker image such that I'd feel comfortable hosting this on the public internet
* No censorship of messages

## The primary approach

A key goal of this project that differentiates it from shabitica is this: **make changes as low-impact and forward-compatible with the main Habitica repository as possible**. That means where changes are needed, they are done as surgically as possible, in a way that reduces the risk of merge conflicts when we pull changes from upstream. I don't plan to take on maintenance of this project full-time, but I do want to be a full-time user of this self-hosted fork. I do want to have all the new features, and if I do stop updating this fork, I want it to be easy for anyone else to take this fork, pull upstream, and be ready to go with as little headache as possible.

## Development flow

Developing and contributing on this fork should be very similar to the main repository, with the following differences:

* Main branch is `dev` instead of `develop`. This allows us to pull upstream changes into `develop`, and have that as a starting point for contributing back to the main repository, without disrupting the self-hosted fork.

Habitica ![Build Status](https://github.com/HabitRPG/habitica/workflows/Test/badge.svg) [![Code Climate](https://codeclimate.com/github/HabitRPG/habitrpg.svg)](https://codeclimate.com/github/HabitRPG/habitrpg) [![Bountysource](https://api.bountysource.com/badge/tracker?tracker_id=68393)](https://www.bountysource.com/trackers/68393-habitrpg?utm_source=68393&utm_medium=shield&utm_campaign=TRACKER_BADGE)
===============

[Habitica](https://habitica.com) is an open source habit building program which treats your life like a Role Playing Game. Level up as you succeed, lose HP as you fail, earn money to buy weapons and armor.

**We need more programmers!** Your assistance will be greatly appreciated. The wiki pages below and the additional pages they link to will tell you how to get started on contributing code and where you can go to seek further help or ask questions:
* [Guidance for Blacksmiths](https://habitica.fandom.com/wiki/Guidance_for_Blacksmiths) - an introduction to the technologies used and how the software is organized.
* [Setting up Habitica Locally](https://habitica.fandom.com/wiki/Setting_up_Habitica_Locally) - how to set up a local install of Habitica for development and testing on various platforms.

Habitica's code is licensed as described at https://github.com/HabitRPG/habitica/blob/develop/LICENSE

**Found a bug?** Please report it to [admin email](mailto:admin@habitica.com) rather than creating an issue (an admin will advise you if a new issue is necessary; usually it is not).

**Have any questions about Habitica or its community?** See the links in the [habitica.com](https://habitica.com) website's Help menu or drop in to [Guilds > Tavern Chat](https://habitica.com/groups/tavern) to ask questions or chat socially!
