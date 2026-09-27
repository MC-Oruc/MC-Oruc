<div align="center">
  <img src="assets/brand/banner.png" alt="Kaan YILDIZ project portfolio banner" width="100%" />
</div>

<h1 align="center">Kaan YILDIZ</h1>

<p align="center">
  <strong>Software Developer</strong><br />
</p>

<p align="center">
  <img src="assets/brand/skills/unreal-engine.svg" alt="Unreal Engine" height="24" />
  <img src="assets/brand/skills/real-time-ai.svg" alt="Real-time AI" height="24" />
  <img src="assets/brand/skills/cplusplus.svg" alt="C++" height="24" />
  <img src="assets/brand/skills/python.svg" alt="Python" height="24" />
  <img src="assets/brand/skills/developer-design-tools.svg" alt="Developer and Design Tools" height="24" />
</p>

<p align="center">
  <a href="https://kaanyildiz.com"><img src="assets/brand/badges/portfolio.svg" alt="Portfolio" height="28" /></a>
  <a href="https://linkedin.com/in/kaan-oruc-yildiz"><img src="assets/brand/badges/linkedin.svg" alt="LinkedIn" height="28" /></a>
</p>

## Secret of Chronicles

&emsp;**Independent neo-noir detective game · Unreal Engine 5.8**

### Gameplay

https://github.com/user-attachments/assets/e6237140-f0b1-4940-9076-d923e491d24e

### AI NPC Dialogue

https://github.com/user-attachments/assets/f5dafd03-0d47-40ee-8ee5-95e3a186d4e0

<p align="center">
  <a href="https://kaanyildiz.com/#showcase"><strong>Explore Secret of Chronicles on my portfolio →</strong></a>
</p>

### Project Overview

&emsp;Secret of Chronicles is an independent neo-noir detective game built with Unreal Engine 5.8. Players question NPCs freely instead of choosing from fixed dialogue options.

&emsp;**TextGen** generates scenario- and gameplay-aware replies with an LLM. **SpeechGen** creates each reply’s voice and synchronized mouth and facial animation at runtime. **ConvCore** validates and coordinates the complete exchange.

### Development Status

- **Completed:** Real-time AI dialogue pipeline.
- **In progress:** World placement and scenario implementation.
- **Steam:** App ID setup is complete. The Steam page and wishlist are planned for the vertical slice.

## Unreal Engine Plugins

&emsp;Plugins for **AI inference, speech, facial animation, procedural level design, and editor workflows**.

### SpeechGen

---

&emsp;Offline **Kokoro-82M** speech synthesis for Unreal Engine.

<details>
<summary><small><em>Click to expand</em></small> · Performance, implementation &amp; benchmark details</summary>

#### Runtime

&emsp;The plugin runs Kokoro through ONNX Runtime. Its runtime is provisioned for the project and staged with packaged builds, so players do not need to download model files at runtime.

#### Performance &amp; Quality

&emsp;The **quality-gated U8/S8 mixed-precision model** measured **3.00× real-time warm synthesis** on a mid-range CPU, with **1.82 dB median mel-spectral error** against FP32.

#### Benchmark Scope

&emsp;The timing starts after model loading. It excludes phonemization, queueing, and audio playback.

<p><a href="https://github.com/MC-Oruc/SpeechGen"><img src="assets/previews/plugins/speechgen.png" alt="SpeechGen GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/SpeechGen) · [Runtime assets](https://github.com/MC-Oruc/SpeechGen-Runtimes)

</details>

### TextGen

---

&emsp;Streaming LLM inference for Unreal Engine, with verified on-demand **CUDA and Vulkan** backends.

<details>
<summary><small><em>Click to expand</em></small> · Runtime and implementation details</summary>

#### Overview

&emsp;TextGen connects Unreal projects to local or remote language-model providers. Its managed `llama.cpp` runtime handles model selection, streamed responses, accelerator capability checks, and runtime lifecycle.

<p><a href="https://github.com/MC-Oruc/TextGen"><img src="assets/previews/plugins/textgen.png" alt="TextGen GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/TextGen)

</details>

### DeepLevelDesignPCG

---

&emsp;An editor-side PCG toolkit for deterministic **city, road, building, and decoration generation** in Unreal Engine 5.8.

<details>
<summary><small><em>Click to expand</em></small> · Procedural generation details</summary>

#### Overview

&emsp;Supports authored spline paths and road-derived building placement, with chunk-aware regeneration of generated decoration.

<p><a href="https://github.com/MC-Oruc/DeepLevelDesignPCG"><img src="assets/previews/plugins/deep-level-design-pcg.png" alt="DeepLevelDesignPCG GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/DeepLevelDesignPCG)

</details>

### UE-LevelInstanceDeepCopy

---

&emsp;Creates isolated Level Instance copies with their project assets and references.

<details>
<summary><small><em>Click to expand</em></small> · Dependency and copy behavior</summary>

