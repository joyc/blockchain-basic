# 什么是区块链

### 比特币与区块链的分离
比特币诞生的几年后，人们开始意识到区块链本身的潜力，于是形成一股力量，开始把区块链从比特币中分离出来。最终区块链被定义为一种去中心化的分布式账本技术，主要用来记录交易信息，其交易记录具备不可篡改性，并且不需要额外的第三方机构来证明记录的正确性。所以，在很多交易场合，区块链都有着巨大的前景。
需要注意的是，这里所说的交易可以理解为一种广义的交易，并不仅仅是简单的货币交换。正是这种认识，整个业界都对区块链报以极大的热情，大量的投资和研发工作因此展开。在健康、保险、供应链、投票等领域都开始出现区块链的身影。到2017年，全世界有15%的银行都开始或多或少地使用区块链。


### 智能合约
2013 年，一名叫维塔利克·布特林（Vitalik Buterin）的年轻人发明了以太坊，并在其中创造性地发明了智能合约，智能合约可以被认为是比特币之后的又一重大发明。
在以太坊被发明出来前，区块链上可进行交易的一般都是像比特币这样的加密货币，然后在交易的附言阶段附带上一些信息。而以太坊扩大了交易的边界，它让交易发生的同时可以执行一段代码。这也就意味着交易本身具备了逻辑，毕竟现实中的很多交易都会伴随着逻辑，比如有的交易要分期付款，或者多方参与的借贷。像保险合同的执行也是有事前约定的条件，这些合约条件都没办法单纯地依靠比特币这样的转账记录来达成。而当交易可以附带一份代码的时候，情况就完全不同了，我们可以通过代码来写出这些合约的执行条件，在条件满足的时候才执行真正的加密货币转账。甚至，交易可以完全不产生货币转账，而是用代码来描述一份数字资产。总之，当区块链中可以存储代码，它的想象空间就是无限的。
智能合约是区块链的又一里程碑事件，在智能合约发明出来之后，区块链已经完全从比特币中分离出来。时至今日，智能合约之后发明出来的新技术，像闪电网络、侧链这些都是根据具体应用场景所作出的一些优化。
在未来可能发生更大的变化之前，区块链的主要历史就到此结束。分布式、防篡改、交易、智能合约成为现今所有区块链的基础特点。


##  什么是区块链
区块链最常见的定义是：去中心化、分布式、公开的数字账本，主要用于记录交易信息。与传统方案不同的是，区块链的交易记录存储在很多不同的计算机上。而任意一个参与记录的计算机都很难修改交易记录，如果想要修改某一条交易信息，那就需要修改之后的所有交易信息。正所谓“牵一发而动全身”，任何微小的修改都会扩散到区块链的所有后续记录上，而这在实际操作中几乎不可能实现。这样的结果就是，所有参与的计算机都可以独立地验证交易或者发起交易，同时这样做的成本还很低。因此，区块链不需要任何独立机构单独维护，却具备不可篡改的特性。正是这种特性，让区块链具备了巨大的潜力。
我们通常把区块链存储交易记录的部分称为“区块链数据库”。区块链数据库和传统数据库也有着巨大的差别，它是存储于点对点的分布式网络之中，和 BT下载等分布式下载技术有相似之处。这也意味着没有任何一家机构拥有区块链数据库，相反，是参与到网络中的所有计算机共同拥有数据。
区块链中存储的信息非常简单，主要就是表示从一个地址到另一个地址的转账信息。而转账的内容被标注为不可重复，这也就意味着，和传统银行账户一样，当你发起转账之后，转账物的拥有权就发生了永久性的转移。但由于区块链本质上是一堆二进制数据，所以转账的数据并不局限在金钱的范畴。比如你完全可以把对某个网站的操作权限进行转移，当转移过后，操作权限就和新的交易地址唯一绑定，而旧的交易地址也就失去了权限。从这个角度出发，我们可以认为区块链其实是一个价值交换网络。任何有价值的东西都可以通过区块链来完成拥有权的转移。

## 代币（token）是什么
需要注意的是，由于区块链记录的是转账信息，自然就会出现一个转账物的概念。如果任意定义这个转账物，那么区块链和传统的存储技术也就没什么太大的区别。因此，大部分区块链都会定义一个通用的转账物，而其他的数字资产可以通过某种规则映射到这个通用转账物上。随着时间的推移，大家就开始使用代币（token）来表示这个通用转账物。
代币是区块链里的一个关键概念，但是考虑到一些特殊的情况，也有可能出现无币区块链。所以代币并不是区块链的必要属性。

