# Changelog

## 0.7.1, build E7F5 (2026-10-29)

**Improvements**
- **Preview instruments before selecting them**  
  In the instrument browser, hold SUB PAD to preview the selected instrument. Turn the encoder while holding SUB PAD to preview other instruments.
- **Switch instruments on the fly**  
  In the instrument editor, press REMAIN and turn the encoder to try different instruments instantly, even while the pattern is playing. Press the encoder to confirm your choice, or EXIT to restore the original instrument.
- **Bounce in place to any empty pad**  
  Press RESAMPLE to open the bounce screen, which shows what will be bounced and how the pattern will be affected. Choose CUT, TAIL or LOOP, select an empty pad, then press RESAMPLE to start recording. Once finished, the new pad is shown on screen.

**Fixes**
- **Mixer solo now uses REMAIN + pad instead of SHIFT**  
  SHIFT + pad previously soloed a track but also triggered the pad's SHIFT functions, such as FIXED VELOCITY. Solo now uses REMAIN + pad, leaving SHIFT + pad to work as expected.
- **Fixed button LED states**  
  Certain buttons previously remained dimly lit when there were turn off or inactive, making it difficult to distinguish their on and off states. The LEDs now behave the same as in the stock screens.

## 0.7, build 0D8C (2026-10-28)

**New**
- **Instruments: 20 sound engines and 11 drum kits**  
  Press SUB PAD + an empty pad to open the instrument browser. Choose a single instrument or a complete 16-pad drum kit. On an instrument track, press START/END to open the instrument editor. Use the encoder to navigate between parameter sections. Press SUB PAD to preview the sound, or SHIFT + pad 4 to play it chromatically.

  To replace an instrument while keeping all its notes, press REMAIN in the instrument editor.

  **Included instruments**
  - BASS, POLY, FM, WAVE, MALLET, PERC
  - Kick, Snare, Clap, Hats, Rim, Bell, Rasp, Kick8, Kick9, Snare8, Snare9, Claps, Tom8, Tom9  <br>
   
  **Included drum kits**
  - 909, 808, 707, 727, 606, CR-78, BOOM, LOFI, TRAP, DUST, and DOOM  <br>
  
- **Arpeggiator**  
  Open the arpeggiator from the new main menu. Use HOLD to keep it playing, or PRINT ARP (in the arp menu) to write the generated notes directly to a track.
- **Parameter locking**  
  Lock instrument parameters to individual steps. Press MARK on an instrument track to enter parameter lock mode, select a step, and adjust its parameters using the knobs. Press MARK again to save your changes, or EXIT to discard them.
- **Live waveform overlay**  
  View live audio waveforms directly over the grid or mixer. Press SHIFT + START/END once to display the main output, or twice to display individual tracks. Use the encoder to select a track.
- **Visual sidechain editor**  
  Configure sidechain compression directly on the audio and FX bus routing diagram. Select a source bus, then a destination bus, and adjust THRESHOLD, RATIO, and RELEASE using CTRL 1-3. A live waveform display with the actual compression envelope shows exactly how the sidechain responds to the audio.
- **3-band parametric EQ per track**  
  Adjust LOW, MID, and HIGH directly in the mixer. In the mixer, press PITCH/SPEED to open the EQ, then use CTRL 1–3 to adjust each band. Select ADV to fine-tune each band's frequency and Q. Up to 16 tracks can have their own EQ settings, which are saved per project.
- **Bounce in place**  
  Press RESAMPLE in DOOM OS to record the selected track, including its effects, onto the next empty pad and replace the original track with the recording. Use SHIFT + RESAMPLE to capture the full output instead.
  
  Choose between CUT, TAIL, and LOOP modes. Undo restores the original track. Mono sources remain mono, and the bounced sample stays in sync with the pattern.

- **Track names in the mixer**  
  The mixer can now display track names while scrolling through tracks. Toggle this with SHIFT + RECORD SETTING, along with other display options.
- **Direct mixer shortcut**  
  Hold RECORD SETTING for 0.6 seconds to open the mixer directly.
- **New main menu**  
  The main menu is now context-aware, with more room for entries and access from any DOOM OS view. The opening order of the two menus has also been reversed.
- **Boot directly into DOOM OS (toggle in DOOM OS settings)** 
- **Hold EXIT to leave DOOM OS**  
  Enable Hold to Exit in the DOOM OS settings and choose a duration between 0.1 and 1.0 seconds. EXIT must then be held for the selected duration to leave DOOM OS, preventing accidental exits from a quick press. 

**Improvements** 
- **Pad muting and soloing in the mixer**  
  Mute or unmute individual pads directly from the mixer by tapping them, or hold SHIFT and tap a pad to solo it. Active pads light up white, while muted pads light up red. 
- **REMAIN + an effect button opens the page of the effect that is on**  
  Pressing the effect button itself turns it on with its page, and again turns it off.
