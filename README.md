# Yoe Alpine

Experiments with Alpine in embedded systems.

See [project board](https://github.com/orgs/YoeDistro/projects/1).

## Why Alpine for Embedded?

Often, server technologies make good embedded technologies because both have to
scale, so the following are important:

- Efficiency
- Deployment

Desktop technologies, where efficiency is not important, often do not scale well
in embedded and cloud deployments.

Another thing that is common is we often don't have physical access to these
devices.

## Running Alpine

### Quickemu

- `quickget alpine latest`
- `quickemu --vm alpine-latest.conf --display spice`
- run `alpine-setup`
  - When it asks for keyboard layout, `us, us` is a common option.
- after install, comment out the iso line in the conf file.

## Installing Simple IoT

- update to edge in `/etc/apk/repositories`
- add testing repo
- `apk add simpleiot`
