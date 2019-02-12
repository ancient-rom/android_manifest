-----------------------------------------------------------------------------

<p align="center">
 <img src="https://github.com/ancient-rom/manifest/blob/pie/ancient.png" > 
</p>

-----------------------------------------------------------------------------
Credits:
=======
 * [**AOSP**](https://android.googlesource.com)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**SuperiorOS**](https://github.com/SuperiorOS)
 * [**DotOS**](https://github.com/DotOS)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**AospExtended**](https://github.com/AospExtended)
 * [**Syberia OS**](https://github.com/syberia-project)
 * [**Nitrogen OS**](https://github.com/nitrogen-project)
 * [**Pixys OS**](https://github.com/PixysOS)
 * [**ArrowOS**](https://github.com/ArrowOS)
 * [**MSM-Xtended**](https://github.com/Project-Xtended)
 * [**HavocOS**](https://github.com/Havoc-OS)
 * [**BootleggersROM**](https://github.com/BootleggersROM)
 * [**ABC**](https://github.com/ezio84?tab=repositories)
 * [**MCAOSP**]()
 * [**AOSIP**](https://github.com/aosip)
 * [**Liquid Remix**](https://github.com/liquidremix)
 * [**Resurrection Remix**](https://github.com/ResurrectionRemix)
 * [**Dirty Unicorns**](https://github.com/DirtyUnicorns)

-----------------------------------------------------------------------------

To get started with the building process, you'll need to get familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

# To initialize your local repository, use a command like this:

```bash
 $ repo init -u git://github.com/ancient-rom/manifest.git -b pie
```

# To initialize a shallow clone, which will save even more space, use a command like this: 

```bash
 $ repo init --depth=1 -u git://github.com/ancient-rom/manifest.git -b pie
```

Then to sync up:- 
================

```bash
 $ repo sync --current-branch --no-tags --no-clone-bundle --optimized-fetch --force-broken --force-sync -j8
```

Start the build:-
=================

```bash
 $ . build/envsetup.sh
 $ lunch ancient_<devicecodename>-userdebug
 $ mka bacon -jx
```
-----------------------------------------------------------------------------
