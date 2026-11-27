# Rray

南京邮电大学 · 计算机科学与技术

**C++ 系统工程 · Agent Harness**

围绕软件故障诊断，实践受控工具、Run 生命周期、证据追踪与 Agent 评测。

[个人网站](https://rrrayy.github.io) · [技术文章](https://rrrayy.github.io/blog/) · [邮箱](mailto:3111937934@qq.com)

---

## 正在构建

### EvidenceOps

面向软件运行故障的本机诊断工作台。每次 Run 将模型调用、受限工具执行、运行证据与诊断报告关联起来，支持历史回查、事件重放和评测。

```mermaid
flowchart LR
    Request[请求] --> Run[Agent Run]
    Run --> Agent[Agent Loop]
    Agent --> Tools[受控只读工具]
    Tools --> Evidence[运行证据]
    Evidence --> Report[诊断报告]
    Report --> Review[规则检查与人工评审]
```

当前实现包含 C++20 日志解析、上下文预算、BM25 / RRF 检索与 20 案例离线诊断评测。最近加入逐条结论与引用证据的人工语义审核。

[项目说明与源码](https://github.com/Rrrayy/EvidenceOps) · [个人网站](https://rrrayy.github.io/projects/evidenceops/)


---

## 技术栈

**C++ 与系统**  
C++17 / C++20 · Linux · Unix · TCP/IP · epoll · 多线程 · 内存管理 · RPC · Protobuf · muduo

**Agent 与后端**  
Python · FastAPI · asyncio · Pydantic · Tool Runtime · Tool Calling · Structured Output · SSE

**数据与检索**  
PostgreSQL · SQLite · pgvector · MySQL · Redis · SQLAlchemy · Alembic · BM25 · RRF

**构建与验证**  
CMake · Make · GDB · Docker · pytest · Git · GitHub Actions · VS Code · Claude Code · Codex

---

## GitHub 活跃度

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Rrrayy&show_icons=true&theme=dark&hide_border=true&bg_color=0d1117&title_color=ef4444&icon_color=f87171" height="165" alt="GitHub 统计"/>
  <img src="https://streak-stats.demolab.com/?user=Rrrayy&theme=dark&hide_border=true&background=0d1117&ring=ef4444&fire=f87171&currStreakLabel=f87171" height="165" alt="GitHub 连续贡献统计"/>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/Rrrayy/Rrrayy/gh-pages/github-contribution-grid-snake-dark.svg?v=5" alt="GitHub 贡献轨迹" width="900"/>
</p>
