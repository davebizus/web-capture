# Deep neural networks can now transfer the style of one photo onto another

_Captured: 2017-03-31 at 20:38 from [www.theverge.com](http://www.theverge.com/2017/3/30/15124466/ai-photo-style-transfer-deep-neural-nets-adobe)_

![](https://cdn0.vox-cdn.com/thumbor/_yj35HH-spcueJmqMPd58ftWcgQ=/0x0:2761x1684/1200x800/filters:focal\(1161x622:1601x1062\)/cdn0.vox-cdn.com/uploads/chorus_image/image/53991377/deep_learning_photos_example.0.jpg)

You've probably heard of an AI technique known as "style transfer" -- or, if you haven't heard of it, you've seen it. The process uses neural networks to apply the look and feel of one image to another, and appears in apps like [Prisma](http://www.theverge.com/2016/11/8/13548798/facebook-live-art-filters-prisma) and [Facebook](http://www.theverge.com/2016/11/8/13562288/facebook-ai-filter-prisma-mobile-app-caffe2go). These style transfers, however, are stylistic, not photorealistic. They look good because they look like they've been painted. Now a group of researchers from Cornell University and Adobe have augmented style transfer so that it can transfer the look of one photo onto another -- while still looking like a photo. The results are impressive.

The researchers' work is outlined in a paper called "[Deep Photo Style Transfer](https://arxiv.org/abs/1703.07511)." Essentially, they've taken the methods of the original style transfer, and added another layer of neural networks to the process -- a layer that makes sure that the details of the original image are preserved.

"People are very forgiving when they see [style transfer images] in these painterly styles," Cornell professor Kavita Bala, a co-author of the study, tells _The Verge_. "But with real photos there's a stronger expectation of what we want it to look like, and that's why it becomes an interesting challenge."

The added neural network layer pays close attention to what Bala calls "local affine patches." There's no quick way to accurately translate this, but it basically means the various edges within the image, wether that's the border between a tree and a lake, or a building and the sky. While style transfer tends to play fast and loose with these edges, shifting them back and forth as it please, _photo_ style transfer preserves them.

There are limits to the technique of course. The algorithms seem to work best with structures like buildings -- the flaws are more obvious with faces. And you can't use massively different photos for transferring style, otherwise the neural networks have a tougher time analyzing elements to copy from picture to picture. "If you have a picture of a lake and you have a scene where you're taking the style from, ideally it would also have a water body in it of some sort," says Bala. "There's no defined limit, but this is a good open research question. We put the code out because we want people to play with it and try it out." (The code is [available here](https://github.com/luanfujun/deep-photo-styletransfer?utm_content=buffer39dd6&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer) on GitHub.)

The question is, how long will it be until we start seeing these sorts of photo style transfer being made accessible to the public. After all, the original style transfer went from a first research paper to Facebook's app, reaching hundreds of millions of users, in less than two years' time. And with Adobe's involvement in this paper, there's obviously an expectation that it's at least a little bit interested in some sort of commercialization. We've reached out to the company to find out more, and will update if and when we hear.

For now, though, the researchers are already thinking about what areas photorealistic style transfer could be applied to next. "The question of how far you can push it is important," says Bala. "Video is a logical thing for it to go to to, and that, I expect, will happen."