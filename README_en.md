# Definition, recognition method and operation suggestion of video re-creation 

## [English Version](https://github.com/JollyToday/GhostCut_Recreate_Video/blob/main/README_en.md "GhostCut re-create videos info") --- [中文介绍](https://github.com/JollyToday/GhostCut_Recreate_Video/blob/main/README.md "鬼手剪辑视频去重中文介绍")

## Background and significance of re-create videos

For platforms recommended by algorithms such as Douyin, Kuaishou, TikTok, and YouTube Shorts, highly innovative materials have extremely high value, which can significantly increase user activity on the platform. Creators will also receive incentives from the traffic provided by the platform, further enhancing their creative passion. Video mixing, re-creation, and deduplicate production can lower the threshold for video making, enabling more customer engagement in video creation and sharing. The platform can attract more users to join, expand the client base and market share, increase the active level and influence of the platform, and bring more commercial value and cooperation opportunities.

However, mass production such as video remixing, video re-creation, and homogeneous videos will also bring a large amount of low-quality and repetitive materials to the platform, destroy User Experience, and reduce the passion of excellent creators. Therefore, how to identify excellent re-creation needs to be balanced and carefully identified from the perspective of the platform. Based on the disclosed creator content plans and video deduplicate processing schemes of ByteDance, Kuaishou, and YouTube, this project summarizes the identification methods and operation suggestions for high-quality videos and re-creation deduplicate videos.

## Identification and judgment criteria for first-release video materials and homogeneous videos

### **First release material definition and judgment criteria**

- First release material refers to highly innovative material that is used for the first time on the platform
- Judgment method:
  - The machine will cut the material into n storyboards
  - When a material with other materials similar storyboard (≤ 10%) in its video accounted for a relatively low , it is judged as the first material

### **Definition and criteria for determining homogeneous materials?**

- Homogeneous materials refer to materials that are not used for the first time on the platform and have a low degree of innovation.
- Judgment method:
  - The similarity recognition of the content dimension of the material is carried out by the system model, without specific rules and scope. For example, only replacing the background music, only replacing the post 3 seconds front, or only adjusting the material tone, brightness, etc. can easily be judged as homogeneous material.
    
Tips : material storyboard picture similarity ≤ 10%, the first release class; material storyboard picture similarity ≥ 60%, the homogeneous material.

## Evaluation criteria and processes for high-quality video materials

- - Douyin, Kuaishou, TikTok, YouTube and other platforms evaluate whether the video material is of high quality. The core rules start from the aspects of sound and picture quality and content value. The material must meet five conditions at the same time to be judged as high quality
  - The five conditions are: sound, picture, consistency of sound and picture, information subject, and information expression
  - The five conditions are judged in a "either negative or positive" manner. Each rule under this rule uses the "passing line" as the execution standard. We hope everyone has the opportunity to create high-quality materials

