<div style="
  display: grid;
  grid-template-columns: auto 1fr 1fr;
  align-items: center;
  column-gap: 20px;
  width: 100%;
  font-family: 'Microsoft YaHei', sans-serif;
">
  <img src="assets/我的照片-四六级.jpg" width="75" style="border-radius: 10px;">
  <div>
    <h2 style="margin: 0;">王勇顺</h2>
    <div style="line-height: 1.6;">
      出生日期：2004-11-13<br>
      性别：男
    </div>
  </div>
  <div style="text-align: left; line-height: 1.6;">
    联系方式：+86 17322974044<br>
    邮箱：wys17322974044@outlook.com<br>
    意向工作城市：深圳
  </div>
</div>

#### <img src="assets/graduation-cap-solid.svg" style="width:1.618rem"> 教育经历

- 数据科学与大数据技术，深圳技术大学(一本)，2022.9–2026.6（预计），绩点3.3/4.5(前50%)
- 语言：大学英语四级、六级(能独立阅读英文技术文档、学术论文)
- 荣誉和认证：蓝桥杯省级程序设计竞赛二等奖、阿里云Apsara Clouder认证、freeCodeCamp前端/后端/数据库证书

#### <img src="assets/project-diagram-solid.svg" style="width:1.618rem"> 项目经历

- **[仿京东商城](https://1821746019.github.io/jd/)**｜独立开发：《web应用开发》课程设计，旨在复刻京东商城首页
  - **技术栈：HTML/CSS/JS、TailwindCSS**
  - 结果：视觉效果相似度达90%+；课程评分A

- **[多人在线拖放式排课系统](https://github.com/1821746019/online_spreadsheet_frontend)**｜组长、测试和运维：传统的纸质课表依赖物理媒介、电子课表虽解决了该问题，但难协同、效率低的问题依旧存在。此系统旨在将传统的线下排课流程数字化、网络化，通过技术手段提升排课工作的效率。
  - **技术栈：HTML/CSS/JS、Vue、Go、MySQL、Linux、Apifox**
  - **主要职责**：
    - **主导全栈协作与问题解决**：作为项目技术核心，澄清数据模型与API用法，协助修复了包括空指针引用、CORS在内的多个关键Bug，保障了开发流程的顺畅。
    - **提升API质量与系统安全**：独立负责API的全面测试，发现并推动修复了用户权限校验缺失等多个安全漏洞。同时为服务配置二级域名及SSL证书，实现全站HTTPS加密通信。
    - **保障服务器高可用与部署效率**：通过性能监控定位问题，创建`swap`分区解决了因Go服务内存耗尽导致的服务器频繁崩溃问题；诊断并调整云服务商的自动更新策略，杜绝了计划外的服务中断；编写自动化部署脚本并集成Webhook，实现了代码的自动化部署。

- **[TradingEnv](https://github.com/1821746019/TradingEnv/tree/portfolio)**｜独立开发：一个期货/加密货币/外汇/指数回测与研究环境，支持多tickers多频OHLCV加载与事件驱动回测。支持策略研发流水线与买卖点可视化，已实现 PremiumIndex、VWAP、CVD 背离、AI agent 等策略框架。
  - **技术栈：Python、PostgreSQL、Redis、pandas、numpy、matplotlib/seaborn**
  - 回测需要OHLCV数据、策略研发可能会用到OpenInterest、PremiumIndex等指标，而Binance只提供了按天或按月分割的数据压缩包，为了能在系统中使用这些数据，我编写Python脚本来自动化地完成数据爬取与导入，成功导入了10W+行数据。
  - 最初的开发注重代码逻辑正确性，未刻意优化性能，SPS只有1000。为了提高回测的速度，我利用line_profile、pyinstrument性能分析工具定位热点代码，然后通过移除或合并冗余调用、将OHLCV以及指标的存储容器从pd.dataframe迁移到np.ndarray等一系列优化手段，将SPS提升到10000，实现了10倍加速。
  - tickers多、回测时间框架低(1m)、时间跨度长(2020-2025)导致数据量大，拉取时间长。为减少等待时间，我引入redis并采用合适的同步机制，避免了缓存击穿和惊群效应，然后使用多线程编程，让不同tickers数据的获取能并发地进行。最终将2W+行数据的获取时间从23s降到1s，大幅提高了回测的启动速度。

- **[SISS Is a Semi-Sandbox](https://github.com/1821746019/PortableAnyApp)**｜独立开发：便携化与软件管控工具，但不像沙盒那样创造强隔离的环境，使用场景有软件连同数据一键迁移新电脑、阻止自更新/扫盘/敏感数据读取
  - **技术栈： C++、CMake、vcpkg、Hook**
  - 有些路径需要重定向/拦截/虚拟化，有些则不需要。为了判断某个路径需要进行什么样的操作，我通过设计一个多叉树结构和toml配置文件，100%正确地将路径映射到了对应的操作，并且性能良好，时间复杂度是O(n).
  - SISS的注册表模块需要支持不同模式(Patch/Virtualize/Redirect)，不同模式下各个函数的逻辑差别较大，使用if-else将不同模式的逻辑耦合在一起。为了提高代码可读性和可维护性，我封装了实现同一接口的三个类，利用继承和多态的特性巧妙地分割了代码，让代码可读性和可维护性提高了66%


#### <img src="assets/tools-solid.svg" style="width:1.618rem"> 技能清单

- **语言/框架**：Python、C++、HTML/CSS/JS/TS、React
- **数据科学**：NumPy、Pandas、Matplotlib/Seaborn
- **数据库与缓存**：PostgreSQL、MySQL、Redis
- **工程与运维**：Linux、Docker、Git、CI/CD、CMake、vcpkg
- **专业能力**：
  - **性能分析与优化**：熟练使用性能分析工具定位代码热点进行细致优化，显著提高代码执行效率
  - **高并发和异步编程**：能够编写多线程/进程代码，利用多核CPU避免GIL的限制。能够使用异步来解决IO密集型任务，避免阻塞。
  - **独立开发和团队协作**：既能独立完成中小型项目，也具有团队合作精神和积极主动的态度

###  其它

- 从小对计算机感兴趣，喜欢操作各种软件，能快速学习并使用各种应用程序

- 曾担任《大数据原理》课程助教：该课程实验课难度较大，有众多新颖的工具和名词，同学们易感到困惑、在实验中卡壳、因迟迟找不到解决办法而丧失积极性。为确保同学们能够理解新工具和命令的使用，在实验课上我积极为同学们答疑解惑。最终确保了同学们作业100%按时提交
- 《计算机组成原理》、《操作系统》、《计算机网络》、《Web应用开发》、《数据库系统》、《云计算技术》、《大数据编程与可视化》等专业课成绩优良(前20%)
