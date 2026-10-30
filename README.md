> [!NOTE]
> **Work in Progress:** This asset library and material system are actively being developed. Planned features include triplanar mapping, proper layer blending, displacement, and potentially water plugin compatible water shaders.

A custom HD-2D material workflow for Unreal Engine designed to combine low-resolution pixel aesthetic rendering with modern dynamic lighting, normal maps, and custom HLSL shader logic. 

---

## 🛠️ Requirements & Compatibility

* **Tested Engine Version:** Unreal Engine 5.8
* **Compatibility:** Designed to work across any 5.X release and should be fully compatible with late 4.X releases (4.26+).
* **Dependencies:** None required. Core shaders run on standard engine Material Expression nodes and custom HLSL blocks.

---

## 🚀 Quick Setup & Installation

Release files will be coming later.

1. **Download** the project source or release `.zip`.
2. Open your target Unreal Engine project directory in your file explorer.
3. Copy the contents of the `Content/` folder from this repository directly into your project's `Content/` folder.
4. Launch Unreal Engine and navigate to the newly added asset folder.

---

## 📐 Best Practices & Guidelines

To achieve crisp pixel grid alignment and avoid rendering artifacts, follow these asset setup guidelines:

* **Consistent Texture Resolution:** Keep source texture resolutions uniform across your materials to prevent mismatched pixel density across different environmental surfaces.
* **Power-of-2 Scaling:** To maintain precise pixel alignment and avoid sub-pixel shimmering, always scale your actors and mesh components using **powers of 2** (e.g., `2.0`, `4.0`, `8.0`, `16.0`).
* **Custom Textures:** Simply add in any texture you need, replace the textures in an existing layer or duplicate existing functions for your new layer and plug them in the material. Make sure your imported textures use a consistent resolution (128x128 for example) and set the texture filtering to nearest.

---

## 📜 Third-Party Licenses & Attribution

This project bundles lightweight sample assets for demonstration purposes. Relevant third-party licenses apply:

* **Landscape Textures:** Provided by [CC0 Textures (AmbientCG)](https://ambientcg.com) and [Poly Haven](https://polyhaven.com). These assets are dedicated to the public domain under the [Creative Commons CC0 License](https://creativecommons.org/publicdomain/zero/1.0/).
