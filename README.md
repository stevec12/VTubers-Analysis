# Hololive-VTubers
Projects related to Hololive or VTubers.

## Prototype
Initial ideas and prototyping: "Hololive Data Analysis Ideas.ipynb"

Prototype scope: Comment Language Makeup, Word and Emoji Analysis, RNN (GRU) training with comments and prompting. One video of one VTuber.

Next scaled product: 50 videos of one VTuber.

Scaling issues and potential solutions: 
- TL quotas: Google Translate API,  Microsoft Azure TL API, transfer learning of pretrained TL model.
- RNN training times: Google Colab GPUs or running locally (rather than from Jupyter Notebooks) to use own GPU.

Possible uses of program:
- Viewer Language Breakdown
- Viewer sentiment through keywords, phrases, punctuation, and emojis
- Comment generation with a prompt: returning a reasonable phrase to complete comments.

## Comment Prompting
Use TensorFlow transformers for Comment Prompting, given a initial prompt: "CommentPrompting3.ipynb"
- Focuses on the EN VTuber 'Ceres Fauna', alievating translation issues of prototyping.
- `temperature` arguement allows for non-deterministic predictions

Possible Next steps:
- implement a model using a dynamic array, rather than using a static preset MAX_TOKENS and always training/inferring using tensors padded to MAX_TOKENS
- model optimization for hyperparameters (KerasTuner) and weights 
- use TensorFlow.js to serve in a web application. 



