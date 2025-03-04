---
title: Participate
menu_title: Participate
menu_icon: briefcase
---

In this page you will find all the instructions to participate in the challenge.

## Explore the tasks and start hacking
### Choose your task
Select the task you want to participate in. See the [tasks page](https://frugalaichallenge.org/tasks/) for more information about the tasks.

### Download the datasets
You can find all the datasets in this [collection](https://huggingface.co/collections/frugal-ai-challenge/frugal-ai-challenge-tasks-673dd5ee724c6659a5b42443) on Hugging Face

You can download them directly in Python using the `datasets` library:
```python
from datasets import load_dataset

dataset = load_dataset("frugal-ai-challenge/frugal-ai-challenge-tasks")
```

### Start coding
You can work and iterate freely on the task in a notebook or your development environment of choice.

### Develop locally using notebooks template
If you clone locally the [submission-template repository](https://huggingface.co/spaces/frugal-ai-challenge/submission-template), you will find notebooks template for each task in the `notebooks` folder with : 
- Loading the dataset
- Tracking the energy consumption and emissions
- Random baseline
- Evaluating the model

## Submit your results
Because we will compute the energy consumption of your model on a private test set, it's not like a typical Machine Learning competition where you submit your predictions. We need you to submit your model with the requirements for us to run them all on the same hardware during the evaluation phase.

So to submit your results, you will need to 
1. Deploy your model as an API (a FastAPI space)
2. Submit your results to the leaderboard

Don't worry, it's all planned with pre-built templates directly on Hugging Face Spaces.

### Create your account on HuggingFace
If you don't have one yet, you can create one [here](https://huggingface.co/join).
This account is free and will allow you to deploy your model as a Hugging Face Space.
You can participate as a team (with a Hugging Face organization) or as an individual.

                        
### Prepare your model submission on a API as a Hugging Face Space
1. Duplicate the template of the submission API by duplicating this space on your own Hugging Face account [https://huggingface.co/spaces/frugal-ai-challenge/submission-template](https://huggingface.co/spaces/frugal-ai-challenge/submission-template)
2. In ``tasks/text.py``, ``tasks/image.py``, or ``tasks/audio.py``, modify the ``evaluate_model`` function to replace the baseline by your model loading and inference within the inference pass where the energy consumption and emissions are tracked.
3. Eventually complete the requirements and/or any necessaries dependencies in your space.
4. Write down your model card in the ``README.md`` file.
5. Deploy your space (FastAPI) and verify that it works.
6. (Optional) You can change the Space hardware to use any GPU directly on Hugging Face.

To check if you API is working, you can use the `/docs` route of your FastAPI space either locally or on Hugging Face.
On Hugging Face you can find the embed link in the space settings.

For example for "frugal-ai-challenge/submission-template" the embed link [https://frugal-ai-challenge-submission-template.hf.space/docs](https://frugal-ai-challenge-submission-template.hf.space/docs)

### Add your token to the space (for the audio task)
You need to add your personal token after having accessed the gated dataset for the audio task. 
The token need to be put in the .env variables as `HF_TOKEN` to validate the access to the dataset.

### (Optional) Submit your model to the public leaderboard
You can now go to the submission portal here [https://huggingface.co/spaces/frugal-ai-challenge/submission-portal](https://huggingface.co/spaces/frugal-ai-challenge/submission-portal)
And as soon as your API is deployed : 
1. Select the task you want to submit your model to
2. Enter the Space URL of your API
3. (Optional) Precise the API route (default is ``/text``, ``/image``, or ``/audio``)
4. Step 1 - Evaluate model: Click on the button to evaluate your model. This will run you model on your API, computes the accuracy on the test set (20% of the train set), and track the energy consumption and emissions.
5. Step 2 - Submit to leaderboard: Click on the button to submit your results to the leaderboard. This will upload the results to the leaderboard dataset and update the leaderboard.
6. You can see the leaderboards at 
    - Text - https://huggingface.co/datasets/frugal-ai-challenge/public-leaderboard-text
    - Image - https://huggingface.co/datasets/frugal-ai-challenge/public-leaderboard-image
    - Audio - https://huggingface.co/datasets/frugal-ai-challenge/public-leaderboard-audio

This step is optional because the results on the public leaderboard will not be used for the final evaluation and are simply informative to position yourself against other participants and improve accordingly. To be eligible for the final evaluation, you need to submit your results to the final evaluation form.

### Submit your model to the final evaluation
You can now go to the final evaluation form here [https://framaforms.org/2025-frugal-ai-challenge-submission-form-1736883260-0](https://framaforms.org/2025-frugal-ai-challenge-submission-form-1736883260-0)