## 什么是区块
区块是区块链中的数据存储单元。每一个区块中存储了一组交易信息以及这些交易信息的哈希数据。这些交易信息的哈希数据编码为默克尔树（Merkle哈希树）存储。
每一个区块还会存储前一个区块的哈希信息，因此区块就能够通过哈希信息链接起来，形成区块链。通过前一个区块的哈希信息去定位，我们就可以不断地往前追溯，直到找到创世区块（区块链启动的时候产生的第一个区块）。由于对区块中交易数据的微小修改都会导致区块自己的哈希信息改变，所以如果篡改了任何一笔记录，就意味着此区块的内容发生了改变，那么此区块的哈希信息也就改变了。由于下一个区块的内容会保存当前区块的哈希信息，那就是说篡改者需要同时修改下一个区块的内容，这同样会导致再下一个区块的哈希信息改变，依此类推，篡改者需要修改后续的所有区块。

### 区块是怎么产生的
每个区块由参与其中的计算机节点独立生成。由于是分布式网络，所以就会有不同的区块在同一时间被生产出来。区块链数据库中的区块通过哈希信息相连构成了一条基于哈希信息的历史链。不同的区块在同一时间产生，系统中就出现了多条历史链。区块链会提供一套算法来对每一条历史链进行打分，以此来留下分数更高的链，同时淘汰分数低的链。
随着时间的推移，区块链的每一个独立节点都在生产自己的区块，同时接收其他节点传递过来的区块。所以节点本地总是会有多条历史链。这时候，节点就需要在本地生产的区块和接收到的区块中进行选择，如果接收到的区块构成的历史链优于自己本地的，那么就会销毁自己刚刚生成的区块，然后以更优的历史链为基础，再生成新的区块并广播给网络中其他的节点。
由于区块生成一直在各个节点中不停地发生，所以从任何一个节点上得到的历史链都无法保证是最优的。但是由于区块链总是把新的区块不停地加到旧的历史链上，每一次添加都会增加这条链的分数。这也就意味着，随着时间的推移，某一个区块后边总是会跟上很多新的区块，当它被广播出去之后，该区块也更可能被更多的机器所识别，并以此为基础构建本地的新链，所以虽然这个区块后边跟随的新区块在不同的历史链上可能不一样，但是就这个区块来说，这个区块被所有节点都认为是有效的可能性会越来越高。到一定的程度之后，我们就可以认为这是一个不可修改的区块。这也是我们经常听到当区块达到一定高度，我们就信任这笔交易的原因。
### 区块生成时间
区块生成时间是指区块链系统中生成一个新的区块所需的平均时间。当一个区块生成时间走完，最新的区块进入可验证的状态。区块生成时间越短，交易完成的速度也会越快。但是由于区块的生成涉及数据打包以及处理软分叉的打分系统，这都需要一定的时间开销。而不同的打分系统会有不同的时间开销，同时如果对安全性、稳定性各方面的要求越高，那么生成一个区块的时间自然也会越慢。所以区块生成时间在不同的区块链中的差别会非常大。比如以太坊的区块生成时间在 14 到 15 秒之间，而比特币是 10 分钟。

## 区块链的硬分叉
区块链就和传统的程序一样，随着时间的推移，软件的设计本身也会发生改变，甚至是在软件中出现严重的漏洞，如果在传统软件中就会产生升级的操作。而升级后是否向下兼容就会对整个软件造成完全不同的影响。区块链也是一样，区块的数据格式、生成区块的算法以及对区块链进行打分的算法都可能会升级。如果这种升级向下不兼容，就会出现两套算法在同时运行的情况。运行旧软件的计算机节点会继续用旧的协议来继续构建区块，而运行新软件的节点就会用新的协议去构建新的区块。通常升级会从某一个固定的区块开始，所以从这个固定的区块开始，就会分叉出两条完全不同的链。两者再也没有互相融合的可能。这就是区块链的硬分叉。
和传统软件升级不一样的是，硬分叉的代价很大，因为节点是否升级所牵扯的面很广，其中除了技术的原因，还有很多利益纠葛，比如有的节点的硬件就是专门为旧的协议设计，无法很好地适配新的协议，那么这些节点升级新协议的可能性就很小，甚至这种升级根本就不可能实现。更进一步，不同的人对区块链的想法不一样，不同的工作组有可能给出完全不同的升级协议，而这些协议都可能被一定数量的节点所接受，结果就是同一个区块链随着时间的推移，可能会发生很多次硬分叉。例如，比特币就被分叉过很多次，在交易市场上，很多和比特币的名字很类似的币，其实就是硬分叉导致的。以太坊也在某一次DAO黑客事件后进行回滚，有的节点不接受这次回滚，结果就是分叉出以太坊和经典以太坊两条链。
要解决硬分叉问题，在技术上并没有什么好的办法。不过随着时间的推移，不同的链在进行公平的竞争，最终总会有一些更好的被留下来，其他一些则被慢慢淘汰。所以，硬分叉到底是不是一个严重的问题，更多的就要看观察角度了。

