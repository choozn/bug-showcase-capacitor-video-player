# Bug Reproduction
A quick showcase project to reproduce the following Bug:
https://github.com/jepiqueau/capacitor-video-player/issues/144

The player is not initialized despite returning a success object and preloading the content.
I've tried the library in both svelte and astro. Same behavior for both.

## Expected Behavior
The player should be initialized as specified in the docs.

## Current Behavior
A success object is returned, but the player is not initialized.
Using the `fullscreen` mode, the sound of the video is played but no player is visible. A fullscreen request is denied.
Using the `embedded` mode, nothing happens besides preloading the content and returning the success object.

```
{
  "method": "initPlayer",
  "result": true,
  "value": true
}
```

## Context (Environment)
- AstroJS / Svelte