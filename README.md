# Hand-Gesture-Control
Controlling a Single Board Computer (Raspberry Pi 4 & Oak D Lite) using various distinct hand Gestures 

Using a python virutal environment, a python System control file and a Luxonis Tensor Processing Unit I was able to control my rasberryPi using my hand. 

I will not go through the whole setup process for the Pi4 (for now) but my paper and attached images (Yolov3 Linux OS) will show what the end process looked like. 

If you want to demo the project yourself I have attached a walkthrough document titled "Walkthrough for Hand Gesture Setup". You will need to run this project using the weights from the Yolov5Weights Folder instead of the Yolov3Weights Folder. Yolov5 is easier to setup than Yolov3tiny, but it is less accurate. 

Tips for running the model:

1. Use a T-shirt

2. Be in a well lit area with no distinct glare. I have noticed bright red shirts tend to worsen the results. I believe its due to the fact that bright red colours can dominate the convolutional process.

3. To run a live video, you will have to have a GPU. If you just want to detect hand gestures on some images, the CPU will work fine. The better the GPU the better the model will preform as speed is an issue even on a smaller neural network. 


General Note:

I collected, agumented, and trained the dataset myself. The dataset is around 2000 photos of myself. This is great for a proof of concept and a small demo, but the small dataset will cause the algorithm to run suboptimally. If I end up taking this product to production, I would retrain my models on a dataset 10-100 times larger than the one I currently have now. Futhermore, I would add more pictures of various individuals (different skin tones, heights, hand shapes ect.) wearing various clothing (hoodies, sweaters, darker clothing, brighter clothing ect.) to diversify my dataset. 

Lastly, the Windows OS folder has examples of the various hand gestures I had configured for this model. The Yolov3Linux Os folder will show what a demo will look like on a Rasberrypi 4 with a Luxonis Camera.
