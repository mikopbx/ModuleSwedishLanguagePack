# ModuleSwedishLanguagePack

Complete Swedish language pack for MikoPBX including UI translations and voice prompts.

## What's Included

- **Voice Prompts**: Swedish voice prompts for system menus, greetings, and notifications
- **UI Translations**: Complete Swedish translation of MikoPBX admin interface

## Installation

1. Download and install the module from MikoPBX Marketplace
2. Enable the module in **Modules** section
3. Go to **General Settings** and select Swedish (Svenska) as the system language

## Requirements

- MikoPBX 2025.1.1 or later

## TTS Attribution

A subset of voice prompts (47 prompts that were missing from the upstream
Asterisk Swedish sound set) was synthesized locally using neural TTS:

- **Engine**: [Piper TTS](https://github.com/rhasspy/piper)
- **Voice model**: `sv_SE-nst-medium` (from
  [rhasspy/piper-voices](https://huggingface.co/rhasspy/piper-voices/tree/main/sv/sv_SE/nst/medium))
- **Sample rate**: 22050 Hz, mono, 16-bit PCM WAV

The text used for each TTS-generated prompt is recorded in
`Sounds/core-sounds-sv-sv.txt` for transparency and regeneration.

On module installation, MikoPBX automatically converts WAV files to all Asterisk
formats (ulaw, alaw, gsm, g722, sln) for codec compatibility.

## License

- Module code: GNU General Public License v3.0
- Sound files: CC BY-SA 4.0 (Asterisk Sound Files)
- TTS-generated prompts: CC BY-SA 4.0 (Piper TTS, https://github.com/rhasspy/piper)

## Copyright

- Module development: © 2017-2026 Alexey Portnov and Nikolay Beketov
- Voice prompts: From official Asterisk release; supplementary prompts
  generated using open-source Piper TTS models
