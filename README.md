# Frost-Client

Frost-Client is a private, non-commercial desktop launcher for Minecraft: Java Edition, built with Electron, React and TypeScript, together with a client-side Fabric mod for Minecraft 1.21.11. It is used by me and a few friends and is not distributed publicly.

Sign-in uses the Microsoft OAuth 2.0 authorization code flow with PKCE (public client, no client secret) against the "consumers" tenant, requesting only the scopes XboxLive.signin and offline_access. After sign-in the launcher exchanges the token for Xbox Live and XSTS tokens, signs in to Minecraft Services and loads the Minecraft profile. If the account does not own Minecraft: Java Edition, the launcher stops. The game can only be started with a signed-in account; the guest view is a read-only preview. There is no offline or cracked mode.

Tokens are stored locally, using the operating system's secure storage where available, and are sent only to Microsoft, Xbox Live and Minecraft services and to the local game process.
