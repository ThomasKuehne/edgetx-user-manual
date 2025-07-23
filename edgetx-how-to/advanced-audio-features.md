---
description: Model Independent and Model Dependent audio!
---

# Advanced Audio Features

## Model Independent

These are the sounds that are not special to any specific model, and are located in `/SOUNDS/language` and `/SOUNDS/language/SYSTEM` on your radio's SD card/on-board storage when correctly configured.&#x20;

The files in `/SOUNDS/language/SYSTEM` are automatically played by the radio in response to specific events, such as turning the radio on, telemetry being lost, switches being in the wrong position, etc.&#x20;

You can also add `Play Track` Global Functions that will play in response to whatever trigger condition you wish.&#x20;

## Model Dependent

These are the sounds that are specific to a  given model, and are located in `/SOUNDS/language` and `/SOUNDS/language/model_name` on your radio's SD card/on-board storage when correctly configured.\
\
The files in `/SOUNDS/language` are available for use with Play Track Special Functions, and will play in response to whatever trigger condition you configure.

In addition to the `Play Track` Special Function, there is also the ability to configure audio be played by simply placing audio files into a directory with the same name as the model.&#x20;

For example, for English, with a model named `Ruxus 5`, you would create a folder named `/SOUNDS/en/Ruxus_5/` (note the need to replace spaces with underscores).&#x20;

Then, just create/copy audio files (of the correct format!) for any of the following trigger events into that folder.&#x20;

### Model Load

Will be played after the switch checks after turning the radio on, or after changed to a new model.&#x20;

Filename: `name.wav`&#x20;

### Switches

Will be played on a change of position of the switch.&#x20;

Filename structure: `switchID-position.wav`

* `SA-up.wav`
* `SA-mid.wav` (if position present)
* `SA-down.wav`

### Multipos / Stepped Switches

Will be played on a change of position of the switch.&#x20;

Filename structure (hyphens only for clarity): `P-switchNumber-position.wav`

* `P11.wav`  (Pot 1, position 1)
* `P16.wav`  (Pot 1, position 6)
* `P24.wav`  (Pot 2, position 4)

### Logical Switches

Will be played when the logical switch changes state.

Filename structure: `switchID-condition.wav`

* `L1-up.wav` (true)
* `L1-down.wav` (false)

### Flight Modes

Will be played on entering or exiting flight mode.&#x20;

Filename structure: `modeName-condition.wav` (Note: No spaces in the flight mode name)

* `ABC–off.wav`
* `ABC–on.wav`



