During the graduation project on the topic: "Automated detection of gastric polyps from endoscopic images using deep learning methods", the main goal was achieved: a deep learning model was developed and implemented for automatic segmentation of areas containing polyps, followed by visualization of the results and implementation in medical practice. This approach makes it possible to increase the accuracy, reproducibility and speed of diagnosis in capsule endoscopy, as well as reduce the burden on medical personnel.

An analysis of the subject area and a review of the literature allowed us to identify the key problems of diagnosing gastric polyps and justify the choice of methods. An important argument in favor of using neural network solutions was the high percentage of pathology omissions during manual image processing and the lack of sufficient automation at the analysis stages.

The selection and preparation of the [KvasirCapsule-Seg] and [Kvasir-SEG] datasets required preliminary data adaptation. Augmentation techniques were applied using the Albumentations library, and polyp masks were prepared for segmentation tasks. It has been shown that even with a limited set, high accuracy can be achieved if the model is correctly architecturally configured and transfer learning methods are applied.

Throughout the project, a complex task was solved, covering the entire cycle: from analyzing modern solutions in the field of machine vision to creating a practical web service available for testing in a clinical setting. The work was based on the use of convolutional neural network (CNN) architectures, in particular the U-Net model, modified for the MobileNetV2-UNet, AutoKeras-ResNet, Ensemble_model task. These architectures have proven to be effective tools for semantic segmentation tasks in medical imaging due to their ability to accurately identify even small anatomical structures.

The construction, modification and training of the U-Net, MobileNetV2-UNet, AutoKeras-ResNet, Ensemble_model models made it possible to compare the effectiveness of the classical architecture and its modified variants. Using MobileNetV2 as an encoder has significantly improved the results, especially with limited data. Dice and IoU metrics were used in the training process, providing an objective assessment of the quality of segmentation. The obtained metric values confirm the high sensitivity and accuracy of the model, especially in the case of MobileNetV2-UNet.

The development of the REST API using Flask ensured the practical integration of the model into the work environment. The system takes images, performs segmentation, and returns the result to the user in the form of a photo of a polyp with a outlined outline. This format is ideal for further visualization in medical systems. Thanks to the use of the OpenCV library, efficient image preprocessing has been performed, as well as scaling of input data.

Integration with the ngrok service made it possible to create a public URL where the model becomes available to external users. This simplified the demonstration of the project and made it possible for doctors and researchers to conduct remote testing without having to host a server on the network. This approach is of particular importance in terms of prototyping and clinical testing of models based on real data.

Key achievements of the project:

• Implemented a polyp segmentation model capable of working in real time;

• High accuracy demonstrated;

• The transfer learning method has been successfully applied;

• An API service has been developed that is suitable for integration into clinical workflows;

• Remote access to the system with the possibility of demonstration is provided.

The project has important practical significance. Given the growing burden on medical professionals and the need to improve the quality of diagnostics, the use of computer vision systems can significantly reduce the number of missed polyps, especially in hard-to-reach and poorly visualized areas of the gastrointestinal tract. Segmentation is a more difficult task than classification, as it requires precise localization of the object. The upgraded MobileNetV2-UNet model showed high resistance to a small amount of training data and was able to achieve a high level of generalization, which is critical in real clinical conditions.

Development opportunities:

Using more complex architectures is the implementation of Attention U—Net, transformers, Reinforcement Learning and Recurrent Neural Networks, RNN.

Feedback from doctors is the introduction of interfaces for manual correction of masks and subsequent retraining of the model (active learning).

The visualization module in the form of a web interface is the creation of a simple browser application for working with images, which will simplify implementation in clinical departments. Connecting the model remotely to streaming video during endoscopic examination of the patient.

Security and compliance with standards — further refinement of the API taking into account GDPR/HIPAA, the addition of authentication, logging, IP filtering.

Working on the project allowed the author to master modern methods of image analysis, deepen his knowledge in the field of machine learning, and learn how to work with neural network architectures and their practical implementation. Special attention was paid to the issues of model validation, interpretation of results, as well as building an effective pipeline — from loading data to obtaining a prediction. In addition to the software implementation, aspects of medical imaging and clinical features of the diagnosis of gastrointestinal diseases were studied.

The project was carried out individually, which required full responsibility for all stages — from setting the task to testing the model in the form of a web service. This provided a comprehensive understanding of the process of implementing AI in medical applications.

Thus, the thesis project is a complete and practically oriented system of automatic segmentation of gastric polyps, ready for clinical testing. Using the upgraded MobileNetV2-UNet architecture in combination with the Flask and ngrok REST API allowed not only to achieve high accuracy rates, but also to ensure the practical applicability of the prototype. The results confirm the potential of deep learning in medical diagnostics and demonstrate how modern technologies can be adapted to meet real-world healthcare challenges.
