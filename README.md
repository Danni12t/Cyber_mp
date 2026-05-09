Cyber mp WIP steps
1. Game starts

2. RED4ext loads:
cp2077_mp_red4ext.dll

3. Plugin loads:
cp2077_mp_bridge.dll

4. Bridge connects to:
ws://127.0.0.1:3001

5. Node server accepts connection

6. Plugin sends snapshot JSON

7. Server broadcasts snapshot

8. Plugin receives snapshot back

9. Snapshot gets written to:
snapshot.json

10. Multiplayer networking is now working


========================================

WHERE FILES GO

========================================

BRIDGE DLL

BUILD OUTPUT:
cp2077_mp_bridge.dll

PUT HERE:
Cyberpunk 2077/bin/x64/


========================================

RED4EXT PLUGIN DLL

BUILD OUTPUT:
cp2077_mp_red4ext.dll

PUT HERE:
Cyberpunk 2077/red4ext/plugins/cp2077_mp_red4ext/

CREATE:
cp2077_mp_red4ext
folder if missing


========================================

SERVER FILES

KEEP HERE:
Desktop/cp2077_mp_server/

RUN:
node server.js


========================================

SOURCE PROJECTS

Desktop/cp2077_mp_bridge/

Desktop/cp2077_mp_red4ext/

Desktop/cp2077_mp_server/


========================================

CURRENT FEATURES

RED4ext plugin loading

Bridge DLL loading

Websocket connection working

Node server working

Snapshot packets sending

Snapshot packets receiving

Remote snapshot writing to file

Multiplayer networking foundation working


========================================

CURRENT DATA FLOW

Cyberpunk 2077
↓
RED4ext Plugin
↓
Bridge DLL
↓
Websocket
↓
Node Server
↓
Other Players


========================================

NEXT PLANS

PHASE 1
Real player coordinates from game

PHASE 2
Two real clients connected together

PHASE 3
Spawn remote player entity

PHASE 4
Movement sync

PHASE 5
Animation sync

PHASE 6
Vehicle sync

PHASE 7
Combat sync

PHASE 8
Dedicated multiplayer server

PHASE 9
Character replication system

PHASE 10
Full multiplayer framework
