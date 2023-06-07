# face-recognition-system
This repository demostrates a face recognition system.

## How a face recognition system works

A facial recognition system usually consists of the following components:
1. a Close-up photo of a person as image input from e.g. static image file, a static video file or a camera input
2. preprocessing(e.g. face detection and face alignment)
3. face embedding(a 128-dimensonal vector) calculation using a DeepLearning Neural Network(e.g. MobilefaceNet)
4. compare the calculated embedding with faces in the database of known persons
5. identify the person if the distance between calculated embedding and the closest known face in the database is smaller than a certain threshold
  
    
In the repo, the MTCNN library from PyPI is used for face detection and face alighment.  
A pre-trained MobileFaceNet model is used for embedding calculation, the training of the model can be find at [Kaggle](https://www.kaggle.com/code/jasonhcwong/mobilefacenet/).  
A video from [YouTube](https://www.youtube.com/watch?v=R32qWdOWrTo) is used for demo of face recognition on video file. The video features Bryce Dallas Howard and Charlie Brooker.  
Some photoes of them are added to the known persons database. 