## 区块链的去中心化

区块链数据库本质上存储在区块链所有的计算机节点上，这是一种经典的点对点网络系统，也就是去中心化的由来。通过去中心化，区块链避免了很多中心化系统的风险。
传统的中心化系统中，如果由于人为的攻击或者其他不可抗力的原因，导致服务器发生了故障，那么整个系统也就彻底瘫痪。在去中心化的区块链系统中，我们可以认为每一个节点都是一个功能完备的系统，除非整个区块链网络中的大部分节点都发生故障，不然区块链始终能正常运行，从这个角度看，去中心化的区块链系统很好地避免了单点故障。
由于每一个区块链节点都存储有一份区块链数据的备份，没有一个所谓权威的数据备份，这也就意味着从数据的角度来看，每一个节点的地位都是对等的，大家不用特别信任某一个节点。每个节点做的事情都一样，接受别的节点的数据，比较本地数据，生成新的数据，然后广播出去。区块链的各种算法会协调这些步骤，最终不断地记录合法的数据，如果系统中有恶意节点，随着时间的推移，由于它们的数据在评分系统中会越来越低，所以它们产生的恶意数据会自动被清除出去。
但是现实通常会更微妙，随着区块链系统的发展，很可能会伴随着去中心化的削弱。因为区块链系统的运行需要一定的计算资源，而这个资源有可能会越来越大，以至于普通的节点无法负担，那么大型资源节点最终就会占据越来越大的优势，最终区块链系统可能会被有限的大型资源节点接管。在比特币的发展中，我们就能看到大型矿池的出现。


## 智能合约（smart contract）
###  什么是智能合约
智能合约是一种电子化的合约，表现为计算机协议的形式。从功能上看，智能合约可以在没有第三方干预的情况下执行合约，并可以随时追踪合约的执行情况。此外，合约本身可以做到绝对无法撤销。智能合约的目标是提供比传统合约更好的安全性。另一方面，在传统的合约执行过程中，需要律师、法院等各种各样的第三方介入，本身的成本非常高。而智能合约着眼于自动执行，以此来减少执行合约的成本。
随着大部分的加密货币都实现了智能合约，现在智能合约的主流实现方式都是基于区块链技术。所以很多时候我们说智能合约，都是特指通过区块链实现的智能合约。
需要注意的是，虽然智能合约中的“合约”二字取材自现实中的合约，但并不是说所有的智能合约必须与现实中存在的合约一一对应。由于智能合约本质上是一组计算机协议，所以智能合约完全可以实现一种现实世界中不存在的协议。

### 智能合约的实现方式
通过区块链实现的智能合约中，智能合约的去中心化属性通过区块链中的分布式一致性算法来保证。分布式一致性算法就成为了智能合约的主要组成部分。除此之外，为了描述智能合约，就需要一种特定的描述语言来支持，这种描述语言一般就是一种特别设计的编程语言。
比特币提供了一种图灵不完备的脚本语言。通过这种脚本语言可以实现有限的智能合约，主要包括支持多重签名的账户、第三方托管服务、跨链交易等。主流语境中人们通常不认为比特币实现了智能合约，但是从这门脚本语言的成果来看，我们可以认为比特币支持了一定程度上的智能合约。
智能合约最有名的实现成果应该是以太坊。以太坊提供了一门几乎图灵完备的编程语言。结果就是理论上开发者可以在以太坊的智能合约上编写任意复杂的逻辑，甚至可以实现自己能想到的任何程序。得益于此，以太坊上出现了形形色色的应用，甚至因此出现DApp这种新的程序类别。