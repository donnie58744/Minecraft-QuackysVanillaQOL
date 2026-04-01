1. Make the changes from the Modrinth pack
2. Log The Changes
3. Update **Client** and **Server** BCC modpack version number
   1. `config/yosbr/bcc.json`
   2. `config/yosbr/bcc-common.toml`
4. **Client Only** Update `config/yosbr/isxander-main-menu-credits.json` to the Modpack version number **X2**
5. Install Mods on a separate instance of the Modpack
   1. Verify if the mod works in Singleplayer
   2. Verify if the mod needs to be on Server if so install it
      1. Verify the mod works on Server
   3. If Client side mods were added then log those mods here [README.md](README.md)
      1. If a Client side mod options were changed then add that config to `config/yosbr/config`
   4. If Server side mods were added then log those mods here [SERVER.md](SERVER.md)
6. Create a new Github branch with the `{modpack version}-{minecraft version}`
7. Update files in Github repo to reflect the changes made from **above** and the **logged changes**.
   1. Double check `mods/`,`config/`,`resourcepacks/`, `shaderpacks/` that any added or removed file was reflected for **Client**
   2. Zip up the following folders for **Client** from **Github repo** `config/`,`mods/`,`resourcepacks/`,`shaderpacks/` name it the following `QuackysVanillaQOL-x.x.x.zip`
   3. Double check `mods/`,`config/` in that any added or removed file was reflected for **Server**
   4. Zip up the following folders for **Server** from **Github repo** `config/`,`mods/` name it the following `QuackysVanillaQOL_Server-x.x.x.zip`
8. Export Modpack in Modrinth by hitting the three dots then `Export Modpack` and export the following
   1. `mods/`
   2. `config/`
      1. `yosbr/`
   3. `resourcepacks/`
   4. `shaderpacks/`
9. Put the version number and write the patch notes in the description
10. Goto [Quackys Vanilla QOL Versions](https://modrinth.com/modpack/donnie58744_quackysvanillaqol/versions) on Modrinth
   1. Create a new version and upload the exported `.mrpack` and the Server `.zip`
11. Update [Modrinth README](https://modrinth.com/modpack/donnie58744_quackysvanillaqol)
12. Upload `QuackysVanillaQOL-x.x.x.zip`, `QuackysVanillaQOL_Server-x.x.x.zip`, and `QuackysVanillaQOL-x.x.x.mrpack` to Github Release
13. Push, Create PR, merge

