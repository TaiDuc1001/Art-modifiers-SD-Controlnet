# Art Modifier with Stable Diffusion and ControlNet

This project explores the use of ControlNet with Stable Diffusion to modify and enhance images based on specific control signals like canny edges and poses. The aim is to demonstrate how these models can be applied to create high-quality image transformations.
## Overview
The Art Modifier project leverages the capabilities of ControlNet and Stable Diffusion to modify images using control signals. ControlNet enhances the functionality of Stable Diffusion by allowing for controlled image generation based on additional input conditions. This project specifically uses canny edge detection and pose estimation as control signals to guide the image generation process.

## Key Features
- **ControlNet Integration:** Utilizes ControlNet models to guide image transformations.
- **Stable Diffusion Backbone:** Employs RunWayML's Stable Diffusion v1-5 model for high-quality image generation.
- **Edge Detection:** Uses canny edge detection to provide control signals for the image modification process.

## Methodology
1. **Model setup:**
   - Install necessary packages: `diffusers` and `controlnet_hinter`.
   - Load `ControlNet` models for canny edge detection.
   - Initialize the `Stable Diffusion` pipeline with the selected ControlNet model.
2. **Image processing:**
   - Download and preprocess the input image.
   - Apply control signals (canny edges or poses) to guide the image generation.
3. **Image generation:**
   - Use the `StableDiffusionControlNetPipeline` to generate modified images based on the control signals.
   - Display and compare the original and modified images.

## Results
### From a picture to canny edge detection to a target style
![Results](https://github.com/TaiDuc1001/Art-modifiers-SD-Controlnet/blob/main/results.png)
### Other variations
![Variations](https://github.com/TaiDuc1001/Art-modifiers-SD-Controlnet/blob/main/variations.png)

## Conclusion
The Art Modifier project demonstrates the potential of combining ControlNet with Stable Diffusion for controlled image generation. By utilizing control signals like canny edges and poses, we can guide the image transformation process to produce diverse and high-quality results.

## References
[Stable Diffusion](https://huggingface.co/runwayml/stable-diffusion-v1-5)

[ControlNet Canny](https://huggingface.co/lllyasviel/sd-controlnet-canny)
