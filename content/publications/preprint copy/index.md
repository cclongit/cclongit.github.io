---
title: "环境经济学视角下中国稀土资源动态配置机理与优化路径研究"
authors:
- admin
date: "2025-05-08T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2030-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: From the perspective of environmental economics, this study focuses on the dynamic optimization of intertemporal allocation of China's rare earth resources. Addressing core contradictions including structural imbalances in production and pricing, environmental externalities, and strategic value depreciation, it innovatively constructs a discount model for dynamic resource allocation (NPV-Model). Breaking through traditional static analytical frameworks, this model incorporates temporal dynamics, environmental value factors, and strategic value factors into allocation decision-making, revealing the rationality and necessity of delayed exploitation. Empirical analysis using USGS data examines China's current rare earth resource allocation patterns. Finally, policy recommendations for optimizing China's rare earth resource allocation are proposed based on economic principles.

# Summary. An optional shortened abstract.
summary: ""

tags:
- Environmental Economics

featured: true

hugoblox:
  ids:
    arxiv: 1512.04133v1

# you can use this link later
# links:
# - type: preprint
#   provider: arxiv
#   id: 1512.04133v1
# - type: code
#   url: https://github.com/HugoBlox/hugo-blox-builder
# - type: slides
#   url: https://www.slideshare.net/
# - type: dataset
#   url: "#"
# - type: poster
#   url: "#"
# - type: source
#   url: "#"
# - type: video
#   url: https://youtube.com
# - type: custom
#   label: Custom Link
#   url: http://example.org

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
math: true  
---

<!-- 或在 Markdown 中直接插入 HTML -->
<script>
window.MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']],
    displayMath: [['$$', '$$'], ['\\[', '\\]']]
  }
};
</script>
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-svg.js" async></script>

<!-- This work is driven by the results in my [previous paper](/publications/conference-paper/) on LLMs. -->

<!-- > [!NOTE]
> Create your slides in Markdown - click the *Slides* button to check out the example.

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
# 注：此为working paper，其中有些地方有待改进，包括公式的渲染等可能也会存在问题。后续会加紧改正

## 一、研究我国稀土资源动态配置的背景

稀土（REE）是稀土元素或稀土金属的简称，包括镧（La）、铈（Ce）、镨（Pr）、钕（Nd）、钷（Pm）、钐（Sm）、铕（Eu）、钆（Gd）、铽（Tb）、镝（Dy）、钬（Ho）、钕（Er）、铒（Tm）、铯（Yb）、镥（Lu）、钇（Y）钪（Sc）通常可分为两组：铈稀土元素或轻稀土元素（镧、铈、镨、钕、镅、钐、铕）、钇组稀土元素或重稀土元素（钆、铽、镝、钬、铒、铥、镱、镨、镥、钇）。现今，稀土已在农业、国防军工、冶金工业、石油化工、玻璃陶瓷、电子、高新材料等13个领域的40多个行业中取得了广泛的应用。随着科学技术的不断发展和稀土新材料的不断研发，稀土已成为当今世界各国改造传统工业、发展高新产业和国防尖端技术不可或缺的战略资源 $ {}^{\left\lbrack  {1}\right\rbrack  } $ $ {}^{\left\lbrack  {2}\right\rbrack  } $。

早在1992年邓小平南巡考察时就说过“东有石油，中国有稀土”，中国是世界上稀土资源储量最丰富的国家，也是矿种最齐全的国家，同时分布的稀土资源分布上不仅面广而且也相对集中。中国稀土资源的集中中国区包括四川凉山、江西赣南、内蒙古的白云鄂博、山东微山以及广东粤北，其中仅内蒙古的白云鄂博已探测到的稀土储量就占全国稀土总储量的83%左右；另外，在广西、湖南、新疆等地也探测到了不少稀土矿床 $ {}^{\left\lbrack  {3}\right\rbrack  } $ 。

