---
layout: post
title:  "ZebraVision 4.0 - Goal Detection"
date:   2016-05-23
excerpt: "Zebravision 4.0 is Team 900's vision system for the 2016 season; FIRST Stronghold. Our work was focused around recognizing the vision goals using shape and color based matching, recognizing the boulders using a neural network, and integrating the detection systems into a tracking system using the StereoLabs ZED stereo camera. One of the main features of Team 900's Zebravision code this year was goal detection. This paper gives an overview of the hardware and code used. The system used a Stereolabs ZED RGB-depth camera and green LED rings to highlight the retroreflective tape around the goal. The image was filtered to look for the reflected LED color and thresholded to turn it into binary green / not green image. The code then extracted contours from the image and applied a number of simple filters to rule out blobs which were obviously not goals. The remaining contours were scored in a number of criteria and the best scoring few objects were assumed to be goals. If more than one valid goal is found, several tiebreakers were used to pick one goal to shoot at. If a valid goal was found, the angle and distance to the target was reported; if none were found, a packet with -1.0 distance and angle was returned to the roboRIO."
authors: Alon Greyber
tags: [Programming, Vision]
---
<ul style="text-align:left">
  <li><a href="https://drive.google.com/open?id=0B8hPVHrmVeDgUWtLbDVmbFV3Y3M" target="\_blank">Paper</a></li>
  <li><a href="https://www.chiefdelphi.com/forums/showthread.php?t=148537" target="\_blank">Chief Delphi Post</a></li>
</ul>
