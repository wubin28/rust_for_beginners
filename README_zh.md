# 《小小白学Rust：从点亮LED到玩转编程》（极简版）

[English Version](README.md)

作者：吾真本

![image_cover.jpeg](image_cover_learn_rust_by_games_3_cartoon_style.jpeg)

**绘图：生成式AI。螃蟹和micro:bit v2开发板边上有一片绿色的树叶，上面有明显的锈菌感染特征。Rust语言的创始者霍尔将这门语言命名为Rust，灵感来自锈菌。这些植物病原体具有复杂的生命周期，涉及多个宿主，增强了它们在不同环境中生存的能力。同样，Rust通过强制执行内存安全规则的"过度工程"，虽然严格，但确保了软件的稳定性。**

## 引言

《小小白学Rust：从点亮LED到玩转编程》（极简版）是一本遵循CC BY-NC-ND 4.0许可协议的有限共享电子书。它以独特方式帮助读者入门Rust编程语言：通过编写游戏（包括嵌入式、Web和命令行）来学习，同时探讨常见陷阱及其规避方法。本书以游戏编程为引子，探索在生成式AI的强大影响下，专业程序员如何用Rust完成软件开发项目。在这个过程中，我们揭示常见的陷阱和错误，旨在让学习过程更加引人入胜、富有乐趣和充满动力。

本书书名中的"小小白"，暗示本书特别适合两类初学者：完全没有编程经验的新手，以及有一些编程经验但未接触过嵌入式开发的人士。

本书将Rust入门知识分为三篇，每篇聚焦一类游戏开发。各篇章内容围绕完成特定游戏项目所需的知识展开。这种安排有一个明显优势：读者能够迅速将所学付诸实践，从而加深对Rust的理解。

**如果你喜欢这本电子书，请给它点个星⭐️！**

本书各章的标题将随着撰写过程不断优化和调整。

## 目录

### 第一篇 点亮LED灯

- 第1章 小小白为何要学Rust
- 第2章 让第一个LED灯闪烁
- 第3章 LED滚动文字显示屏
- 第4章 不小心改错了代码与自动化测试
- 第5章 记忆挑战游戏学习与变量
- 第6章 电子宠物游戏与所有权
- 第7章 打地鼠游戏与结构体
- 第8章 防盗报警系统与错误处理
- 第9章 反应测试游戏与生存期
- 第10章 贪吃蛇游戏与unsafe Rust

### 第二篇 打造多线程web游戏

- 第11章 在线井字棋游戏与Cargo
- 第12章 多人聊天室与包、crate和模块
- 第13章 可定制卡牌对战游戏与泛型
- 第14章 多人在线狼人杀与trait
- 第15章 协作式拼图游戏与智能指针
- 第16章 实时排行榜与并发
- 第17章 即时战略游戏服务器与异步

### 第三篇 制作有趣的命令行游戏

- 第18章 数独游戏与常用集合类型
- 第19章 文字冒险游戏与枚举
- 第20章 谜语猜猜看与模式匹配
- 第21章 单词频率统计器与迭代器
- 第22章 定制化计算器与闭包
- 第23章 命令行小游戏引擎与宏
- 第24章 角色扮演游戏与面向对象
- 第25章 多功能命令行工具与高级类型
- 第26章 发布游戏到crates.io分享快乐
- 附录

## 版权许可协议

