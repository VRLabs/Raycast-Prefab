<div align="center">

# Raycast Prefab

[![Generic badge](https://img.shields.io/github/downloads/VRLabs/Raycast-Prefab/total?label=Downloads)](https://github.com/VRLabs/Raycast-Prefab/releases/latest)
[![Generic badge](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/VRLabs/Raycast-Prefab/blob/main/LICENSE)
[![Generic badge](https://img.shields.io/badge/Unity-2019.4.31f1-lightblue.svg)](https://unity3d.com/unity/whats-new/2019.4.31)
[![Generic badge](https://img.shields.io/badge/SDK-AvatarSDK3-lightblue.svg)](https://vrchat.com/home/download)

[![Generic badge](https://img.shields.io/discord/706913824607043605?color=%237289da&label=DISCORD&logo=Discord&style=for-the-badge)](https://discord.vrlabs.dev/)
[![Generic badge](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dvrlabs%26type%3Dpatrons&style=for-the-badge)](https://patreon.vrlabs.dev/)

Places an object at the hit point of a raycast.

![Alt text](https://raw.githubusercontent.com/VRLabs/Raycast-Prefab/main/Media/trollcull.gif)

### ⬇️ [Download latest Unitypackage](https://github.com/VRLabs/Raycast-Prefab/releases/latest)

<!-- 
### 📦 [Add to VRChat Creator Companion]() -->

</div>

---

## How it works

* Limb IK hierarchy is used with a grounder to cast an object onto collider surfaces.

## How to use

* If you dont already have FinalIK installed, download and install the [FinalIK Stub](https://github.com/VRLabs/Final-IK-Stub).
    * Note: Testing in Unity is not possible when using the FinalIK Stub!
* Drag & drop the ``Raycast`` prefab into the base of your Hierarchy.
* Right click and unpack the prefab, then drag & drop it onto your avatar.
* By default, the raycast aims down from the ``Casting Target`` Object.
  * If needed, you can move and rotate the ``Casting Target`` object until the it "aims" at your target.
* World particles must go inside the "Container", which is constrained to the "Grounder" object, because of "Fix Transforms" affecting the emission location.

When using the actual Final IK package:
* VRChat uses Final IK v1.9, and if you use a different version you may experience differences in behavior.

## Performance stats

```c++
Constraints:        2
Colliders:          1
```

## Hierarchy layout

```html
Raycast
|-Container
|  |-Cube
|  |-Cube
|-IK
|  |-Grounder
|  |  |-Offset
|  |  |  |-End
|-Floor
|-Casting Target
```

## Contributors

* [lin](https://github.com/oofdesu)

## License

Raycast Prefab is available as-is under MIT. For more information see [LICENSE](https://github.com/VRLabs/Raycast-Prefab/blob/main/LICENSE).

​

<div align="center">

[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/VRLabs.png" width="50" height="50">](https://vrlabs.dev "VRLabs")
<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Empty.png" width="10">
[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Discord.png" width="50" height="50">](https://discord.vrlabs.dev/ "VRLabs")
<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Empty.png" width="10">
[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Patreon.png" width="50" height="50">](https://patreon.vrlabs.dev/ "VRLabs")
<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Empty.png" width="10">
[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Twitter.png" width="50" height="50">](https://twitter.com/vrlabsdev "VRLabs")

</div>

---
