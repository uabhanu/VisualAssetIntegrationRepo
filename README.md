# 🎨 Visual Asset Integration

**Project Name:** VisualAssetIntegration | **Status:** Implementation Phase | **Platform:** PC (High Fidelity)

---

## 💡 Overview
This project demonstrates the professional workflow for integrating high-fidelity 3D assets into **Unity's Universal Render Pipeline (URP)**. It focuses on the translation of raw art assets into a game-ready environment, emphasising correct PBR material setup, lighting strategies, and scene optimisation.

This portfolio piece serves as proof of **Technical Art proficiency**, bridging the gap between raw 3D models and the real-time engine rendering.

## 🧱 Core Architectural Concepts

### 1. PBR Material Workflow (URP)
* **Implementation:** Utilises the **URP Lit Shader** standard. Configurations include the correct assignment of Texture Maps (Albedo, Normal, Metallic/Smoothness) to ensure physically accurate light interaction.
* **Benefit:** Guarantees visual consistency across different lighting conditions and separates material properties from lighting data, adhering to modern rendering standards.

### 2. Hybrid Lighting Architecture
* **Implementation:** Implements a Mixed Lighting setup combining **Baked Global Illumination (GI)** for static geometry with Realtime lights for dynamic elements. Utilises **Light Probes** and **Reflection Probes** to integrate dynamic objects.
* **Benefit:** Balances high visual fidelity with runtime performance by pre-calculating complex light bounces while maintaining interactivity.

## ⚙️ Technical Stack
| Category | Detail | Purpose |
| :--- | :--- | :--- |
| **Engine** | Unity 2023+ (Unity 6.2) | The base development environment. |
| **Pipeline** | URP (Universal Render Pipeline) | Performant, scriptable rendering backbone. |
| **Lighting** | Progressive Lightmapper | Baking Global Illumination (GI) and Ambient Occlusion. |
| **Post-Processing** | Volume Framework | Colour Grading, Bloom, and Tonemapping for final visual polish. |

## 💾 Key Assets & Structure
| Category | File / Path | Purpose |
| :--- | :--- | :--- |
| **Art (Models)** | Art/Models/Environment/ | Contains imported FBX/OBJ meshes with correct Scale and Rig settings. |
| **Art (Materials)** | Art/Materials/URP_Lit/ | Configured .mat files using the URP Lit shader with packed masks (Metallic/Smoothness). |
| **Scenes** | ShowcaseScene.unity | The staging area containing the Lighting Setup, Light Probes, and Volume configurations. |

## 🗓️ Roadmap
| Status | Task | Feature Branch |
| :--- | :--- | :--- |
| ✅ | **Setup:** Repository creation and URP Project initialisation. | `main` |
| 🚧 | **Asset Import:** Import raw 3D models and configure Import Settings. | `feature/asset-setup` |
| ⬜ | **Material Pipeline:** Create and assign URP Lit materials with correct texture slots. | `feature/material-setup` |
| ⬜ | **Lighting & Polish:** Configure Lights, Probes, and bake the scene. | `feature/lighting-polish` |
