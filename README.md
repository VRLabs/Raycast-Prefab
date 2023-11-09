<div align="center">

# Raycast Prefab

[![Generic badge](https://img.shields.io/github/downloads/VRLabs/Raycast-Prefab/total?label=Downloads)](https://github.com/VRLabs/Raycast-Prefab/releases/latest)
[![Generic badge](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/VRLabs/Raycast-Prefab/blob/main/LICENSE)
[![Generic badge](https://img.shields.io/badge/Unity-2019.4.31f1-lightblue.svg)](https://unity3d.com/unity/whats-new/2019.4.31)
[![Generic badge](https://img.shields.io/badge/SDK-AvatarSDK3-lightblue.svg)](https://vrchat.com/home/download)

[![Generic badge](https://img.shields.io/discord/706913824607043605?color=%237289da&label=DISCORD&logo=Discord&style=for-the-badge)](https://discord.vrlabs.dev/)
[![Generic badge](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dvrlabs%26type%3Dpatrons&style=for-the-badge)](https://patreon.vrlabs.dev/)

Places an object at the hit point of a raycast

![Raycast](https://github.com/VRLabs/Raycast-Prefab/assets/76777936/e06c6089-c2f2-49b2-8339-80ffe8642423)


### ⬇️ [Download Latest Version](https://github.com/VRLabs/Raycast-Prefab/releases/latest)

<!-- 
### 📦 [Add to VRChat Creator Companion]() -->

</div>

---

## How it works

* [Limb IK](http://www.root-motion.com/finalikdox/html/page12.html) hierarchy is used with a [Grounder](http://www.root-motion.com/finalikdox/html/page9.html) to cast an object onto collider surfaces.

## Install Guide

https://github.com/VRLabs/Raycast-Prefab/assets/76777936/b97b4dd0-0615-430b-9f10-9a4c40f94d43

* If you dont already have [Final IK](https://assetstore.unity.com/packages/tools/animation/final-ik-14290) installed, download and install the [Final IK Stub](https://github.com/VRLabs/Final-IK-Stub).
  * Note: Testing in Unity is not possible when using the Final IK Stub!
* Drag & drop the ``Raycast`` prefab into the base of your Hierarchy.
* Right click and unpack the prefab, then drag & drop it onto your avatar.
* By default, the raycast aims down from the ``Casting Target`` object.
  * If needed, you can move and rotate the ``Casting Target`` object until it "aims" at your target.
 
## How to Use

* Place the objects you want to raycast under the ``Container`` GameObject or constrain them to the ``Container`` GameObject.
  * World Particles can't be Constrained to the ``Container`` GameObject and have to be parented to the ``Container`` object instead due to "Fix Transforms" affecting the emission location.
* In game, the ``Container`` object will raycast down from the ``Casting Target`` onto any Collider which matches the Layers set up in the ``Grounder``'s Grounder IK Script (by default this is: ``Default``, ``Ignore Raycat``, ``Water`` and ``Environment``).
  * Note that you can't change layers on your avatar. Local avatar layers will always be ``PlayerLocal`` and ``MirrorReflection``, and remote avatar layers will always be ``Player`` (with the exception of UIMenu).

## Additional notes

* VRChat uses Final IK v1.9. If you are using a different version you may experience differences in behavior when testing with Final IK.

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