![image](https://github.com/JollyToday/GhostCut_Remake_Video/assets/128401459/85841450-dc3f-42da-aabb-28058661368c)

- The evaluation of high-quality materials is launched after the materials are uploaded, and whether they are of high quality is confirmed by both machine and manual review
- When a video starts to upload and reaches a certain exposure level, it automatically enters the high-quality material evaluation process, and the creator does not need to go through additional operations
  - Materials with evaluation results that are not of high quality may also have normal publish streaming without negative impact
  - If the evaluation result is inferior material, the system will give prompts, including but not limited to excessive repetition, infringement, low image quality, unsuitable content, etc

![image](https://github.com/JollyToday/GhostCut_Remake_Video/assets/128401459/754567ca-867b-46b6-8a10-d3be26623776)


The official and system allow for the exploration of material minor modifications within a reasonable range, which is mainly determined by the supply of system, algorithm, and market content. Therefore, in a single period of time, it is not necessary to have a certain amount of high-quality materials, nor does it mean that low-quality materials cannot explode. Even slightly modified materials may receive good traffic, because the evaluation and recommendation status of the algorithm at each time point is unstable, and short-term positive and negative feedback is a case. Therefore, the re-creation video materials processed by video deduplicate should avoid entering the low-quality | duplicate material judgment area and strive to enter.

## What is video re-create and why do we need to do it?

The existence of video deduplicate has its practical significance. Video re-creation can reduce the threshold of video making and enable more customers to engage in video creation and sharing. In recent years, with the increasing importance of videoization and algorithms, the life cycle of short videos has further shortened, which puts forward higher requirements for the production speed and quality of short videos. On the one hand, video editing is limited by the insufficient number of video materials, and on the other hand, the system requires continuous production of innovative videos, which is difficult for most small and micro creators. In product sales and food exploration areas, the shooting and editing capabilities of merchants themselves are limited, and the quantity of SKU products is limited. Therefore, video re-creating and mixed editing are a low-cost and efficient production method.

The official platform and algorithm system allow material micro-modification exploration within a reasonable range, but "homogeneous material" belongs to materials with high similarity, such as **only replacing background music, only replacing 3 seconds front of the video, or only adjusting material tone, light and shade , etc. It is not enough**; in addition, each editing software and video downloaded by each video platform will be embedded in fingerprint information by the video platform to prohibit the transfer of other people's materials to infringe.

When we need to copy and edit other people's materials, or when we don't have enough materials on hand, we need to re-edit these materials. Therefore, we need to use the logic of deduplicate.

Video re-creation is a kind of video material editing operation that achieves a certain degree of innovation through micro-modification. By adjusting the video storyboard, sound, sound effects, music, picture, subtitles, expression structure, etc., the processed video is non-homogeneous with the original video, avoiding the judgment logic of "homogeneous material". Similar definitions and operations include video mixing, video re-creation/secondary modification, video rewriting, video deduplication, etc., most of which have similar logic.

## Judgment criteria and cases for repetitive and homogeneous materials

The following are the standards and cases of duplicate and low-quality materials organized according to official materials such as ByteDance, Douyin, TikTok, etc., which are not worth using a single deduplicate method:

| Adjust direction | Neutron direction | Re-creation detection rules |
| --- | --- | --- |
| Timing sequence | Adjust duration | Only a small amount of clips are edited from the same material, reducing the duration. |
|  |  | Only add a small amount of clips for the same material, such as posting a few seconds ago or a few seconds later, to increase the duration. |
|  | Adjust order | The exact same material, only adjust the order of the segments. |
| Visual | Detail adjustment | Adjust the brightness only |
|  |  | Add subtitles only |
|  |  | Only add some special effects |
|  |  | Only add part of the template border |
|  |  | Only change the transition method |
|  |  | Only change the shooting angle or distance |
|  | Product adjustment | The main body of the video is exactly the same, only changing the color, position, angle, etc. of the product. |
|  | Mixed clipping of fragments | Completely similar fragments are mixed with each other, and the content repetition is extremely high. |
| Sound | Background sound | Only replace background music |
|  | Dubbing | Only change the dubbing tone, a small amount of copy, etc. |


In the above official rules and cases, we found that simply trying to achieve video deduplicate through a single measure is basically ineffective. The system uses various techniques to comprehensively identify the timing of material clips, slight changes in visual images, and detection of sound changes. Therefore, the deduplicate methods you see on the market, including but not limited to: changing MD5 , picture clipping, video acceleration and deceleration, video frame extraction, video picture-in-picture and other video processing methods, are relatively basic solutions and have gradually become ineffective.

To solve this problem, we need to create more innovative video materials. Editing that reflects the labor of "intelligence" can usually be welcomed by the official. For details, please refer to the following rules

| Account rating |  | Handling | Low-cost secondary creation | High-cost secondary creation | Normal |
| --- | --- | --- | --- | --- | --- |
| Processing strategy |  | Filter/block/block | Cautious support/filtering/blocking/blocking | Support/Cautious support | Support |
| Content judgment basis | Editing technique | There is no editing, and there are watermarks on the screen recording content of others. | High definition and uniform style but no simple editing (including but not limited to fixed text, stickers, emoticons) | Increase high-cost processing such as subtitles and commentary, and increase multiple editing methods | External links exist, authenticated or can prove to be original or original potential |
| Account judgment basis | Content as a percentage | The above content alone or collectively reaches 30% of the last 30 contents of the account. | The above content alone or collectively reaches 50% of the last 30 contents of the account. | The above content alone or collectively reaches 50% of the last 30 contents of the account. |  |

Due to factors such as energy, manpower, cost, and time, the official has recommended some methods that can improve the originality of videos and achieve the effect of deduplicate. Let's follow the official to see how to achieve advanced deduplicate.

## Video re-creation under official guidance

The official and system allow for exploration of material minor changes within a reasonable range, but "homogeneous material" belongs to materials with extremely high similarity, such as only replacing background music, only replacing 3 seconds ago, or only adjusting material tone, brightness , etc. It is not enough; in order to avoid extremely high similarity, the official has the following suggestions (incomplete version) for re-creation editing, including
1. The content remains unchanged, but the form of expression changes
2. Typesetting & animation do addition and subtraction
  1. Add design-oriented parts to make new materials independent in design perception
  2. The number of elements in the picture remains unchanged, rearranged and combined
  3. Self-designed position layout, size combination, color matching
3. Need to be related to sound and picture
Let's understand the above suggestions
1. Need new copy, script or commentary
2. There needs to be significant changes to the picture, including new stickers, sales boost, sound effects, and subtitles. The combination of these things needs to be creative and aesthetic
3. Need new dubbing
Therefore, comprehensive "surgery" must be carried out on the picture, sound, music, rhythm, shots, etc. of the video in order to truly achieve the perfect effect of "video plastic surgery".

## Comprehensive video re-creation through video rewriting to achieve efficient deduplicate.
GhostCut innovatively uses AI to rewrite videos, which can regenerate images, subtitles, dubbing, layout, stickers, etc. in one go to improve the deduplicate ratio. GhostCut can complete the following operations at one time


| Classic re-create | Visiual re-create | Subtitles re-create | Voice re-create | Music re-create | AI Template |
| --- | --- | --- | --- | --- | --- |
| Basic deduplicate | Random mirroring | Erase original subtitles | AI dubbing | Match specified music | Good stuff |
| Modify md5 | Random transition | Override new subtitles | Dozens of tones | Intelligent music | Add Progress Bar |
| Remove video fingerprints | Stochastic acceleration | AI rewrites subtitles | * Sound cloning | Keep the original background music | Smart matching sticker |
| Intelligent color grading | Random movement | Change subtitle style |  | * Smart matching sound effects |  |
| Cut off the head and tail. | Smart scaling | Change subtitle base color |  |  |  |
| Screen sharpening | Mirroring inversion | Translate subtitles |  |  |  |
| Intelligent frame extraction |  |  |  |  |  |

After the above video rewriting, each video has undergone significant innovative changes in graphics, subtitles, voice, music, and template effects compared to the original video.


If all of the above operations can be completed at once, do you want to give it a try? The video after the above rewriting can get better traffic support from the platform.

## Through advanced re-creation of GhostCut, complete video rewriting of audio, video, and subtitles at once

The GhostCut developed by JollyToday Technology has been using AI to provide video editing services for the majority of users. Today, it has been a super big update on the video deduplicate function（Video Re-Creation）!
![image](https://github.com/JollyToday/GhostCut_Remake_Video/assets/128401459/fc3fc123-d9b1-449b-b0d4-95f4fc112fba)



The advanced re-creation function added by GhostCut can not only automatically rewrite video content, but also add sound and subtitles to your video, making your content look brand new! This is a boon for creators of oral endorsement content.

## Advanced Re-creation Operation of GhostCut

GhostCut innovatively regenerates images, sounds, subtitles, layout, stickers, and storyboards with AI . The AI-rewritten copy makes the content of each product different. The change of AI dubbing makes each video regain its sound machine. GhostCut has Chinese and English versions, and also supports WeChat Mini Program and computer version. The specific operation process on the mobile phone is as follows:
Open the GhostCut Mini Program, click Advanced re-creation/oral endorsement re-creation, enter the operation page, as follows, a total of three steps
1. Upload a video
2. Choose the line processing method and deduplicate method
3. Submit waiting results
![image](https://github.com/JollyToday/GhostCut_Remake_Video/assets/128401459/added423-d4ab-408a-b13c-4873229c5f93)


## GhostCut Advanced re-creation Technology

The advanced re-creation core of GhostCut is video rewriting, which means first extracting the content of your original video, and then using a method similar to deduplicating a paper to change the wording of the original video while maintaining the same meaning in different words. Then, the rewritten content is dubbed and subtitled. The specific operation is as follows:

1. Extract video copy
2. Rewrite video copy
3. Erase original video subtitles
4. Intelligent deduplicate operation of video: change md5 , crop, acceleration and deceleration, picture-in-picture, frame capture, random mirroring, random transition, dynamic scaling and so on
5. Add subtitles to new videos
6. Dubbing according to the subtitles of the new video
7. Calculate the position of new dubbing, subtitles, and images based on the alignment position of the original video subtitles, voice, and image for audio-visual alignment
8. Add template borders
9. According to the new video copy, intelligently add new stickers and sound effects
10. Finish video synthesis
    
AI rewritten copy makes the content of each product different. The change of AI dubbing makes each video regain its beautiful sound .

## GhostCut video Re-creation advantages?

GhostCut offers an intelligent video re-creation product. It uses AI technology and video processing technology to process the MD5 , fingerprint information, visual information, audio information, subtitle information, etc. of the video, helping everyone to better and faster re-creation of the video. Compared with using CapCut or PR template deduplicate editing, its characteristics are: fully automatic, multi-mode, supporting the combination of subtitles and voice, which belongs to more advanced secondary creation.
This feature of GhostCut has the following advantages:

#### 1. Automated processing
GhostCut doesn't require you to edit each video yourself. It can automatically recognize similar content and rewrite it. This means you can save a lot of time and effort and spend more time on creation.

#### 2. Improve content uniqueness
Traditional video deduplicate methods simply delete similar content, but GhostCut can cleverly rewrite the content to maintain the original theme while having a new way of expression. This makes your video more unique and attracts more viewers.

#### 3. Provide sound and subtitles re-write
GhostCut is not just a video deduplicate tool, it can also add sound and subtitles to your videos. This makes your videos more attractive and suitable for different languages and audiences.

GhostCut innovatively AI regenerates images, sounds, subtitles, layout, stickers, and storyboards. The AI-rewritten copy makes the content different every time it is produced. GhostCut has Chinese and English versions, and also supports WeChat Mini Program and computer version. GhostCut will soon launch many AI video deduplicate functions such as sound cloning, video mixing, one-to-many etc. Welcome everyone's attention and experience.

### Tips: Q & A related to video originality, video homogenization, and video deduplicate

| Category | Ask | Answer |
| --- | --- | --- |
| Definition | How to distinguish between homogeneity, originality, first release, and innovation? | Original, first release, homogenization, and similar materials all belong to the concept of creative ecology innovation |
|  | What is the difference between first release and high quality? | Both the first release and high-quality are sub-projects of the creative ecosystem, and both have incentive strategies. If the material is both first release and high-quality, it will enjoy the incentives of both. |
| Recognition | Why wasn't my original material judged as the first release? | The concept of first release only represents the material uploaded for the first time on the platform. The same batch of video clips only replaces multiple videos generated in chronological order, and probably only the first uploaded one is the first release. |
|  | Similar materials uploaded by the same account, only one is judged as the first release, and the rest are judged as non-first release? | If multiple similar innovative materials are uploaded to the same account, only the first one uploaded will be judged as the first release, and the rest will be judged as non-first release. |
|  | Will materials marked as first released become non-first released materials in the future? Will materials marked as non-first released materials become first released materials? | No. |
|  | Is the first release "original script + original shooting"? | First release recognition is based on the model's similarity judgment of video storyboards. It is recommended to prioritize the use of "original shooting" images in new materials to improve the proportion of first release materials. |
|  | How to understand storyboard, similarity, and proportion? Can it be understood as video clips, the same clips, and the proportion of time? | 1. Similar storyboards: A shot in a video can be regarded as one storyboard. Generally, a fixed shot + fixed model action will be regarded as one storyboard, and a video with multiple shots will be regarded as multiple storyboards
2. Similarity ratio: At the same time, assess the proportion of similar duration and similar duration in the material, and multiple similar storyboards for short periods will accumulate similar duration. |
|  | Is it the first release or non-first release to release material after it has been released for a period of time and then release it again? | 1. If a material (with the same creative ID dimension and content) is judged to be the first release, it will easily not change its status
2. After modifying the title , transition, end credits and other content of the same video, it is regarded as a new material and needs to be re-judged whether it is first released |


### Tips: What is video fingerprint information?
Generally speaking, directly downloaded watermark-free videos usually contain the following key information
1. MD5 of the original video;
2. The meta information of the original video is placed in the video fingerprint information of the social media platform; [Refer to the table below]
3. Hidden watermark formed by other video algorithms, also known as hidden watermark.
Video fingerprint is the most basic element of duplicate detection. The basic operation of video deduplicate is to remove these video fingerprint information first.

### Tips: The video fingerprint information will change after being processed by the GhostCut.

Through the table below, you can find out what metrics have changed in the video.

In the base MD5 and video fingerprint information, the GhostCut is fully automatic to make changes.

| Type | Directly use watermark-free software | Download directly from social media (with platform watermark). | GhostCut Re-creation | Note |
| --- | --- | --- | --- | --- |
| File size | 720 | 720 | 720 | Support 1080p |
| Document duration | 9 s 567 ms | 12 s 567 ms | 8 s 745 ms | Duration changes randomly |
| Description information |  |  | kGKBf4vhCEe5J95owhfZ1y8cOAUrtJoLIDeGroNW7igVKRMbRdxd/vDVtJfUMQlz | Randomly add |
| Copyright information |  |  |  |  |
| Digital signature | AZ6e6gmu4XqJutoDL8i5aiDHRSid | AaGf7KMzw1W5Xt1wDAyXVlW2x3ix | ARpWxirh3AnpeNYJ6Y+E7c97l02g | Random change |


### Tips: What factors are related to the quality of deduplicate and the approval of dou + and vermicelli?
The quality of deduplicate is generally related to the level of the account, the popularity of the material, and the time of re-creation
- The level of the published account itself needs to be of high quality. The newer the account and the account that has been risk controlled by the platform, the higher the requirement for deduplicate degree.
- The more popular the material, if it comes from popular or celebrity materials, the higher the requirement for deduplicating the material.
- The closer the time, such as the hottest material of the day, the higher the requirement for deduplicate.
- If it is uploaded on the same platform, the deduplicate requirement is also very high, and cross-platform will be easier.
It is recommended that the popular content be re-imported into the CapCut, and then add other commentary, subtitles and material fragments, etc., and then choose 1080p, 60 frames re-exported and uploaded.

### Note: It is strongly recommended to communicate with the original author and MCN organization to obtain the copyright of the original material to avoid copyright disputes caused by the use of other people's materials.
The official and system allow for the exploration of material minor modifications within a reasonable range, which is mainly determined by the supply of system, algorithm, and market content. Therefore, in a single period of time, it is not necessary to have a certain amount of high-quality materials, nor does it mean that low-quality materials cannot explode. Even slightly modified materials may receive good traffic. This is because the evaluation and recommendation status of the algorithm at each time point is unstable, and short-term positive and negative feedback is a case. In the long run, continuously contributing to the platform and content that users like will receive long-term positive feedback .

### Reference
- [Creative Ecology] Launch Material Project Introduction
- Material Innovation - How to Innovate at Low Cost
- The "Homogeneous Materials" documentation (external) is continuously updated.
- ByteDance Ads-Massive-Low Quality Material Standard Detailed Rules
