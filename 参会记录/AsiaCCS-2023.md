# AsiaCCS 2023参会记录
## 学术记录
### 复旦老师Keynote
安全的研究点最好可以放在common to real-world application，其研究点属于硬件安全攻击或者是操作系统安全攻击。

攻击方面：out-of-range可以导致Driver Failure，cross-sensing可以导致ghost action，adversarial input可以影响预测结果,side-channel可以窃取应用层的信息：因为不同devices有不同的频率。

防御方面：重新设计操作系统或底层代码；实时的检测与防御
### 联邦学习隐私保护
作为参与者，保护本地数据的一部分属性
### 成员推理攻击
成员数据存在overfitting，可以通过样本的置信度判断。根据用户的置信度来区分成员与非成员，其中置信度使用扰动来衡量。

现有的防御思路：Dropout，L1与L2正则化，差分隐私加到本地模型上

其攻击思路LDL：使得成员与非成员在confidence上不可以区分，方法是向训练数据家高斯噪声。
### 联邦学习图学习下的隐私保护
图学习：node、sub-graph、graph三个层次

中心服务器可以发动成员推理攻击，判断sub-graph是否在某个用户
### 针对鲁棒联邦学习的推理
面临的攻击：成员推理攻击（degrading attack），使用一些评估样本即可发动攻击

poison membership inference、backdoor membership inference
### 无监督学习下隐私检验
记不清了....但是无监督学习具有很大的impact，以它为研究工具或者研究目标都很好
### 防御联邦学习下的拜占庭攻击
攻击类型：数据中毒与模型中毒、目标与无目标（恶意用户协作上传错误的参数）

防御思路：考虑用户的声望权重，考虑了非常多的隐私做优化，权重大的保留从而消除后门
### 联邦学习下贝叶斯网络的遗忘学习
遗忘目标：在贝叶斯模型下遗忘数据。考虑到贝叶斯的概率模型，可以使用抵消的思路遗忘指定数据，有简单的数学证明。

检验遗忘的效果：使用了后门数据。若达成效果，后门的攻击成功率下降。
**（不一定非得看深度学习，机器学习也有很大的潜力）**
### 联邦学习下的后门攻击
防御思路：恶意模型更新是相似的，利用聚类筛除异常模型；观察重新训练后的性能，效果差的过滤；根据历史更新创建声望权重，过滤差的用户

攻击思路：不同类别的触发器，不同的攻击目标，很难过滤

---
## 会议经历
第一次参加国际会议，一群不认识的大牛、小牛、老师、博士生和硕士生，超级尴尬，安慰自己还好有茶歇，可以吃蛋糕喝牛奶，要不然身上只有100AUD得在墨尔本挨饿了。来之前，我就在想，肯定是要赖在酒店里面，每一顿都不能错过。

第零天，达到墨尔本，和高老师联系，去吃了午饭。越南粉还可以，吃着蛮饱的。之后去了会场，第一次见了朱老师，小小地交流了一下。哈哈哈，晚上高老师请客吃了大盘鸡，第一天很顺利。**评价：劳累的一天！**

第一天，基本上一个人都不是人，超级尴尬。因为自己是单独一个人，也不太好意思跟别人聊天，自闭中...可以的话我真的想做完pre就跑。第一天，努力认识了一个北大的兄弟，Peking University我脑子一懵，问人家是不是美国的什么大学，我真该死呀！不得不佩服这个北大的兄弟，动手能力极强，英文讲的也很溜，名校崇拜我可以理解了。简单跟高老师沟通了一下，结束了第一天。**评价：社恐的一天！**

第二天，重复第一天的动作，干饭+听报告。不过，这次主动跟北大的兄弟约了午饭，下午他的pre确实精彩。晚上，参加了另外一个会议scisec，小红书认识了一个Dekin的学生，聊了聊签证、工作与论文的事情。今天成就：和朱老师聊了下，认识了一些博士和硕士。晚上，用现金吃了一顿香锅，异国他乡吃着很满足。**评价：充实的一天！**

第三天，上午听到了UTS余老师学生的汇报，研究的方向很相似，主动和他们交流了一天，中间认识了很多有趣的人。下午，去了淘金镇参加旅游活动，实际上冻的不轻，一群人在外面烤火。晚上，吃了一顿“美味”的大餐，中国胃吃不惯呀，领了Distinguished Paper Award。吃完饭，已经很晚了，车上跟高老师讨论了研究进度还有一些思路，虽然有些尴尬，但是收获还是很多的。**评价：有意义的一天！**

第四天，上午在住处练习pre。中午出发，吃了午饭，哈哈哈，我就是个干饭人。下午做pre的人超级少，听的人也不多了，我就是主会场的倒数第二，真的没什么人，有一个莫纳什的师兄愿意帮我提问一下。很尴尬的是，我接的并不是很好，磕磕巴巴的英语，还需要再练习英语呀。pre语速也是偏快了，因为第一次上台说英语还是紧张了，20分钟的内容，16分钟结束了。松弛一点，放松一点。晚上，和莫纳什的师兄聊了很多，八卦还有生活。最后，白吃了一顿中餐，真的是我这几天吃过最好的一顿了，我要哭了。晚上，我一个人逛了逛，买了袋鼠制品，巧克力等等**评价：放松的一天！**

**总结：开会最重要的是交流，后几天开会会主动问别人，不会社恐了。而且别人会很乐意跟你交流，很棒的体验。**

