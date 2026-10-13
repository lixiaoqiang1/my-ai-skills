# 给新技能加 Codex 联接

Cursor 读整个 `F:\my-ai-skills`（含 `common\`、`yuanxingtu\`）；Codex 需给每个技能加联接。

## 新增技能必做（每次都要同步）

1. **技能目录含 `SKILL.md`**
2. **`yuanxingtu` 内技能：`SKILL.md` 顶部（YAML frontmatter 之后）必须有中文简介**，格式：

   ```markdown
   > **中文简介：** ……一句话说明用途与触发场景……
   ```

3. **加 Codex 联接**（见下方命令）
4. **同步更新根目录 [SKILLS.md](SKILLS.md)**：补全结构树，并在名称后写简短中文介绍

## common 技能

```powershell
cmd /c 'mklink /J "C:\Users\李晓强\.codex\skills\技能名" "F:\my-ai-skills\common\技能名"'
```

例：`agent-browser`

```powershell
cmd /c 'mklink /J "C:\Users\李晓强\.codex\skills\agent-browser" "F:\my-ai-skills\common\agent-browser"'
```

## yuanxingtu 技能

```powershell
cmd /c 'mklink /J "C:\Users\李晓强\.codex\skills\技能名" "F:\my-ai-skills\yuanxingtu\技能名"'
```

例：`brainstorming`

```powershell
cmd /c 'mklink /J "C:\Users\李晓强\.codex\skills\brainstorming" "F:\my-ai-skills\yuanxingtu\brainstorming"'
```

## 删联接（不删实体）

```powershell
cmd /c 'rmdir "C:\Users\李晓强\.codex\skills\技能名"'
```

删技能后同样要同步改 [SKILLS.md](SKILLS.md)。
