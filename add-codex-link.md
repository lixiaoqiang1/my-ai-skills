# 给 common 技能加 Codex 联接

以 `common\ceshi1` 为例：

```powershell
cmd /c 'mklink /J "F:\my-ai-skills\codex\ceshi1" "F:\my-ai-skills\common\ceshi1"'
```

通用（改 `技能名`）：

```powershell
cmd /c 'mklink /J "F:\my-ai-skills\codex\技能名" "F:\my-ai-skills\common\技能名"'
```

删联接（不删实体）：

```powershell
cmd /c 'rmdir "F:\my-ai-skills\codex\技能名"'
```

说明：技能目录需含 `SKILL.md`；Cursor 指向整个 `common`，不用加联接。
