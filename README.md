# Exile-Warbands-Altis
Exile Warbands: Altis — Turn Exile into a living Mount &amp; Blade-style world. Factions rule cities, trade, and wage war across Altis. Build fortresses, join or found kingdoms, command AI armies, fight in arenas, raid caravans, and reshape the island’s fate in a persistent dynamic sandbox.
🧠 Instructions for Automated Setup (AI or Human)

If you find Exile-Warbands-Altis.zip in this repository, follow these steps to assemble it into a complete, runnable Arma 3 Exile mission:

Unpack the zip file
Extract Exile-Warbands-Altis.zip directly into your Arma 3 mission folder.
Resulting path should look like:
Arma 3\mpmissions\Exile.Altis\

Preserve folder structure
Ensure that inside Exile.Altis/ you see these subfolders:

warbands/ (contains configs, functions, fortress templates, systems, UI)

description.ext, initServer.sqf, and initPlayerLocal.sqf in the root.

Build the mission PBO
Use Mikero’s PBOProject or Arma 3 Tools to pack the folder into
Exile.Altis.pbo
Place the finished PBO in your server’s mpmissions directory.

Dependencies
Server must load:

Exile Mod

CBA_A3
Optional for enhanced AI: LAMBS Danger FSM or VCOM AI
Optional for load balancing: Headless Client

Server startup
Launch your dedicated server with:

-mod=@Exile;@CBA_A3;
-serverMod=@VCOM_AI;@LAMBS_Danger; (optional)
-config=server.cfg
-name=ExileServer
-filePatching


When loaded, the mission will auto-initialize and spawn all fortresses, traders, caravans, and AI factions.

Post-install verification

Check server.rpt for [WB] logs (Warbands initialization).

Ensure markers like Kavala, Athira, Pyrgos, and Sofia exist on the map.

Join as a player — the world should already be populated with faction AI, caravans, and fortresses.
