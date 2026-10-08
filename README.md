# 八股文 · 面试实战版

一份面向后端面试的八股文速查笔记，覆盖 Redis、JVM、集合、框架、MySQL、JUC、RocketMQ 七个高频主题，共 30 道题，每道题都按「面试怎么问 → 怎么答 → 追问怎么接」的思路整理。

已通过 GitHub Pages 发布，可直接在浏览器打开，手机端也可阅读：

**在线地址：<https://littleye-yee.github.io/eight-essay/>**

## 内容概览

| 章节 | 主题 | 题量 |
| --- | --- | --- |
| 一 | Redis | 9 |
| 二 | JVM | 3 |
| 三 | 集合 | 3 |
| 四 | 框架 | 1 |
| 五 | MySQL | 5 |
| 六 | JUC | 3 |
| 七 | RocketMQ | 6 |
| | **合计** | **30** |

题目涵盖：Redis 数据类型 / 淘汰策略 / 过期删除 / 持久化 / 集群 / 缓存击穿·穿透·雪崩 / 缓存一致性；JVM 类加载、内存结构、垃圾回收；ArrayList、HashMap、ConcurrentHashMap 底层原理；Spring Boot 自动装配；MySQL 索引与 B+ 树、索引优化、事务与隔离级别、MVCC、三种日志；synchronized 与 Lock、ThreadLocal、线程池参数；RocketMQ 整体架构。

## 目录结构

```
.
├── index.html          # 单页 HTML 版（GitHub Pages 首页），样式与脚本全部内联，无外部依赖
├── 八股文-精简版.md     # Markdown 源文件，便于编辑和二次加工
├── .nojekyll           # 关闭 GitHub Pages 的 Jekyll 处理，保证文件原样输出
└── README.md
```

## 本地查看

直接双击 `index.html` 即可在浏览器中打开，不需要安装任何依赖或启动服务。

如果想在本地起一个静态服务（更接近线上环境）：

```bash
python -m http.server 8000
# 然后访问 http://localhost:8000/
```

## 部署说明

本项目用 GitHub Pages 托管，方式为「从分支部署」：

- 发布源：`main` 分支，根目录 `/`
- 首页文件：`index.html`
- 仓库需保持 public（GitHub Pages 的免费额度仅对公开仓库开放）

## 更新内容

改完文件后提交推送，Pages 会自动重新构建（通常 1 分钟内生效）：

```bash
git add -A
git commit -m "更新八股文内容"
git push
```

如果改了 HTML，记得同步维护 `八股文-精简版.md`，保持两份内容一致。

## 说明

笔记内容为个人整理，用于面试复习，不保证覆盖全部考点，也不构成标准答案；如有表述不准确的地方欢迎指出。
