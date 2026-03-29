1. Log The Changes
2. Update **Client** and **Server** BCC modpack version number
   1. `bcc.json`
   2. `bcc-common.toml`
3. **Client Only** Update `config/isxander-main-menu-credits.json` to the Modpack version number **X2**
4. Install Mods on a separate instance of the Modpack
   1. Verify if the mod works in Singleplayer
   2. Verify if the mod needs to be on Server if so install it
      1. Verify the mod works on Server
   3. If Client side mods were added then log those mods here [README.md](README.md)
      1. If a Client side mod options were changed then add that config to `config/yosbr/config`
      1. Client side config options that should be forced with updates should go to `config/` not `config/yosbr/config`
   4. If Server side mods were added then log those mods here [SERVER.md](SERVER.md)
5. Create a new Github branch with the `{modpack version}-{minecraft version}`
6. Update files in Github repo to reflect the changes made from above.
   1. Double check `mods/`,`config/`,`resourcepacks/`, `shaderpacks/` that any added or removed file was reflected for **Client**
   2. Zip up the following folders for **Client** from **Github repo** `config/`,`mods/`,`resourcepacks/`,`shaderpacks/` name it the following `QuackysVanillaQOL-x.x.x.zip`
   3. Double check `mods/`,`config/` in that any added or removed file was reflected for **Server**
   4. Zip up the following folders for **Server** from **Github repo** `config/`,`mods/` name it the following `QuackysVanillaQOL_Server-x.x.x.zip`
7. Export Modpack in Modrinth by hitting the three dots then `Export Modpack` and export the following
   1. `mods/`
   2. `config/`
      1. `yosbr/`
      2. `bcc.json`
      3. `bcc-common.toml`
      4. `betterblockentities.json`
      5. `isxander-main-menu-credits.json`
      6. `loadsupport.toml`
   3. `resourcepacks/`
   4. `shaderpacks/`
8. Put the version number and write the patch notes in the description
9. Goto [Quackys Vanilla QOL Versions](https://modrinth.com/modpack/donnie58744_quackysvanillaqol/versions) on Modrinth
   1. Create a new version and upload the exported `.mrpack` and the Server `.zip`
10. Update [Modrinth README](https://modrinth.com/modpack/donnie58744_quackysvanillaqol)
11. Upload `QuackysVanillaQOL-x.x.x.zip`, `QuackysVanillaQOL_Server-x.x.x.zip`, and `QuackysVanillaQOL-x.x.x.mrpack` to Github Release
12. Push, Create PR, merge

