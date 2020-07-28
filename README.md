# Grarbage-detection

The algorithm can distinguish PET, plastic, light_bulb, paper and cardboard garbages.
It had 16 FPS in average on a Tesla P100-PCI-E-16GB 

## Project steps
1. Record the video
2. Create a custom dataset by annotating 50 frames with [CVAT](https://github.com/opencv/cvat)
3. Train yolov4 on the small dataset
4. Generate pseudo labels with the trained model
5. Import, and fix the generated iamges manually in CVAT
6. Retrain the model on the larger dataset
7. Process the video

## Tested models:
1. yolov4
