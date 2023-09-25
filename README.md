<div align="center">

# Raycast Prefab

[![Generic badge](https://img.shields.io/github/downloads/VRLabs/Raycast-Prefab/total?label=Downloads)](https://github.com/VRLabs/Raycast-Prefab/releases/latest)
[![Generic badge](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/VRLabs/Raycast-Prefab/blob/main/LICENSE)
[![Generic badge](https://img.shields.io/badge/Unity-2019.4.31f1-lightblue.svg)](https://unity3d.com/unity/whats-new/2019.4.31)
[![Generic badge](https://img.shields.io/badge/SDK-AvatarSDK3-lightblue.svg)](https://vrchat.com/home/download)

[![Generic badge](https://img.shields.io/discord/706913824607043605?color=%237289da&label=DISCORD&logo=Discord&style=for-the-badge)](https://discord.vrlabs.dev/)
[![Generic badge](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dvrlabs%26type%3Dpatrons&style=for-the-badge)](https://patreon.vrlabs.dev/)

Places an object at the hit point of a raycast

![Alt text]()

### ⬇️ [Download latest Unitypackage](https://github.com/VRLabs/Raycast-Prefab/releases/latest)

<!-- 
### 📦 [Add to VRChat Creator Companion]() -->

</div>

---

## How it works

* [Limb IK](http://www.root-motion.com/finalikdox/html/page12.html) hierarchy is used with a [Grounder](http://www.root-motion.com/finalikdox/html/page9.html) to cast an object onto collider surfaces.

## How to use

* If you dont already have [Final IK](https://assetstore.unity.com/packages/tools/animation/final-ik-14290) installed, download and install the [Final IK Stub](https://github.com/VRLabs/Final-IK-Stub).
  * Note: Testing in Unity is not possible when using the Final IK Stub!
* Drag & drop the ``Raycast`` prefab into the base of your Hierarchy.
* Right click and unpack the prefab, then drag & drop it onto your avatar.
* By default, the raycast aims down from the ``Casting Target`` object.
  * If needed, you can move and rotate the ``Casting Target`` object until it "aims" at your target.
* World particles must go inside ``Container``, which is constrained to the ``Grounder`` object, because of "Fix Transforms" affecting the emission location.

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
