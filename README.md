<p align="center">
  <img width="200" height="200" src="./luckydog_logo.png">
</p>

<div align="center">
	<h1>LuckyDog</h1>
	<h2>锦鲤</h2>
	<h3>Just For Fun</h3>
</div>


## 游戏规则

1. 3 个 EOS 参与一次游戏
（如果你在我开发的界面来操作的话，那应该只会扣除你 3 个EOS，你也可以通过命令行的方式来参与，但是如果你一不小心，比如说你使用了 4 个 EOS 的话，那可不会退还哦，在链上数据只会记录3个）。
2. 10 个为一轮
这个 10 个是怎么解释的呢？  你可以用一个账户分 10 次来参与，这样也算满一轮，按照 10 次参与为一轮。

3. 3 个踩雷
在每一轮游戏中，都会有 3 个账户的 EOS 清零，这 9 个 EOS 会相应的分给系统账户和中奖账户（luckydog），关于系统账户的分配，请看下面的解释。这3个踩雷的账户将会获得不算少的代币（虽然现在不值钱，但是万一我的开发欲望暴涨的话，那么你就可以用他来参与我之后开发的游戏，关于代币的说明，请看下面）。

4. 6个 EOS 会平均分配给获奖的6个账户，这6个获奖账户看似公平，其实分配的时候并不公平，因为会随机的抽出踩雷的3位用户，那么就还有7位用户可以有幸获奖，但是这7位用户获奖是按照你参与的顺序来排出前6位获得EOS的。所以。。。

5. 1个轮空，没有踩雷的第7位用户不会扣除你参与的 EOS， 但是你也不会获得 EOS 奖励， 但是呢？为了每个人都会获得 "参与奖"， 第七位用户将会获得一些代币分配。

<b>我开发了这个游戏，但是所有的代码都会开源，可能我都没有足够的 EOS 来将它部署在 EOS 主网上，所以我会将奖励分配方案都写成变量的形式，如果你有足够的资金去将它放在主网上，我这里有个小小的愿望是希望能将开发奖励帐号设置成我的 "zhangzhichao"， 不设置也没有关系，你可以随意修改变量来控制奖励分配方案，如果你修改完需要帮助，比如说你不会编译～， 可以联系我（邮箱：zhichaozhang3@gmail.com, 微信：zzc960316），我会提供帮助。 </b>

## 3个EOS奖励分配方案
这3个 EOS 会分给在游戏部署过程，宣传过程提供帮助的人。分别是：


1. Security company（安全公司） 0.2000 EOS

我的想法是请安全公司做个代码验证，但是我没有足够的资金一次性付费，所以我才用持续奖励的方法，我个人感觉，如果比较好玩的话，这个持续奖励收益也还算可观。

2. development team (开发团队) 0.8000 EOS

团队奖励只设置一个帐号是因为链上转账太贵了，所以如果团队开发的话可以链下来分配。（这么设置也有可能目前是我一个人在开发，所以～）

3. nodeprovider (full node 节点提供者) 0.1000 EOS

因为在前端界面中可能会通过数据同步的方式来展示一些信息，这样就需要通过full node来获取这些数据，所以～

4. resourceprovider (CPU,NET,RAM 提供者) 0.9000 EOS

这个是我的设置，但是在实际部署的过程中可能这点消耗都不够资源提供者的本金，所以如果你来部署的话，你可以调整一下。

5. serverprovider (服务器提供者) 0.4000 EOS

这部分的奖励是为了奖励给提供服务器的，对我买不起好点儿的服务器～～， 如果你自己提供服务器的话，你可以将这部分奖励奖励到你自己的账户即可。

6. spreadsource (宣传奖励)  0.6000 EOS 

这个是分给本游戏宣传的账户，暂时会放在程序部署者的一个账户中，然后链下统计分给宣传的账户，我在代码中目前只会一级奖励，之后时间充裕的话可能会做成三级乃至多级的。这部分放在链下是因为转账太贵了～～～， 但是在我的代码中我的前端界面应该会提供一个宣传账户填写，然后会将他记录在链上，保证不能耍赖。


## 合约中发币合约的用处

1. 开发基金
    这个合约的发币功能是用来为之后的dapp的开发提供 token.
    1. 为什么要有这个 token 呢？
    
    通过 token 来补偿在游戏中失败的账户，获得这些 token 的账户可以在我之后开发的 dapp 中，如果我的开发资金允许的情况下，可以充当代币的作用，比如说在下个游戏中如果你其他玩家需要拿 EOS 来玩这个游戏，但是如果你的账户中有这个合约中获得 token 的话，你可以通过一定的比例来代替 EOS 的消耗。
    
    2. 怎么获得本合约发行的相关代币。
    
    本合约的代币是有我个人发行，因此，本代币只有通过玩这个游戏来获得，除此之外不会再有获得这个代币的渠道（如果你愿意放到交易所去卖，那可能会有其他渠道来或得，但是我感觉应该没有人会买吧～）。
    
    3. 这个合约将要发行的代币的种类。
    
    在这个合约中我个人会承诺只发行一种代币，并且只有这种代币来在其他我开发的 dapp 中能以相应的比例来抵消 EOS 的消耗。
    
    
## 开发计划 (业余时间完成，因此只会有计划，但是不会有具体的截止时间)
1. 发币功能迁移（完成）。
2. 合约逻辑（WIP）。
3. 前端界面编写（WIP）。
4. scatter、tp、麦子钱包这些合约调用过程中的钱包协议兼容（WIP）。

## 部署
等开发完成或者第一版完成，完善～～

## 如何贡献
1. 暂时只有我自己在开发，所以如果你也对这个小游戏感兴趣，只要遵循github工作流来一起完成即可。然后如果你能坚持，我会在开发团队中私下给你分发奖励，我不会使用你的那部分为之后的dapp，用户持有代币来兑换，这部分我之后使用我分的那部分，也就是说如果有幸这个游戏有一定的可玩性，你会获得一部分EOS的奖励，同时也有可能锻炼你的智能合约开发经验（大佬请忽略这句话～）。
2. 如果你不会写代码，没关系，你也可以帮忙将中文翻译一下。（也可能会有一些奖励哦）
3. 如果你发现有BUG，欢迎来提交。（也会有一些奖励哦）

## 关于文档
之后一些详细的实现文档会放到wiki中，如果你不部署这个游戏，你也可以从文档中获得一些启发吧（起码是我开发这个游戏的记录）。
文档会随着开发慢慢加到wiki中。


------
Icon made by Freepik from www.flaticon.com, special thanks~