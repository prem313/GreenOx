## Task 1: Training YOLOv5 on a Custom Dataset

In this task, we implement the training of a YOLOv5 model on a custom dataset. The dataset consists of the following classes:

- 'pet_bottle'
- 'wine_bottle'
- 'beer_bottle'
- 'aluminium_can'
- 'barcode'
- 'tetrapack'

### Using Ultralytics YOLOv5 Colab Notebook

We utilized the Ultralytics YOLOv5 Colab notebook for custom dataset training. This notebook comes pre-configured with YOLOv5 and simplifies the training process.
After 10 epochs we got an average accuracy but it works effectively in detection of different bottles.


## Task 3: Instance Retrieval

In this task, we implement instance retrieval on the dataset created in Task 1. The goal is to fetch images of 'pet_bottle' (water bottle) from the dataset based on reference images of transparent water bottles from the internet.

### Methodology

We leveraged the Dinov2 model, an instance retrieval model, for this task. The Dinov2 model is a powerful tool for content-based image retrieval.

### Implementation Details

1. **Data Sources:**
   - We utilized reference images of transparent water bottles from the internet as query images.

2. **Dinov2 Model:**
   - We obtained the Dinov2 model from [Facebook Research's GitHub repository](https://github.com/facebookresearch/dinov2).

3. **Training on Task 1 Dataset:**
   - We fine-tuned the Dinov2 model using the custom dataset created in Task 1, allowing us to retrieve instances effectively.
