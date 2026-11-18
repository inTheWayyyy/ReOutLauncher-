<h1 align="center">ReOut Launcher</h1>

<p align="center">
  <img src="./reout_logo.png" width="220" alt="ReOut Launcher logo">
</p>

<p align="center">
  A Minecraft: Java Edition launcher for Android, by <b>Wertel</b> 🇮🇶<br>
  Based on <a href="https://github.com/MojoLauncher/MojoLauncher">MojoLauncher</a>, which is based on <a href="https://github.com/PojavLauncherTeam/PojavLauncher">PojavLauncher</a>
</p>

<p align="center">
  <a href="https://discord.gg/spSgdxAxX8"><img src="https://img.shields.io/badge/Discord-ReOut-7389D8?logo=discord&logoColor=ffffff" alt="Discord"></a>
  <a href="../../releases"><img src="https://img.shields.io/badge/Download-Releases-9B4DFF" alt="Releases"></a>
</p>

* ReOut Launcher is a launcher that allows you to play Minecraft: Java Edition on your Android device, with its own name, purple and dark-black look, and community.

* It is built on top of MojoLauncher, which can run almost every version of Minecraft and supports installing modloaders such as [Forge](https://files.minecraftforge.net/) and [Fabric](http://fabricmc.net/).

## Navigation
- [Introduction](#introduction)
- [Getting ReOut Launcher](#getting-reout-launcher)
- [Building](#building)
- [Current roadmap](#current-roadmap)
- [Known issues](#known-issues)
- [License](#license)
- [Contributing](#contributing)
- [Credits & Third party components and their licenses](#credits--third-party-components-and-their-licenses-if-available)
- [بالعربي](#بالعربي)

## Introduction
* ReOut Launcher is a Minecraft: Java Edition launcher for Android, forked from [MojoLauncher](https://github.com/MojoLauncher/MojoLauncher) (itself based on [PojavLauncher](https://github.com/PojavLauncherTeam/PojavLauncher)).
* The core features (running Java and the game on Android, version support, Forge and Fabric support) come from MojoLauncher and PojavLauncher. ReOut adds its own branding, theme and community on top.
* ReOut is **not** affiliated with Mojang Studios or Microsoft. Minecraft is a trademark of Mojang Studios, and you need to own Minecraft: Java Edition to play it.

## Getting ReOut Launcher

1. Download the prebuilt APK from the [Releases](../../releases) page, then install it. You may need to allow "Install from unknown sources".
2. Or get early builds from [GitHub Actions](../../actions).
3. Or [build](#building) it from source.

## Building
* Build the launcher (it will automatically download all required components)
```
./gradlew :app_mojo:assembleDebug
```
If you are building on Windows:
* Replace `./gradlew` with `.\gradlew.bat`
* Make sure `mojoexec`, `sdl`, `glfw` are symlinked into `app_mojo/src/main/jni/`

## Current roadmap
- [x] New name, icon and logo
- [x] Purple and dark-black theme (colors)
- [x] Our own Discord community link inside the app
- [ ] Recolor remaining blue buttons, sliders and switches
- [ ] Replace remaining MojoLauncher names and links in the app
- [ ] ReOut Loader: our own lightweight mod loader (starting with Minecraft 1.8.9)
- [ ] Signed release builds

## Known issues
These are inherited from MojoLauncher:
- Some physical mice may have very slow mouse speed
- On Holy GL4ES, large texture atlases may be distorted (resulting in stretched/blocky textures in modpacks)

## License
- ReOut Launcher is a fork of MojoLauncher and is licensed under [GNU LGPLv3](./LICENSE), the same license as the project it is based on.
- The original copyright notices and licenses are kept in this repository. If you redistribute ReOut Launcher, follow the license terms.

## Contributing
Bug reports and ideas are welcome. Open an issue here, or join our [Discord](https://discord.gg/spSgdxAxX8).

Any code change to this repository should be submitted as a pull request. The description should explain what the code does and give steps to execute it.

## Credits & Third party components and their licenses (if available)
ReOut Launcher exists thanks to **MojoLauncher** and **PojavLauncher** and all of their contributors.

- [MojoLauncher](https://github.com/MojoLauncher/MojoLauncher): [GNU LGPLv3 License](https://github.com/MojoLauncher/MojoLauncher/blob/v3_openjdk/LICENSE)
- [PojavLauncher](https://github.com/PojavLauncherTeam/PojavLauncher): [GNU LGPLv3 License](https://github.com/PojavLauncherTeam/PojavLauncher/blob/v3_openjdk/LICENSE)
- Android Support Libraries: [Apache License 2.0](https://android.googlesource.com/platform/prebuilts/maven_repo/android/+/master/NOTICE.txt).
- [Holy GL4ES](https://github.com/artdeell/gl4es_extra_extra/): [MIT License](https://github.com/ptitSeb/gl4es/blob/master/LICENSE).
- [OpenJDK](https://github.com/PojavLauncherTeam/openjdk-multiarch-jdk8u): [GNU GPLv2 License](https://openjdk.java.net/legal/gplv2+ce.html).
- [GLFW](https://github.com/MojoLauncher/glfw): [zlib license](https://github.com/MojoLauncher/glfw/blob/glfw34/LICENSE.md)
- [SDL](https://github.com/MojoLauncher/MojoSDL): [zlib license](https://github.com/MojoLauncher/MojoSDL/blob/main/LICENSE.txt)
- [LWJGL2-GLFW](https://github.com/MojoLauncher/lwjgl2-glfw): 3-Clause BSD license
- [LWJGL3](https://github.com/LWJGL/lwjgl3): [BSD-3 License](https://github.com/LWJGL/lwjgl3/blob/master/LICENSE.md).
- [mojoexec](https://github.com/MojoLauncher/mojoexec): [MIT License](https://github.com/MojoLauncher/mojoexec/blob/master/LICENSE)
- [Mesa 3D Graphics Library](https://gitlab.freedesktop.org/mesa/mesa): [MIT License](https://docs.mesa3d.org/license.html).
- [pro-grade](https://github.com/pro-grade/pro-grade) (Java sandboxing security manager): [Apache License 2.0](https://github.com/pro-grade/pro-grade/blob/master/LICENSE.txt).
- [Authlib-Injector](https://github.com/yushijinhun/authlib-injector) (Used for authorisation via ely.by): [AGPL-3.0](https://github.com/yushijinhun/authlib-injector/blob/develop/LICENSE).
- [alsoft](https://github.com/kcat/openal-soft/) (Audio output library): [GNU Library General Public License](https://github.com/kcat/openal-soft/blob/master/COPYING) and [Modified PFFFT](https://github.com/kcat/openal-soft/blob/master/LICENSE-pffft).
- [oboe](https://github.com/google/oboe): [Apache License 2.0](https://github.com/google/oboe/blob/main/LICENSE).
- Thanks to [Mineskin](https://mineskin.eu/) for providing Minecraft avatars.

---

<div dir="rtl">

## بالعربي

**ReOut Launcher** لانشر لماينكرافت جافا على الأندرويد، بتصميم بنفسجي وأسود، من **Wertel** 🇮🇶

هو فورك من **MojoLauncher** المبني على **PojavLauncher**. الشغل الأساسي (تشغيل جافا واللعبة على الأندرويد ودعم النسخ والمودات) من جهدهم، وReOut يضيف اسمه وشكله ومجتمعه.

- **التحميل:** من صفحة [Releases](../../releases)، وانصب الـ APK (فعّل "التثبيت من مصادر غير معروفة" لو طلب).
- **الديسكورد:** https://discord.gg/spSgdxAxX8
- **الرخصة:** GNU LGPLv3، نفس رخصة المشروع الأصلي، وحقوق المطورين الأصليين محفوظة.
- ReOut غير تابع لـ Mojang Studios ولا Microsoft، ولازم تملك ماينكرافت جافا الأصلية عشان تلعب.

</div>
