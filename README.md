# Mugens App

Welcome friends! This is the codebase for the Mugens Network app.

Mugens is a cross-platform application for Web, iOS, and Android built on the AT Protocol and based on the open-source Bluesky Social app.

## Branches

This repository keeps the upstream Bluesky Social app and the Mugens app separated by branch:

- **`main`**: mirror of the upstream [`bluesky-social/social-app`](https://github.com/bluesky-social/social-app) repository.
- **`mugens`**: Mugens Network application branch, containing Mugens-specific branding, features, configuration, and integrations.

The `main` branch should stay as close as possible to upstream. Mugens development should happen on the `mugens` branch.

## Get the app

Mugens is currently in development. Public app links will be added here when available.

<!--
- **Web: [mugens.app](https://mugens.app)**
- **iOS: [App Store](#)**
- **Android: [Play Store](#)**
-->

## Development Resources

This is a [React Native](https://reactnative.dev/) application, written in the TypeScript programming language. It builds on the `atproto` TypeScript packages (like [`@atproto/api`](https://www.npmjs.com/package/@atproto/api)), which are also open source, but in [a different git repository](https://github.com/bluesky-social/atproto).

There is a small amount of Go language source code (in `./bskyweb/`), for a web service that returns the React Native Web application.

The [Build Instructions](./docs/build.md) are a good place to get started with the app itself.

The Authenticated Transfer Protocol ("AT Protocol" or "atproto") is a decentralized social media protocol. You don't *need* to understand AT Protocol to work with this application, but it can help. Learn more at:

- [Overview and Guides](https://atproto.com/guides/overview)
- [GitHub Discussions](https://github.com/bluesky-social/atproto/discussions) 👈 Great place to ask questions
- [Protocol Specifications](https://atproto.com/specs/atp)
- [Blogpost on self-authenticating data structures](https://bsky.social/about/blog/3-6-2022-a-self-authenticating-social-protocol)

## Contributions

> [!NOTE]
> Mugens is currently in early development. While contributions are welcome, the project may prioritize foundational architecture, upstream synchronization, and Mugens-specific product direction.

**Rules:**

- We may not respond to every issue or PR.
- We may close an issue or PR without much feedback.
- We may lock discussions or contributions if moderation becomes difficult.
- We may not provide support for all build issues while the fork is still being adapted.

**Guidelines:**

- Check for existing issues before filing a new one please.
- Open an issue and give some time for discussion before submitting a large PR.
- Keep changes focused and easy to review.
- Avoid PRs that make upstream synchronization harder without a clear reason.
- Stay away from PRs like...
  - Large refactors without prior discussion.
  - Replacing core dependencies without a migration plan.
  - Adding entirely new features without prior discussion.
  - Making broad branding or product changes outside the Mugens direction.

The `main` branch tracks the upstream Bluesky Social app. Pull requests for Mugens-specific work should target the `mugens` branch unless explicitly stated otherwise.

## Forking guidelines

This application is already a fork of the Bluesky Social app, adapted for Mugens Network.

If you fork this repository, please be clear to users when you're giving them a fork of Mugens.

Please be sure to:

- Change all branding in the repository and UI to clearly differentiate from Mugens and Bluesky.
- Change any support links, feedback links, email addresses, terms of service, privacy policy, and other project links to your own systems.
- Replace any analytics or error-collection systems with your own systems.
- Review any default service endpoints before publishing your fork.
- Preserve upstream license notices where required.

## Security disclosures

If you discover any security issues in Mugens-specific code, please send an email to:

```txt
security@mugens.org
```

If the issue affects the upstream Bluesky Social app, please report it to Bluesky through their official security disclosure process.

## Are you a developer interested in building on atproto?

AT Protocol is a flexible technology for building decentralized social applications. With atproto, third-party integration can be seamless through custom feeds, federated services, clients, AppViews, lexicons, and more.

Mugens builds on this foundation to explore manga, novels, catalog data, reading communities, and social interaction on top of an open protocol.

## License (MIT)

See [./LICENSE](./LICENSE) for the full license.

This repository is based on the Bluesky Social app. Please preserve upstream copyright and license notices where applicable.

Bluesky Social PBC has committed to a software patent non-aggression pledge. For details see [the original announcement](https://bsky.social/about/blog/10-01-2025-patent-pledge).

## P.S.

We ❤️ open protocols, open-source software, and everyone helping build the Mugens Network.