# Image-Segmentation
Image Segmentation - ACRE Cascade Competition on CodaLab for the course of Artificial Neural Network and deep learning at Politecnico di Milano



ACRE is the Agri-food Competition for Robot Evaluation, part of the METRICS project funded by the European Union’s Horizon 2020 research and innovation program under grant agreement No 871252. Autonomous robots compete to demonstrate their ability to perform agricultural tasks (such as removing weeds or surveying crops down to individual-plant resolution). At field campaigns, participants collect data that are then made available for online competitions (Cascade Campaigns) like the one you are seeing. For more information about ACRE and METRICS visit the official website.

After years of decline, the number of undernourished people began to slowly increase again in 2015. Food Security requires that everyone can have enough food produced in a sustainable manner. The topic is increasingly gaining attention as food scarcity is worsened by a continuously growing population. Also, food production is threatened by climate change. The topic is so relevant that is part of one of the 17 Sustainable Development Goals of the UN 2030 Agenda. In particular, Food Security is a pillar of SDG number 2, Zero Hunger.

In this context, the agricultural sector is going under a process of revolution by the introduction of digital technologies. The Digital Agricultural Revolution can help to reduce the use of resources (water, fertilizers, and pesticides), thus diminishing the environmental contamination and the costs for the farmers. Also, it could increase the climate resilience of crops and their productivity.

Automatic crop and weed segmentation can be a driver of innovations to optimize the agricultural processes. Indeed, automatic weed detection can be exploited by a ground robot for mechanical weeding. Thus, pesticides could even be completely avoided. By joining this challenge you can contribute to advance the application of digital technologies in agriculture. We hope you will enjoy the competition :)

2-stage competition
This is a 2-stage competition. 

Stage 1 - Development: in this stage, participants are required to train their models on the Training set and submit predictions of the Test_Dev set. The submissions will be evaluated and the leaderboard results will be updated. At the end of the Development stage, we will release the labels of the Test_Dev set and the new, unseen and unlabeled, Test set.
Stage 2 - Final: in this stage, participants are required to submit predictions of the new Test set. During this stage, the leaderboard results will not be showed. 
At the end of Final stage, winners will be announced and the final leaderboard will be shown.


Dataset overview
The dataset is composed of images captured by different sensors in different moments and are about two kinds of crops: haricot and maize. Data comes from the 2019 ROSE Challenge where four teams have competed with agricultural robots. Each team has collected images of the same two crops, but in different moments and with different sensors (RGB cameras).

Images in the dataset are divided into different folders based on the team that acquired the image, i.e., Bipbip, Pead, Roseau, Weedelec. For each team, we have two different sub-folders named as the type of crop present in the images, i.e., Haricot and Mais. Finally, for each crop, we provide the captured RGB images, in the Images folder, and the corresponding ground-truth segmentations, in the Masks folder. 

We provide both the training data, collected in the Training directory, and the test data, which is used by the scoring program to evaluate participants and whose directory changes depending on the current competition stage, which can be Development (1st) or Final (2nd) stage. In particular, we refer to the test set of the Development stage as Test_Dev and to the test set of the Final stage as Test. Corresponding folders in the dataset have the same names.

Test_Dev images are provided from the first stage (Development) without any ground-truth mask. Participants are required to provide the segmentations for the Test_Dev images by submitting the solution with the correct submission format. In the second stage (Final) ground-truth masks will be provided also for the Test_Dev set, while the participants are required to provide the segmentations for the new Test images, whose ground-truth will not be provided. 
