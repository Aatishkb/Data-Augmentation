# Data-Augmentation


1. **Imports**: The code imports necessary libraries such as `os` for file handling, `cv2` (OpenCV) for image processing, and `numpy` for random selection.

2. **random_augmentation Function**: This function applies random augmentation techniques to an input image. The augmentation techniques include flipping, rotating, blurring, and adjusting brightness. The number of augmentation techniques applied to each image is randomly selected.

3. **Input and Output Folder Paths**: The input folder contains the original images that will be augmented. The output folder is where the augmented images will be saved.

4. **Create Output Folder**: If the output folder doesn't exist, it creates the folder using `os.makedirs()`.

5. **Desired Number of Images to Generate**: The variable `desired_num_images` specifies the total number of augmented images desired.

6. **Image Augmentation Loop**: It iterates through each file in the input folder. For each image file, it loads the image using OpenCV, applies random augmentation using the `random_augmentation` function, and saves the augmented image to the output folder. It stops once the desired number of images is generated.

7. **Output Image Naming**: Each augmented image is saved with a unique identifier (`num_generated`) appended to the filename to avoid overwriting existing files.

8. **Completion Message**: Once the augmentation is completed, it prints a message indicating that the process is finished and the images are saved to the output folder.

