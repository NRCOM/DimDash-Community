# DimDash Community

Welcome to the official community hub for **DimDash**, the native iOS/iPadOS dashboard kiosk and auto-dimming app for wall-mounted smart home displays.

DimDash turns an iPhone or iPad into a full-screen dashboard for Home Assistant, Grafana, Dashy, Homarr, Glance, Node-RED Dashboard, Flame, or any custom web dashboard. It keeps your dashboard visible, dims intelligently when idle, and wakes instantly when you interact with it.

> This repository contains no app source code. DimDash is currently closed-source, and this repo exists for community support, bug reports, feature requests, setup notes, discussions, and public documentation.

## Useful Links

- Website: https://www.nick-renard.com/dimdash
- Privacy Policy: https://www.nick-renard.com/privacy
- Terms of Use: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/
- App Store: https://apps.apple.com/us/app/dimdash/id6768683806
- Bug reports: https://github.com/NRCOM/DimDash-Community/issues/new?template=bug_report.md
- Feature requests: https://github.com/NRCOM/DimDash-Community/issues/new?template=feature_request.md
- Discussions: https://github.com/NRCOM/DimDash-Community/discussions

## What DimDash Does

DimDash is built for people who use an iPad as a smart home wall panel but want something more purpose-built than Safari, Guided Access alone, or browser workarounds.

Core features include:

- Native iOS/iPadOS full-screen dashboard wrapper
- Auto-dimming overlay with configurable idle timeout
- Adjustable overlay opacity and fade duration
- Prevent screen sleep while the dashboard is active
- Pull-to-refresh for stuck dashboard pages
- Local HTTP/HTTPS dashboard support
- Integration templates for common self-hosted dashboards
- Home Assistant OAuth setup, dashboard picker, and silent token refresh
- Privacy-first, on-device operation with no account and no analytics

## Supported Integrations

DimDash works with any web dashboard URL, and includes templates for:

- Home Assistant
- Grafana
- Dashy
- Homarr
- Glance
- Node-RED Dashboard
- Flame
- Custom URLs

## Home Assistant Support

DimDash includes a native Home Assistant setup flow:

- Local network discovery for Home Assistant instances
- OAuth sign-in
- Secure Keychain credential storage
- Dashboard picker using Home Assistant's WebSocket API
- Silent re-authentication through Home Assistant external auth
- Ability to add more dashboards from an existing Home Assistant connection
- Kiosk URL options for hiding Home Assistant chrome where supported

## DimDash Pro

DimDash Pro is an App Store subscription that unlocks the full kiosk experience.

Pro features include:

- Multi-dashboard support for up to 5 dashboards
- Proximity Detection using the front camera and Apple's Vision framework
- Scheduled Night Mode for quiet-hours dimming
- Custom overlay colors
- JavaScript injection for advanced dashboard customization

Proximity Detection is processed locally on-device. No video is recorded, stored, transmitted, or used for analytics.

## Getting Help

Use **GitHub Discussions** for:

- Setup questions
- Home Assistant connection help
- Local network and certificate troubleshooting
- Camera permission questions
- Integration requests
- General feedback

Use **GitHub Issues** for:

- Reproducible bugs
- App crashes
- Incorrect behavior
- Broken setup flows
- UI issues with clear steps to reproduce

## Before Opening an Issue

Please include as much detail as possible:

- Device model, for example `iPad Pro 11-inch` or `iPad mini`
- iOS/iPadOS version
- DimDash app version and build number
- Dashboard type, for example Home Assistant, Grafana, Dashy, or custom URL
- Whether the dashboard is local HTTP, local HTTPS, or public HTTPS
- Steps to reproduce the problem
- What you expected to happen
- What actually happened
- Screenshots or screen recordings, if helpful

For Home Assistant issues, also include:

- Home Assistant version
- URL format used, without passwords or tokens
- Whether OAuth setup completed successfully
- Whether the problem happens on first setup, app relaunch, or token refresh
- Whether local network permission has been granted

For Proximity Detection issues, include:

- Whether DimDash Pro is active
- Whether Proximity Detection is enabled
- Camera permission status in iOS Settings
- What the DimDash Proximity Detection status screen shows
- Whether camera frames are arriving
- Whether presence is detected at all

## Privacy and Security

Please do not post secrets, tokens, passwords, private URLs, or screenshots containing sensitive dashboard data.

DimDash stores dashboard credentials in the iOS Keychain. Home Assistant OAuth credentials are used only to authenticate your own Home Assistant instance and refresh access silently inside the app.

## Feature Requests

Feature ideas are welcome. Good requests usually include:

- The problem you are trying to solve
- The dashboard/integration involved
- How often you would use it
- Whether it should be free or Pro
- Any screenshots, examples, or links to related projects

## Community Guidelines

Please keep discussions practical, kind, and focused on helping people build better smart home dashboard setups. DimDash is built for the self-hosted and Home Assistant communities, and the goal of this repo is to make support and feedback easy to follow.

## Project Status

DimDash is actively developed by [Nick Renard](https://github.com/nrcom). This repository is for community support and documentation, not the private app source code.

Thanks for helping make iPad wall dashboards less annoying and a lot more useful.
