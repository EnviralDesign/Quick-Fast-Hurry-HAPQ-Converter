# Quick Fast Hurry HAPQ Converter
 ~300-1000+ fps HAPQ converter built in TouchDesigner
 
  ***You must be in Perform Mode to get indiciated performance***
 
## Why HapQ?
 
 Most of you know about the pros and cons of HapQ for TouchDesigner, but a note for those who may not:
 
HapQ is a very efficient codec that strains the cpu minimally and gets the video data onto the GPU quickly. The one drawback is file size, your HapQ encoded video will be way bigger. However with ample storage and modern fast SSD speeds this is a tradeoff worth making in most cases where multiple video need to be played in TD, or CPU time is needed for other tasks in your software.

## Why so fast?
 
 This works so quickly because it disables TD's real-time flag, and also turns off the perform COMP's draw parameter which drastically speeds up the video transcoding process by decoupling the network cookrate from the monitors refresh rate.
 
 Your performance of course will vary based on SSD/M2 drive type , cpu clock, video card, video's resolution, and video codec. This is primarily a CPU heavy process, and will take full advantage of all your physical cores and clock speed. However, it will also be using your video card as well, so having a moderately fast or better GPU is a factor too.
 
 ## Specs & performance

### Rig
- i7-5930K ( 4.1 GHz )
- GeForce GTX 1070
- 970 EVO ( NVMe SSD )

### Video Example 1
- Media Resolution: 1920 x 1080
- Media Codec: Webm
- Media FPS: 25
- Media Duration: 4:14
- Transcode FPS: ~550
- Transcode Duration: 0:26

### Video Example 2
- Media Resolution: 1920 x 1080
- Media Codec: h264
- Media FPS: 30
- Media Duration: 12:21
- Transcode FPS: ~675
- Transcode Duration: 1:09

 ## Screenshots
 
![image](https://user-images.githubusercontent.com/10091486/126179785-bfa16da3-2f3e-4116-9419-829fc559a1e0.png)

![image](https://user-images.githubusercontent.com/10091486/126187525-28d89853-daac-438c-ba36-630da1444558.png)
