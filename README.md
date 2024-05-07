# Visual Anagrams and Audio Illusions Replication

This repository contains our replication of the work described in the paper [**Visual Anagrams: Generating Multi-View Optical Illusions with Diffusion Models**](https://arxiv.org/pdf/2311.17919). We have implemented their approach to explore how these concepts apply to visual and audio illusions.

## Folder Structure
- **Visual-Anagrams.ipynb**: We reimplement the visual anagrams code from the paper. It demonstrates how to generate optical illusions using diffusion models.
  
- **/audio-illusions**: Contains adapted code to create similar anagrams and illusions but applied to audio, speech specifically:
  - **audio-illusion-low-mem.ipynb**: Low-memory version of the audio anagram code adapted for audio diffusion models. This implementation seeks to adapt the original visual model architecture but highlights challenges when applying it directly to audio.
  - **audio-illusions.ipynb**: General code adapted from the visual anagrams paper to audio diffusion models.

- **hammer-hitting.wav**: Generated audio with the prompt "The sound of a hammer hitting a wooden surface," without transcription and using the negative prompt "low quality."
- **speech-text.wav**: Generated audio using the prompt "a female saying the word 'cap.'"
- **text-speech-cap.wav**: Generated audio using the prompt "a female voice saying the word 'cap' in a clear, neutral tone," also with the negative prompt "low quality."

- **/overlay**: Contains adapted code to create base and overlay images that can be superimposed to create particular images based on input text prompts.


## Diffusion Models Used
We used the following diffusion models available in the `diffusers` module from [Hugging Face](https://huggingface.co/):

### Image Diffusion Model
- **DeepFloyd/IF-I-XL-v1.0**: This model generates visual illusions through text-based prompts.

### Audio Diffusion Models
- **cvssp/audioldm2**: An audio-text diffusion model for general audio generation.
- **anhnct/audioldm2_gigaspeech**: An adaptation of the audio-text diffusion model, specialized for speech generation.

Both models are documented in the [AudioLDM2 API](https://huggingface.co/docs/diffusers/main/en/api/pipelines/audioldm2).



 

## Usage
1. Open the respective Jupyter notebook and follow the code instructions.
2. Modify prompts and settings according to your desired audio or visual outputs.
3. Ensure you have all required dependencies by checking the import statements in the notebooks.



