---
layout: post
title:  "用仓颉在iOS上重拾形码输入法的乐趣"
date:   2017-02-08 06:09:27 +0800
categories: cangjie
---
汉字输入法有形码和声码两个流派。作为大陆形码的主要代表，五笔输入法在二十世纪九十年代曾风靡一时，很多地方中小学生上电脑课的主要活动就是学习五笔打字。可惜对于当时大多数人来说，即使学会了，生活中也并没有使用的机会。到了新世纪电脑逐渐普及之时，这一技能早已忘却，人们纷纷拿起学习时间更长以至于近乎本能的拼音，作为与数字世界交互的工具。

但是世界的任何一个方面都不是浑然一体。依然有一些人在继续使用五笔，我就是其中一员。虽然随着拼音输入法逐渐进化至云词库时代，普通五笔使用者在输入日常用语时比拼音并没有多少速度优势，但是一方面可以对文字有更多的掌控感，另一方面也可以保有作为小众的骄傲。比如网络流行语，拼音使用者很多时候会随着输入法的词库更新不知不觉用上，事实上，有不少流行语本身就是拼音输入法的自动词组功能造就的，比如「神马」，「歪果仁」等；而五笔用户要真的喜欢真的想用才会主动打出。

##无奈与探索

但在移动设备的舞台上，则长期没有五笔的位置。功能机时代数字键盘无法与五笔兼容，智能机时代操作系统普遍不会自带五笔，iOS 中更是长期不支持第三方输入法。事实上，五笔用户依赖的是在实体键盘上手指移动形成的肌肉记忆，即使在触摸屏上实现了五笔支持，打字的感觉也与实体键盘完全不一样，需要重新思考和适应。我在 iOS 8 开放第三方输入法之后试用了新出的一些五笔输入法，可以一玩，但还是没有实体键盘那样流畅的快感。

iOS 9 作为 iPad 的重大更新，不仅有了多任务，还增加了对外接键盘的支持。我又想起五笔，既然触屏不好打，不如趁此良机购入一蓝牙键盘，畅快打字与便捷操控兼备，岂不快哉？

可是等买来键盘才发现，我付费购买的五笔输入法在连接键盘时居然无法调出。搜寻资料后才知，所有第三方输入法都无法在外接键盘时使用，可能是出于安全方面的考虑。花钱买输入法买键盘，难道到头来还是一场空？

在 iOS 系统中，简体中文只有拼音、笔画、手写三种输入方法，显然支持外接键盘的只有拼音一种。可是我在电脑上多年来只用五笔，手指早已熟悉，没有道理反而在这里接个键盘只为打拼音。我失望地在系统输入法选单里浏览，忽然看见了繁体中文，心中一动，然后在这里找到了新希望。

iOS 系统自带的繁体中文输入法有六种，除了与简体相同的拼音、笔画、手写之外，还有注音、仓颉、速成三种。注音是声码不提，仓颉是源于台湾的成熟形码方案，在台湾和香港都使用广泛；而速成是仓颉的简化版，只打仓颉的首尾两码，在学习仓颉初期拆字不熟练时，可以作为过渡方案，但重码多需要选字，不符合使用形码的本意。

所以，仓颉是目前 iOS 设备外接键盘时唯一可用的形码输入法。(注: 2020年 iOS 14 中已支持简体中文五笔输入法。)

可是这是繁体中文输入法啊，我日常使用以简体字为主，仓颉可以打出来吗？

可以的，现在字符编码都是 Unicode，各种字形都在其中，事实上在简体中文拼音输入法之下不也有繁体字吗？只是排在很后面而已。如果用注音输入法，肯定是繁体字排在前面，简体字在后面，打起来很不方便。而仓颉是形码，不需要选字，想打什么字形，就把那个字形拆分后直接打出即可。

那么用仓颉替代五笔，作为日常使用的主力输入方案是否可行？

##认识仓颉

之前只会五笔，难以想象形码还能有什么别的可能，就好像用 Mac 之前觉得 Windows 中各种操作逻辑都是天经地义一样。经过一番研究，我发现仓颉相对于五笔有以下优点：

###字库大，兼容简繁

仓颉最初由朱邦复先生于七十年代后期在台湾研发成功，当时并非只为做汉字输入法，而是为中文提供应对数字时代的全面解决方案，是集编码、存储、查询、输入为一体的大工程。所以从一开始，其设计就是以囊括所有汉字字形为目标，第三版即可打出康熙字典中的四万汉字，第五版又为简化字优化了个别编码。

而五笔只为简体字设计，在八十年代诞生时只能打 GB2312 标准中的几千个字，字根设计中有不少简体专有的部分，而一些繁体常见的元素则难以打出，可扩展性不强。直到现在，标准五笔依然打不出「喆」「玥」「赟」这些较为常见的人名用字；而仓颉不要说这些，即使是「囧」「兲」「槑」也不在话下。

###重码率低

虽然形码阵营整体都以重码率低为特色，但其中又有高下之分。五笔重码率为 20% 左右，而仓颉在字库大得多的前提下还将重码率控制在 8%。仓颉拆字时将汉字分为字首和字身，分别取码，有效识别出全字结构，是重码率低的重要原因；而五笔所有字都取一二三末四码，对首尾相同而中间不同的字难以区分，如赢（钱）、嬴（政）、羸（弱）三个字，五笔编码相同，而仓颉则能有效区分。

###设计合理，字根易记

仓颉选取二十四个基本字作为仓颉字母，本身既是常用字，又频繁用作复合字的组件。这二十四个字分成四组，按英文字母顺序排列，每个仓颉字母上再附带几个由与该字相关的辅助字形，全部字根只有一百出头。