[《小小白学Rust：从点亮LED到玩转编程》（极简版）](https://github.com/wubin28/learn_rust_by_games)© 2024 作者 [吾真本](https://github.com/wubin28) 采用 [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/?ref=chooser-v1) 许可协议授权。

本书采用知识共享署名-非商业性使用-禁止演绎 4.0 国际许可协议（CC BY-NC-ND 4.0）进行许可。

该协议允许你分享本书，但有以下严格限制：

- 署名（BY）：分享时必须注明吾真本为原作者，不得隐瞒或更改此信息。
- 非商业性使用（NC）：本书仅限非商业用途，不得用于盈利或商业项目。
- 禁止演绎（ND）：你可以分享本书的原始版本，但不得改编、修改或重新创作。换言之，不能对本书内容进行任何改变或添加。

这个协议具体意味着：

- 可以分享，但不得更改：你可以在网上分享本书，但必须保持原样，不得修改任何内容。
- 禁止商业用途：本书不得用于任何商业环境，如广告、出版物或付费项目。
- 保护原作完整性：此协议帮助原作者维护作品的完整性和原创性，防止他人进行二次创作或商业利用。

简而言之，CC BY-NC-ND 4.0 是一个相对严格的协议。它允许自由分享本书，但禁止任何形式的改编或商业利用。

## 本书代码

本书代码可在GitHub上的[https://github.com/wubin28/learn_rust_by_games](https://github.com/wubin28/learn_rust_by_games)代码库中下载。每个代码清单都标注了其在代码库中的具体位置，方便读者查找和运行。代码库按章节组织，格式为chxx（xx为章节编号）。

## 开发环境准备

要运行本书代码，请根据你的操作系统准备以下设备和软件：

| **你的计算机的操作系统** | **Linux（原生或在Windows 10/11的WSL2中使用）或macOS** | **Windows 10/11** |
| --- | --- | --- |
| micro:bit v2开发板 | 1块 | 1块 |
| USB micro数据线 | 1根 | 1根 |
| 命令行shell | zsh | Windows PowerShell |
| 命令行shell配置框架 | Oh My Zsh | Oh My Posh |
| Git | 需要 | 需要 |
| Rust | 需要 | 需要 |
| Visual Studio Code (VS Code) 或 Cursor AI | 需要 | 需要 |
| VS Code的rust-analyzer插件 | 需要 | 需要 |

由于在Windows 10/11的WSL2中使用Linux对初学者来说较为复杂，本书暂不详述。其他操作系统的开发环境配置详见第1章。

## 使用的图标

在本书中，我们使用特定的图标来突出显示不同类型的信息：

- ✅ 行动号召
- ⚠️ 需要特别注意的警告或重要细节
- 🔎 深入探讨主题——可选但有助于扩展知识
- 🤔练习题
- 💡 练习提示

## 致谢

感谢人民邮电出版社编辑杨海玲老师。她敏锐地察觉到Rust编程这一热门趋势，以专业出版物的标准为本书前几章提供了批注，并建议作者向读者分享电子版，以获取更多反馈来提升本书质量。正是她的这些努力促成了本电子书的诞生。

感谢网友"别打小兰"对本书内容构思提供的宝贵建议。他提出了三个极具启发性的观点：一是编程新手在学习Rust时希望能完成一个从头到尾的完整项目；二是探讨新手为何选择学习Rust；三是增加英文版，以获取国外（Rust在那里可能更受欢迎）读者的反馈。这些见解促使作者重新考虑了本书的目标读者群体，将其从"至少掌握一门编程语言的读者"扩展到"编程或嵌入式开发可以是零基础的读者"，并将英文版作为默认语言版。

## 常见问题

### 1. 这本书适合编程小白吗？

本书特别适合两类小白：完全没有编程经验的新手，以及有编程经验但未接触过嵌入式开发的人士。

### 2. 这本书与其他 Rust 学习资源有何不同？

本书采用了独特的方法，通过编写丰富多彩的游戏（尤其是第一部分的嵌入式游戏）来教授Rust的各种概念。同时，它探索了学习Rust过程中常见的错误和陷阱，帮助读者深入理解Rust的特性和最佳实践。

### 3. 这本书完成了吗？

这本书正在持续撰写中，预计2025年7月底前后写完。我们会定期添加和更新章节。请经常回来查看最新的内容和更新。

### 4. 我如何为这本书做出贡献？

我们热烈欢迎各种形式的贡献！如果你发现任何错误、有改进的想法，或想添加新内容，请在这个GitHub仓库上提交PR或开启一个issue。你的宝贵意见将帮助这本书变得更好，惠及所有Rust初学者。如果你的贡献给我留下深刻印象，我会在本书的致谢部分特别感谢你。

### 5. 这本书为何是极简版？

本书计划通过出版社出版。在创作过程中，我们以有限共享的极简版形式获取读者反馈，以便改进内容。出版社版本将包含更多内容。两个版本的主要区别在于：极简版提供小小白开发软件项目全过程的核心要点，而出版社版本则在此基础上增加了如何向生成式AI提问、学习Rust过程中的常见陷阱、陷阱形成原因及避免方法等增值内容，以提升出版社版本的价值。

### 6. 这本书有其他语言版本吗？

目前，这本书正在用英语和中文编写。如果你有兴趣将本书翻译成其他语言，请通过在这个GitHub仓库上开启一个issue来联系作者。

### 7. 如果我按照书中内容操作遇到问题该怎么办？

你可以先尝试根据出错信息在网上搜索解决方案，或者咨询你常用的生成式AI。如果仍然无法解决，可以茄作者薇薪wuzhenben001（请备注"bygames"），我会抽空为你解答。

---

感谢你对《小小白学Rust：从点亮LED到玩转编程》（极简版）的兴趣！我们希望这本书能成为你Rust学习之旅中的宝贵资源。请记住，在为入门Rust而编写游戏的过程中，你踩的坑和避的坑越多，学习速度就越快。毕竟，那些“坑”往往是我们最好的老师！