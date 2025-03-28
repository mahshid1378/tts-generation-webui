<h1 align="center">TTS Generation WebUI / Harmonica</h1>

<div align="center">

  <h3 align="center">
 ||
  [Installation](#installation) ||
  [Docker Setup](#docker-setup) ||
  [Feedback / Bug reports](https://forms.gle/2L62owhBsGFzdFBC8)
  
  </h3>

  [![GitHub stars](https://img.shields.io/github/stars/rsxdalv/tts-generation-webui?style=social)]
  [![GitHub](https://img.shields.io/github/license/rsxdalv/tts-generation-webui)]
  [![Discord](https://img.shields.io/discord/1258772280071295018?label=discord&logo=discord&logoColor=white)](https://discord.gg/V8BKTVRtJ9)
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rsxdalv/tts-generation-webui/blob/main/notebooks/google_colab.ipynb)
  [![GitHub forks](https://img.shields.io/github/forks/rsxdalv/tts-generation-webui?style=social)]

</div>

<div align="center">

## Videos

</div>

| [![Watch the video](https://img.youtube.com/vi/Y8J717tr9t0/sddefault.jpg)](https://youtu.be/Y8J717tr9t0) | [![Watch the video](https://img.youtube.com/vi/ScN2ypewABc/sddefault.jpg)](https://youtu.be/ScN2ypewABc) | [![Watch the video](https://img.youtube.com/vi/JXojhFjZ39k/sddefault.jpg)](https://youtu.be/JXojhFjZ39k) |
| :------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------: |

<div align="center">

## Models

| Text-to-speech                | Audio/Music Generation       | Audio Conversion/Tools        |
|-------------------------------|------------------------------|-------------------------------|
| [Bark] | [MusicGen] | [RVC] |
| [Tortoise] | [MAGNeT] | [Demucs] |
| [Maha TTS]| [Stable Audio] | [Vocos] |
| [MMS] | [(Extension) Riffusion] | [Whisper] |
| [Vall-E X] | [(Extension) AudioCraft Mac] | 
| [StyleTTS2] | [(Extension) AudioCraft Plus] | 
| [SeamlessM4T] | | |
| [(Extension) XTTSv2] | | |
| [(Extension) MARS5] | | |
| [(Extension) F5-TTS] | | |
| [(Extension) Parler TTS]| | |

</div>

<div align="center">

## Examples

</div>


| <video src="https://github.com/user-attachments/assets/16ac948a-fe98-49ad-ad87-19c41fe7e65e" width="300"></video> | <video src="https://github.com/user-attachments/assets/55bde4f7-bbcc-4ecf-8f94-b315b9d22e74" width="300"></video> | <video src="https://github.com/user-attachments/assets/fcee8906-a101-400d-8499-4e72c7603042" width="300"></video> |
| :-----------------------------------------: | :-----------------------------------------: | :-------------------------------: |

<div align="center">

## Screenshots

</div>

| ![react_1](./documentation/screenshots/react_ui%20(1).png) | ![react_2](./documentation/screenshots/react_ui%20(2).png) | ![react_3](./documentation/screenshots/react_ui%20(3).png) |
| :-----------------------------------------: | :-----------------------------------------: | :-------------------------------: |

| ![gradio_1](./documentation/screenshots/gradio%20(1).png) | ![gradio_2](./documentation/screenshots/gradio%20(2).png) | ![gradio_3](./documentation/screenshots/gradio%20(3).png) |
| :-----------------------------------------: | :-----------------------------------------: | :-------------------------------: |

## Changelog

Mar 21:
* Add CosyVoice extension [Unstable] and GPT-SoVITS [Alpha] extension

Mar 20:
* Add executable macOS script for double-click launching
* Add unstable CosyVoice extension

Mar 18:
* Remove old rvc files
* Fix missing torchfcpe dependency for RVC

Mar 17:
* Upgrade Google Colab to PyTorch 2.6.0, add Conda to downgrade Python to 3.10
* No longer abort when the automatic update fails to fetch the new code (Improving offline support #457)
* Upgrade Tortoise to v3.0.1 for transformers 4.49.0 #454
* Prevent running in Windows/System32 folder #459

## February 2025

Feb 15:
* Fix Stable Audio to match the new version

Feb 14:
* Pin accelerate>=0.33.0 project wide
* Add basic Seamless M4T quantization code

Feb 13:
* Fix Stable Audio and Seamless M4T incompatibility
* Make Seamless M4T automatically use CUDA if available, otherwise CPU

Feb 10:
* Improve installation instructions in README

## January 2025


## December 2024

Dec 17:
* Attempt fix of #429, #428, #427

## November 2024

Nov 23:
* Add linux fairseq wheel for better pip compatibility.

Nov 22:
* Switch to wheels, add one-shot install prompt.

Nov 15:
* upgrade to gradio 5.5.0, add Resemble Enhance (#420)

Nov 14:
* Add experimental Windows deepspeed wheel.
* Add more languages to Bark voice clone.

Nov 11:
* Switch to a fixed fairseq version for windows reducing installation conflicts and speeding up updates.

## October 2024

<details>
<summary>Click to expand</summary>

Oct 28:
* Added installer tests, model downloader, and pip CPU-only option for Torch.

Oct 24:
* Downgraded Gradio to 5.1.0 due to a bug.
* Added test workflows and fixed minor bugs.

Oct 22:
* Fixed Dockerfile issues for smoother deployment.

Oct 21:
* Redesigned README: improved Whisper extension, added changelogs for August, September, and October, updated screenshots, and reorganized content.

Oct 19:
* Fixed extension logs and added new extensions.

Oct 18:
* System improvements: formatted project, fixed `xformers+cuda` install, added log system, uninstall extension button, and F5 TTS extension.

Oct 16:
* First install now uses `pip` instead of `uv`.
* Bumped major version and fixed Google Colab.
* Added pip fallback to stable audio.
* Fixed Demucs, changed Postgres port.
* Fixed `huggingface_hub` install and Bark model loader.
* Major upgrades: switched to Gradio 5, lazy loading for tabs, Docker fixes, optimized UI speed, added .env.user feature, improved logs, and upgraded React UI extensions.

Oct 3:
* Fixed GPU info tab and added `nvidia-ml-py`.
* Created workaround for Audiocraft install bug.
* Fixed automatic MSVC install and set server to `127.0.0.1`.
* Fixed `.git_version` path and removed `iconv` to eliminate `node-gyp` requirement.
* Improved installer error handling, added upgrade hash logging.
* Upgraded Node.js to 22.9.0, added PostgreSQL support, grouped tabs in React UI.

</details>


## September 2024

<details>
<summary>Click to expand</summary>

Sep 23:
* Automatically use CUDA for MMS.

Sep 22:
* Added ffmpeg metadata extension to React UI.
* Added mono-only notice for Maha TTS.
* Hotfix to avoid Node 20.17.0 installation failure.

Sep 21:
* Added stable audio demo to React UI.
* Improved UI layout.

Sep 19:
* Upgraded React UI visual look with new Sliders and better layout.
* Optimized RVC UI, fixed Colab, and added a search command box.
* Upgrade Node.js to 20.17.0.

Sep 2:
* Fixed Dockerfile and updated docker-compose.yml.
* Fixed bug in npz loading.

</details>


## August 2024

<details>
<summary>Click to expand</summary>

Aug 31:
* Upgrade model inference framework to decorators.
* Moved Python files from `src` to `tts_webui` folder.
* Rewrote the MusicGen tab and fixed related bugs.

Aug 20:
* Upgraded to Gradio 4 and added theme.
* Added model loading messages for Tortoise.
* Fixed ReactUI's RVC.
* Refactored hyperparameters.
* Added management to extensions list, XTTS-Simple extension.

Aug 5:
* Fix Bark in React UI, add Max Generation Duration.
* Change AudioCraft Plus extension models directory to ./data/models/audiocraft_plus/
* Improve model unloading for MusicGen and AudioGen. Add unload models button to MusicGen and AudioGen.
* Add Huggingface Cache Manager extension.

Aug 4:
* Add XTTS-RVC-UI extension, XTTS Fine-tuning demo extension.

Aug 3:
* Add Riffusion extension, AudioCraft Mac extension, Bark Legacy extension.

Aug 2:
* Add deprecation warning to old installer.
* Unify error handling and simplify tab loading.

Aug 1:
* Add "Attempt Update" button for external extensions.
* Skip reinstalling packages when pip_packages version is not changed.
* Synchronize Gradio Port with React UI.
* Change default Gradio port to 7770 from 7860.

</details>

## July 2024

<details>
<summary>Click to expand</summary>

July 31:
* Fix React UI's MusicGen after the Gradio changes.
* Add unload button to Whisper extension.

July 29:
* Change FFMpeg to 4.4.2 from conda-forge in order to support more platforms, including Mac M1.
* Disable tortoise CVVP.

July 26:
* Whisper extension
* Experimental AMD ROCM install support. (Linux only)

July 25:
* Add diagnostic scripts for MacOS and Linux.
* Add better error details for tabs.
* Fix .sh script execution permissions for the installers on Linux and MacOS.

July 21:
* Add Gallery History extension (adapted from the old gallery view)
* Convert Simple Remixer to extension
* Fix update.py to use the newer torch versions (update.py is only for legacy purposes and will likely break)
* Add Diagnostic script and Force Reinstall scripts for Windows.

July 20:
* Fix Discord join link
* Simplify Bark further, removing excessive complexity in code.
* Add UI/Modular extensions, these extensions allow installing new models and features to the UI. In the future, models will start as extensions before being added permamently.
* Disable Gallery view in outputs
* Known issue: Firefox fails at showing outputs in Gradio, it fails at fetching them from backend. Within React UI this works fine.

July 15:
* Comment - As the React UI has been out for a long time now, Gradio UI is going to have the role of serving only the functions to the user, without the extremely complicated UI that it cannot handle. There is a real shortage of development time to add new models and features, but the old style of integration was not viable. As the new APIs and 'the role of the model' is defined, it will be possible to have extensions for entire models, enabling a lot more flexibility and lighter installations.
* Start scaling back Gradio UI complexity - removed _send to RVC/Demucs/Voice_ buttons. (Remove internal component Joutai).
* Add version.json for better updates in the future.
* Reduce Gradio Bark maximum number of outputs to 1.
* Add unload model button to Tortoise, also unload the model before loading the next one/changing parameters, thus tortoise no longer uses 2x model memory during the settings change.

July 14:
* Regroup Gradio tabs into groups - Text to Speech, Audio Conversion, Music Generation, Outputs and Settings
* Clean up the header, add link for feedback
* Add seed control to Stable Audio
* Fix Stable Audio filename bug with newlines
* Disable "Simple Remixer" Gradio tab
* Fix bark voice clone & RVC once more
* Add "Installed Packages" tab for debugging

July 13:
* Major upgrade to Torch 2.3.1 and xformers 0.0.27
  * All users, including Mac and CPU will now have the same PyTorch version.
* Upgrade CUDA to 11.8
* Force python to be 3.10.11
* Modify installer to allow upgrading Python and Torch without reinstalling (currently major version 2)
* Fix magnet default params for better quality
* Improve installer script checks to avoid bugs
* Update StyleTTS2

July 11:
* Improve Stable Audio generation filenames
* Add force reinstall to torch repair
* Make the installer auto-update before running

July 8:
* Change the installation process to reduce package clashes and enable torch version flexibility.

July 6:
* Initial release of new mamba based installer.
* Save Stable Audio results to outputs-rvc/StableAudio folder.
* Add a disclaimer to Stable Audio model selection and show better error messages when files are missing.

July 1:
* Optimize Stable Audio memory usage after generation.
* Open React UI automatically only if gradio also opens automatically.
* Remove unnecessary conda git reinstall.
* Update to lastest Stable Audio which has mps support (requires newer torch versions).

</details>

## June 2024

<details>
<summary>Click to expand</summary>
June 22:
* Add Stable Audio to Gradio.

June 21:
* Add Vall-E-X demo to React UI.
* Open React UI automatically in browser, fix the link again.
* Add Split By Length to React/Tortoise.
* Fix UVR5 demo folders.
* Set fairseq version to 0.12.2 for Linux and Mac. (#323)
* Improve generation history for all React UI tabs.

May 17:
* Fix Tortoise presets in React UI.

May 9:
* Add MMS to React UI.
* Improve React UI and codebase.

May 4:
* Group Changelog by month

</details>

## April 2024


<details>
<summary>Click to expand</summary>
Apr 28:
* Add Maha TTS to React UI.
* Add GPU Info to React UI.

Apr 6:
* Add Vall-E-X generation demo tab.
* Add MMS demo tab.
* Add Maha TTS demo tab.
* Add StyleTTS2 demo tab.

Apr 5:
* Fix RVC installation bug.
* Add basic UVR5 demo tab.

Apr 4:
* Upgrade RVC to include RVMPE and FCPE. Remove the direct file input for models and indexes due to file duplication. Improve React UI interface for RVC.

</details>

## March 2024

<details>
<summary>Click to expand</summary>

Mar 28:
* Add GPU Info tab

Mar 27:
* Add information about voice cloning to tab voice clone

Mar 26:
* Add Maha TTS demo notebook

Mar 22:
* Vall-E X demo via notebook (#292)
* Add React UI to Docker image
* Add install disclaimer

Mar 16:
* Upgrade vocos to 0.1.0

Mar 14:
* StyleTTS2 Demo Notebook

Mar 13:
* Add Experimental Pipeline (Bark / Tortoise / MusicGen / AudioGen / MAGNeT -> RVC / Demucs / Vocos) (#287)
* Fix RVC bug with model reloading on each generation. For short inputs that results in a visible speedup.

Mar 11:
* Add Play as Audio and Save to Voices to bark (#286)
* Change UX to show that files are deleted from favorites
* Fix images for bark voices not showing
* Fix audio playback in favorites

Mar 10:
* Add Batching to React UI Magnet (#283)
* Add audio to audio translation to SeamlessM4T (#284)

Mar 3:
* Add MMS demo as a notebook
* Add MultiBandDiffusion high VRAM disclaimer

</details>

## February 2024

<details>
<summary>Click to expand</summary>

Feb 21:
* Fix Docker container builds and bug with Docker-Audiocraft
</details>

## January 2024

<details>
<summary>Click to expand</summary>

Jan 21:
* Add CPU/M1 torch auto-repair script with each update. To disable, edit check_cuda.py and change FORCE_NO_REPAIR = True

Jan 16:
* Upgrade MusicGen, adding support for stereo and large melody models
* Add MAGNeT

Jan 15:
* Upgraded Gradio to 3.48.0
  * Several visual bugs have appeared, if they are critical, please report them or downgrade gradio.
  * Gradio: Suppress useless warnings
* Supress Triton warnings
* Gradio-Bark: Fix "Use last generation as history" behavior, empty selection no longer errors
* Improve extensions loader display
* Upgrade transformers to 4.36.1 from 4.31.0
* Add SeamlessM4T Demo

Jan 14:
* React UI: Fix missing directory errors

Jan 13:
* React UI: Fix missing npm build step from automatic install

Jan 12:
* React UI: Fix names for audio actions
* Gradio: Fix multiple API warnings
* Integration - React UI now is launched alongside Gradio, with a link to open it

Jan 11:
* React UI: Make the build work without any errors

Jan 9:
* React UI
  * Fix 404 handler for Wavesurfer
  * Group Bark tabs together

Jan 8:
* Release React UI

</details>

## Upgrading (For old installations)
*In case of issues, feel free to contact the developers*.

<details>
<summary>Click to expand</summary>

### Upgrading from v6 to new installer

#### Recommended: Fresh install
* Download the [new version] and run the start_tts_webui.bat (Windows) or start_tts_webui.sh (MacOS, Linux)
* Once it is finished, close the server.
* Recommended: Copy the old generations to the new directory, such as favorites/ outputs/ outputs-rvc/ models/ collections/ config.json
* With caution: you can copy the whole new tts-generation-webui directory over the old one, but there might be some old files that are lost.

#### In-place upgrade, can delete some files, tweaks
* Update the existing installation using the update_*platform* script
* After the update run the new start_tts_webui.bat (Windows) or start_tts_webui.sh (MacOS, Linux) inside of the tts-generation-webui directory
* Once the server starts, check if it works.
* With caution: if the new server works, within the one-click-installers directory, delete the old installer_files.

#### *Is there any more optimal way to do this?*

Not exactly, the dependencies clash, especially between conda and python (and dependencies are already in a critical state, moving them to conda is ways off). Therefore, while it might be possible to just replace the old installer with the new one and running the update, the problems are unpredictable and **unfixable**. Making an update to installer requires a lot of testing so it's not done lightly.

</details>

## Installation
* Download the [latest version] and extract it.
* Run start_tts_webui.bat or start_tts_webui.sh to start the server. It will ask you to select the GPU/Chip you are using. Once everything has installed, it will start the Gradio server at http://localhost:7770 and the React UI at http://localhost:3000.
* Output log will be available in the installer_scripts/output.log file.
* Note: The start script sets up a conda environment and a python virtual environment. Thus you don't need to make a venv before that, and in fact, launching from another venv might break this script.

### Manual installation (not recommended)
* These instructions might not reflect all of the latest fixes and adjustments, but could be useful as a reference for debugging or understanding what the installer does. Hopefully they can be a basis for supporting new platforms, such as AMD/Intel.

* Install conda (https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)
  * (Windows) Install Visual Studio compiler / Visual Studio Build Tools https://visualstudio.microsoft.com/visual-cpp-build-tools/
* Set up an environment: `conda create -n venv`
* Install git, node.js `conda install -y -c conda-forge git python=3.10.11 conda-forge::nodejs=22.9.0 conda pip==23.3.2 conda-forge::uv=0.4.17 conda-forge::vswhere`
* a) Either Continue with the installer script
  * activate the environment: `conda activate venv` and
  * (venv) `node installer_scripts\init_app.js`
  * then run the server with (venv) `python server.py`
* b) Or install the requirements manually
  * Set up pytorch with CUDA or CPU (https://pytorch.org/audio/stable/build.windows.html#install-pytorch):
    * (venv) `conda install -y -k conda-forge::uv=0.4.17 conda-forge::vswhere  conda-forge::postgresql=16.4 conda-forge::nodejs=22.9.0 conda-forge::ffmpeg=4.4.2[build=lgpl*] pytorch=2.3.1 torchvision torchaudio cpuonly  -c pytorch` for CPU/Mac
    * (venv) `conda install -y -k conda-forge::uv=0.4.17 conda-forge::vswhere  conda-forge::postgresql=16.4 conda-forge::nodejs=22.9.0 conda-forge::ffmpeg=4.4.2[build=lgpl*] pytorch[version=2.3.1,build=py3.10_cuda11.8.*] pytorch-cuda=11.8 torchvision torchaudio cuda-toolkit ninja  -c pytorch -c nvidia/label/cuda-11.8.0 -c nvidia` for CUDA
  * Clone the repo: `git clone https://github.com/rsxdalv/tts-generation-webui.git`
  * Install the requirements:
    * install all the requirements*.txt (this list might not be up to date, check ):
      * (venv) `pip install -r requirements.txt`
      * (venv) `pip install -r requirements_audiocraft.txt`
      * (venv) `pip install -r requirements_bark_hubert_quantizer.txt`
      * (venv) `pip install -r requirements_rvc.txt`
      * (venv) `pip install hydra-core==1.3.2`
      * (venv) `pip install -r requirements_styletts2.txt`
      * (venv) `pip install -r requirements_vall_e.txt`
      * (venv) `pip install -r requirements_maha_tts.txt`
      * (venv) `pip install -r requirements_stable_audio.txt`
      * (venv) `pip install soundfile==0.12.1`
      * (venv) `pip install nvidia-ml-py`
    * build the react app: (venv) `cd react-ui && npm install && npm run build`
  * (optional) setup the database: (venv) `node installer_scripts/js/applyDatabaseConfig.js`
  * run the server: (venv) `python server.py`


#### React UI

* Install nodejs (if not already installed with conda)
* Install react dependencies: `npm install`
* Build react: `npm run build`
* Run react: `npm start`
* Also run the python server: `python server.py` or with `start_tts_webui` script

### Docker Setup

tts-generation-webui can also be ran inside of a Docker container. Using CUDA inside of docker requires (NVIDIA Container Toolkit)[https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html]. To get started, pull the image from GitHub Container Registry:

```
docker pull ghcr.io/rsxdalv/tts-generation-webui:main
```

Once the image has been pulled it can be started with Docker Compose:
The ports are 7770 (env:TTS_PORT) for the Gradio backend and 3000 (env:UI_PORT) for the React front end.

```
docker compose up -d
```

The container will take some time to generate the first output while models are downloaded in the background. The status of this download can be verified by checking the container logs:

```
docker logs tts-generation-webui
```

#### Building the image yourself
If you wish to build your own docker container, you can use the included Dockerfile:

```
docker build -t tts-generation-webui .
```
Please note that the docker-compose needs to be edited to use the image you just built.

## Ethical and Responsible Use
This technology is intended for enablement and creativity, not for harm.

By engaging with this AI model, you acknowledge and agree to abide by these guidelines, employing the AI model in a responsible, ethical, and legal manner.
- Non-Malicious Intent: Do not use this AI model for malicious, harmful, or unlawful activities. It should only be used for lawful and ethical purposes that promote positive engagement, knowledge sharing, and constructive conversations.
- No Impersonation: Do not use this AI model to impersonate or misrepresent yourself as someone else, including individuals, organizations, or entities. It should not be used to deceive, defraud, or manipulate others.
- No Fraudulent Activities: This AI model must not be used for fraudulent purposes, such as financial scams, phishing attempts, or any form of deceitful practices aimed at acquiring sensitive information, monetary gain, or unauthorized access to systems.
- Legal Compliance: Ensure that your use of this AI model complies with applicable laws, regulations, and policies regarding AI usage, data protection, privacy, intellectual property, and any other relevant legal obligations in your jurisdiction.
- Acknowledgement: By engaging with this AI model, you acknowledge and agree to abide by these guidelines, using the AI model in a responsible, ethical, and legal manner.

## License

### Codebase and Dependencies

The codebase is licensed under MIT. However, it's important to note that when installing the dependencies, you will also be subject to their respective licenses. Although most of these licenses are permissive, there may be some that are not. Therefore, it's essential to understand that the permissive license only applies to the codebase itself, not the entire project.

That being said, the goal is to maintain MIT compatibility throughout the project. If you come across a dependency that is not compatible with the MIT license, please feel free to open an issue and bring it to our attention.

Known non-permissive dependencies:
| Library     | License           | Notes                                                                                     |
|-------------|-------------------|-------------------------------------------------------------------------------------------|
| encodec     | CC BY-NC 4.0      | Newer versions are MIT, but need to be installed manually                                  |
| diffq       | CC BY-NC 4.0      | Optional in the future, not necessary to run, can be uninstalled, should be updated with demucs |
| lameenc     | GPL License       | Future versions will make it LGPL, but need to be installed manually                      |
| unidecode   | GPL License       | Not mission critical, can be replaced with another library, issue: https://github.com/neonbjb/tortoise-tts/issues/494 |


### Model Weights
Model weights have different licenses, please pay attention to the license of the model you are using.

Most notably:
- Bark: MIT
- Tortoise: *Unknown* (Apache-2.0 according to repo, but no license file in HuggingFace)
- MusicGen: CC BY-NC 4.0
- AudioGen: CC BY-NC 4.0


## Compatibility / Errors

Audiocraft is currently only compatible with Linux and Windows. MacOS support still has not arrived, although it might be possible to install manually.

### Torch being reinstalled

Due to the python package manager (pip) limitations, torch can get reinstalled several times. This is a wide ranging issue of pip and torch.

### Red messages in console
These messages:
```
---- requires ----, but you have ---- which is incompatible.
```
Are completely normal. It's both a limitation of pip and because this Web UI combines a lot of different AI projects together. Since the projects are not always compatible with each other, they will complain about the other projects being installed. This is normal and expected. And in the end, despite the warnings/errors the projects will work together.
It's not clear if this situation will ever be resolvable, but that is the hope.