相关数据表明，我国稀土资源的研究以矿业专业期刊为主、经济学相关期刊较少。其中研究的主要内容主要集中于：1、稀土资源的储量和产量及分布。2、稀土资源开采的技术。3、稀土资源开采过程中的环境污染分析。4、稀土资源缺乏国际定价权的问题。有关于技术层面的研究较多，同时经济学层面的研究主要集中在买方垄断 $ {}^{\left\lbrack  {4}\right\rbrack  } $ 上面，而关于稀土资源时间上动态配置方面的相关研究则较少。

本研究聚焦于稀土资源时序动态配置，主要具有以下几方面的理论和实践意义。首先，由于我国稀土资源长期存在过度开采的问题，并且开采过程中伴随着多方面的环境污染，因此实现合理配置有助于保护环境、实现资源与环境的可持续发展。其次，因为稀土资源开采过度没有限额，加上稀土资源贸易的定价权缺失，我国稀土资源在出口方面出现了“贸易利得损失”的现象。因此实现资源的合理配置，降低目前的开采量也可以维护我国在国际稀土市场上的利益。总而言之，研究我国稀土资源时间上的动态配置，为深入理解稀土资源和国家战略、可持续发展等提供了一个新颖的视角。

## 二、描述稀土资源动态配置的理论框架 NPV-Model

下面我们将结合我国稀土资源的三个重要性质：资源垄断地位、环境外部性、战略地位特殊性，以此来构建稀土资源动态配置的理论框架 NPV-Model。具体的构建和推导过程如下。

由于我国稀土资源经过过去几十年的大量勘探和开采已经趋于饱和，我们不妨假设我国已知的稀土资源总量是不变的，用Q表示。(1)

由于稀土市场具有一定的垄断性质，因此我们可以假设稀土的价格是关于产量Q的函数，P=P(Q)，其中P'(Q)<0，即P关于Q的一阶导数为负，代表了随着产量的下降，稀土资源变得稀疏，从而价格提高。(2)

由（1）（2）两个式子可以得出，稀土资源的收益可以表示为：

$$ \text{Profit}=P(Q)*Q $$

对于稀土开采的成本而言，我们将它分解为两部分：直接成本C1和机会成本C2。为研究方便，我们假设直接成本是关于开采量的线性函数 $ C_{1}=k_{1}*Q $（Q），其中k1代表了每单位稀土开采的直接成本。对于机会成本而言，我们主要关心稀土开采带来的环境损失，由于开采技术的发展和进步，稀土开采过程中带来的环境损失应该会变小，设环境损失因子p只与时间t有关，并且将第一期的环境损失因子p设为1，为简化分析，使用反比例函数形式刻画环境损失因子p=1(5)；并且环境损失应该也是和开采量成正比的，记单位开采的环境损失为k2，因此我们得到 $ C_{2}=k_{2}*Q^{p}*Q^{q}*r^{1} $ 。(6)。

由（4）（6）两个式子可以得出，稀土开采的总成本为：

$$ \text{Cost}=\mathrm{C}_{1}+\mathrm{C}_{2}=\mathrm{k}_{1}*\mathrm{Q}+\mathrm{k}_{2}*\mathrm{Q}*\mathrm{r}^{1} $$

(7)

结合开采的收益和总成本（3）（7）两式，稀土资源的总利润为：

$$ \pi=\text { Profit }-\text { Cost }=\text { P(Q)*Q }-\text { k}_{1}*\text { Q }-\text { k}_{2}*\text { Q }^{*}\text { r }^{1} $$

(8)

接下来我们考虑时间上的动态规划，我们的核心目标是通过折现模型来计算净现值NPV，进而分析最大化净现值的策略，从而得出稀土资源开采的规划配置方案。

首先，我们先来估算折现因子，为简化分析，我们将折现因子r定义为实际利率，因此t期的收益折算到当期应该乘上折现因子(1-r)；其中的经济学含义是：当期带来的收益更加大，因为人们总是不耐心并关注于近期的。(9)

同时，由于稀土资源作为战略资源的重要地位，稀土资源在未来的价值是会逐渐上升的，我们用g代表战略带来的价值收益，可以设定稀土资源的价值应该乘上战略因子(1+g)。 (10)