而五笔字根多达二百，只依首笔为横竖撇捺折，在键盘上画区排列。而在各区内部，多数字根排列毫无规律，可能是计算机辅助得到的优化结果，但对于人来说难学难记。官方提供了拗口的口诀助记字根位置，可惜口诀本身的繁难就已经吓退了很多人。即使背下口诀，从口诀到键位还是不能直接对应上，需要进一步的记忆和练习。

###输入逻辑统一

仓颉没有简码，没有词组。打字时，二十四个仓颉字母直接按对应键打出，其他字全都按照同样的规则拆分。而五笔则有多套输入逻辑，首字根、其他字根、一般汉字输入逻辑各不相同，再加上简码和不同字数的词组，让人不堪其乱。

词组的本意自然是为了提高打字速度，可是增加了认知负担，让人在打单字还是打词组之间犹豫，欲速则不达。汉语以两字词居多，三字以上词出现频率低，难以形成肌肉记忆，每次用时还得现拆，击键次数虽少，但所花时间不一定比凭借肌肉记忆打单字短。两字词虽然见的多打的快，可是提高了重码率。而且各种版本的五笔词库及重码排列顺序有很大不同，在一台机器上打熟的词换一台可能并不存在，按词组编码打完发现没有，还得删掉重新打单字。仓颉则化繁为简，不搞这些捷径，只要一个一个字打就好。

###拆字符合直觉

五笔与仓颉在拆字上有很大的不同。五笔严格按照简体字形的笔画和笔顺来拆，有些时候颇需要一些想象力，因为有些笔画相交很难轻易看出拆得的字形。而仓颉只要能拆成合适部件，笔画可任意截断；顺序则依照从上到下、从左到右、从外到内的原则，而不考虑笔顺。汉字本来就是先以会意、指事、形声等构字法成字，然后为了书写方便有时会发生几画合并；而笔顺也是为了书写方便，各人或有不同。仓颉这样也更符合汉字本意。

比如「我」，五笔把那一横看作一笔归了左边的提手旁，而右边剩下的部分只能按单笔画来拆；而在仓颉之中，「我」字拆作「丿扌戈」，简单明了。再比如「事」，五笔拆成「一口⺕亅」，而仓颉则拆作「十中肀」。

##开始学习

如果读者看了以上介绍对仓颉有了兴趣，想学习它也并不困难。维基教科书 这里有很好的教程，只要花上几个小时看一遍拆字原理，再熟悉一下键位分布，就可以把字根表摆在旁边开始练习了。因为仓颉字形比五笔字根少的多，更重要的是同一键位上的字形之间有联系，入门过程比五笔要快的多。若想全面深入了解还可以看看发明人朱邦复先生的书《第五代仓颉输入法说明》。

因为从最开始朱先生就放弃了专利权，任何人都可以免费使用仓颉输入法，所以今日各个操作系统平台只要有繁体中文语言选项，基本都会内置仓颉输入法，如 Windows, Mac, iOS, 原生 Android。这样手边有什么机器都可以拿来练习和使用仓颉。国产安卓手机不了解。不过各个平台上的仓颉输入法在有些字的编码上可能会略微不一致，对简体字的支持力度也有差别。如果惯用平台比较单一，则这并不是一个问题。

从 iOS 10 开始，系统词典中增加了一本繁体中文的《五南国语活用辞典》，不仅可查汉字意思，还同时显示仓颉编码。iOS 设备上选中文字后，在弹出菜单中选择「查询」，即可查看释义和仓颉编码。这算是当下在 iOS 上学习仓颉的一个便利条件。

##得与失

我从 2016 年 3 月开始萌生学习仓颉的想法，先是用了一周时间断断续续看完了拆分原则，又把各个键位上的仓颉字母、辅助字形和例字抄写一遍，算是有了基本的了解。可是后来多次转换都未能成功，初学新输入法的打字速度实在难以满足日常所需，总是练几天就放弃。到年底时终于下定决心只用仓颉，有不会的字一一查询后记录下来。

在熬过最初几天的力不从心之后，我慢慢体会到此中乐趣，熟练度逐渐提高。到一个月后，重新找到以前运指如飞的感觉。而现在更可以无论简繁，想打就打，像写字一样自由。不管是在电脑前端坐还是只带 iPad 和键盘外出，打字的感觉一样好。这算是我的 2016 数字生活中变化最大的部分，而我也将长久受益于此。

另外需要说明的是，学习仓颉的代价除了时间和精力，还要忘掉五笔。毕竟两套输入法的基本字形还是有不少相同部件，而这些相同部件大部分处于不同的键位。大脑似乎难以同时保持两套不同的连接，我在练习仓颉初期有一些键位会受到五笔记忆的干扰，有不会的字也还会换用五笔打出来查询；到后来来自五笔的干扰越来越少，可是同时也失去了五笔打字的能力，再有不会打的字切换成五笔时脑子一片空白，只好换用拼音，或者借助于词语联想。也许在练习仓颉的同时复习五笔有可能做到自如切换，不过应该是一条更难的路，似乎也没什么必要。

仓颉输入法适合于想在 iPad 外接键盘上使用形码的人，对汉字有兴趣探索的人，想打繁体字又不满足于输简出繁的人，古文字、古代历史、古代思想文化的学习与研究者，以及愿意付出时间精力学习新技能的人。如果完全没有打繁体字的需要也不觉得正在用的输入法有任何问题，可能也确实没必要学，适合自己就好。

Happy typing.

(本文原发[少数派](https://sspai.com/post/37338))