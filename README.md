# Personalised Travel Ad Generation System

A creative system for generating customised travel advertisements using real-time user behavior, AI models, and scene-aware visual composition. This project combines structured label extraction, prompt generation, illustration-style image synthesis, slogan creation, and dynamic layout to produce engaging ad creatives.  

## Workflow  

1. **User Input**  
   Recent search behavior and registration info are collected.  
   Label dimensions include: budget, travel purpose, age group, etc.  

2. **Label Extraction**  
   Keywords are mapped to label categories using LLaMA3 + rules.  
   Conflicts (e.g. high budget search vs. medium history) are resolved by priority.  

3. **Prompt Construction**. 
   Tags are converted into structured natural language descriptions.  
   Prompts include visual scene layers (foreground, midground, background).  

4. **Image & Slogan Generation**. 
   Image generated via Stable Diffusion + Ghibli-style LoRA.  
   Text slogan created via LLaMA3 using user tags + image context.  

5. **Layout & Animation**. 
   DETR detects objects in the image.  
   Text is placed to avoid overlap.  
   Final ad is exported as an animated `.gif`.  

## Key Features

**User-Centered**: Combines long-term and recent interests for accurate targeting.  
**Stylised Illustration**: Avoids uncanny realism; adds emotion and charm.  
**Multi-Model Architecture**: Integrates LLaMA3, Stable Diffusion, and DETR.  
**Animated Output**: Final ads are visually dynamic and ready for delivery.  
**Cross-Platform UI**: Works for both mobile and desktop travel apps.  

## Mockup  
### splash screen  
![](splash_screen.gif)

### mobile version. 
<img src="mobile_version.png" width="300" />

### pc version  
<img src="pc_version.png" width="400" />