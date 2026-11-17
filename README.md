# Morrow

*A better way to begin tomorrow.*

Morrow is a calm Christian wake-up app, made for Romania, in English and Romanian (and German and Swiss German in the app). The iPhone app is where the alarm lives: gentle wake missions, a wake streak, bedtime and the morning after. On a computer, Morrow keeps you company through the day: Focus, Today, Ask Morrow and Talk to Morrow, with the verse of the day from a real Bible text, never invented or paraphrased.

This repository holds only the desktop installers. Website: https://levi-gavril.github.io/morrow-site/

## Download

Always the newest version:

| Computer | Installer |
|---|---|
| Windows 10 and 11, 64-bit (most PCs) | [Morrow-Setup-x64.exe](https://github.com/levi-gavril/morrow-releases/releases/latest/download/Morrow-Setup-x64.exe) |
| Mac with Apple silicon (M1 to M5) | [Morrow-Mac-arm64.dmg](https://github.com/levi-gavril/morrow-releases/releases/latest/download/Morrow-Mac-arm64.dmg) |
| Mac with an Intel processor | [Morrow-Mac-x64.dmg](https://github.com/levi-gavril/morrow-releases/releases/latest/download/Morrow-Mac-x64.dmg) |

Every version is on the [Releases](https://github.com/levi-gavril/morrow-releases/releases) page.

**Windows on ARM** is not in this release: Morrow Agent and the built-in voices need an x64 PC for now.

**iPhone:** coming soon to the App Store.

## The first time you open it

- **Windows:** the installer is not signed yet, so Windows says "Windows protected your PC". Choose **More info**, then **Run anyway**. Morrow installs for you alone, without admin rights. Installed copies update themselves: a new version downloads quietly and is installed the next time Morrow quits.
- **Mac:** open the .dmg and drag Morrow to Applications. The app is not signed with an Apple Developer ID yet, so the first time macOS says Morrow cannot be opened: go to **System Settings**, then **Privacy & Security**, and choose **Open Anyway**. Mac copies do not update themselves yet: download each new version here.
- **Morrow's voices, speech recognition and Morrow Agent** (the small AI that runs on your computer) are downloaded once, when you say so, a few gigabytes. Until then Morrow speaks with its recorded voice packs. After that, they work without the internet.
- **On a Mac**, the built-in voices and speech recognition are not there yet. Morrow speaks with its recorded voice packs or the system voice, and you write to Morrow instead of talking.
- The desktop app does not ring alarms. The phone does.

## Your data

Everything stays on your computer. No account is needed. Morrow goes online only for what you turn on (the weather, a cloud model you connect with your own key, the model downloads, the day's Romanian verse read online) and, on Windows, to check this page for a new version.

## Licences and credits

**Scripture.** The bundled Bibles are public domain, from eBible.org: World English Bible, King James Version (Crown copyright applies in the UK), Berean Standard Bible, Biblia Liberă (New Testament) and Lutherbibel 1912. In Romanian the day's verse can also be read online, one verse a day, from [getBible](https://getbible.net) (Cornilescu 1924) and [bolls.life](https://bolls.life) (NTR and Cornilescu 1931). Those texts are fetched by the app for that one verse and never bundled.

**Morrow Agent.** Google's Gemma 4 instruct models (E2B and 12B, GGUF conversions by Unsloth), Apache-2.0, downloaded by the app at first run. They run with [llama.cpp](https://github.com/ggml-org/llama.cpp), MIT.

**Speech recognition.** [whisper.cpp](https://github.com/ggml-org/whisper.cpp), MIT, with OpenAI's Whisper large-v3 turbo, MIT, and the Silero VAD, MIT. On computers without an NVIDIA graphics card: NVIDIA's Parakeet TDT 0.6B v3, CC-BY-4.0 (conversion by ggml-org). The models are downloaded by the app at first run. NVIDIA's CUDA runtime, for graphics cards that use it, is downloaded under NVIDIA's redistribution terms and is not in the installer.

**Built-in voices.** [omnivoice.cpp](https://github.com/ServeurpersoCom/omnivoice.cpp) and ggml, MIT. The OmniVoice weights by k2-fsa are licensed CC-BY-NC 4.0 (the GGUF conversion by Serveurperso is Apache-2.0). Morrow is free and uses them non-commercially. The app downloads them from their source, Hugging Face, at first run; they are never in an installer.

**Weather.** [Open-Meteo](https://open-meteo.com), CC-BY 4.0, when you turn the weather on.

**Voices, sounds and music.** Morrow's recorded voices, ringtones, nature sounds and music were made with [ElevenLabs](https://elevenlabs.io) and [Cartesia](https://cartesia.ai).

**App.** Built with Electron (MIT). Copyright © 2026 Morrow.