结合(8)(9)(10)以及净现值的计算公式，我们可以得出最终的净现值：

$$ \mathrm{NPV}=\sum_{\mathrm{t}=1}^{\mathrm{n}}\left[\mathrm{P}\left(\mathrm{Q}^{\mathrm{n}}\right)^{*}\mathrm{q}_{\mathrm{t}}-\mathrm{k}_{1}^{*}\mathrm{q}_{\mathrm{t}}-\mathrm{k}_{2}^{*}\mathrm{q}_{\mathrm{t}}^{*}\mathrm{r}^{1}\right]*(1+\mathrm{r})^{-t}*(1+\mathrm{g})^{t} $$

其中 $ \mathrm{Q}=\sum_{\mathrm{t}=1}^{\mathrm{n}}\mathrm{q}_{\mathrm{t}} $

下面我们结合净现值的总公式做分析，可以得到下面的结论：尽量延后开采时间，减缓当期开采量不是企业的最佳选择。主要原因有如下几点：i、企业遵循利润的最大化原则，如果当期开采量过大，稀土的市场价格下降幅度可能大大，企业利润反而降低。

ii.如果考虑社会成本，企业选择延后开采的成本较低，自然利润可以得到提高。iii.在一般情况下，稀土资源重要的科学意义和战略意义使得战略效益g应该比较高，可以假设g>r，因此实际的折现率可以近似于负值，因此在经过折现计算后晚开采的效益应该更高，这是稀土资源作为战略资源的特殊性。

如果要求解该模型的解析解，需要使用拉格朗日乘数法：

$$ \mathrm{L}=\sum_{\mathrm{t}=1}^{\mathrm{n}}\left[\mathrm{P}\left(\mathrm{Q}^{\mathrm{n}}\right)^{*}\mathrm{q}_{\mathrm{t}}-\mathrm{k}_{1}^{*}\mathrm{q}_{\mathrm{t}}-\mathrm{k}_{2}^{*}\mathrm{q}_{\mathrm{t}}^{*}\mathrm{r}^{1}\right]*(1+\mathrm{r})^{-t}*(1+\mathrm{g})^{t}+\lambda^{*}\left(\mathrm{Q}-\sum_{\mathrm{t}=1}^{\mathrm{n}}\mathrm{q}_{\mathrm{t}}\right) $$

一阶条件为 $ \frac{\partial L}{\partial q_{t}}=0 $ ， $ t=1,2,\cdots,n $； $ \frac{\partial L}{\partial \lambda}=0 $ 。

可根据方程组求解出每一期的最优产量 $ q_t $。

需要指出的是，这个动态模型是一个侧重理论层面的机理分析，具体实际的参数如P(Q)函数的选取，k1，k2的确定，时间跨度n的选取，以及折现因子(1+r)-t，(1+g)t的估算，都需要大量的实际数据和研究进行支撑。本模型考虑了稀土资源的战略意义以及环境污染带来的损失，为分析我国稀土资源配置提供了简单的理论框架。

 
## 三、我国稀土资源配置的现状分析
正如前文所提到，我国稀土资源在近几十年出现了乱开采、过度开采等现象，造成了一系列不包括于恶性竞争、土壤污染等等问题。根据本文第二部分推导的净现值公式，现就公式的三方面（垄断定价层面、战略地位层面、可持续发展层面）对我国稀土资源的配置现状进行简单分析。
就稀土资源的垄断层面而言，根据美国地质调查局的矿业数据Mineral Commodity Summary 2010-2024显示[5]，中国稀土资源的储量长期保持在4400万吨左右，而稀土资源的产量则是由逐年上升的趋势，尤其在2020-2024年间迅速上升（图一）。对比之前对净现值模型NPV-Model的结论，我国的稀土产量处于明显过高的情况，这与我国稀土资源缺乏定价权，稀土市场存在恶性竞争以及国际局势的波动是密切相关的。根据净现值公式，我国在稀土资源出口配额方面还应该做严格控制，这样一方面能够维护本土企业的利润，另一方面也为未来的资源配置提供可发挥空间。

