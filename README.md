整个视频元素包含三个部分： 语音，字幕，课件内容视频。
最终输出的视频要同步三种要素。

视频生产的环节：
1. 课件内容（整个课件内容由课件内容区构成，内容区可实现不同元素，以及自定义行为。可以支持文本，图片，动画等）
课件录完后是静态的，在命令的驱动下控制内容区的显示（后台实现实时录屏）（用户可以一边说话录音，一边控制内容的展示）。录制过程中支持返回到之前的位置，从那个位置重新录制（也就是说每次采样结果会有时刻信息便于定位） 。后续还可以考虑支持剪辑拼接。

2. 字幕可以基于语音自动生成，并和语音同步。


命令
1. 整个课件就是一篇完整的文章，课件内容从前到后基于播放命令从前到后展示课件中的元素；（支持播放命令）
2. 支持建立索引，在录屏时可以滚动到课件已讲解的元素，然后可以基于控制命令切换到之前的位置。（也就是说支持元素定位命令，在已播放元素之间跳转）


课件内容录入

实现不同的课件内容
