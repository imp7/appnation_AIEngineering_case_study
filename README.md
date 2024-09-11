# App Nation AI Engineering Case Study

## Overview
This project implements a workflow using framework named **ComfyUI** in order to transform a input image into a Van Gogh style image by using Stable Diffusion, preprocessors and ControlNet models. Users are allowed to upload upload an image and get an output image styled in Van Gogh's technique. 

## Features
- JPEG and PNG formats image inputs.
- Automated image preprocessing.
- Style transfer using Stable Diffusion and ControlNets.
- Option to apply multiple ControlNets to enhance image transformation.
- Positive and Negative prompts.
## Getting Started
### Prerequisites
- Python 3.8+
- ComfyUI
- [Stable Diffusion XL 1.0 pre-trained model](https://civitai.com/models/122822/crystal-clear-xl)
- [ControlNet Models (Canny, Depth, Scribble)](https://huggingface.co/xinsir)

### Setting up Project
1. Load ComfyUI:
   - Open ComfyUI in your local machine.
   - Load the provided workflow file (app_nation_case_study_workflow.json) by using the load button from menu.
   - You might have missing nodes in the project you will have an alert once you open it and you can download it from [ComfyUI Manager]((https://github.com/ltdrdata/ComfyUI-Manager))(highly recommended)
2. Configure Parameters:
   - Adjust the strength, pixel, seed, batch, sampler, scheduler, denoise, prompts which respect to your choice.
3. Upload an Image
   - Use the load image input node to upload an image.
   - The image will be preprocessed.
4. Run the workflow
   - After setting up press queue.
   - The final output will be displayed and saved on the output file on the ComfyUI file.

## Troubleshooting
### Common Issues
  1. System Crashes or Freezes:

   -If using multiple ControlNets, ensure your GPU has sufficient memory (preferably 8 GB+ VRAM).
   -Reduce image resolution if needed to avoid memory overuse.

  2. Output Doesn’t Look Like Van Gogh Style:

   -Check the guidance strength of the ControlNet models.
   -Adjust the positive prompt to better capture Van Gogh's unique features (e.g., swirling skies,  color theory).
    
  3. Slow Processing:

   -Try reducing the number of steps or adjusting the ControlNet guidance strength to speed up the process.

## Workflow

Over 200 images were generated using different models, prompts, and parameters. To achieve the best results for image-to-image generation in the style of Vincent van Gogh, his artworks were studied in depth. By analyzing his brushstrokes, color palette, and compositional techniques, gained insights into how to replicate his distinctive style. Through experimentation and generation of new images, it was found that a combination of the Canny, Depth, and Scribble ControlNets, along with carefully tuned final parameters, gave the most visually accurate results. This approach allowed us to capture Van Gogh’s signature swirling patterns, vibrant colors, and thick impasto textures in the generated images. Each model and prompt adjustment was made to enhance the authenticity of the style transfer, ensuring that the output remained true to Van Gogh’s artistic vision.

### Sample Images
These images are trained on the same parameters, workflow and models.

![landscape_with_tree](https://github.com/user-attachments/assets/5bc78bb4-27dc-49ce-b932-405b72c1628d)
![ComfyUI_00180_](https://github.com/user-attachments/assets/0e9227be-387a-4b61-bc9f-0f61f7bb423b)
![cemyilmaz](https://github.com/user-attachments/assets/d1e9e951-972e-4109-9d9d-ad2dce40d3fc)
![ComfyUI_00202_](https://github.com/user-attachments/assets/cba759fd-a60a-4af5-a98c-e901901cb2b4)
![Muzeyyen_senar_sergi2](https://github.com/user-attachments/assets/240372e3-fb09-4d72-b976-d9574b4a67f1)
![ComfyUI_00199_](https://github.com/user-attachments/assets/4ab60cae-5997-453e-85ec-058dd2cd08b9)
