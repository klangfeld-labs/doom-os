# Changelog

## 0.6.2-alpha, build 3824 (2026-10-06)

- **The AUTO TRIG shortcut no longer freezes the box on MARK**
- **The patcher shows the checksums the stock firmware and patched firmware**  

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