值得注意的是，从2013年起，随着世界范围内新的稀土矿藏不断发现（如2011年在阿富汗发现了一个千万吨级的大型稀土矿，朝鲜、越南等地相继发现新的稀土矿），我国占世界稀土资源已探明储量的相对比例会有所下降[6]。

我国稀土资源的垄断地位减弱，相应的对价格的控制权也在逐步下降，这对我国未来的稀土资源配置是一个新的挑战。如何实现开采规模调控与战略地位维护的权衡取舍，是我国稀土资源中未来配置研究中亟待突破的关键课题。
就稀土资源的战略地位层面而言，我国目前主要存在两个值得探讨的问题：一是虽然我国稀土资源总类丰富，门类齐全，但我国的稀土资源以氟碳铈矿和独居石等富轻稀土的矿物为主(如白云鄂博和川西牦牛坪矿床), 而磷钇矿和褐钇铌矿等富重稀土为主的矿物资源量却较少[7]。在重稀土富集资源的勘探开发层面，特别需要构建资源安全与市场调控并重的动态管理体系。二是从战略应用而言，我国是全球稀土消费第一大国，消费量占全球的57%（2020，国信证券），然而稀土资源的应用大部分只停留在采选和冶炼分离环节，稀土的高端消费不足，例如在高纯稀土金属制备技术、磁性材料等领域当中，虽然我国在不断跟踪、模仿，但实际技术仍和国外领先水平存在差距[8]。
就稀土资源的可持续发展层面而言，在我国稀土资源开采、运输和应用过程当中，产生了一系列的环境污染问题，包括但不限于化学污染（如放射性污染、重金属污染、氟污染、氨氮和硫酸根污染）、大气污染（粉尘和尾矿堆积造成）、土壤污染（水土流失和滑坡等）、生态系统污染（生物多样性受到损失）[9]。这些环境的污染问题不仅对生态系统和人类健康造成了负面影响，并且还难以用金钱来度量[10]，想要对稀土利用过程当中污染所造成的负外部性进行矫正十分困难。政府会面临如何征收合适的环境税或环保费用的巨大问题。这在前文净现值的NPV-Model模型当中可以直观体现为单位开采造成的污染k2难以估量的问题。如果估计k2过大，企业将会在成本端受到巨大损失、减少产量过多，对经济增长造成不良影响；如果估量k2过小，则不能够有效矫正污染带来的负外部性问题，并且压低产量qt也没有达标，不利于实现企业的净现值最大。


