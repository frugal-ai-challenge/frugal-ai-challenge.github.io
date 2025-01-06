---
title: Participate
menu_title: Participate
menu_icon: join
---

In this page you will find all the instructions to participate in the challenge.

To submit your results in one of the three tasks, please follow the steps below:
                        
## Prepare your model submission
1. Duplicate the template of the submission API by duplicating this space on your own Hugging Face account.
2. In ``tasks/text.py``, ``tasks/image.py``, or ``tasks/audio.py``, modify the ``evaluate_model`` function to replace the baseline by your model loading and inference within the inference pass where the energy consumption and emissions are tracked.
3. Eventually complete the requirements and/or any necessaries dependencies in your space.
4. Write down your model card in the ``README.md`` file.
5. Deploy your space (FastAPI) and verify that it works.
6. (Optional) You can change the Space hardware to use any GPU directly on Hugging Face.
                        
## Submit your model to the leaderboard in the ``Model Submission`` tab
When your API is deployed : 
1. Select the task you want to submit your model to
2. Enter the Space URL of your API
3. (Optional) Precise the API route (default is ``/text``, ``/image``, or ``/audio``)
4. Step 1 - Evaluate model: Click on the button to evaluate your model. This will run you model on your API, computes the accuracy on the test set (20% of the train set), and track the energy consumption and emissions.
5. Step 2 - Submit to leaderboard: Click on the button to submit your results to the leaderboard. This will upload the results to the leaderboard dataset and update the leaderboard.
6. You can see the leaderboards at 
    - Text - https://huggingface.co/datasets/frugal-ai-challenge/public-leaderboard-text
    - Image - https://huggingface.co/datasets/frugal-ai-challenge/public-leaderboard-image
    - Audio - https://huggingface.co/datasets/frugal-ai-challenge/public-leaderboard-audio