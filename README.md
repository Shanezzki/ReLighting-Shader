# ReLighting

**Near-vanilla shaders with realistic lighting.** Textures, the sky, and clouds remain vanilla, but standard Minecraft lighting is replaced with physically plausible lighting: the sun, moon, and torches cast shadows, and backlit objects feature a light rim.

## Features

- **Sun and moon shadows.** Soft edges and smooth light color transitions: orange at sunset, cool blue at night.
- **Torchlight.** Warm, slightly flickering light. Torches themselves, lava, and glowstone emit a soft glow.
- **Torch shadows.** Objects near a torch cast shadows. These are approximate shadows calculated in screen space (details below).
- **Rim lighting.** If a light source is behind an object, a light border appears along its edge, similar to backlit photography.
- **Ambient Occlusion (SSAO).** Dark corners and junctions between walls, floors, and ceilings gain a sense of depth.
- **Nether and End.** Dedicated lighting for these dimensions.
- **Fog** at the render distance limit, as well as underwater and in lava.

## Compatibility

- **OptiFine** and **Iris** (including via Sodium).
- **Minecraft 1.16.5 – 26.3.**
- A single archive works for all versions.

## Settings

**Low / Medium / High / Ultra** profiles, plus individual parameters:

- shadow resolution, range, and softness;
- sun and torch brightness, torchlight range;
- torch shadows and their quality;
- ambient occlusion; - rim light intensity;
- exposure.

If the game lags, start with the **Low** profile or disable torch shadows.

## Limitations

- Torch shadows are approximated: they are calculated based on the screen view, so they may appear slightly grainy and can disappear near the edges of the frame. True shadows from individual light sources are not available in OptiFine or Iris.
- Vanilla block-face shading is baked into the block colors, so block sides may appear slightly darker than they would with completely "clean" lighting.
- If torchlight seems weak, reduce the torch falloff setting or increase the torch brightness.
