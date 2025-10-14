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
    邮箱：1821746019@qq.com<br>
    意向工作城市：深圳
  </div>
</div>


#### <img src="assets/graduation-cap-solid.svg" style="width:1.618rem"> 教育经历

- 数据科学与大数据技术，深圳技术大学(一本)，2022.9–2026.7（预计）
- 语言：大学英语四级、六级通过，读写是强项，能够独立阅读英文技术文档、学术论文
- 荣誉和认证：蓝桥杯省级程序设计竞赛二等奖、阿里云Apsara Clouder认证

#### <img src="assets/project-diagram-solid.svg" style="width:1.618rem"> 项目经历

- **多人在线排课系统**｜组长、测试和运维：专为老师定制的拖放式排课系统

  **Go、MySQL、Vue、Linux、Apifox**

  - **介绍**：传统的纸质课表依赖物理媒介、电子课表虽解决了该问题，但难协同、效率低的问题依旧存在。此系统旨在将传统的线下排课流程数字化、网络化，通过技术手段提升排课工作的效率。
  - **主要职责**：
    - **主导全栈协作与问题解决**：作为项目技术核心，澄清数据模型与API用法，协助修复了包括空指针引用、CORS在内的多个关键Bug，保障了开发流程的顺畅。
    - **提升API质量与系统安全**：独立负责API的全面测试，发现并推动修复了用户权限校验缺失等多个安全漏洞。同时为服务配置二级域名及SSL证书，实现全站HTTPS加密通信。
    - **保障服务器高可用与部署效率**：通过性能监控定位问题，创建`swap`分区解决了因Go服务内存耗尽导致的服务器频繁崩溃问题；诊断并调整云服务商的自动更新策略，杜绝了计划外的服务中断；编写自动化部署脚本并集成Webhook，实现了代码的自动化部署。

- **TradingEnv**｜独立开发：量化回测与策略研发系统

  **Python、PostgreSQL、Redis、pandas、numpy、matplotlib/seaborn**

  - 构建期货/加密货币/外汇/指数回测与研究环境，支持多tickers多频OHLCV加载与事件驱动撮合。
  - 支持策略研发流水线与指标可视化；实现 PremiumIndex、VWAP、CVD 背离（在研）、AI agent 等策略框架。
  - 使用redis以及合适的同步机制，避免了缓存击穿和惊群效应
  - 拥有健全的异常处理与日志追踪便于排查问题。
  - 高性能：经过优化，SPS从一开始的1000提升到了10000，10倍加速；简化缓存有效性验证逻辑，将2020-2024年间1m级别共2M+行数据的获取时间从23s降到了1s

- **SISS is Not a Sandbox**｜独立开发：便携化与软件管控工具，但不像沙盒那样创造强隔离的环境

  **C++、CMake、vcpkg、Hook**

  - **软件+数据一键迁移新电脑**：对特定文件/注册表路径进行重定向，实现软件便携化。
  - **一定程度管控软件，保护隐私安全。**：拦截特定路径访问，阻止开机自启、自更新、扫盘、敏感数据读取(如 QQ 读取浏览器历史)

#### <img src="assets/tools-solid.svg" style="width:1.618rem"> 技能清单

- **语言/框架**：Python、C++
- **数据科学**：NumPy、Pandas、Matplotlib/Seaborn
- **数据库与缓存**：PostgreSQL、MySQL、Redis
- **工程与运维**：Linux、Docker、Git、CI/CD、CMake、vcpkg
- **专业能力**：
  - **性能分析与优化**：熟练使用性能分析工具定位代码热点进行细致优化，显著提高代码执行效率
  - **高并发和异步编程**：能够编写多线程/进程代码，利用多核CPU避免GIL的限制。能够使用异步来解决IO密集型任务，避免阻塞。
  - **独立开发和团队协作**：既能独立完成中小型项目，也具有团队合作精神和积极主动的态度


###  其它经历
- 《大数据原理》课程助教：该课程实验课难度较大，有众多新颖的工具和名词，同学们易感到困惑、在实验中卡壳、因迟迟找不到解决办法而丧失积极性。我的职责是确保同学们能够理解新工具和命令的使用，在实验课上我积极为同学们答疑解惑。最终确保了每位同学都能按时提交作业，得到了老师的认可。
