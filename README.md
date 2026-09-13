# My Minecraft Launcher

An independent Minecraft: Java Edition desktop launcher under development using Electron and TypeScript.

## Current development status

The local Windows prototype currently supports:

- A basic desktop launcher interface.
- Microsoft account sign-in through the system browser using authorization code flow with PKCE.
- Xbox Live and XSTS authentication.

Minecraft Services authentication currently returns "Invalid app registration". Minecraft profile retrieval and entitlement verification have not yet been validated. API access approval is being requested.

This repository currently provides project documentation. The prototype source code has not yet been uploaded, and no downloadable release is available.

## Intended Minecraft API usage

The launcher needs Minecraft Services access to authenticate the signed-in user, verify their Java Edition entitlements, and retrieve their Minecraft profile.

Game access is intended for users with a valid Minecraft: Java Edition entitlement.

## Planned features

- Minecraft version selection and downloads.
- Vanilla, Fabric, and Forge support.
- Configurable Java runtime, JVM arguments, and memory allocation.
- Separate game instances and optional modpack management.
- Support for additional desktop platforms.

## Authentication and privacy

The current prototype opens Microsoft sign-in in the user's system browser. It does not collect Microsoft account passwords.

Authentication tokens are handled in the Electron main process and are not sent to the renderer UI. Persistent token storage has not yet been implemented.

## Affiliation

This is an independent project and is not affiliated with, endorsed by, or an official product of Mojang Studios or Microsoft.
