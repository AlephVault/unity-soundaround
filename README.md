# Unity SoundAround

This package provides sound-related utilities to be used in games.

# Install

This package is not available in any UPM server. You must install it in your project like this:

1. In Unity, with your project open, open the Package Manager.
2. Either refer this Github project: https://github.com/AlephVault/unity-soundaround.git or clone it locally and refer it from disk.
3. This package has no dependencies.

# Usage

There are some behaviours in this package.

## Behaviours

There's a single class at namespace `AlephVault.Unity.SoundAround.Authoring.Behaviours`: `AudioLoop`.

### `AudioLoop`

This behaviour converts an audio source into a loop. There are some properties here:

- `private bool relativeToFrequency`: If true, the values of `loopAt` and `loopTo` are expressed in seconds instead of frames.
- `private float loopAt`: When this frame (or second fraction) is reached, then a loop will be performed.
- `private float loopTo`: When a loop is performed, this is the frame (or second fraction) the pointer will jump to.

