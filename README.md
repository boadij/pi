# Pi

Small Pi Coding Agent extensions and skills with narrow responsibilities.

This repo is the index for Pi-related extensions, skills, and conventions. Extension implementations stay in their own repositories. Small skills can live directly in `skills/` until they need their own package or release flow.

## Extensions

| Name | Responsibility | Install |
|---|---|---|
| [Downshift](https://github.com/boadij/pi-downshift) | Starts strong, preserves context, then switches to a cheaper model when context pressure crosses a threshold. | `pi install npm