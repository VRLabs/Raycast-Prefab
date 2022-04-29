# Raycast Prefab
  
[![Generic badge](https://img.shields.io/badge/Unity-2019.4.31f1-informational.svg)](https://unity3d.com/unity/whats-new/2019.4.31)
[![Generic badge](https://img.shields.io/badge/SDK-AvatarSDK3-informational.svg)](https://vrchat.com/home/download)
[![Generic badge](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/VRLabs/Raycast-Prefab/blob/main/LICENSE)
[![Generic badge](https://img.shields.io/github/downloads/VRLabs/Raycast-Prefab/total?label=Downloads)](https://github.com/VRLabs/Raycast-Prefab/releases/latest)

Grounder IK prefab. Requires Final IK v1.9

## How it works

Limb IK hierarchy is used with the grounder to cast an object onto collider surfaces.

## How to use

Add "Raycast.prefab" to your scene and enter play mode. Rotate "Casting Target".

World particles must go inside the "Container", which is constrained to the "Grounder" object, because of "Fix Transforms" affecting the emission location.

VRChat uses Final IK v1.9, and if you use a different version you may experience differences in behavior.

## Downloads

You can grab the latest version of the Raycast Prefab in [Releases](https://github.com/VRLabs/Raycast-Prefab/releases/latest).

## License

Raycast Prefab is available as-is under MIT. For more information see [LICENSE](https://github.com/VRLabs/Raycast-Prefab/blob/main/LICENSE).

## Contact us

If you need help, our support channel is on [Discord](https://discord.vrlabs.dev).
