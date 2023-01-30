
# 区块链诞生与比特币

## 区块链诞生之前
我们通常把比特币的发明看成是区块链诞生的标志性事件。但区块链就像很多技术一样，并不是凭空出现，通常都会有一些渊源。
1991年，比特币发明出来的17年前，斯图尔特·哈伯（Stuart Haber）和W.斯科特·斯托内塔（W. Scott Stornetta）就提出了区块链的前身。他们创造性地把一系列区块链接起来，最终保证了电子文档的时间戳不可篡改。一年之后，他们升级了这套系统，往其中加入默克尔（Merkle）树。得益于此，系统的效率大大提升，可以在一个区块中放入一组文档。
链接在一起的区块、防篡改特性、默克尔（Merkle）树，这些最终都成为区块链技术的重要组成部分。

## 区块链的诞生标志 —— 比特币

2008年10月31日，一名叫中本聪（Satoshi Nakamoto）的用户在密码学的邮件组中发了一个链接，链接指向一篇叫作《比特币：点对点的电子现金系统》（Bitcoin: A Peer-to-Peer Electronic Cash System）的论文，标志着比特币的诞生。

![点对点的电子现金系统](https://img.learnblockchain.cn/pics/20230130141821.png)


论文中详细介绍了如何使用点对点技术创建一种电子货币（数字货币）。

2009年1月3日，中本聪挖出了比特币的创世区块，标志着比特币网络正式上线。中本聪在挖出创世区块的过程中获得了50个比特币的矿工奖励，同时他在创世区块中留下了这句话：
The Times 03/Jan/2009 Chancellor on brink of second bailout for banks.（2009年1月3日，财政大臣正处于实施第二轮银行紧急援助的边缘）
这句话是英国《泰晤士报》当天的头版文章标题。通过对头版头条的引用证明了比特币的实际上线时间。



<details>
  <summary>早期数字货币探索</summary>
  <div>
    1983年，戴维·查姆（David Chaum）和史蒂芬·布兰德斯（Stefan Brands）开发了ecash协议，基于ecash协议，不少人发明了多种电子现金系统。
    <br/>
    1997年，亚当·巴克（Adam Back）开发了hashcash协议，主要是为了解决垃圾邮件泛滥的问题，其中用到的技术就是后来被比特币使用的工作量证明算法（proof-of-work）。
    <br/>
    1998年，戴伟（Wei Dai）发明了b-money，尼克·萨博（Nick Szabo）发明了bit gold。两者被认为是最早的分布式加密货币。
    <br/>
    这一切可以被认为是比特币的前身，它们都或多或少地影响了比特币的设计。
    <br/>
    2008年8月18日, bitcoin.org 域名注册, 2008年10月31日，密码学（cryptography）邮件列表中收到了一个叫中本聪的人发表论文《比特币：点对点的电子现金系统》。
  </div>
</details>



<details>
  <summary>比特币历史事件</summary>
    <div>2009年1月9日，知名代码托管网站SourceForge上发布了第一个开源版本的比特币客户端。
    <br/>
    2009年1月9日，作为比特币的早期支持者和贡献者的程序员哈尔·芬尼（Hal Finney）下载了比特币客户端，2009年1月12日，哈尔·芬尼（Hal Finney）收到了中本聪的 10 枚比特币的转账，这是比特币历史上的第一次转账。
    <br/>
    2010年5月22日，程序员拉斯洛·汉耶兹（Laszlo Hanyecz）用10000枚比特币购买了Papa John‘s的两份披萨。这是有记录的第一次在现实中发生的比特币交易行为。
    <br/>
    2012年9月，比特币基金会成立，旨在通过开源的协议来加速比特币在全球范围内的增长。
    <br/>
    2013年10月29日，加拿大公司发布第一个比特币 ATM，允许用户在咖啡馆里直接购买和出售比特币。
    <br/>
    2017年8月1日，比特币发生共识分裂，分叉出 Bitcoin Cash (BCH) 链。
    <br/>
    2017年11月28日，比特币价格首次突破1万美元。
    <br/>
    2021年11月10日，比特币创下历史最高价达68928.9美元
  </div>
</details>
 
## 比特币如何运作

比特币是一种基于分布式网络的数字货币，与传统的货币不同，比特币不是在任何政府的支持下发行的货币，也不依赖银行来记录相应的账本。
在比特币的点对点分布式网络中，定义了发行货币的一套规则及每个个体（节点）如何独立验证交易有效性，所有的交易形成了一个公共的账本。

### 共识

在分布式系统中，如何多台计算机如何同时运行同一个任务，一直是一个“难题”，在比特币系统中，需要如何保持各个节点的账本数据（通常称为“状态”）一致呢。
这就需要各节点达成一个“共识”，所有节点按统一的规则行事。

比特币网络中的所有节点都会接收到一组交易记录（记录作为一个区块保存），然后把这个区块更新到本地的账本记录中。如果节点都随意增加记录，那么整个比特币网络中的记录就无法保持一致。为了保持记录一致，那么必须确认哪个区块被优先写入，也就是需要以某一个节点的操作为准。但如果人为规定以某个节点为准，就意味着这个节点比其他节点更权威，相当于变成了一个中心节点，那么去中心化的优势就荡然无存。

比特币使用的共识算法叫做PoW共识机制，全称是Proof of Work（“工作量证明”），率先完成工作量证明的节点，拥有区块写入权，其他的节点以此区块的基础上进行后续交易记录的工作量证明。

工作量证明中最重要的是计算一个数学难题，解此难题唯一的方式是不断的尝试，直到试出“答案”，率先完成解答的节点可以获取一笔奖励，最初奖励是每个区块50个比特币，之后每大约4年减半，当前为每区块 6.25 比特币。由于完成工作量证明有一定的随机性，通常这个过程也称为“挖矿”。


<details>
  <summary>比特币发行量小知识</summary>
    <div>比特币发行量都来自于比特币的出块奖励，按共识规则初始出块奖励是 50 比特币，之后每隔21万个区块奖励减半，每个区块的生成时间大概是10分钟，因此大致是4年减半一次，大约到 2140 年，比特币的出块奖励就趋于零，此时产出的所有比特币数量将非常接近 2100 万枚。
  </div>
</details>


## 如何持有比特币

### 所有权问题

### 地址 及 UTXO 



## 比特币特点

从比特币的特点上来看，比特币是去中心化的，主要特点如下：

比特币不需要任何权威机构的背书。
比特币是点对点网络，没有中心化的服务器存在。
比特币的账本数据存储在区块链中，而区块链本身存储在千千万万的节点中，没有一个中心化的存储设备。
比特币账本数据面向所有人公开，任何人都可以把它存储到自己的机器中。
比特币网络没有管理员，比特币网络中的所有节点共同管理比特币网络，维持比特币网络的运行。
任何人都可以成为比特币网络的一个节点，从而具备和别人同等的管理权。
比特币网络中任何节点都是同等地位，它们都可能获得下一个区块的记账权。
由于比特币可能由任意节点凭空产生，所以比特币的供应也是去中心化的。
和传统银行不同，任何人都可以生成任意数量的比特币账户，不需要任何中心化机构的审批。
任何人都可以在比特币网络中发起转账，不需要任何中心化机构的审批。

但是，在现实中，比特币也有一些中心化的倾向，由于奖励机制是凭空生成的比特币，所以比特币网络中的节点争夺记账权的欲望通常比较强大，结果造成了大量的节点联合起来，共同去争夺记账权。当联盟中的任意节点获得记账权，就会把得到的比特币和联盟中的其他节点分享。因此，这种联盟造成了比特币网络节点某种程度上的中心化。这种联盟就是我们经常听说的比特币矿场。


