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
- [Stable Diffusion XL 1.0 pre-trained model]((https://civitai.com/models/122822/crystal-clear-xl))
- [ControlNet Models (Canny, Depth, Scribble)]((https://huggingface.co/xinsir))

### Setting up Project
1. Load ComfyUI:
   - Open ComfyUI in your local machine.
   - Load the provided workflow file (app_nation_case_study_workflow.json) by using the load button from menu.
   - You might have missing nodes in the project you will have an alert once you open it and you can download it from [ComfyUI Manager]((https://github.com/ltdrdata/ComfyUI-Manager))(highly recommended)
2. Configure Parameters
   - Adjust the strength, pixel, seed, batch, sampler, scheduler, denoise, prompts which respect to your choice.
3. Upload an Image
  - Use the load image input node to upload an image.
  - The image will be preprocessed.
4. Run the workflow
  - After setting up press queue.
  - The final output will be displayed and saved on the output file on the ComfyUI file.

### Sample Images
The images are trained on the same parameters, workflow and models.

![cemyilmaz](https://github.com/user-attachments/assets/d1e9e951-972e-4109-9d9d-ad2dce40d3fc)
![ComfyUI_00202_](https://github.com/user-attachments/assets/cba759fd-a60a-4af5-a98c-e901901cb2b4)
![Muzeyyen_senar_sergi2](https://github.com/user-attachments/assets/240372e3-fb09-4d72-b976-d9574b4a67f1)
![ComfyUI_00201_](https://github.com/user-attachments/assets/f25040fb-bac8-45a8-b40c-9532fec5c1a9)
![landscape_with_tree](https://github.com/user-attachments/assets/5bc78bb4-27dc-49ce-b932-405b72c1628d)
![ComfyUI_00180_](https://github.com/user-attachments/assets/0e9227be-387a-4b61-bc9f-0f61f7bb423b)
