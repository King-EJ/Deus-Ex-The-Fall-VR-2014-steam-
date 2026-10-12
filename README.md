# Deus-Ex-The-Fall-VR-2014-steam-
Mod for Deus Ex: The Fall


<img width="448" height="442" alt="Adobe" src="https://github.com/user-attachments/assets/e9a790b9-a52c-473c-81b5-149531cf32e4" />

DEUS EX: THE FALL VR  -  VR mod for "Deus Ex: The Fall" (Unity 4.3.4, 32-bit, Mono)
=================================================================================

Version 0.1.8 (test build on Quest 3 VDXR).

CHANGES
0.1.8 - Option to hide the first-person arms so only the gun is in your hand 

0.1.7 - Use things by pointing at them with the right controller 
        Options to swap Y <-> left trigger and B <-> X 
        
0.1.6 - Every gun has its own place in your hand, adjusted live: with a gun out, hold BOTH stick clicks 1.5 s
        A = done.
        
0.1.5 - Laser shows whenever hand aiming is on and the weapon isn't holstered 

0.1.3 - Aim with the right controller: your shots go where it points, and a red laser + dot shows where they hit
        

INSTALL
-
1. unzip files into game folder

2. In Steam: right-click Deus Ex: The Fall > Properties > Launch Options, enter:
        -force-d3d11 -force-gfx-direct
   (Direct3D 11 is needed for VR; -force-gfx-direct lets the mod send each frame to the headset.)
   
3. Start your VR runtime first (Quest Link / Air Link, Virtual Desktop, or SteamVR)


CONTROLS (the game is played with its own Xbox controller layout)
-
  Left stick ............ move
  
  Right stick left/right ... turn (snap 30 degrees)
  
  Left stick click ...... crouch 
  
  Right stick up/down ...... d-pad up/down (augmentations)
  
  Right trigger ......... fire (where the right controller points)
  
  Right stick click + left/right ... d-pad left/right
  
  Left trigger (or Y if swaped).......... cover
  
  Hold right stick click (stick centred) 1.2 s ... re-centre the view
  
  A ..................... vault / move between cover, confirm
  B ..................... takedown, back
  X (of B if swaped)..................... interact / reload
  
  Y (or LT if swaped)..................... holster (hold = choose weapon)
  
  Left grip ............. item (hold + up/down = choose item)       = Xbox LB
  
  Right grip ............ grenade (hold + up/down = choose grenade) = Xbox RB
  
  Left menu button ...... tap = pause menu (Start), hold = Back
  
  Hold Y + left stick click 1 s ... VR settings menu (stick = choose / change, A = select, B = close)
  
  Hold both stick clicks 1.5 s .... adjust the gun in your hand (left grip = grab it, A = done, B = default)
  
  In menus: left stick / A / B like on a gamepad, right stick up/down scrolls.
  

HOW IT WORKS
-
- First person: you look around freely; "use" and the walking direction follow your head, your gun is in
  your right hand and shoots where it points (red laser). Your head movements (leaning) move the view too.
- In cover you stand just behind your character and look around freely; aim with the right controller.
- Takedowns and cutscenes: you stand where the game's camera is; the view turns with the camera when the shot
  changes ([Camera] CinematicYaw).
- The HUD and the menus are on a screen in front of your eyes, exactly as big as the game's view, so markers
  sit on what they mark.
- The game window shows the left eye.

CONFIG 
-
-    BepInEx\config\deusexthefall.vr.cfg (created on the first start)
  If the headset picture is upside down: [General] FlipEyes. Too dark / washed out: [General] SrgbOutput.
  HUD too dark / too faint: [UI] UIBlend = Alpha (Solid shows the whole screen with its background).
  HUD blurry: set the game's resolution to 1920 x 1080 (the HUD is drawn at the game's resolution).
  HUD size / distance: [UI] UIScale, UIDistance.
  Sharper picture: [General] RenderScale (1.2 - 1.5) and EyeMSAA (2 or 4).

Issues
-
- cover dont work well
- some guns save as others
- all lasers or nit accurate 

LICENSES
-
  The mod and its OpenXR bridge (dxfxr.dll) are free to use and change. The bridge is built with the Khronos
  OpenXR headers (Apache License 2.0).
