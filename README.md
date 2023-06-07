# Football Player Stamina Estimation using CV

Objective: To develop an object detection system that can accurately calculate the stamina of football players based on camera video from a match.

Architecture Overview:

**1.**

Data collection and preparation: The first step involved collecting a dataset of Bundesliga football players and labeling the images to prepare them for use in training and testing the object detection models.

**2.**

Model selection: Three different object detection models were trained and evaluated on the dataset: yolov5, yolov7, and yolov8. Based on performance metrics such as accuracy, speed, and efficiency, yolov5 was selected as the best model for this project.

**3.**

Object tracking: To accurately track the movements of individual players over time, a state-of-the-art tracker called ByteTracker was added to the system. This tracker assigned a unique ID to each player, allowing their movements to be tracked and analyzed over time.

**4.**

Stamina calculation: A script was developed to calculate the stamina of each player based on two parameters: (a) the distance the player moved on screen, and (b) the number of frames the player was in possession of the ball. The proximity for ball detection was set to 30 pixels, which allowed the script to detect when a player was in possession of the ball. The stamina value for each player was calculated by summing the distances for a chosen number of frames and comparing it to a threshold value. The stamina threshold and the number of frames required to detect a drop in stamina were customizable by the user, allowing them to fine-tune the script for their specific use case. If the distance traveled was less than the previous threshold value for three consecutive frames, the stamina value was reduced by 1%, Or if the player was the first or second in terms of ball time possestion his stamina is reduced by 0.5%.

**5.**

Display and storage of results: The stamina values for each player were displayed in real-time next to their unique tracker ID. Additionally, the entire history of each player's stamina was saved to a CSV file for further analysis.

**6.**

Conclusion: This object detection system accurately calculates the stamina of football players based on camera video from a match. It uses state-of-the-art object detection models, object tracking, and customized stamina calculation scripts to provide real-time and accurate information about the performance of individual players over time.

## Samples


![Imgur Image](https://imgur.com/a/Zqd8DYt)

<blockquote class="imgur-embed-pub" lang="en" data-id="a/Zqd8DYt"><a href="//imgur.com/Zqd8DYt"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>
