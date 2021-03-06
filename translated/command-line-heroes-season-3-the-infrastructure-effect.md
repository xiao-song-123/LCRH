  [#]: collector: (bestony)
  [#]: translator: (messon007)
  [#]: reviewer: ( )
  [#]: publisher: ( )
  [#]: url: ( )
  [#]: subject: (Command Line Heroes Season 3: The Infrastructure Effect)
  [#]: via: (https://www.redhat.com/en/command-line-heroes/season-3/the-infrastructure-effect)
  [#]: author: (RedHat https://www.redhat.com/en/command-line-heroes)

  命令行英雄第三季: 基础设施的影响
  ======
  **00:00** - _Saron Yitbarek_

  1904年，纽约市地铁首次开始运营时，它被惊叹为现代的一个奇迹。但是……当今天的通勤者仍依赖一个多世纪前设计的基础设施时，会发生什么？ 火车挤满了人，而且常常晚点。 纽约每年有20亿人次地铁出行，再也没有人感到惊叹了。 我们还在依赖昨日过时的基础设施，我们必须找到新的聪明的方法来使用它。

  **00:44** - _Saron Yitbarek_

  基础设施项目通常是些可见的大而具体的事物，例如地铁。 而且由于这种物理可见性，它们损坏时也显而易见。 高速公路开裂，电线杆跌落。 我们很清楚这些东西何时需要维修。 为了使我们的生活与老化的基础设施保持协调，大量的工作是必不可少的。

  **01:12** - _Saron Yitbarek_

  但是事情并不总是那么明显。 如今，我们还拥有 IT 基础设施，在偏僻地区嗡嗡作响的服务器农场，跨越海洋的光纤电缆以及软件基础设施。 老的操作系统或没人敢替换的 shell 脚本。 当所有这些IT基础设施变得陈旧和破旧时，我们是无法看出的。 但是，造就了今日发展的基础设施却正在老化，就像旧的地铁轨道一样。 这可能会扰乱我们的现代生活。 如今命令行英雄们正努力确保我们不会被过去束缚，因此出现了大量新的挑战。

  **02:02** - _Saron Yitbarek_

  这是我们编程语言世界探索季的第5集。 我们正在研究2种(编程)语言，它们与最初设计的目标基础设施密切相关。 COBOL 是大型机的原生语言，而 Go 是云计算的原生语言。他们都深受其起源的影响。了解这一点可能会拯救将来的开发者，避免他们像挤在宾州车站的《纽约客》那样走到最后。

  **02:33** - _Saron Yitbarek_

  我是 Saron Yitbarek， 这里是 Red Hat 的原创播客，命令行英雄的第3季。

  **02:43** - _Grace Hopper_

  我们面前有很多事情需要去做，但是我们首先需要大量相关的且易于访问的信息。 我们才刚刚开始。

  **02:53** - _Saron Yitbarek_

  海军上将 Grace Hopper 在1940年代和50年代率先开发了高级编程语言。 当时的基础设施大型计算机使得她能够取得巨大的飞跃。

  **03:08** - _Chris Short_

  嗨，我叫 Chris Short. 

  **03:10** - _Saron Yitbarek_

  Chris是红帽 （Red Hat） 的首席产品营销经理，而且他也是一位历史爱好者。

  **03:17** - _Chris Short_

  40年代的 Hopper 上将创造了 FLOW-MATIC， 在当时是革命性的，她被广泛认为是 COBOL 的祖母。 因此，她能够坐在那里说：“嘿，只需将其放在大型机上”，或“嘿，只需将其存储在大型机上”即可。

  **03:31** - _Saron Yitbarek_

  这是一个重大的游戏改变者。 突然，您有了这种机器无关的语言，即 COBOL， 它是大型机环境特有的。 可能性开始逐步打开。

  **03:42** - _Chris Short_

  大型机和 COBOL 真正使得每个组织能够说它们不再需要充满了带着铅笔，纸，计算器和滑尺的人的办公室，他们可能只需要半个办公室来安装大型机。 然后，他们可以雇人用 COBOL 来编写一些应用程序来完成整个财务团队做的所有的数学，逻辑运算以及账目分类。 因此，您需要的财务团队人数少了，仅仅是因为更多的输入可以被数字化，而不是全手动操作。

  **04:17** - _Saron Yitbarek_

  如果你是新的 COBOL 程序员之一，那感觉你将有一份终生的工作。 因为您的工作所基于的基础设施(所有那些大型机)，始终会在那里。

  **04:30** - _Chris Short_

  那时侯摩尔定律还未到来，所以您可能可以整整十年都在同一个大型机上工作，对吧？就像您不必担心下一个操作系统，或者下一个类型的容器编排器，又或者下一个随之而来的东西以及 AI 一样。 您可能会整个职业生涯都在从事 COBOL。 而且您知道自己将会非常稳定。

  **04:55** - _Saron Yitbarek_

  但是，摩尔定律最终到来了。 新的基础设施也出现了。 现如今，程序员不太可能去学习一种半个世纪前的旧语言。 但实际上，那些旧的大型机并没有消失。 这意味着我们对 COBOL 开发人员的需求也没有消失。

  **05:17** - _Chris Short_

  寻找 COBOL 开发者变得越来越困难。 最终会发生的事情是这些大型机可能已经存在了50年。 这些仍然可以编写出色 COBOL 程序的 COBOL 开发人员将获得巨额收入，以帮助项目运行并完成大型机中的数据重组。 而且，该技能肯定会绝迹，并且正在成为一个利润丰厚的职业领域，如果您(您知道的)……您现在绝对可以靠写 COBOL 赚很多钱。

  **05:49** - _Saron Yitbarek_

  尤其是在制造业和金融业。 您无法超越几十年前建立的所有基础设施。 老代码遍及全球。 忽略旧的基础设施及其相关的语言，将是一个巨大的错误。

  **06:08** - _Chris Short_

  由于存在2000亿行代码，因此很难重构所有这些代码。 不，我认为在有生之年我们肯定不会看到它消失。

  **06:21** - _Saron Yitbarek_

  Chris Short 是 Red Hat 的首席产品营销经理。

  **06:28** - _Saron Yitbarek_

  我想花一秒钟解释一下 Chris 的观点。 想象一下， COBOL 已经纳入了95％的 ATM 交易中。 那就是我们与这种语言的紧密联系。 但是， COBOL 程序员的平均年龄并不比该语言年轻。 他们45岁，或者55岁。 新人并不感兴趣。 这就是为什么我想向您介绍某人。

  **06:56** - _Ritika Trikha_

  嘿，我是 Ritika Trikha。

  **06:59** - _Saron Yitbarek_

  Ritika 是一名技术编辑，曾在 HackerRank 工作。 她对这个 COBOL 问题，以及人们对它是后大型机时代无意义的残留品的假设着迷。

  **07:12** - _Ritika Trikha_

  如今的开发人员根本没有考虑过 COBOL，见也没见过，想也没想过。

  **07:17** - _Saron Yitbarek_

  但这可能是灾难的根源。

  **07:21** - _Ritika Trikha_

  如今，仍然有大量的 COBOL 代码在为驱动企业的业务。 每年至少新增15亿行新 COBOL 代码。 我认为当您查看特定行业时，非常有趣。 就像美国国税局有5000万行代码。 社会保障局有6000万行代码。 因此，这些单位和实体正在处理一些如今最敏感，重要的信息，如果我们不继续为大型机提供支持和维护，那么它可能真的会被破坏。

  **08:04** - _Saron Yitbarek_

  因此，如果我们无法摆脱旧的基础设施，又无法挥舞魔杖来重建整个大型机业务，我们该怎么办？ 有时仅仅考虑未来的编码人员该如何开始适应过去？ 我们首先需要直面该问题。

  **08:25** - _Ritika Trikha_

  您知道，年轻一代将不得不重拾这些技能。 或者，必须对这些大型机进行某种现代化。 无论哪种方式，这个问题都不会消失。 这就是为什么 COBOL 还活着。

  **08:35** - _Saron Yitbarek_

  这并不容易。 Ritika 认为我们已经忽略这个问题太长时间了。

  **08:42** - _Ritika Trikha_

  这非常昂贵，艰巨，并且替换数十亿行 COBOL 代码的风险也非常高。 它是关键任务代码，像社会保障和财务信息。 COBOL 是专门为此类大交易量而设计的。 因此，它由 Grace Hopper 在60年代为商业交易而设计。 自60年代以来，一直存在“如果没有损坏，为什么要修复它”的说法，现在我们处于这样一个关头，即延续了数十年的大量的高价值数据运行在 COBOL 上。

  **09:22** - _Saron Yitbarek_

  从某种意义上说， Ritika 呼吁文化转变。内在和外在的态度发生变化。 由于发展的世界开始获得越来越久的历史，我们必须更加与自己的历史保持联系。 您无法摆脱老化的基础设施。 这意味着您也不能忽略语言的历史。

  **09:47** - _Ritika Trikha_

  有些事情必须得做。 当我在 HackerRank 时，我亲眼看到了多少银行和金融机构对 COBOL 开发人员造成伤害，并且几乎绝望了。 这不是一个将被解决的问题，我认为要么对系统进行某种现代化，要么我们继续培训人员并激励他们。 我个人认为将会有 COBOL 再次出现的一天。 真的，当所有拥有 COBOL 知识的开发人员退休并且没有新一代的开发人员学 COBOL 时，将会发生什么？ 一定要付出，对吧？ 因此，还需要进行更多的系统化和制度化的变革才能开始从 COBOL 转向新的基于云的基础设施。

  **10:37** - _Saron Yitbarek_

  Ritika Trikha 是一名旧金山的技术编辑。

  **10:49** - _Saron Yitbarek_

  那么 Ritika 提到的那些基于云的基础设施又会怎么样呢？ 我们今天建立的基础设施是否会将后代绑定到特定的语言，像我们仍绑定到 COBOL 一样？ 亚马逊2006年推出的 Web Services（AWS） 可能是最大的单片云设施。 Google 云平台于2008年问世，微软 Azure 于2010年问世。 Go 语言以并发为重点，定位于在新的云基础设施上蓬勃发展。 这是这个时代的语言。

  **11:26** - _Carmen Andoh_

  嗨，我叫 Carmen Andoh， 我是谷歌 Go 小组的项目经理。

  **11:34** - _Saron Yitbarek_

  Carmen 对 Go 语言与今天的基础设施有怎样的联系有内幕消息。 它起源于 Go 的创作者和语言历史的紧密联系。

  **11:47** - _Carmen Andoh_

  Robert Pike，Robert Griesemer 和 Ken Thompson。 自从1960年代以来，这些名字就已经出现了。 Ken Thompson 发明了B语言，然后他在夏天休假后继续发明 UNIX 操作系统。 Rob Pike 发明了字符串编码 UTF-8 和 ASCII 。 他帮助 Ken Thompson 共同编写了 UNIX 编程环境。 因此，这两个人已经合伙很长时间了，他们一直在用以前的编程语言(包括 Ken Thompson 和 Dennis Ritchie 最终帮助编写的 C 在内)研究和发明操作系统。

  **12:28** - _Saron Yitbarek_

  Pike，Griesemer 和 Thompson 在 Google 工作之后，他们发现了一个严重的问题。 并没有产生大规模并发。 人们等待了几个小时来汇总草案。 他们使用的是 C++，并且不得不编写所有这些回调和事件派发器。 那是2009年，而且我们的基础设施再次发生了变化。 诸如 C++ 之类的语言与新的现状越来越不协调。

  **12:59** - _Carmen Andoh_

  多核处理器，网络系统，海量计算集群和 Web 编程模型等正在引入这些问题。 而且，也就是这个行业的增长和程序员数量在2010年将要达到成千上万。因此，直到那时所有的编程语言都是在规避问题而不是在正面解决问题。

  **13:24** - _Saron Yitbarek_

  最终，将达到一个临界点，必须开始改变。

  **13:30** - _Carmen Andoh_

  嘿，我们讨厌 C++ ，我说：”好吧，让我们看看我们是否能发明些新的东西“。

  **13:37** - _Saron Yitbarek_

  新语言需要完美地适应我们最新的基础设施。

  **13:43** - _Carmen Andoh_

  2005年云技术到来以后，您不再需要自己的计算机，任意地方只需要租用它，您就可以得到一个分布式系统。 但是分布式系统和云的问题是，在分布式系统之间存在并发消息传递问题。 您需要确保采用异步对您来说没有问题。 Go 缺省就是异步的编程语言。 基本上，这意味着您执行的每个操作（例如将所有这些不同的消息发送给系统中的另一个计算机）都无需等待另一个机器对您的响应即可完成。 因此，它可以在任何给定时间处理多个消息。

  **14:28** - _Carmen Andoh_

  就是说，云计算是分布式的。 因此开发了 Go 来满足这一确切的需求。 Go 早就成为进行这种分布式计算的标准方法之一。 这就是为什么我认为它立即引起了开发人员的广泛关注。 Go 绝对是云基础设施的语言，无论是其设计，还是所有云基础设施工具以及在过去十年中如雨后春笋般出现的模块的生态。

  **15:06** - _Saron Yitbarek_

  很快，诸如 Kubernetes 之类的关键应用都用 Go 编写了。 谷歌还创建了 Go 云，这是一个开源库和一系列工具，使得 Go 更具吸引力。 很显然，它是新生态系统的语言。 它是云的语言。 创造者因开发持久的语言而享有声誉，这绝对没有坏处。

  **15:33** - _Carmen Andoh_

  我认为业界的其他人会说：“嘿，我认为这不会很快消失。”这种语言的发明者恰巧也发明了已经有50年或60年历史的语言。

  **15:47** - _Saron Yitbarek_

  Carmen Andoh 是谷歌 Go 团队的项目经理。

  **15:54** - _Saron Yitbarek_

  因此，我们有了一种新的语言 Go ，旨在提供云基础设施必需的并发性。 听起来不错。 Go 的设计师倾向于创造可以持续半个世纪的语言。 也很棒。 但是我的问题是，从现在起50年后，当 Go 更像是 COBOL 时，这到底意味着什么？ 当世界上充满了只有老开发人员才能理解的旧版 Go 代码时，这意味着什么？ 在当今的云基础设施老化的时候，我们是否会做好准备？ 我们是否正在从 COBOL 和大型机领域吸取教训，可以帮助我们为 Go 和云设计更美好的未来？

  **16:40** - _Saron Yitbarek_

  幸运的是，我找到了问所有这些问题的合适人选。 下面就来看看。

  **16:51** - _Saron Yitbarek_

  我们如何使我们的语言能面向未来？ 我们知道他们与当今的基础设施息息相关。 而且我们知道，随着数十年的发展，新的基础设施必将取代旧的基础设施。 那么，我们今天做些什么以确保将来能平滑演进？

  **17:10** - _Kelsey Hightower_

  我是 Kelsey Hightower ，我在 Google 是一名开发人员拥护者，我致力于引入开放性技术并将它们应用于 Google Cloud 上的产品。

  **17:19** - _Saron Yitbarek_

  Kelsey 花了大量时间思考编程的未来。 我很好奇，是否有一天我们将陷于握有 Go 语言技能的是另一批老龄化的程序员的问题，就像我们现在缺少 COBOL 的引导一样。 我们是否在为这个长远的未来做计划？ 因此，我和 Kelsey 坐下来进行讨论。

  **17:42** - _Kelsey Hightower_

  ...等等。 但是，如果您考虑到今天面临的一些新的挑战，如应对 Internet ，网络，您将面临许多用户，数十万个并发用户，以及不同的机器和体系结构的组合。 考虑到这些新的场景，因此您通常希望有一种新的语言来解决。 例如， JavaScript 是用于 We b的，您不会想改造 COBOL ，以便可以用它来进行 Web 编程。 最终，我们今天已经建立了数百种相当完善的语言，而且它们都非常专注于他们的优势。

  **18:15** - _Saron Yitbarek_

  那么，在那种情况下，我们是否需要积极推动人们走向 COBOL ？ 如果我们正在为这些新问题开发新语言并且它们是高度定制化的，并且 COBOL 仍在坚持，我们是否需要鼓励人们选择它，以便我们可以维护我们的旧代码？

  **18:32** - _Kelsey Hightower_

  好吧，我认为这将对企业构成挑战，对吗？ 如此，您已经在 COBOL 上发展了10到20年，没有人会主动想学习一些新的 COBOL 。 或者您不会像“我要加倍努力……”那样从大学毕业。

  **18:45** - _Saron Yitbarek_

  是的。

  **18:46** - _Kelsey Hightower_

  “ ...这种语言比我父母的年龄都大。” 因此，在那个领域，您必须问自己，继续使用 COBOL 的风险是什么？未来是否仍然有意义？我认为它仍然有益于某些类型的工作负载，但是我们必须问自己一个问题，是时候推进了吗？ 是时候发展一点了吗？ 因此，如果您仍然有数十亿行的 COBOL 代码，那么您将必须寻找所有剩余的 COBOL 人才并将其招进来，但也许我们该开始考虑其他语言能从 COBOL 学习些什么，并将某些功能和库加入到其他语言中。

  **19:26** - _Saron Yitbarek_

  COBOL 终止以后的日子，将会是一个巨大的基础设施项目。用我对纽约地铁的比喻，就像是要替换每条地下隧道。因此，展望未来，我想知道我们是否可以预见到这些问题，甚至将来对自己也能有所帮助。

  **19:48** - _Saron Yitbarek_

  如果我们将今天的云与大型机进行比较，我们是否会在最终到达同一条船上, 有着这些旧代码库, 使用着旧的但非常稳定的语言，而且我们也不得不做出选择的时候。 我们应该继续前进还是保持不变？

  **20:05** - _Kelsey Hightower_

  云有点不同的是它不是来自一个制造商，对吗？许多云提供商通常提供了一系列技术集，这样您就可以选择编程语言，编程范式，无论您是要事件驱动还是基于 \[HTTP\] 的全 Web 服务。 这意味着您可以选择编程的方式，然后只需专注于要解决的问题。 因此，数据将会输入，数据将会输出，但是您来选择处理数据的方式。

  **20:36** - _Kelsey Hightower_

  大型机通常只有一个主界面，对吗？ 就像您编写一份任务一样，这就是您提交任务的方式，这就是您监控任务的方式，这就是结果。 这本身就是一个限制。 如果您考虑一些较新的大型机，它们也会支持些较新的技术，因此即使在大型机领域，您也会开始看到可用于运行任务的编程语言扩展。

  **20:58** - _Kelsey Hightower_

  那么我们开始问自己，好吧，假设我有了新的选项，该什么时候离开这种特定的编程范式？ 我认为我们不会陷入困境。

  **21:08** - _Saron Yitbarek_

  是的。

  **21:08** - _Kelsey Hightower_

  我认为新的分布式机器很不错，可能起步成本更低，您不必购买整个大型机即可开工。 但是我们仍然希望易用性和之前一样：给您我的工作，您为我运行它，完成后告诉我。

  **21:24** - _Saron Yitbarek_

  当然。您看看当今的语言都发生了什么，或者 COBOL 发生了什么？ 以 Go 语言做例子，您看到我们在努力地改进 Go 从而吸引人们在30年内都还想用 Go ？

  **21:38** - _Kelsey Hightower_

  我认为所有语言都会遭受这种命运，对吗？ 如果您想一下，其实 Python 已经存在很长时间了。 我认为接近20年，甚至更久。 因此，我认为会发生…… Python 重新流行起来了，它是机器学习的基础语言。

  **21:53** - _Saron Yitbarek_

  嗯。

  **21:54** - _Kelsey Hightower_

  对于 Tensorflow 之类的库，如果我们仅用时间来衡量，我认为这可能不是看待它的正确方式。还应该有社区是否活跃？语言的适配意愿是否活跃？我认为 Python 做得确实非常出色……社区看到了应该使其他语言更易于使用。例如， Tensorflow 底层有很多 C++ ，使用这种语言编程可能没有 Python 这样的用户友好性。您可以用 Python 并用它来生成人们正在使用的一些东西，例如 Tensorflow 。现在机器学习非常热门，人们将 Python 引入了这个新领域，那么您猜怎么着？ Python 仍然是活跃的，并且在未来的一段时间内都是活跃的。对于 Go 来说，这同样适用。如果 Go 能够继续保持活跃度，那么，它就像许多基础设施工具和许多云库的基层一样，它也将保持活跃。因此，我认为都是那些社区确保了它们将来占有一席之地，并且当未来出现时确保那里有它们的故事。

  **22:58** - _Saron Yitbarek_

  是的。 那么，我们如何对语言进行过时的验证？ 就是说，我们如何有意地设计一种语言能使其持续存在并在20、30年内都保持活跃呢？

  **23:10** - _Kelsey Hightower_

  使用语言的人，我认为这在开源世界中确实是独一无二的。 现在，我们已经不再使用商业语言了，对吧，过去曾经来自 Microsoft 的语言或 Sun Microsystems 的如 Java™ ，那时侯，每个人都依赖供应商来尽心尽力来对语言能干什么以及在运行时进行新的改进。 现在，我们看到的诸如 Go，Node.js，Ruby 之类的东西，所有这些都是社区支持的，并且社区专注于运行时和语言。 这样任何人都可以添加新库，对吗？ 有一个新的 \[HTTP\] 规范，对， \[HTTP/2\] 几年前问世，每个社区都有贡献者添加了那些特定的库，猜猜现在怎么样？ 所有这些语言现在都兼容与大部分的未来网站。

  **24:01** - _Kelsey Hightower_

  我认为现在是个人真正地拥有了更多的控制权，如果他们想让语言适用于新的用例，只需要自己实现即可。 因此，我们不再受限于一两家公司。 如果公司倒闭，那么运行时可能会因此而消亡。 我们不再有这个问题了。

  **24:23** - _Saron Yitbarek_

  我们之前在这个播客上已经说过了。 未来是开放的。 但是，令人着迷的是考虑怎样能做到再过几十年，过去也将是开放的。 他们将继承能够变形和演进的基础设施和语言。

  **24:39** - _Kelsey Hightower_

  太棒了，感谢您的加入，我期待人们的工作而且大型机仍然有意义。 它们是经典技术，因此我们不称其为遗产。

  **24:47** - _Saron Yitbarek_

  哦，我喜欢，经典，非常好。

  **24:51** - _Saron Yitbarek_

  Kelsey Hightower 是 Google 的开发倡导者。

  **24:57** - _Saron Yitbarek_

  我正在想象一个充满经典编程语言以及尚未诞生的新语言的未来。 那是我为之兴奋的未来。

  **25:07** - _Speaker_

  请离关着的门远一点。

  **25:12** - _Saron Yitbarek_

  要知道，2017年州长安德鲁·库莫 （Andrew Cuomo） 宣布纽约市地铁进入紧急状态。 他的政府拨出90亿美元投资于老化的基础设施。 这应该提醒我们，迟早我们得注意遗留的系统。 您不仅需要继续前进，面向未来。您还背着历史包袱。

  **25:37** - _Saron Yitbarek_

  在开发世界中，我们倾向于偏向未来。 我们认为我们的语言仅在它们流行时才有用。 但是，随着信息基础架构的不断老化，开发的历史变得越来越真实。 事实证明，过去根本没有过去。 记住这一点是我们的工作。

  **26:05** - _Saron Yitbarek_

  您可以前往 [redhat.com/commandlineheroes](//www.redhat.com/zh-CN/command-line-heroes） ，以了解有关 COBOL 或 Go 或本季我们要介绍的其他语言的更多信息。 那里有很多很棒的材料在等你。

  **26:19** - _Saron Yitbarek_

  下一集谈 Bash 。 我们将探索 shell 脚本的起源以及自动化的关键。

  **26:30** - _Saron Yitbarek_

  Command Line Heroes 是 Red Hat 的原始播客。 我是 Saron Yitbarek 。 在下一次之前，请继续编码。

  --------------------------------------------------------------------------------

  via: https://www.redhat.com/en/command-line-heroes/season-3/the-infrastructure-effect

  作者：[Red Hat][a]
  选题：[bestony][b]
  译者：[messon007](https://github.com/messon007)
  校对：[校对者ID](https://github.com/校对者ID)

  本文由 [LCRH](https://github.com/LCTT/LCRH) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出
  [a]: https://www.redhat.com/en/command-line-heroes
  [b]: https://github.com/bestony
