# Team Hawk 



<!-- Intro and about the project -->

This is a unfinished version and a subject to various changes where this machine predicts the disease of the leaf image of the given plant using Deep Learning and machine learning, while the other parts of this provide the alerts for the project.

## Technologies Used

<!-- Tech stack, libraries etc -->

`Python, Tensorflow, FastAPI, Skimage`

## Workflow

<!-- In some detail of how this works -->

- An image is uploaded to the server
- Checking is done to ensure that the image has adequate quality (brightness, contrast etc.) before it is sent for prediction. This step is performed using `image processing`
- Once checked, an `AutoEncoder` model checks if the data belongs to the distribution the data is trained on or not (i.e Outlier check).
- The model predicts the disease the plant.We use a Transfer Learning based classifier with `Inception v3` as backbone
- In case of error, it sends an error message

## Results

### Classifier Results

| Metric   | Score |
| -------- | ----- |
| Accuracy | 89%   |

### AutoEncoder Results

| Metric | Score |
| ------ | ----- |
| MSE    | 0.05  |
| MAE    | 0.2   |

## How to Run

<!-- Installation and Running Steps -->

- Clone the repo
- Install python requirements using `$ pip install -r requirements.txt`
- Run the server using `$ python main.py`




