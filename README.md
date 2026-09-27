<div align="center">
  <img src="assets/brand/banner.png" alt="Kaan YILDIZ project portfolio banner" width="100%" />
</div>

<h1 align="center">Kaan YILDIZ</h1>

<p align="center">
  <strong>Independent Software Developer</strong><br />
  Unreal Engine · Real-time AI · C++ · Python · Developer & Design Tools
</p>

<p align="center">
  <a href="https://kaanyildiz.com">Portfolio</a> ·
  <a href="https://linkedin.com/in/kaan-oruc-yildiz">LinkedIn</a> ·
  <a href="mailto:kaanyildizhouse@hotmail.com">Email</a>
</p>

## Featured Project — Secret of Chronicles

**Gameplay — Unreal Engine 5.8**

https://github.com/user-attachments/assets/55694b13-0928-4e7d-bb70-94260f6b9ef3

**Real-time AI dialogue — generated voice and facial animation**

https://github.com/user-attachments/assets/472ee16a-4e15-48f8-a57f-3e21415358c1

<p align="center">
  <a href="https://kaanyildiz.com/#showcase"><strong>See Secret of Chronicles on my website →</strong></a>
</p>

An independent neo-noir detective game built with Unreal Engine 5.8. Players can question NPCs freely: **TextGen** uses an LLM to write scenario- and gameplay-aware replies, **SpeechGen** generates their voice and synchronized mouth and facial animation at runtime, and **ConvCore** validates and manages the full exchange.

The real-time AI dialogue pipeline is complete; world placement and scenario implementation continue. Steam App ID setup is complete, and the Steam page and wishlist are planned for the vertical slice.

## Unreal Engine Plugins — AI, Speech, Facial Animation, Level Design & Tools

<details>
<summary><strong>SpeechGen</strong> <small>· Click to expand</small> — Offline Kokoro-82M speech synthesis; custom CPU inference reaches 3.00× real-time warm synthesis.</summary>

An Unreal Engine plugin for offline voice generation with Kokoro and ONNX Runtime. Its runtime is provisioned for the project and staged with packaged builds, so players do not download model files at runtime.

The **quality-gated U8/S8 mixed-precision model** measured 3.00× real-time warm synthesis on a mid-range CPU, with 1.82 dB median mel-spectral error against FP32. This benchmark starts after model loading and excludes phonemization, queueing, and playback.

<p><a href="https://github.com/MC-Oruc/SpeechGen"><img src="assets/previews/plugins/speechgen.png" alt="SpeechGen GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/SpeechGen) · [Runtime assets](https://github.com/MC-Oruc/SpeechGen-Runtimes)

</details>

<details>
<summary><strong>TextGen</strong> <small>· Click to expand</small> — Streaming LLM inference for Unreal Engine, with verified on-demand CUDA and Vulkan backends.</summary>

Connects Unreal projects to local or remote language-model providers. Its managed <code>llama.cpp</code> runtime handles model selection, streamed responses, accelerator capability checks, and runtime lifecycle.

<p><a href="https://github.com/MC-Oruc/TextGen"><img src="assets/previews/plugins/textgen.png" alt="TextGen GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/TextGen)

</details>

<details>
<summary><strong>DeepLevelDesignPCG</strong> <small>· Click to expand</small> — Procedural city, road-network, building, and decoration workflows for Unreal Engine 5.8.</summary>

An editor-side PCG toolkit for deterministic city layouts. It supports authored spline paths and road-derived building placement, plus chunk-aware regeneration of generated decoration.

<p><a href="https://github.com/MC-Oruc/DeepLevelDesignPCG"><img src="assets/previews/plugins/deep-level-design-pcg.png" alt="DeepLevelDesignPCG GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/DeepLevelDesignPCG)

</details>

<details>
<summary><strong>UE-LevelInstanceDeepCopy</strong> <small>· Click to expand</small> — Creates isolated Level Instance copies with their project assets and references.</summary>

Scans map dependencies, duplicates project-local assets, redirects hard and soft references, and supports World Partition external actor packages. Conflict policies can reuse compatible assets or stop before overwriting.

<p><a href="https://github.com/MC-Oruc/UE-LevelInstanceDeepCopy"><img src="assets/previews/plugins/level-instance-deep-copy.png" alt="UE-LevelInstanceDeepCopy GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/UE-LevelInstanceDeepCopy)

</details>

<details>
<summary><strong>ProcessRuntime</strong> <small>· Click to expand</small> — Launches and manages external processes from Unreal Engine, with IPC support.</summary>