- **Pattern changes now wait until the current pattern ends**  
  Hold PATTERN SELECT and select another pattern during playback. The current pattern will finish before switching, just like in the stock pattern screen. Hold SUB PAD + PATTERN SELECT + PAD to switch immediately.
- **Finer note length adjustments**  
  Hold a step and turn CTRL 2 while holding SHIFT to adjust its length in 1/128-note increments. The top line now displays note lengths as fractions, such as LEN 3/32.
- **GATE, LOOP, REVERSE and BPM SYNC work in the pattern view**
- **Various textual improvements to the Help menus**  
- **Waking the SP from the screensaver by pressing a button no longer triggers that button's underlying function**  
- **SHIFT + pad 16 opens the bus effects settings in DOOM OS**    
- **Holding SUB PAD shows which pads have samples, similar to TR-REC mode**  
- **Hold SUB PAD to hear the selected track**  
  In the mixer and wherever SUB PAD has no other use.
- **16 Velocity record mode**  
  REC's fourth mode plays the selected track at sixteen velocities across the pads, like the stock 16 VELOCITY. SHIFT + pad 2 turns it on in the pattern view directly.
- **Stock protected banks are now respected**
- **A pattern in DOOM OS can now contain 16,384 notes instead of several hundred**  
  Due to memory limitations DOOM OS can't display more than 16,384 notes in a single pattern. If you try to load a pattern that contains even more notes, a message will be shown. It will still load and play, but won't show all notes on the grid.
- **The grid and the mixer now show up to 160 tracks instead of just 18** 

**Fixes**
- **Mixer levels, pan and bus are now retained after switching off**  
- **Various undo/redo bugs**  
  Various undo/redo related bugs were fixed. Most of them were edge cases related to switching between projects. Undo/redo should be more solid now.
- **Fixed an issue where disconnecting or turning off a USB device could cause DOOM OS to exit to the stock firmware's main menu**  
- **A sample with a changed speed or tempo now plays at the correct speed or tempo within DOOM OS** 
- **Effect settings on the second page are now retained when you close the effect with EXIT in the editor**
- **The grid view selected with SHIFT + RECORD SETTING is now retained after switching off**
- **The volume knob now works consistently on every screen of DOOM OS**  
- **Various pad behavior fixes**  
  Under certain circumstances underlying views would stay open when opening screens within DOOM OS, causing unexpected pad behavior. This is now fixed and as a result occasional strange pad behavior shouldn't happen anymore. 
- **A pad no longer keeps playing in the automation screen when you press BANK while holding it**  
- **The piano roll's keys no longer overlap with the track names**
- **The notes in chromatic mode are now in the correct order (high notes at the top, low notes at the bottom)**
- **Fixed unintended shortcuts when editing steps 9 and 16**  
  Holding step 9 or 16 and pressing SHIFT no longer toggles the metronome or opens the bus effects. SHIFT + CTRL 1 now adjusts their pitch correctly, just like any other step.
- **Various small bugs involving edge cases** 

**Miscellaneous**
- **The underlying codebase has been completely rewritten in preparation for future features and improved stability, particularly to prevent hangs**
- **Fixed an issue with mono recording in the stock firmware**  
  Corrected a sample-reading bug in the SP's original mono recording code.
- **Removed the redundant PAD + VALUE shortcut for the piano roll. Use VALUE on a selected track instead**  

## 0.6.2-alpha, build 3824 (2026-10-06)

**Fixed**
- **The AUTO TRIG shortcut no longer freezes the SP on MARK**

**Improvements**
- **The patcher shows the checksums of the stock firmware and patched firmware**  

## 0.6.1-alpha, build ED5E (2026-10-04)

**New**

- **Pattern Follow (autoscroll) can be toggled with SHIFT + HOLD**  
  The pattern will stay on the currently selected measure or follow the playback head.
- **Solo is now mapped to SHIFT + ROLL**    
  The **ROLL** button blinks when solo is active.
- **The metronome can be activated with SHIFT + PAD 9**  
  Press once to toggle default metronome behavior (active during playback), press twice to toggle recmode (only active during recording)
- **EXT SOURCE can be toggled with EXT SOURCE** 
- **Time signatures visible in pattern menu**  
  Currently only show the time signature, the ability to change it will be added at a later stage.

**Fixed**
- **Playback of a new pattern with empty tracks is now supported**  
  This allows you to rehearse and record with a running metronome. Previously, an empty pattern was not playable, and adding empty tracks to the pattern would get them removed. This issue made it impossible to record patterns without creating a track with at least one note in it first.
- **REC button flickering fixed**
- **Various smaller bugs involving edge cases**

**Improvements**
- **REC button dimmed when not recording**.  
  The REC button was brighter than on the stock firmware, which could lead users to mistakenly assume REC mode was enabled.

**Miscellaneous**
- **The pattern mode now supports various time signatures internally**  
  For future stock compatibility reasons.

## 0.6-alpha, build 0C34 (2026-09-28)

The first public release, for firmware 5.52.
