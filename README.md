# snesrev-launcher

### Change Log
1. Automatically find the right rom and rename it, just drop them into the same folder as the appimage.
2. Added command line parameters for .desktop files or to run from other apps.
3. (update 1) Recompiled super metroid, it fixed crashing/graphical bugs.
(https://github.com/TheRealYasri/sm/actions/runs/24377734056)
4. (update 2) added back zenity gui, no sub menus.
5. (update 2) Made every game variation that shares ini files each get there own that is copied in when launched.
6. (update 2) Added text output on what the script is doing as it runs.
7. (update 3) Launcher now stores its files in srl-saves, srl-roms, srl-config per game version.
8. (update 3) On game launch, symlinks for that game version's configs, saves,and rom are created.
9. (update 3) it cleans up old links from past runs, when a game is started.
10. (update 4) included info where to get the zelda 3 redux translation
11. (Update 5) Added option (default: disabled) to install .desktop files with auto update if you move the directory.
12. (Update 5) Refactored some sections and added a cache for some parts to speed up the script.
13. (Update 6) Recompiled smw for lag issues.
(https://github.com/TheRealYasri/smw/actions/runs/24545395292)
14. (Update 6) Added super metroid redux, needed a seperate executable. (https://github.com/TheRealYasri/sm/actions/runs/24582028652)
15. (Update 7) Removed many unneeded libraries. 181 MB > 55.1 MB
16. (Update 7) Changed appimage maker to [Anylinux-AppImages](https://github.com/pkgforge-dev/Anylinux-AppImages) 
17. (Update 8) Super Metroid Redux will auto patch if base rom is available.
18. (Update 8) Zelda 3 Redux will auto patch if base rom is available.
19. (Update 9) Removed even more unneeded files. 55.5 MB > 18MB
```
-------------------------------------------------------
 SNESREV Command Line Launcher
-------------------------------------------------------
 Usage: ./snesrev.appimage [command]

 Configuration:
  desktop    Toggle Desktop Shortcuts (Disabled)
  help       Show this message

 Base Game Commands:
  z3         Zelda 3 (US)      6D4F10A8B10E10DBE624CB23CF03B88BB8252973
  z3-redux   (Redux)           B2A07A59E64C498BC1B2F28728F9BF4014C8D582
  sm         Super Metroid     da957f0d63d14cb441d215462904c4fa8519c613
  sm-redux   SM Redux          0F4133F2E6BDD275B0CEEC3E348E2D6BF1C8189E
  smw        Super Mario World 553CF42F35ACF63028A369608742BB5B913C103F|6B47BB75D16514B6A476AA0C73A683A2A4C18765
  smb1       Super Mario Bros. 4A5278150F3395419D68CB02A42F7C3C62CDF8B4
  smbll      The Lost Levels   493E14812AF7A92D0EACF00BA8BB6D3A266302CA
  smas       (Extraction Src)  C05817C5B7DF2FBFE631563E0B37237156A8F6B6

 Zelda Commands (Requires US ROM + Lang ROM):
  z3-de      (German)          2E62494967FB0AFDF5DA1635607F9641DF7C6559
  z3-fr      (French)          229364A1B92A05167CD38609B1AA98F7041987CC
  z3-fr-c    (French Can.)     C1C6C7F76FFF936C534FF11F87A54162FC0AA100
  z3-es      (Spanish)         461FCBD700D1332009C0E85A7A136E2A8E4B111E
  z3-pl      (Polish)          3C4D605EEFDA1D76F101965138F238476655B11D
  z3-pt      (Portuguese)      D0D09ED41F9C373FE6AFDCCAFBF0DA8C88D3D90D
  z3-nl      (Dutch)           FA8ADFDBA2697C9A54D583A1284A22AC764C7637
  z3-sv      (Swedish)         43CD3438469B2C3FE879EA2F410B3EF3CB3F1CA4
```

### Special Thanks
This appimage for linux is made using the work of these people below...
```
Original appimage maker         https://github.com/qurious-pixel/zelda3/releases/tag/launcher
Appimage tooling                https://github.com/pkgforge-dev/Anylinux-AppImages

##Decomplation Source
Mario Source                    https://github.com/galaxyhaxz/smw-src
Super Metroid Source            https://github.com/strager/supermetroid
Zelda 3 Source                  https://github.com/snesrev/zelda3

##Ports/Patches
PC Porter                       https://github.com/snesrev
Super Mario World lag patch     https://github.com/snesrev/smw/pull/44
Super Metroid Redux PC Port     https://github.com/testyourmine/sm-redux
Super Metroid updated builder   https://github.com/LaserEyess/sm/tree/cmake

##Rom Hacks
Zelda 3 Redux                   https://www.romhacking.net/translations/6657/
Super Metroid Redux             https://www.romhacking.net/hacks/4963/
Flips Patcher                   https://github.com/Alcaro/Flips
```