A reusable runtime plugin for process lifecycle management and inter-process communication.

<p><a href="https://github.com/MC-Oruc/ProcessRuntime"><img src="assets/previews/plugins/process-runtime.png" alt="ProcessRuntime GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/ProcessRuntime)

</details>

<details>
<summary><strong>TextureGeneration</strong> <small>· Click to expand</small> — Deterministic texture generation and import workflows for Unreal Editor.</summary>

Editor tools connect generated texture and material assets to an organized, repeatable Unreal workflow.

<p><a href="https://github.com/MC-Oruc/TextureGeneration"><img src="assets/previews/plugins/texture-generation.png" alt="TextureGeneration GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/TextureGeneration)

</details>

<details>
<summary><strong>BackupFileBrowser</strong> <small>· Click to expand</small> — Browse and restore project-asset backups without leaving Unreal Editor.</summary>

An editor utility for keeping asset backup and recovery workflows close to the project content.

<p><a href="https://github.com/MC-Oruc/BackupFileBrowser"><img src="assets/previews/plugins/backup-file-browser.png" alt="BackupFileBrowser GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/BackupFileBrowser)

</details>

## Other Projects

Independent projects across speech animation, embedded security testing, developer tooling, AI, and desktop software.

<details>
<summary><strong>Duskfall</strong> <small>· Feature Showcase · Discontinued · Click to expand</small></summary>

An archived Unity action-RPG prototype built around a lumberjack’s revenge. Development has been discontinued; this showcase documents its gameplay, combat, character systems, and level-design work.

**Technical Achievements**

- **Advanced Foot IK System** — Realistic character movement on uneven terrain.
- **Dynamic Camera System** — Smooth transitions between perspectives with zoom controls.

<div align="center">

**Camera System in Action**

https://github.com/user-attachments/assets/eee3a327-ac33-48d9-aab2-ba5abd0166f1

**Level Design Showcase**

<table>
  <tr>
    <td><img src="assets/projects/duskfall/gameplay/forest-gameplay.png" alt="Duskfall gameplay in a forest environment" width="300" /></td>
    <td><img src="assets/projects/duskfall/gameplay/forest-level.png" alt="Duskfall forest level" width="300" /></td>
    <td><img src="assets/projects/duskfall/gameplay/aerial-level.png" alt="Duskfall level viewed from above" width="300" /></td>
  </tr>
  <tr>
    <td><img src="assets/projects/duskfall/gameplay/bridge.png" alt="Duskfall bridge environment" width="300" /></td>
    <td><img src="assets/projects/duskfall/characters/antagonist.png" alt="Duskfall antagonist character" width="300" /></td>
    <td><img src="assets/projects/duskfall/maps/world-map.png" alt="Duskfall world-map layout" width="300" /></td>
  </tr>
</table>

**Technical Systems**

<table>
  <tr>
    <td width="50%">
      <img src="assets/projects/duskfall/systems/foot-ik.png" alt="Duskfall character and foot IK setup in the Unity Editor" width="100%" /><br />
      <img src="assets/projects/duskfall/gameplay/boss-fight.png" alt="Duskfall boss encounter" width="100%" />
    </td>
    <td width="30%"><img src="assets/projects/duskfall/systems/character-inspector.png" alt="Duskfall movement and camera settings in the Unity Inspector" width="100%" /></td>
  </tr>
</table>

**Dungeon Architecture**

<table>
  <tr>
    <td><img src="assets/projects/duskfall/dungeon/isometric-01.png" alt="Dungeon layout, view 1" width="190" /></td>
    <td><img src="assets/projects/duskfall/dungeon/isometric-02.png" alt="Dungeon layout, view 2" width="190" /></td>
    <td><img src="assets/projects/duskfall/dungeon/isometric-03.png" alt="Dungeon layout, view 3" width="190" /></td>
    <td><img src="assets/projects/duskfall/dungeon/isometric-04.png" alt="Dungeon layout, view 4" width="190" /></td>
    <td><img src="assets/projects/duskfall/dungeon/isometric-05.png" alt="Dungeon layout, view 5" width="190" /></td>
  </tr>
</table>

**Level Design Blueprints**

<table>
  <tr>
    <td><img src="assets/projects/duskfall/blueprints/dungeon-layout-01.png" alt="Dungeon blueprint, layout 1" width="400" /></td>
    <td><img src="assets/projects/duskfall/blueprints/dungeon-layout-02.png" alt="Dungeon blueprint, layout 2" width="400" /></td>
    <td><img src="assets/projects/duskfall/blueprints/dungeon-layout-03.png" alt="Dungeon blueprint, layout 3" width="400" /></td>
    <td><img src="assets/projects/duskfall/blueprints/dungeon-layout-04.png" alt="Dungeon blueprint, layout 4" width="400" /></td>
  </tr>
