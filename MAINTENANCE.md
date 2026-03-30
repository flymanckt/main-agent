# main-agent 维护说明

## 主维护目录
以后 `main-agent` 的所有 Git 操作都在这里进行：

```bash
/home/kent/repos/main-agent
```

不要再从下面这个目录对 `main-agent` 做 git push：

```bash
/home/kent/.openclaw/workspace
```

## 常用命令

### 进入主目录
```bash
cd /home/kent/repos/main-agent
```

### 查看状态
```bash
git status
```

### 拉取最新代码
```bash
git pull --rebase
```

### 提交修改
```bash
git add .
git commit -m "your message"
```

### 推送
```bash
git push
```

## 当前远端
```bash
git@github.com:flymanckt/main-agent.git
```

## 规则
1. `main-agent` 后续只在 `/home/kent/repos/main-agent` 维护
2. finance 旧仓库不要再当作主仓库继续开发
3. 运行态文件不要随便提交：
   - `runtime/alert_state.json`
   - `runtime/last_snapshot.json`
   - `runtime/akshare_spot_cache.json`
   - `review-ledger-live.md`
   - `.venv/`

## 备注
如果需要把 OpenClaw workspace 里的变更同步到独立仓库，优先手动比对后复制，不要直接在 workspace 根目录 git push。