&emsp;Scans map dependencies, duplicates project-local assets, redirects hard and soft references, and supports World Partition external actor packages. Conflict policies can reuse compatible assets or stop before overwriting.

<p><a href="https://github.com/MC-Oruc/UE-LevelInstanceDeepCopy"><img src="assets/previews/plugins/level-instance-deep-copy.png" alt="UE-LevelInstanceDeepCopy GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/UE-LevelInstanceDeepCopy)

</details>

### ProcessRuntime

---

&emsp;Launches and manages external processes from Unreal Engine, with inter-process communication support.

<details>
<summary><small><em>Click to expand</em></small> · Plugin preview and repository</summary>

&emsp;A reusable runtime plugin for process lifecycle management and IPC.

<p><a href="https://github.com/MC-Oruc/ProcessRuntime"><img src="assets/previews/plugins/process-runtime.png" alt="ProcessRuntime GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/ProcessRuntime)

</details>

### TextureGeneration

---

&emsp;Deterministic texture generation and import workflows for Unreal Editor.

<details>
<summary><small><em>Click to expand</em></small> · Editor workflow and preview</summary>

&emsp;Editor tools connect generated texture and material assets to an organized, repeatable Unreal workflow.

<p><a href="https://github.com/MC-Oruc/TextureGeneration"><img src="assets/previews/plugins/texture-generation.png" alt="TextureGeneration GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/TextureGeneration)

</details>

### BackupFileBrowser

---

&emsp;Browse and restore project-asset backups without leaving Unreal Editor.

<details>
<summary><small><em>Click to expand</em></small> · Editor utility and preview</summary>

&emsp;An editor utility for keeping asset backup and recovery workflows close to project content.

<p><a href="https://github.com/MC-Oruc/BackupFileBrowser"><img src="assets/previews/plugins/backup-file-browser.png" alt="BackupFileBrowser GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/BackupFileBrowser)

</details>

## Other Projects

&emsp;Independent work across **speech animation, embedded security testing, developer tools, AI, and desktop software**.

### Duskfall

---

&emsp;**Feature Showcase · Development discontinued**

<details>
<summary><small><em>Click to expand</em></small> · Archived gameplay, character systems &amp; level-design gallery</summary>

#### Project Overview

&emsp;Duskfall is an archived Unity action-RPG prototype about a lumberjack’s revenge. Development has ended; this feature showcase records its gameplay, combat, character systems, and level-design work.

#### Technical Achievements

- **Advanced Foot IK System** — Adapts character movement to uneven terrain.
- **Dynamic Camera System** — Blends camera perspectives and provides zoom control.

#### Camera System

https://github.com/user-attachments/assets/eee3a327-ac33-48d9-aab2-ba5abd0166f1

#### Environment &amp; Level Design

<table align="center">
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

#### Character &amp; Combat Systems

<table align="center">
  <tr>
    <td width="50%">
      <img src="assets/projects/duskfall/systems/foot-ik.png" alt="Duskfall character and foot IK setup in the Unity Editor" width="100%" /><br />
      <img src="assets/projects/duskfall/gameplay/boss-fight.png" alt="Duskfall boss encounter" width="100%" />
    </td>
    <td width="30%"><img src="assets/projects/duskfall/systems/character-inspector.png" alt="Duskfall movement and camera settings in the Unity Inspector" width="100%" /></td>
  </tr>
</table>

#### Dungeon Architecture

<table align="center">
  <tr>
    <td><img src="assets/projects/duskfall/dungeon/isometric-01.png" alt="Dungeon layout, isometric view 1" width="150" /></td>
    <td><img src="assets/projects/duskfall/dungeon/isometric-02.png" alt="Dungeon layout, isometric view 2" width="150" /></td>
    <td><img src="assets/projects/duskfall/dungeon/isometric-03.png" alt="Dungeon layout, isometric view 3" width="150" /></td>
    <td><img src="assets/projects/duskfall/dungeon/isometric-04.png" alt="Dungeon layout, isometric view 4" width="150" /></td>
    <td><img src="assets/projects/duskfall/dungeon/isometric-05.png" alt="Dungeon layout, isometric view 5" width="150" /></td>
  </tr>
</table>

#### Level-Design Blueprints

<table align="center">
  <tr>
    <td><img src="assets/projects/duskfall/blueprints/dungeon-layout-01.png" alt="Dungeon blueprint, layout 1" width="180" /></td>
    <td><img src="assets/projects/duskfall/blueprints/dungeon-layout-02.png" alt="Dungeon blueprint, layout 2" width="180" /></td>
    <td><img src="assets/projects/duskfall/blueprints/dungeon-layout-03.png" alt="Dungeon blueprint, layout 3" width="180" /></td>
    <td><img src="assets/projects/duskfall/blueprints/dungeon-layout-04.png" alt="Dungeon blueprint, layout 4" width="180" /></td>
  </tr>
