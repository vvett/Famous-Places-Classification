# Famous-Places-Classification
#This provides instructions on how to classify images of one of the "50 most famous places" from https://www.listchallenges.com/top-250-famous-attractions-in-the-world/list/7

1. Fork repository to Jetson Nano
2. Move Repository to jetson-inference/python/training/classification/models/
3. Go to jetson-inference/python/training/classification/
4. Enter both lines into terminal:
   NET=models/Famous-Places-Classification
5. Enter line into terminal: 
   imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$NET/labels.txt <image file path> <desired end image name>
6. View classified image directly in Nano or copy to host machine
