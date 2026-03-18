1. Log The Changes
2. Update **Client** and **Server** BCC modpack version number
   1. `bcc.json`
   2. `bcc-common.toml`
3. **Client Only** Update `isxander-main-menu-credits.json` Modpack version number **X2**
4. Install Mods on a separate instance of the Modpack
   1. Verify if the mod works in Singleplayer
   2. Verify if the mod needs to be on Server if so install it
      1. Verify the mod works on Server
   3. If Client side mods were added then log those mods here [README.md](README.md)
      1. If a Client side mod options were changed then add that config to `config/yosbr/config` **Not Including `bcc.json` and `bcc-common.toml`**
   4. If Server side mods were added then log those mods here [SERVER.md](SERVER.md)
5. Create a new Github branch with the `{modpack version}-{minecraft version}`
6. Update files in Github repo to reflect the changes made from above.
   1. Double check `mods/`,`config/`,`resourcepacks/`, `shaderpacks/` that any added or removed file was reflected

7. Zip up the following folders for **Client** `config/`,`mods/`,`resourcepacks/`,`shaderpacks/` name it the following `QuackysVanillaQOL-x.x.x.zip`
8. Zip up the following folders for **Server** `config/`,`mods/` name it the following `QuackysVanillaQOL_Server-x.x.x.zip`
9. Export Modpack in Modrinth by hitting the three dots then `Export Modpack`
10. Put the version number and write the patch notes in the description
11. Goto [Quackys Vanilla QOL Versions](https://modrinth.com/modpack/donnie58744_quackysvanillaqol/versions) on Modrinth
    1. Create a new version and upload the exported `.mrpack` and the Server `.zip`
12. Update [Modrinth README](https://modrinth.com/modpack/donnie58744_quackysvanillaqol)
13. Upload `QuackysVanillaQOL-x.x.x.zip`, `QuackysVanillaQOL_Server-x.x.x.zip`, and `QuackysVanillaQOL-x.x.x.mrpack` to Github Release
14. Push, Create PR, merge

