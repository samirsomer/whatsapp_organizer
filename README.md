# whatsapp_organizer


In this experiment I'm trying to use [fastai](https://docs.fast.ai) deep learning to classify my [WhatsApp](https://www.whatsapp.com) images into separate folders based on the image classification.

FastAi library is a high-level library build on PyTorch, which allows us to build models using only a few lines of code. Furthermore it implements some of the newest state-of-the-art technics taken from research papers that allow you to get state-of-the-art results on almost any type of problem.

For more information about the installation visit the [official guide](https://docs.fast.ai/install.html).

## Project Structure

- **datasets**: This contains the training images, each category will be downloaded as a subfolder.
- **models**: Directory to save and load the model from.
- **urls**: contains the URL list to download the training images
- **whatsapp**: contain my WhatsApp images.
- **output**: This will be the output after organizing the images.

```
.
├── 01-prepare_dataset.ipynb
├── 02-model_train_fit.ipynb
├── 03-run_model.ipynb
├── LICENSE
├── README.md
├── datasets
│   ├── Greetings
│   ├── People
│   └── Screenshots
├── models
│   └── whatsapp_cleaner_stage-1.pkl
├── output
│   ├── Greetings
│   ├── People
│   └── Screenshots
├── urls
│   ├── greetings.txt
│   ├── people.txt
│   └── screenshots.txt
└── whatsapp
.
```


## Notebooks

- **01-prepare_dataset**: This will download the training data
- **02-model_train_fit**: This will create a model called "whatsapp_cleaner_stage-1.pkl" and saves it in the model directory.
- **03-run_model**: This will load the model and loop through the whatsapp media folder and move it to the appropriate output subfolder


## Todo
> Add Model Optimization notebook

> Deploy REST API for production