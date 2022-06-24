# Famous-Places-Classification

1. Fork repository to Jetson Nano
2. Move Repository to jetson-inference/python/training/classification/models/
3. Go to jetson-inference/python/training/classification/
4. Enter both lines into terminal:
   NET=models/Famous-Places-Classification
5. Enter line into terminal:
   imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$NET/labels.txt <image file path> <desired end image name>
