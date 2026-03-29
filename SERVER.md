## Velocity Proxy

### Mods(Server)

- [CrossStitch](https://modrinth.com/mod/crossstitch)
- [FabricProxy-Lite](https://modrinth.com/mod/fabricproxy-lite)
  1. Put the mod into the mods folder
  2. Start the server to generate the config
  3. Configure Velocity `player-info-forwarding-mode` to `modern` and setting `forwarding-secret`
  4. Configure `secret` for the server in `config/FabricProxy-Lite.toml` to match Velocity secret

### Plugins(Velocity)

- [Simple Voice Chat](https://modrinth.com/mod/simple-voice-chat)
  1. Allow port 25565/udp (Default Minecraft Port) on Proxy
  2. Allow port 24454/udp (Default Voice Chat Port) on Server
  3. Port forward 24454/udp (Default Voice Chat Port) on the router connected to Server
  4. Move the plugin `.jar` into the Velocity plugin folder `plugins/`
  5. The plugin will automatically forward traffic to the correct Server

### Velocity JVM flags

- `-Xms400M`
- `-Xmx800M` 
- `-XX:+UseG1GC` 
- `-XX:G1HeapRegionSize=4M` 
- `-XX:+UnlockExperimentalVMOptions` 
- `-XX:+ParallelRefProcEnabled` 
- `-XX:+AlwaysPreTouch` 
- `-XX:MaxInlineLevel=15`
- `-Dvelocity.max-plugin-message-payload-size=1048576`
  - Increase Message Payload Size for mods that send large amounts of data such as `REI`
- `-Dvelocity.packet-decode-logging=true`

#### Complete Startup Command

`java -Xms400M -Xmx800M -XX:+UseG1GC -XX:G1HeapRegionSize=4M -XX:+UnlockExperimentalVMOptions -XX:+ParallelRefProcEnabled -XX:+AlwaysPreTouch -XX:MaxInlineLevel=15 -Dvelocity.packet-decode-logging=true -Dvelocity.max-plugin-message-payload-size=1048576 -jar velocity-3.5.0-SNAPSHOT-583.jar`