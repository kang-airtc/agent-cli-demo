# agent-cli-demo

关注 B 站 **光谷老亢** 学习更多 AI WebRTC 知识 🎯

一个演示如何用 Node.js（TypeScript）和 Python 构建 AI Agent CLI 工具的项目。

## 项目结构

```
agent-cli-demo/
├── my-agent-node-cli/     # Node.js + TypeScript 版本
└── my-agent-python-cli/   # Python 版本
```

## my-agent-node-cli

基于 Node.js + TypeScript 实现的 AI Agent 命令行工具。

### 安装与使用

```bash
cd my-agent-node-cli
npm install
npm run build
npm link

opencode --help
```

## my-agent-python-cli

基于 Python 实现的 AI Agent 命令行工具。

### 安装与使用

```bash
cd my-agent-python-cli
pip install -e .

# 或使用安装脚本
bash install.sh
```