</table>

</div>

</details>

<details>
<summary><strong>VocaRig</strong> <small>· Click to expand</small> — Streaming speech-to-face animation, mapping 21 audio-driven channels to 52 ARKit blendshape outputs.</summary>

A standalone speech-driven 3D facial-animation system with synthetic-data preparation, GRU training, evaluation metrics, ONNX export, and a FastAPI lab dashboard.

<p><a href="https://github.com/MC-Oruc/VocaRig"><img src="assets/previews/projects/vocarig.png" alt="VocaRig GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/VocaRig)

</details>

<details>
<summary><strong>FaceRig</strong> <small>· Click to expand</small> — Predicts 3D facial-rig weights from continuous emotion parameters.</summary>

A PyTorch workspace for synthetic expression data, recurrent GRU training, ONNX export, and a local dashboard for inference and model metrics.

<p><a href="https://github.com/MC-Oruc/FaceRig"><img src="assets/previews/projects/facerig.png" alt="FaceRig GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/FaceRig)

</details>

<details>
<summary><strong>K4MPUS_R00TK1T</strong> <small>· Click to expand</small> — Pico W / ESP32 hardware for authorized Bluetooth beacon-filtering and Company ID tests.</summary>

An embedded security-testing project with a LittleFS-based web interface. Intended for controlled, authorized validation of Bluetooth filtering systems.

<p><a href="https://github.com/MC-Oruc/K4MPUS_R00TK1T"><img src="assets/previews/projects/k4mpus-rootkit.png" alt="K4MPUS_R00TK1T GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/K4MPUS_R00TK1T)

</details>

<details>
<summary><strong>UE 5.7 MCP PortKit</strong> <small>· Click to expand</small> — Backports UE 5.8 MCP tools and Atomic Material Graph workflows to UE 5.7.</summary>

Includes a token-efficient material-graph DSL with schema validation, batched graph edits, and compile diagnostics, alongside compatibility tooling for editor workflows.

<p><a href="https://github.com/MC-Oruc/UE57-MCP-PortKit"><img src="assets/previews/projects/ue-57-mcp-portkit.png" alt="UE 5.7 MCP PortKit GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/UE57-MCP-PortKit)

</details>

<details>
<summary><strong>Chimera</strong> <small>· Click to expand</small> — Full-stack AI chat and image-generation workspace built with Next.js and Go.</summary>

Combines a responsive chat interface, Firebase authentication and real-time sync, AI chat, and image-generation workflows.

<p><a href="https://github.com/MC-Oruc/Chimera"><img src="assets/previews/projects/chimera.png" alt="Chimera GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/Chimera)

</details>

<details>
<summary><strong>MessageHub</strong> <small>· Click to expand</small> — Qt/PySide6 interface demo with eight themes, animated transitions, and custom widgets.</summary>

A desktop UI project focused on visual design and reusable components, including photo galleries, sliders, hover buttons, and multi-select lists.

<p><a href="https://github.com/MC-Oruc/PySide6-PyQt-UI-Demo"><img src="assets/demos/messagehub.gif" alt="MessageHub desktop interface demo" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/PySide6-PyQt-UI-Demo)

</details>

<details>
<summary><strong>People Counter</strong> <small>· Click to expand</small> — Real-time people counting from camera, video, or RTSP streams with YOLO and YuNet.</summary>

Offers both headless processing and a Qt interface with live preview, a draggable counting line, and annotated-video export.

<p><a href="https://github.com/MC-Oruc/people-counter"><img src="assets/previews/projects/people-counter.png" alt="People Counter GitHub social preview" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/people-counter)

</details>

<details>
<summary><strong>File Organizer Tool</strong> <small>· Click to expand</small> — Cross-platform file organization with GUI, CLI, preview, undo, and ten languages.</summary>

A lightweight Python desktop utility that sorts files by filename prefixes and can reverse an organization or export a directory tree.

<p><a href="https://github.com/MC-Oruc/File-Organizer-Tool"><img src="assets/previews/projects/file-organizer.png" alt="File Organizer Tool interface" width="720" /></a></p>

[Repository](https://github.com/MC-Oruc/File-Organizer-Tool)

</details>

<p align="center">
  More project demos and implementation notes: <a href="https://kaanyildiz.com">kaanyildiz.com</a>
</p>
