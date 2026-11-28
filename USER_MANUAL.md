# Push 3 for Logic Pro user manual

For version 0.15.9. Use Ableton Push 3 over USB to play instruments, mix, edit plug-ins, launch Live Loops and program Logic’s Step Sequencer. When you’re done, release Push from the companion and open Ableton Live as usual.

[Download the installer](https://github.com/iamcaptaine/Push3Logic-Releases/releases/latest)

- [Install and connect](#install-and-connect)
- [Mixer and resets](#mixer-and-resets)
- [Smart Controls, instruments and effects](#smart-controls-instruments-and-effects)
- [Play pads and quantize](#play-pads-and-quantize)
- [Transport, recording and project shortcuts](#transport-recording-and-project-shortcuts)
- [Live Loops](#live-loops)
- [Step Sequencer](#step-sequencer)
- [Switch back to Ableton](#switch-back-to-ableton)
- [Updates and troubleshooting](#updates-and-troubleshooting)

## Install and connect

You need an Apple silicon Mac with macOS 13 or later, a compatible installation of Logic Pro and a Push 3 connected via USB. Put Push in **Control Live** mode, including on standalone models. Use the Apple silicon package from Releases. The package is unsigned and unnotarized, so macOS may require explicit approval to open it.

1. Open **Push 3 for Logic Pro** from Applications. macOS asks for **Accessibility** to operate Logic dialogs and editing controls, and **Screen Recording** to read the Step Sequencer window for pad LEDs. Follow the prompts in **System Settings → Privacy & Security** and relaunch if macOS requests it. Screen Recording can be skipped if you don’t need Step Sequencer pad feedback. The Push display uses USB independently.
2. In **Manage License…**, choose **Start 15-Day Trial** or enter your Polar license key. The trial starts when you click the button and works offline. The one-time US$39.99 license covers two Macs. First activation requires internet access. Each successful Polar check allows 30 days offline. Connect to the internet to verify again after that. Existing activations need one online check after updating to establish the offline window. Use **Manage License…** or the [Polar Customer Portal](https://polar.sh/airscape-records/portal) to manage activations.
3. Connect Push. **Overview** shows when the Mac sees its User ports, even before connection. Click **Launch & Connect**. The companion opens Logic if needed, switches Push to User Mode, enables the instrument pads and connects the screen. If prompted, quit Ableton Live so the companion can take over the hardware.
4. Open an existing project or choose one from Logic’s Project Chooser. Locally stored projects are available offline. On first setup, open **Logic Pro → Control Surfaces → Setup**, then **New → Install** and add **Mackie Control**. Click the new surface and set its ports exactly as shown below.
5. Select a software instrument track. Route **Push 3 for Logic Pro Pads** to it for musical input. Exclude the raw Push User port and the companion Control port from musical input to avoid duplicate notes or stray MIDI.
6. Press **Play** on Push, turn one of the eight knobs above the screen in **Mixer → Volume**, then press **Note** and play a pad. These checks cover transport, mixer feedback and instrument routing.

| Logic control surface | Input Port | Output Port |
| --- | --- | --- |
| Mackie Control | Push 3 for Logic Pro Control | Push 3 for Logic Pro Feedback |
| Launchpad X, for Live Loops | Push 3 for Logic Pro Loops Control | Push 3 for Logic Pro Loops Feedback |

The Mackie ports appear during connection. The Loops ports appear when you first enter **Session**. The companion picks the matching **Ableton Push 3 User Port** for both hardware directions. Use **Advanced → Push ports** if you have several units or need to choose the pair manually.

Click the Dock icon or choose **Show Main Window** from the companion’s menu bar icon to reopen the window. **Overview** shows connection state and a preview of the hardware screen. Use **Mixer**, **Sounds**, **Pads** and **Play & record** during a session. **Setup & help** shows first-run steps and the hardware shortcut guide. **Advanced** contains port selection, display controls, custom button mappings and diagnostics.

## Mixer and resets

The eight knobs above the screen, called **encoders**, control the eight visible channel strips. Press a screen button directly under or above the on-screen item you want. In this guide a shortcut written **A + B** means hold A, then press or touch B.

| On Push | What it does |
| --- | --- |
| **Mix** | Return to the mixer. |
| **Shift + Mix** in Mixer | Cycle Volume, Pan and Send Level. You can also choose a mode in the companion’s Mixer panel. |
| Turn a screen encoder | Adjust the matching strip’s volume, pan or current send. Configure a send on the Logic channel strip before adjusting it. |
| **Shift + Page Left / Right** in Sends | Choose the previous or next send slot. The display shows the slot, such as **S1**. |
| Upper screen row | Select the corresponding track. Its name stays visible and the highlight follows the selection. |
| Lower screen row | Select tracks by default. It can also control mute, solo or record arm. |
| D-pad **Left / Up** or **Right / Down** | Select the previous or next track. |
| **Page Left / Right** | Move a mixer bank left or right, normally eight strips with one Mackie surface. |
| **Mute** or **Solo** | Toggle on the selected track. Hold either button and press a track’s screen button to target that track directly. |
| **Record + track button** | Toggle record arm for that track. |
| **Lock + Mute / Solo / Record** | Assign that function to the lower row. **Shift + Lock** returns it to Select. |
| **Duplicate + track button** | Duplicate the track with its settings and content. |
| **Delete + track button** | Request removal of that track. Review any native Logic dialog before confirming. |

In Volume view each strip shows a continuous vertical signal meter in green, yellow and red alongside a horizontal fader bar and percentage. Both are visible while you adjust the fader. The selected track is highlighted across the entire strip. Pan and Send Level show horizontal value bars. To follow selections made with the mouse, enable **Control surface follows track selection** in Logic’s Control Surfaces settings.

### Reset a value

Hold **Delete** and touch the top of the assigned encoder. If touch doesn’t register, keep holding Delete and turn the same encoder slightly. Watch the display or Logic for the result.

| Control | Result |
| --- | --- |
| Track volume encoder | Requests Logic’s fader default. |
| Pan encoder | Returns pan to center. |
| Send encoder | Requests Logic’s default for the assigned send. |
| Big **Volume** knob | Returns **Stereo Out** to **0 dB**. |
| **Tempo** knob | Returns project tempo to **120 BPM**. |
| Smart Control or open plug-in parameter encoder | Requests the native default or toggles a switch according to Logic’s mapping. |
| Step Sequencer pad or encoder | Delete + pad clears a step. Delete + assigned encoder resets the step in the current edit mode. |

The same Delete modifier removes tracks and effects when used with their **screen buttons**. Use the encoder gesture for resetting values.

## Smart Controls, instruments and effects

1. Select a track. Use **Sounds** in the companion or press **Device** on Push to cycle Smart Controls, Instrument and Effects. **Shift + Device** goes to Effects directly.
2. Smart Controls are ready when their names and values appear. For an instrument or effect, press the screen button under **Open** for the occupied slot.
3. Turn the eight encoders to edit the displayed parameters. **Page Left / Right** changes parameter pages. In the parameter view, **Shift + Mix** refreshes page context. Use D-pad **Up / Down** to change tracks.
4. The page number stays on Push as the live values update. To find a control such as Logic Compressor’s Threshold, open **Sounds → Build parameter guide**, search for **Thresh**, then select the matching page. Logic sends abbreviated names, so try a shorter search if needed.
5. Press **Device** while editing a plug-in to return to its slot list. **Mix** takes you back to the mixer.

In the Effects slot list, hold **Mute** and press the effect’s screen button to toggle bypass. Hold **Delete** and press the same screen button to remove the effect. These commands target existing slots. Load new plug-ins through Logic or use **Add** on Push to open Logic’s plug-in search.

## Play pads and quantize

| On Push | What it does |
| --- | --- |
| **Note** | Return to instrument pads from Session or another settings view. |
| **Scale** | Open layout and root settings. Choose Chromatic, Major, Minor or Drums, then use root −/+ or the first encoder to transpose. |
| **Layout** | Cycle pad layouts. |
| **Octave Up / Down** | Transpose the instrument pad range by an octave. |
| **Accent** | Toggle full-velocity notes. |
| **Repeat** | Retrigger held notes at the selected division and displayed tempo. The companion times the repeats. |
| Right-hand division buttons | Choose the grid for Repeat and Quantize. Hold **Shift** with the **1/4** button for **1/2**. |
| **Quantize** | Apply the grid to the selected region in Logic. Select the region first. |
| Hold **Quantize**, use **Swing**, or press the **Tempo** knob | Open quantize settings. Use screen buttons or encoders to choose a division, use arrows or Page buttons to switch pages, and choose **Apply**. |

The right-hand buttons choose scenes in Session and note rows in Steps, so return to Note for the division shortcuts. The Pads panel also offers layout, root and **Panic** for releasing a stuck note.

Velocity, pressure, pitch bend and MPE expression are routed through the companion Pads port. Set Push expression and the instrument’s MPE member channels and bend range to match. Quantize sets Logic’s Region Inspector quantization for the selection. Logic’s own editors remain available for detailed note editing.

## Transport, recording and project shortcuts

| On Push | What it does |
| --- | --- |
| **Play** | Toggle play/stop. |
| **Record** | Start or stop recording using Logic’s transport. |
| **Stop Clips** | Stop Logic’s transport. In Session, **Lock + Stop Clips** uses the selected-track stop action. |
| Tap **Metronome** | Toggle the click. Hold for Metronome Settings. **Shift + tap** toggles Count In. |
| **Tap Tempo** | Tap twice or more at the desired pace. Turn the Tempo knob for whole BPM or hold **Shift** for tenths. |
| Turn big **Volume** knob | Adjust speakers connected to Push’s Out 1 and 2. The dB readout follows the knob as you turn. When you stop, the companion reads back the speaker gain and the display returns to its previous view. Select **Ableton Push 3 Audio** as the output device in Logic’s Audio settings to hear Logic through those outputs. |
| **Shift + turn** / press big **Volume** knob | Adjust Logic’s Stereo Out fader / open Logic’s Mixer. |
| **Fixed Length** | Toggle Cycle. **Shift + Fixed Length** opens bounded Tracks recording settings. |
| **Automate** | Toggle Touch/Read. **Shift + Automate** requests Read. Hold **Automate** to choose Read, Touch, Latch or Write, or show automation. Erase automation in Logic’s editor. |
| **Clip** | Open the region controls and Piano Roll. Screen buttons can quantize, repeat, set locators by selection, toggle Cycle or open Steps and Automation. |
| **Double Loop** or tap **Duplicate** | Repeat the selected region once in Logic. |
| **Capture** | Invoke Logic’s Flashback Capture. |
| **New** or **Shift + Add** | Open New Tracks. Choose Software Instrument, Mic or Line, Guitar or Bass, External MIDI, Drummer or Bass Player, then Create or Cancel on Push or in Logic. |
| **Add**, **Swap**, **Convert** | Open plug-in search, open the Browser, or convert selected regions to a new sampler track, respectively. |
| **Select** | Open Logic’s track search. |
| **Undo** / **Shift + Undo** | Undo / redo. |
| **Save** / **Shift + Save** / **Duplicate + Save** | Save / Save As / Save a Copy. |
| **Set** | Open project shortcuts for Save, Save As, Save a Copy, New, Open and Create Marker. |
| Jog wheel | Turn to move the playhead. Use its left/right controls for previous/next marker, or press it to open Go To Position. |
| **Help** / **Setup** | Show hardware help or setup shortcuts. |

To record a fixed take in Tracks, stop playback, turn Cycle off and start at a bar line. Press **Shift + Fixed Length**, select **1, 2, 4, 8 or 16 bars**, then press Record. Count In can be turned off for a predictable first test. The companion stops recording based on Logic’s reported playhead, so the stop can land slightly after the target. Choose **Off** on the same page to return to regular recording.

## Live Loops

### Set up once

Press **Session** on Push or use **Pads → Live Loops → Open Live Loops on Push** to expose the two Loops ports. In Logic’s **Control Surfaces → Setup → New → Install**, add **Launchpad X** alongside Mackie Control. Set **Orientation** to **90° Right** and assign the two Launchpad X ports from the table above. Open Logic’s Live Loops grid.

### Play and navigate

| On Push in Session | What it does |
| --- | --- |
| Tap a pad | Launch the cell at that track row and scene column. |
| Right-hand buttons top to bottom, or either screen row left to right | Launch scenes 1–8 in the current window. |
| **Up / Down** | Move one track. **Shift + Up / Down** moves eight tracks. |
| **Left / Right** | Move one scene. **Shift + Left / Right** moves eight scenes. |
| **Shift + Session** | Open Live Loops tools. |
| **Note** | Return to instrument pads. |

Empty cells are dark. Occupied pads show the nearest Push palette match to the clip color Logic sends. Queued cells flash green and playing cells pulse green. Logic handles when launches happen.

### Record and edit cells

Select one cell or scene in Logic. In **Shift + Session**, the arrows move the selection and the screen buttons act on it.

| Page | Controls |
| --- | --- |
| Performance | **Stop Grid**, **Stop Track**, **Queue**, **Retrigger**, **Record**, **Capture**, **Edit**, **Back**. Stop Track needs a visible empty slot on the selected track. Retrigger uses Logic’s default key command and needs the grid in focus. |
| Edit | **Repeat**, **Shift + Clear**, **Loop**, **Rec-Length**, **Rec Mode**, **Rec End**, **Perform**, **Back**. Repeat duplicates content, and Loop toggles looping. |

Use **Record** on an empty cell. To record over an occupied cell, set **Rec Mode** to Replace first. For a bounded cell recording, set its numeric length in Logic, choose **Rec-Length → Cell Length**, then **Rec End → Play Cell**. Numeric cell and loop lengths are edited in Logic’s Cell inspector. To capture a performance to the timeline, use **Capture** to enable Logic’s Performance Recording, press Record, launch clips and scenes, then stop and check the Tracks area.

## Step Sequencer

1. Select a native pattern region in Logic. Press **Shift + Clip** to enter Steps. Keep the Logic project and its Step Sequencer visible for the feedback capture.
2. In Logic’s **On/Off** edit mode, tap a pad to toggle a step. The top-left pad is step 1 of the first visible note row. Active steps are red. Inactive or unreadable steps are dark. Push taps update the lights immediately once the step state is known. Mouse edits are reflected as Logic’s window is read.
3. Use **Up / Down** to scroll one row and **Shift + Up / Down** to scroll eight. Use **Left / Right** or **Page Left / Right** to move eight steps across. Use the right-hand buttons to select a visible note row. The rightmost screen button toggles Preview.
4. Choose **Velocity**, **Gate**, **Chance** or **Start Offset** in Logic. Tap a pad to choose its row, then turn the encoder for the step column. **Delete + pad** clears a step. **Delete + touch** or **Delete + turn** on an encoder resets the current step value when Logic supports it.
5. Press **Note** to play instrument pads again, or **Mix** to return to mixer control.

## Switch back to Ableton

1. Click **Switch to Ableton** in the companion, or use **⌘⇧A** with the companion focused.
2. Wait for the release to finish. The companion sends note-offs, releases its MIDI and USB display connection, and returns Push to Live Mode.
3. Open Ableton Live. Confirm its native display, pads, buttons and lights respond. To go back to Logic, quit Live normally, then click **Launch & Connect** again.

## Updates and troubleshooting

- **Update the app.** Choose **Check for Updates…** in the app or menu bar. The updater verifies the installer against the release checksum and puts it in Downloads. Quit the app and run that installer. Automatic checks are enabled by default and can be turned off in the Updates panel.
- **Push is detected but Logic has no feedback.** Check the Mackie input and output against the ports table and confirm Logic’s control surfaces are enabled. Keep the Mackie entry assigned to the companion’s Control and Feedback ports. A leftover test surface is unnecessary for this setup. Keep any separate surface you intentionally use for other gear.
- **A mixer strip says Awaiting or a send doesn’t respond.** Open More mixer options to reapply the mixer assignment. In Sends view, verify the shown send slot exists on that Logic strip. After switching banks, give Logic time to report the new strips.
- **Pads don’t play or play twice.** Press Note, select a software instrument and verify that the track receives the companion Pads source. Remove direct raw Push MIDI from the track’s musical input. Use **Panic** if notes get stuck.
- **The screen doesn’t connect.** Verify USB and Control Live mode, quit Live if it’s open, then use the screen reconnect control in Advanced. You can use MIDI controls without the screen.
- **Native actions or Step LEDs stop after an update.** Check Accessibility and Screen Recording for the installed copy and relaunch after approving them. The current signing setup can cause macOS to ask again. Open and expose the actual pattern editor for Step LEDs. Some editing actions depend on Logic’s English menu labels or default key commands.
- **The hardware was unplugged or the Mac slept.** Reconnect by USB and use **Launch & Connect**. **Advanced → Connection diagnostics** shows which stage has completed.
- **A button behaves differently from the guide.** These are the factory companion mappings. **Advanced → Custom button mappings** offers Learn, Test and Restore Push defaults. Learned mappings override the defaults.
