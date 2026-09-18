# BioField Launcher

BioField Launcher, registered in Azure as “My Minecraft Launcher,” is a Windows desktop launcher under development for approximately 20 friends.

Its purpose is to simplify installing the required mods and joining our Minecraft Java Edition server. The server is planned to run on the developer’s personal computer. There are no plans to offer paid products.

## Implementation

The current prototype is based on MRS Launcher / Helios Launcher and uses Electron and JavaScript. The local project retains the upstream MIT license and copyright notices.

The launcher uses the developer’s own Microsoft application ID, rather than the upstream developer’s application ID.

Upstream projects:
- https://github.com/peunsu/MRSLauncher
- https://github.com/dscalzi/HeliosLauncher

## Intended functionality

- Install and verify the mods required for our server.
- Authenticate users with their own Microsoft accounts.
- Launch Minecraft Java Edition and connect to our server.

Users are intended to have valid access to Minecraft Java Edition. The launcher is not intended to bypass authentication or game ownership requirements.

## Authentication and development status

The current implementation displays Microsoft's sign-in page in an Electron window and uses the OAuth authorization-code flow, followed by Xbox Live, XSTS, and Minecraft authentication.

Microsoft and Xbox authentication have completed during testing, but Minecraft token issuance returns “Invalid app registration.”

The previous AppID approval request was declined. A request for reconsideration is being prepared. Successful end-to-end Minecraft login, game launch, and server connection have not been validated.

## Repository scope

This repository currently contains project documentation. The prototype source code and downloadable builds are not published here.

This is an independent project and is not affiliated with or endorsed by Mojang or Microsoft.
