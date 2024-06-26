## v1.1.0 - 26/04/2024
* Reworked disabling player fade for third person by request, only disables fading when needed. Note: SSE Display Fixes and/or OStim supercedes it.
* Fixed weapon node misalignment when third person arms are active.
* Disabled Headbob combat for now (might stay this way) as it causes weapon node misalignment issue(s).
* Fixed bow aim positioning whilst riding a horse.
* Updated default profile values.
* Support for GOG 1.6.1179.
* Removal of Fixes menu. First Person Overhaul toggle(s) moved to General.
* Archery Gameplay Overhaul (AGO) auto detection and activation of patch.
* Smooth Animation Transition auto activates when headbob rotation(s) are > 0.0f.
* fControllerBufferDepth has been removed. Note: You can set this manually inside of your skyrim.ini.
* Added note to Camera section for CTRL+CLICK the slider boxes to input a value.
* Drastically increased the controllable camera distances from 500 to 8192.
* Cameras have been updated to get the correct displacement value(s) which fixes various issues.
* Added a new hook for NearDistance which fixes water turning opaque. Note: Weird brightness is due to weathers (fine on clear day) will be looked at after release.
* Added CaptureWarmer detection to fix seeing the camera spinning around crazily for users with large mod lists.
* Added fFirstPersonDefault=15.000000 as requested this works outside of fPitchThreshold. (big hats!)
* Added Immersive Equipment Displays detection to state hiding weapons will not work and to use IED instead on the Hide menu.
* Added sync option for headbob rotation so all sliders move at once.
* Changed camera positioning due to internal updates.
* Re-added High Heels support. Note: There is a bug with HH if switching from female save to male save which causes the camera to be lower.
* Fixed camera issue when the target is not the player or on a horse.
* Fixed camera when werewolf feeding.
* Fixed ad-hoc scripted events when exiting sometimes placed you back into third person instead of first person.
* Fixed controlmap crash issue on SkyrimSE v1.6.1130+
* Added bOverrideVanillaArmsOnMovement by Kruziikrel13.
* Added bEnableThirdPersonTorchBlock as requested.
* Fixed left arm issue with magic using third person arm when equipped with a weapon in the right.
* Update imgui to 1.89.9 and fixed a crash issue which is present in previous builds.
* Removed bQuickLightLighting due to not working as intended and causing more problems than it is worth.
* Added official support for latest SkyrimSE v1.6.1170.
* Fixed Paragliding, now is enforced into third person with fake first person support.
* Fixed Camera acting oddly, visible body when looking down.
* Removed fSwitchPOVDetectDistance.
* Fixed Third Person Arms toggle so all third person options underneath are disabled.
* Updated OpenSans font.
* Added FontAwesome v6 font. Prettifies the menu.
* Various issues with vendor modules not playing nicely with latest Visual Studio 2022.

## v1.0.5 - 16/09/2023
* Fixed double arm issue when IED is not installed.
* Removed camera moving downwards to keep feet aligned for non-headbob.

## v1.0.4 - 15/09/2023
* Added support for Paragliding.
* Fixed flickering issue when switching stances.
* Fixed height issues switching characters on same session.
* Fixed headtracking by taking control of it in first person.
* Added support for high heels.
* Fixed default camera to only move the camera and not the body.
* Fixed killcam for magic.
* Fixed camera misalignment due to fBodyHeightOffset.
* Fixed some positional issues with the body for headbob and non-headbob.
* Support for Take a Peek FOV changes.
* Fixed CFPAO Sprint Jumping + Swimming.
* Added PushActorAway to ResetState.
* Fixed RaceSex Menu hiding first person body upon exit.
* Fixed losing arms with MapMenu opened. (Indoors)
* Fixed *fControllerBufferDepth for third person whilst sprinting.
* Fixed weapon(s) still visible when sitting down in first person.
* Fixed AnimationGraph registration.
* Fixed misc furniture markers. (No more spinning the camera!!)
* Added support for Ultimate Animated Potions NG.
* Misc fixes for arms.
* Removed Variable::bJournalDisabled no longer required.
* Removed Sleeping states no longer required.
* Potential crash fix(es) with HeadNode if it returns nullptr. This shouldn't really happen!
* Updated some of the hooks.
* Updated Weapon detection routine.
* Added FindNode function much easier to work with.
* Added GetHighHeelsOffset function.

## v1.0.3 - 24/07/2023
* Fixed crash with menu being disabled.
* Added compatibility for Show Player In Menus.
* Added bEnableThirdPersonTorch.
* Added error msg when skse_loader.exe is not found.
* Fixed printscreen for enb/reshade when ui is displayed.
* Fixed left shift so it releases properly upon closing the menu.

## v1.0.2 - 21/07/2023
* Fixed changing views with Dialogue Menu.
* Fixed tfc missing magic fx.
* Added minimum supported SKSE64 due to trampoline api. (SkyrimSE v1.5.97)
* Changed CheckCompatibility=0 due to Vortex.
* Fixed Hide menu not active.
* Fixed touring carriages to use "Fake first person" only.
* Fixed crashing issue with BSAnimationGraphEvent.
* Fixed headbob issue with Tween Menu.
* Refactored MenuMode=2.

## v1.0.1 - 03/07/2023 (compared to PR5-hotfix3 - 15/03/2023)
* Updated to CommonLibSSE-NG library.
* Fixed bEnableBodyConsole not working.
* Fixed bEnableShadows not working.
* Fixed events occurring at closest zoom level in third person.
* Fixed various arm issues, third person arm is visible where it makes sense.
* Fixed elderscroll reading event not triggering correctly.
* Fixed MenuMode=1 not regaining focus if clicking on Skyrim window when it is next opened.
* Fixed Triumvirate mod crash when transforming into a Deer. (Internal workaround)
* Fixed camera positioning for horse combat.
* Fixed controller issues with switching pov's.
* Fixed CC fishing to behave itself.
* Fixed first person local scale not working as intended.
* Fixed exiting furniture issue where in third person you could not target objects properly unless directly on top of them.
* Fixed headtracking with Scripted events.
* Fixed dismounting when on horse/dragon to switch back to First Person if you were in Fake First Person.
* Updated Reset State from the menu it should help better with certain stuck states.
* Added various combat camera settings.
* Added shield and block toggles to use third person arms.
* Added crossbow and aim toggles to use third person arms.
* Removed HookInput and MediaKeys, activates when on MenuMode=2 where it is needed.
* Support for Smoothcam to fix various conflicts.
* Support for TDM to fix various conflicts.
