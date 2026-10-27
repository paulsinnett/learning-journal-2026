# My Learning journal

## 26 10 2026

We have a bug in our game. When you play for a few minutes, occasionally one frame turns black. To find this we recorded the game, and played back until the black frame showed. With the game paused I could then turn off parts of the game until we detected that the issue was due to a single particle effect.

The issue with particle was that the shader could occasionally output an invalid value for 1 pixel, which then got exploded over the whole screen by the bloom post effect.

## 27 10 2026

I need to pass the dialogue content from the scriptable to the an object in the scene. How? I made a reference to the `DialogueBox` in the `DialogueTrigger` script.

But when I move my character into the trigger, nothing happens.
