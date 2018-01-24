## Facial-Recognition-with-Deep-Nueral-Networks

![screen shot 2017-04-17 at 3 24 41 pm](https://user-images.githubusercontent.com/12654784/35335115-8f50c5a8-013a-11e8-8650-5ee8ae4a17a0.png)

This demo does the full face recognition pipeline on every frame. In practice, object tracking like dlib's should be used once the face recognizer has predicted a face.

In the edge case when a single person is trained, the classifier has no knowledge of other people and labels anybody with the name of the trained person.

The web demo does not predict unknown users and the saved faces are only available for the browser session. If you're interested in predicting unknown people, one idea is to use a probabilistic classifier to predict confidence scores and then call the prediction unknown if the confidence is too low. See the classification demo for an example of using a probabilistic classifier.
