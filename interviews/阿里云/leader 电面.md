1. 有没有推动新技术落地到项目中的经历？可以介绍下
    1. 介绍了pwa
    2. 面试官质疑 pwa 的兼容性，在 can i use 中各浏览器对其的兼容性并不好。相反像 webassembly/webgl 这样的技术，各大浏览器都在积极跟进。
    3. 作为创业团队的前端技术负责同学，技术判断力和技术嗅觉还有待坚强，经验还有所不够。
2. 假设让你做一个巨大的地图，上面需要绘制几十万个节点的信息，而且他们需要更新，可能一次就是更新几个万个节点的信息，你判断会有哪些技术难点？如何解决？
    1. 一开始答了前后端通信的一个协议机制。面试官反馈说，底层的通信协议如 tcp/ip 都会实现这些东西，没有必要在业务层再考虑这些问题。
    2. 会用 canvas 实现，应该会用 webgl 来处理。
    3. 说性能瓶颈可能在于浏览器的绘制。面试官说像魔兽这样的游戏，它有多少点要处理？如果它能处理过来，应该就没问题。
    4. 然后说瓶颈可能在于内存的占用。面试官问，你会如何衡量能够支持多大的数据量，能够支持什么级别的数据渲染？
        1. 答以对内存占用进行计算
    5. 然后问
3. 现在服务器需要处理一个csv，这个csv有10g大，但服务器只有5g内存空间，然后可以进行压缩，压缩后可以降低至2g以下，然后将压缩后的文件传至云盘上，如何解决？
    1. 答以对文件进行拆分，然后流式处理
    2. 面试官说现在都支持流式处理。


现在需要你绘制一个地图，上面要展示几十万个战士的信息，每个战士相当于一个gps定位点，需要它能实时地反应其真实位置。如何设计前后端系统来完成这个需求？