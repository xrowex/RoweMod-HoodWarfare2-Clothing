# Studio 0.2.121 beta

Studio prepares Rowe Clothing automatically when opening MetaHuman Creator.
The precompiled plugin installs into the character project, checks the exact
Unreal build and verifies its files. Missing files are repaired on the next
launch; modified or manually installed project plugins are preserved. No C++
compiler, Visual Studio or manual plugin copying is required.

Rowe Clothing provides garment import, placement, fit and weight transfer,
separate saved shaped meshes, and clickable movement/rotation controls in the
Creator viewer. Initial hoodie controls estimate shoulder, elbow and cuff
positions from the garment mesh. Fit remains specific to the selected character;
this does not add universal clothing or guarantee a clip-free result.

Blender and Microsoft runtime setup retain their existing official-installer
flow. Unreal and Creator Core Data use Epic Launcher; sign-in, license and Windows
permission prompts still require the user. The private tattoo plugin is excluded.

The candidate passed nine isolated dependency-installation checks, 34 existing
handoff checks, and an actual Unreal commandlet load of the automatically installed
plugin in a fresh project. The existing interactive viewer controls were confirmed
by the local user. The newer mesh-estimated positions passed native geometry
checks; their final interactive appearance remains a beta test. An earlier viewer
attempt ran out of GPU memory while another game was running.

Save and close Creator before updating its loaded plugin. Open the character from
the updated Studio; dependency setup and the clothing panel open automatically.
Keep GPU-heavy games closed while using Creator when video memory is limited.
Existing character assets and artwork are not included in the download. Runtime
gameplay, two-PC multiplayer and fresh-machine gameplay are not newly verified.