</table>

</details>

### VocaRig

---

&emsp;Streaming speech-to-face animation, mapping **21 audio-driven channels to 52 ARKit blendshape outputs**.

<details>
<summary><small><em>Click to expand</em></small> · Model pipeline &amp; visual preview</summary>

&emsp;A standalone system for speech-driven 3D facial animation. It includes synthetic-data preparation, GRU training, evaluation metrics, ONNX export, and a FastAPI lab dashboard.

<p><a href="https://github.com/MC-Oruc/VocaRig"><img src="assets/previews/projects/vocarig.png" alt="VocaRig GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/VocaRig)

</details>

### FaceRig

---

&emsp;Predicts 3D facial-rig weights from continuous emotion parameters.

<details>
<summary><small><em>Click to expand</em></small> · Training pipeline &amp; visual preview</summary>

&emsp;A PyTorch workspace for synthetic expression data, recurrent GRU training, ONNX export, and a local dashboard for inference and model metrics.

<p><a href="https://github.com/MC-Oruc/FaceRig"><img src="assets/previews/projects/facerig.png" alt="FaceRig GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/FaceRig)

</details>

### K4MPUS_R00TK1T

---

&emsp;Raspberry Pi Pico W / ESP32 tool for authorized Bluetooth beacon-filtering and Company ID tests.

<details>
<summary><small><em>Click to expand</em></small> · Hardware, test scope &amp; preview</summary>

&emsp;An embedded security-testing project with a LittleFS-based web interface. Intended for controlled, authorized validation of Bluetooth filtering systems.

<p><a href="https://github.com/MC-Oruc/K4MPUS_R00TK1T"><img src="assets/previews/projects/k4mpus-rootkit.png" alt="K4MPUS_R00TK1T GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/K4MPUS_R00TK1T)

</details>

### UE 5.7 MCP PortKit

---

&emsp;Backports Unreal Engine 5.8 MCP tools and Atomic Material Graph workflows to UE 5.7.

<details>
<summary><small><em>Click to expand</em></small> · Tooling details &amp; visual preview</summary>

&emsp;Includes a token-efficient material-graph DSL with schema validation, batched graph edits, and compile diagnostics, alongside compatibility tooling for editor workflows.

<p><a href="https://github.com/MC-Oruc/UE57-MCP-PortKit"><img src="assets/previews/projects/ue-57-mcp-portkit.png" alt="UE 5.7 MCP PortKit GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/UE57-MCP-PortKit)

</details>

### Chimera

---

&emsp;Full-stack AI chat and image-generation workspace built with Next.js and Go.

<details>
<summary><small><em>Click to expand</em></small> · Application overview &amp; visual preview</summary>

&emsp;Combines a responsive chat interface, Firebase authentication and real-time sync, AI chat, and image-generation workflows.

<p><a href="https://github.com/MC-Oruc/Chimera"><img src="assets/previews/projects/chimera.png" alt="Chimera GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/Chimera)

</details>

### MessageHub

---

&emsp;Qt/PySide6 interface demo with **eight themes**, animated transitions, and custom widgets.

<details>
<summary><small><em>Click to expand</em></small> · Interface preview &amp; project details</summary>

&emsp;A desktop UI project focused on visual design and reusable components, including photo galleries, sliders, hover buttons, and multi-select lists.

<p><a href="https://github.com/MC-Oruc/PySide6-PyQt-UI-Demo"><img src="assets/demos/messagehub.gif" alt="MessageHub desktop interface demo" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/PySide6-PyQt-UI-Demo)

</details>

### People Counter

---

&emsp;Real-time people counting from camera, video, or RTSP streams with **YOLO and YuNet**.

<details>
<summary><small><em>Click to expand</em></small> · Detection workflow &amp; preview</summary>

&emsp;Offers headless processing and a Qt interface with live preview, a draggable counting line, and annotated-video export.

<p><a href="https://github.com/MC-Oruc/people-counter"><img src="assets/previews/projects/people-counter.png" alt="People Counter GitHub social preview" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/people-counter)

</details>

### File Organizer Tool

---

&emsp;Cross-platform file organization with GUI, CLI, preview, undo, and **ten languages**.

<details>
<summary><small><em>Click to expand</em></small> · Workflow preview &amp; project details</summary>

&emsp;A lightweight Python desktop utility that sorts files by filename prefixes and can reverse an organization or export a directory tree.

<p><a href="https://github.com/MC-Oruc/File-Organizer-Tool"><img src="assets/previews/projects/file-organizer.png" alt="File Organizer Tool interface" width="720" /></a></p>

&emsp;[Repository](https://github.com/MC-Oruc/File-Organizer-Tool)

</details>

<p align="center">
  More project demos and implementation notes: <a href="https://kaanyildiz.com">kaanyildiz.com</a>
</p>
