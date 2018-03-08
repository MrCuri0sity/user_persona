###  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Big picture of user persona
**我想强调的是，同一个人有多个自画像。与其追求照相般的相似性，不如深入发掘相似处。<br> 
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ——Vincent  van gogh**
![vincent van gogh](https://github.com/MrCuri0sity/user_persona/blob/master/photos/vincent.png?raw=true)<br>

#### 0. 写在前面<br>
本文仅为本人学习使用，了解用户画像的读书笔记，文中大部分内容来自互联网，如有侵权，请联系我(792706244@qq.com)删除

#### 1. 什么是用户画像<br>
persona(also user persona, customer per	sona, buyer persona)最初在腾讯被叫做用户画像，wiki上的解释是a fictional character created to represent a user type， 简单说就是给用户打标签，展示用户的全貌。譬如用户画像的标签可以是**姓名、年龄、家庭状况、收入、工作、用户场景、计算机技能等.**用户画像提出者Alan Cooper 将用户画像分为以下三个类别：<br>

- Marketing persona：focus on demographic information, buying motivations and concerns, shopping or buying preferences, marketing message, media habits and such. Marketing personas are good for determining what types of customers will be receptive to certain products or messages, or for evaluating potential ROI of a product. What they are not good for is for defining a product or service – what it is, how it will work, and how it will be used; or for prioritizing features in a product or service.<br>

- Proto—personas：are used when there is no money or time to create true research—based personas – they are based on secondary research and the team’s educated guess of who they should be designing for. According to Cooper, using a proto—persona to drive design decisions is still better than having no persona at all — though of course they should be validated with research! <br>

- Design personas focus on user goals, current behavior, and pain points as opposed to their buying or media preferences and behaviors. They are based on field research and real people. They tell a story and describe why people do what they do in attempt to help everyone involved in designing and building a product or service understand, relate to, and remember the end user throughout the entire product development process. Design personas are good for communicating research insights and user goals, understanding and focusing on certain types of users, defining a product or service, and avoiding the elastic user and self—referential design.<br>

#### 2. 建立用户画像<br>
大方向上，建立用户画像包括如下四个步骤：<br>

- step1战略解读：企业选择构建用户画像平台，可以实现不同的战略目的，如提升产品服务质量、精准营销等。根据战略目的的不同，用户画像的构建也有所区别。因此首先需要明确用户画像平台的战略意义、平台建设目标和效果预期，进而有针对性的开展实施工作。
- step2建模体系：对用户画像进行数据建模，结合客户实际的需求，找出相关的数据实体，以数据实体为中心规约数据维度类型和关联关系，形成符合客户实际情况的建模体系。
- step3维度分解：以用户、商品、渠道三类数据实体为中心，进行数据维度分解和列举。根据相关性原则，选取和战略目的相关的数据维度，避免产生过多无用数据干扰分析过程。
- step4应用流程：针对不同角色人员的需求(如市场、销售、研发等)，设计各角色人员在用户画像工具中的使用功能和应用/操作流程。

其中建模体系主要包括如下流程：<br>
![](https://github.com/MrCuri0sity/user_persona/blob/master/photos/model_steps.png?raw=true)
(1) 数据收集<br>
&nbsp; &nbsp; &nbsp; &nbsp;数据收集大致分为网络行为数据、服务内行为数据、用户内容偏好数据、用户交易数据这四类。当然，收集到的数据不会是100%准确的，都具有不确定性，这就需要在后面的阶段中建模来再判断，比如某用户在性别一栏填的男，但通过其行为偏好可判断其性别为“女”的概率为80%。还得一提的是，储存用户行为数据时最好同时储存下发生该行为的场景，以便更好地进行数据分析。<br>

- 网络行为数据：活跃人数、页面浏览量、访问时长、激活率、外部触点、社交数据等
- 服务内行为数据：浏览路径、页面停留时间、访问深度、唯一页面浏览次数等
- 用户内容便好数据：浏览／收藏内容、评论内容、互动内容、生活形态偏好、品牌偏好等
- 用户交易数据（交易类服务）：贡献率、客单价、连带率、回头率、流失率等

(2) 行为建模<br>
&nbsp; &nbsp; &nbsp; &nbsp;该阶段是对上阶段收集到数据的处理，进行行为建模，以抽象出用户的标签，这个阶段注重的应是大概率事件，通过数学算法模型尽可能地排除用户的偶然行为。这时也要用到机器学习，对用户的行为、偏好进行猜测，好比一个 y＝kx＋b 的算法，X 代表已知信息，Y 是用户偏好，通过不断的精确k和b来精确Y。在这个阶段，需要用到很多模型来给用户贴标签。模型举例如下：<br>

- 用户汽车模型:根据用户对“汽车”话题的关注或购买相关产品的情况来判断用户是否有车、是否准备买车
- 用户忠诚度模型:通过判断＋聚类算法判断用户的忠诚度
- 身高体型模型:根据用户购买服装鞋帽等用品判断
- 文艺青年模型:根据用户发言、评论等行为判断用户是否为文艺青年
- 用户价值模型:判断用户对于网站的价值，对于提高用户留存率非常有用（电商网站一般使用RFM 实现）

(3) 用户画像基本成型<br>
&nbsp; &nbsp; &nbsp; &nbsp;该阶段可以说是二阶段的一个深入，要把用户的基本属性（年龄、性别、地域）、购买能力、行为特征、兴趣爱好、心理特征、社交网络大致地标签化。为什么说是基本成型？因为用户画像永远也无法100％地描述一个人，只能做到不断地去逼近一个人，因此，用户画像既应根据变化的基础数据不断修正，又要根据已知数据来抽象出新的标签使用户画像越来越立体。关于“标签化”，一般采用多级标签、多级分类，比如第一级标签是基本信息（姓名、性别），第二级是消费习惯、用户行为；第一级分类有人口属性，人口属性又有基本信息、地理位置等二级分类，地理位置又分工作地址和家庭地址的三级分类。<br>	

#### 3. 用户画像的作用<br>
简而言之，用户画像为了让团队成员在产品设计的过程中能够抛开个人喜好，将焦点关注在目标用户的动机和行为上进行产品设计。具体包括:<br>

- 精准营销，分析产品潜在用户，针对特定群体利用短信邮件等方式进行营销
- 用户统计，比如中国大学购买书籍人数 TOP10，全国分城市奶爸指数；
- 数据挖掘，构建智能推荐系统，利用关联规则计算，喜欢红酒的人通常喜欢什么运动品牌，利用聚类算法分析，喜欢红酒的人年龄段分布情况；
- 进行效果评估，完善产品运营，提升服务质量，其实这也就相当于市场调研、用户调研，迅速下定位服务群体，提供高水平的服务；
- 对服务或产品进行私人定制，即个性化的服务某类群体甚至每一位用户（个人认为这是目前的发展趋势，未来的消费主流）。比如，某公司想推出一款面向5－10岁儿童的玩具，通过用户画像进行分析，发现形象＝“喜羊羊”、价格	区间＝“中等”的偏好比重最大，那么就给新产品提供类非常客观有效的决策依据。
- 业务经营分析以及竞争分析，影响企业发展战略

####4. 关键技术<br>
（1）打标签<br>
&nbsp; &nbsp; &nbsp; &nbsp; 用户标签是表达人的基本属性、行为倾向、兴趣偏好等某一个维度的数据标识，它是一种相关性很强的关键字，可以简洁的描述和分类人群。比如好人和坏人、90后80后，星座、白领等。具体流程一般是从纷乱复杂、琐碎的用户行为流（日志）中挖掘用户在一段时间内比较稳定的特征，即给用户打上标签，标签的确定，一般是先人工筛选小样本规则，进行验证标注，规则合理后，在通过算法扩展。最后是评估画像的好坏：小样本的真实验证；A/B Test； 在实际的case 中迭代验证，这点从技术角度而言会有些挑战，比如怎么保证准确率和覆盖率。

- 属性标签：比如自然属性标签里的性别、年龄、星座等，社会属性里的职业、社交、出生地、电话号码等。这块有一定的门槛，因为不再是基于事件行为的事实统计了，需要一定的挖掘算法做预测，咱们以性别为例：
性别属于个人隐私，不是每个用户都愿意填写，而且出于保护自己或者其它目的，填了也不一定是真实的，此时你想给用户打上性别标签，就需要用到机器学习相关的算法了，而且需要对准确性和覆盖率负责。
- 事实标签：比如购买行为、位置包括常驻地出差地等、使用设备、社交属性等，这类一般都可以直接从日志中直接提取，加以简单的聚类算法辅助即可。
- 营销标签：这块比较偏业务属性了，往往带有明确的业务目标建模而成的，比如LTV用户价值、活跃度、忠诚度、兴趣爱好、白领、高奢、有房一族、购买偏好等。
- 预测标签：比如之前提到的性别，其实在大部分场景下也属于一个预测标签，一般而言，我们需要一定的数据挖掘算法，集合用户日志提取APP特征、事件特征、浏览内容特征，对非结构化数据来说，通常要经历“分词”、“过滤”和“特征提取”三个步骤。

（2）用户画像验证<br>
&nbsp; &nbsp; &nbsp; &nbsp; 按事件的发展过程来看， 用户画像准确性验证分为事中和事后，其中事中指用户开发过程中，而事后则是指画像上线运用于业务后。不同阶段的验证方法也有所不同。<br>
&nbsp; &nbsp; &nbsp; &nbsp;**事中验证**主要基于画像开发过程中所选模型及统计方法，对于三类画像，有以下三种验证指标：<br>

- 模型验证指标：常用的模型指标验证主要用户前两类画像的验证，通用的为AUC、KS、ROC、Confusion Matrix等。对于基于聚类的用户画像没有较常用的验证指标。通常情况下，聚类效果图不能很好的说明问题，还需结合业务及每个群体用户覆盖度进行相应调整，最后的验证通常也是基于事后的业务反馈效果。
- 抽样验证：业务中用户画像通常涉及千万级甚至上亿级用户，不可能一一验证，这种情况下可以采取分层抽样验证或随机抽样验证。当然由于抽样验证的数据量相对较小，因此说服度不高。
- 交叉验证：通常情况下，一些画像类的指标间会存在一些相关性，此时可进行交叉验证。譬如收入与资产存在一定的相关性，通常收入越高资产也会越高，此时就可用这两个画像评分进行交叉验证。

&nbsp; &nbsp; &nbsp; &nbsp;**事后验证**主要基于随业务发展增加的数据源（真实数据）及应用于业务后的反馈数据。

- 真实数据验证：随着业务发展，一些用户画像信息会从无到有慢慢积累，毋庸置疑的是，将真实数据用于验证画像类指标是最准确的。
- A/B Test：A/B Test 是互联网公司最常用的验证方法，一般基于用户画像制定的策略在上线时都会进行严格的对比试验，以测试画像的准确性。
- 业务反馈数据验证：用户画像中的第二类（用户行为画像）和第三类（用户分群画像）与业务有紧密联系，源于业务也用于业务，因此由实际业务数据反馈来验证画像准确性是相对来说最有效的。验证方法主要看业务反馈排序与画像模型排序模型是否呈现单调性。

(3) 数据采集和整合<br>
&nbsp; &nbsp; &nbsp; &nbsp;**数据整合**。数据是构建用户画像的核心, 需要通过整合各类数据从而描述完整的用户图像。

- 用户数据，包括静态信息数据和动态信息数据。静态信息数据是指：用户相对稳定的信息，主要包括人口属性、商业属性等方面数据。这类信息，自成标签，如果企业有真实信息则无需过多建模预测，更多的是数据清洗的工作。动态信息数据是指：用户不断变化的行为信息，用户搜索了什么商品，浏览了哪个页面，赞了哪条微博消息，发布了积极或消极的评论……这些都是互联网上的用户行为，将成为用户画像中偏好特征和消费行为特征的主要依据。
- 商品数据，包括客观商品属性和主观商品定位。客观商品属性是指：商品的功能、颜色、能耗、价格等事实数据。主观商品定位是指：商品的风格、定位人群等。商品数据可以认为是商品的标签，需要和用户标签进行关联和匹配。
- 渠道数据，包括信息渠道和购买渠道。信息渠道是指：用户在信息渠道上获得资讯，如微信、微博等社交网络。购买渠道是指：用户在购买渠道上进行商品采购，例如商品官网、电商平台等。不同类型的用户对渠道有不同的偏好，精准的选择对应的渠道才能提高效率和收益。

(4)数据建模方法<br>
&nbsp; &nbsp; &nbsp; &nbsp;有了上述三类数据之后，需要根据用户行为构建相应的数据模型产出标签和权重。每一次的用户行为，可以详细描述为：什么用户，在什么时间，什么地点，发生了什么事。<br>
&nbsp; &nbsp; &nbsp; &nbsp;**什么用户**：即用户识别，其目的是为了区分用户。互联网主要的用户识别的方式包括Cookie，注册ID，微信微博，手机号等，获取方式由易到难，不同企业的客户信息数据化程度有所不同，用户识别的方式也可按需选取。<br>
&nbsp; &nbsp; &nbsp; &nbsp;**什么时间**：在用户行为中，普遍认为近期发生的行为将更反映用户当下的特征，因此过往行为将表现为在标签权重上的衰减。<br>
&nbsp; &nbsp; &nbsp; &nbsp;**什么地点**：即用户的接触点，包含了两个潜在信息：网址和内容。内容决定标签，网址决定权重。例如，一瓶矿泉水，超市卖1元，景区卖3元，酒店卖5元，商品的售卖价值，不在于成本，而在于售卖地点，这里的权重可以理解为用户对矿泉水的需求程度不同，相应的也有不同的支付意愿。类似的反映到互联网，用户在天猫浏览了iPhone6的信息和在苹果官网浏览也将存在权重的差异，因此，网址的内容反映了标签信息，网址本身则表征了标签的权重。<br>
&nbsp; &nbsp; &nbsp; &nbsp;**做了什么**：用户的行为类型，例如浏览、搜索、评论、点赞、收藏等，同样反映的是标签的权重。
&nbsp; &nbsp; &nbsp; &nbsp;从上述建模方法中，我们可以简单勾画出一个用户行为的标签权重公式：<br>
&nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;**标签权重=时间衰减（何时）×网址权重（何地）×行为权重（做什么）**<br>
&nbsp; &nbsp; &nbsp; &nbsp;举个直观的例子，“B用户今天在苹果官网购买了iPhone6”反映出的用户标签可能是“果粉1”；而“A用户三天前在天猫收藏了iPhone6”反映出的标签可能只是“果粉0.448”，这些不同用户的标签及相应的权重将在后续的营销决策中发挥指导作用。

#### 5. 案例和应用<br>
(1). 阿里云的[画像分析](https://data.aliyun.com/product/porana)服务<br>
&nbsp; &nbsp; &nbsp; &nbsp;画像分析将您分布在多个存储资源的数据整合起来，在标签模型上构建大数据画像类的交互式分析应用，让您的业务人员可以自由灵活的分析这些对象各种属性与行为之间的关联性。可以广泛应用于用户行为、设备管理、企业档案、地理分布等多种画像分析等多个场景当中。<br>
(2). 百度的[百度移动统计](https://mtj.baidu.com/web/demo/visit/attribute?appId=468475)<br>
&nbsp; &nbsp; &nbsp; &nbsp;百度移动统计是一款专业免费的移动应用统计分析工具，支持android，ios平台。<br>
(3). 美团[基于用户画像的广告粗排](https://tech.meituan.com/targeting_agentscore.html)<br>
&nbsp; &nbsp; &nbsp; &nbsp;用户兴趣对于广告转化有着显著影响。在用户画像基础上，向不同兴趣的用户推荐不同类型的广告，对广告的点击和转化皆能带来较大提升。

#### 6. refs<br>
&nbsp; &nbsp; [1]. [用户画像从入门到挖坑](https://juejin.im/entry/593f606ea0bb9f006b64e918)<br>
&nbsp; &nbsp; [2]. [用户画像如何验证准确性？](https://www.zhihu.com/question/36422121)<br>
&nbsp; &nbsp; [3]. [如何用数据挖掘的方法做比较准确的用户画像？](https://www.zhihu.com/question/23037437)<br>
&nbsp; &nbsp; [4]. [wiki:Persona (user experience)](https://en.wikipedia.org/wiki/Persona_(user_experience))<br>
&nbsp; &nbsp; [5]. [什么是用户画像呢？一般用户画像的作用是什么？](https://www.zhihu.com/question/19853605)<br>
&nbsp; &nbsp; [6]. [用户画像系统实践](http://7xnz4l.com1.z0.glb.clouddn.com/Arch043.pdf)<br>
&nbsp; &nbsp; [7]. [永洪BI:手把手教您搞定用户画像](http://news.yesky.com/prnews/280/85552280.shtml)<br>
&nbsp; &nbsp; [8]. [Creating Personas](http://www.uxbooth.com/articles/creating-personas/)<br>
&nbsp; &nbsp; [9]. [Personas](https://www.usability.gov/how-to-and-tools/methods/personas.html)<br>


			
