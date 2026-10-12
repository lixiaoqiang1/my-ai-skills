# 给新技能加 Codex 联接

Cursor 会自动读整个本目录；Codex 需要给每个技能加一条联接。

以 `agent-browser` 为例：

```powershell
cmd /c 'mklink /J "C:\Users\李晓强\.codex\skills\agent-browser" "F:\my-ai-skills\agent-browser"'
```

通用（改 `技能名`）：

```powershell
cmd /c 'mklink /J "C:\Users\李晓强\.codex\skills\技能名" "F:\my-ai-skills\技能名"'
```

删联接（不删实体）：

```powershell
cmd /c 'rmdir "C:\Users\李晓强\.codex\skills\技能名"'
```

技能目录需含 `SKILL.md`。
