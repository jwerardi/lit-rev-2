James Erardi
Literature Review II
3-18-2018

For my second literature review, I decided to look into advancements in image processing. One may not know it, but they participate in advancing image processing technology almost every day they use the internet. Tagging pictures on social media websites has been a major source of data for image processing engineers, where they'll be able to slowly construct models based on data derived from humans tagging things as other things on social media. Captchas are another major source of information for image processing technology. I've noticed that, over the past year, most image related captchas now revolve around classifying images that are involved in driving - challenges like selecting the stop signs in a photo, selecting the road signs in a photo, selecting different storefronts in a photo. All of this data goes towards building image recognition software, and more specifically, image recognition software that goes into autonomous automobiles. I think it's pretty cool that every time you complete a captcha challenge, you're doing your part to advance AI technology.

One of the articles I chose delves into image recognition when it comes to classifying where a crosswalk is in a low resolution photograph. It is quintessential for an autonomous vehicle to understand where crosswalks are, otherwise they could hit unsuspecting pedestrians by accident. Another benefit for machine learning to understand where crosswalks are is for accessibility purposes, specifically for those who are visually impaired. The article I chose goes into great length speaking about this, how they've developed software for mobile devices that will help visually impaired persons find crosswalks. The way the software works is fascinating to me; first, the software figures out where the user is based on GPS coordinates derived from their smartphone's geographical sensors. Then, the coordinates are sent up to a cloud computing system which will look the coordinates up on Google maps, take a snapshot of what Google maps shows for their street view (street view is a feature of Google maps where it will show a real photograph of the location you're looking at). The cloud computers will then process the snapshot derived from Google maps in order to figure out where the crosswalk resides within the snapshot. Finally, there is a difference calculated between the crosswalk and the user, which is then relayed to the user in a form similar to how Google's navigation app works (ie, 'Take 10 steps to your left to get to the nearest stopwalk'). This entire process has an amazing 96.9% accuracy! The authors cite that there is still a lot of room for improvement, specifically in the initial process of retrieving the GPS coordinates of the user.

The second article I chose relates to the need for immense computing power to process these images. In my previous article, when the coordinates were sent up to the cloud, all of the image processing was localized to the cloud, in other words, no images were relayed back to the client. But what if the user wanted to see the crosswalk? Which, I know is a bit ironic considering the app was designed for the visually impaired - but bare with me for example's sake. If the user wanted to see the processed crosswalk on their device, it would require an immense amount of computing power that just isn't feasible to have in a compact device such as a smartphone. This is where SCIs, also known as Screen Content Image, come into play. SCIs are images that have been previously processed by an advanced computing system, nailing out all of the minor details which take massive computing power, which are then sent to a client's device for their high resolution viewing pleasure.

The way SCI works involves complicated mathematical equations which will offload the more computationally intense aspects of rendering an image to a cloud computer, such as figuring out the Gaussian window or optimizing the best compression path. A lot of the article delves into the math behind processing the images, which I will admit is a bit over my head, but the bottom line is that by preprocessing much of the complicated aspects of rendering an image, researchers were able to serve complicated graphical interfaces nearly 10% faster than traditional ways. This may not seem significant, but optimization is a slow and grueling process and this is a huge feat for such a complicated situation.


@ARTICLE{7478448,
author={M. C. Ghilardi and J. Jacques Junior and I. Manssour},
journal={IEEE Computer Graphics and Applications},
title={Crosswalk Localization from Low Resolution Satellite Images to Assist Visually Impaired People},
year={2018},
volume={38},
number={1},
pages={30-46},
keywords={Global Positioning System;handicapped aids;image classification;image resolution;image sensors;object detection;smart phones;support vector machines;Google Road Map;SVM classifier;assist visually impaired people;crosswalk detection;crosswalk localization;embedded GPS;false alarms;image noise;low resolution satellite images;nearest detected crosswalk;visually impaired person;Computational modeling;Global Positioning System;Image processing;Image resolution;Object recognition;Rendering (computer graphics);Satellites;Image Based Modeling and Rendering;accessibility technologies;image processing;image segmentation},
doi={10.1109/MCG.2016.50},
ISSN={0272-1716},
month={Jan},}



@ARTICLE{7478441,
author={S. Wang and K. Gu and K. Zeng and Z. Wang and W. Lin},
journal={IEEE Computer Graphics and Applications},
title={Objective Quality Assessment and Perceptual Compression of Screen Content Images},
year={2018},
volume={38},
number={1},
pages={47-58},
keywords={data compression;image coding;statistical analysis;graphically rich services;information content;local quality assessment;newly proposed quality assessment measure;objective quality assessment approach;perceptual compression;perceptual screen content;perceptually optimal SCI compression schemes;pictorial regions;quality assessment method;screen content image;structural similarity;textual/graphical content;virtual desktops;visual field adaptation;wireless displays;Distortion;Image coding;Quality assessment;Rendering (computer graphics);Visualization;computer graphics;image quality assessment;perceptual compression;screen content image},
doi={10.1109/MCG.2016.46},
ISSN={0272-1716},
month={Jan},}