## 四、稀土资源动态配置的优化路径研究
鉴于在以往的研究当中，我国不同专业领域的专家学者都对稀土资源配置的优化路径提供了许多良好可行的建议：如实行进口配额制、加强稀土应用技术开发、合并稀土企业、纳入环境税等等。这些建议其实已经非常全面和深入了，笔者不想对这些建议做过多的叙述和阐释。这里，笔者想回归经济学当中的十大原理——人们总是在进行权衡取舍(trade-off)[11]。结合前文的净现值模型NPV-Model，笔者想从经济学思想的角度为我国未来的稀土资源优化路径提出一点自身的看法和建议。我将其归纳为“做好三个权衡取舍”。
一是做好价格和产量的权衡取舍。我国的稀土资源目前正处于一个关键的“瓶颈期”，稀土资源的世界占比正在不断下降，不像以往几十年前具有绝对优势和地位了，另外，高新稀土应用技术还处于萌发阶段，碰到了许多“卡脖子”的问题。同时，我国在宏观战略上也已经从高速发展转变为高质量发展。基于这样的问题和背景，如何合理控制我国稀土的资源的产量和出口量就尤为关键了。目前，我国主要通过实施稀土出口配额来控制稀土出口量。该政策虽然面临着国际和西方社会对所谓“贸易保护”的“指责”，但是该制度对我国绝对是利大于弊的，应该在未来继续推行。同时，我们也应该清楚地认识到，如何规划控制限额，绝对不能由政府官员直接拍板就决定的，而是需要科学合理考虑。应吸取相关专家学者的估计和预算，应用博弈论、垄断市场、折现模型、环境度量等跨学科知识，做好统计和预测，提供一个接近最优解的国际出口配额，并进行动态规划和调整。
二是做好当期和未来的权衡取舍。在经济学当中，折现率r代表着人们的耐心程度，r的值越大说明未来相同的价值折算到当期就会越少，人们也会更加不耐心。对于稀土资源，由于考虑了战略的价值溢价g，实际的折现率呈现出负值，也就意味着对于稀土资源，我们要保持百分之一百二十的耐心。然而当期发展也十分重要，“在长期当中，我们都死了”（凯恩斯），我们不能一味地考虑储藏资源为未来使用，也要兼顾当期的经济协调与稳定。因此，我们既要兼顾长期均衡发展，也应关注短期经济稳定。同理，对于稀土资源的转型发展和配置而言，我们不能“一刀切”，而是要“小步走”，应该实施多阶段的阶梯计划，逐步促进稀土相关企业向高技术、高附加值转型，以期未来的可持续发展。
三是做好发展和环保的权衡取舍。矿产资源开发利用都会面临着开采造成污染的难题，而治理环境问题势必要损失经济，开采和环保属二元对立关系。企业本身具有搭便车的激励，不会过多甚至不考虑环境问题，导致出现市场失灵的现象。这时候需要政府及时出台相关法规，对市场的负外部性矫正，至少应矫正达到或超过“经济最优点”。法规也是值得探索的，需要综合直接管控、经济管控和产权管控等多种方式，结合我国地方特色实践，制定具有中国特色的制度法规。同时，也应加大力度支持绿色开采冶炼技术的创新发展，如近年来不断发展的混合型稀土矿冶炼技术、离子吸附型冶炼技术等[12]。这需要国家给予相关的政策激励和补贴，促进企业研发相关绿色稀土技术。


## 五、参考文献
[1]黄小卫,张永奇,李红卫.我国稀土资源的开发利用现状与发展趋势[J].中国科学基金,2011,25(03):134-137.DOI:10.16262/j.cnki.1000-8217.2011.03.015.
[2]季根源,张洪平,李秋玲,等.中国稀土矿产资源现状及其可持续发展对策[J].中国矿业,2018,27(08):9-16.
[3]黄静丽.世界稀土资源储量分布及供需现状分析[J].中国集体经济,2015,(06):109-110.
[4]宋文飞,李国平,韩先锋.稀土定价权缺失、理论机理及制度解释[J].中国工业经济,2011,(10):46-55.DOI:10.19581/j.cnki.ciejournal.2011.10.005.
[5]Mineral Commodity Summary. USGS 2011-2024. https://www.usgs.gov/
[6]邹君宇,王建平,柳振江,等.中国稀土资源现状和问题及对策的思考[J].矿业研究与开发,2014,34(02):119-123.DOI:10.13827/j.cnki.kyyk.2014.02.032.
[7]何宏平,杨武斌.我国稀土资源现状和评价[J].大地构造与成矿学,2022,46(05):829-841.DOI:10.16539/j.ddgzyckx.2022.05.001.
[8]郑国栋,王琨,陈其慎,等.世界稀土产业格局变化与中国稀土产业面临的问题[J].地球学报,2021,42(02):265-272.
[9]高志强,周启星.稀土矿露天开采过程的污染及对资源和生态环境的影响[J].生态学杂志,2011,30(12):2915-2922.DOI:10.13292/j.1000-4890.2011.0421.
[10]王学军.环境质量经济价值度量的若干问题[J].管理世界,1994,(03):193-197.DOI:10.19744/j.cnki.11-1235/f.1994.03.031.
[11]曼昆, N. G. (2014). 经济学原理 (梁小民, 梁砾译, 第7版). 北京大学出版社
[12]谢东岳,伏彩萍,唐忠阳,等.我国稀土资源现状与冶炼技术进展[J].矿产保护与利用,2021,41(01):152-160.DOI:10.13779/j.cnki.issn1001-0076.2021.01.022.