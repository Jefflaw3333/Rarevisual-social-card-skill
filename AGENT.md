# Agent 工作约定 (Rare Visual fork)

## 项目说明

这个目录是 `rarevisual-social-card-skill` 的 Skill 本体,**fork 自 [guizang-social-card-skill](https://github.com/op7418/guizang-social-card-skill) v0.15**,为 **Rare Visual** (rarevisual.com, premium handcrafted accessories DTC brand) 重新调整了色板、词库、品类路由,视觉工作流与 28 个 layout 骨架完全继承。

它面向的产出包括:

- 小红书 / Rednote 3:4 图文组图。
- 微信公众号 21:9 头图 + 1:1 分享卡封面对。
- 文章封面、产品更新卡片、礼盒攻略图、教程拆页等静态信息流视觉内容。
- Live Photo 实况动图(单视频、二/三/四宫格拼图、三连拼贴、长视频诊断)。
- **Rare Visual 专属调整**:warm-brass Editorial 默认主题、rv-gold Swiss 默认锚色、品牌词库(handcrafted / gold-filled / everyday 等)。

这个仓库的根目录应该保持为 Skill 可安装、可维护的结构。根目录主要放:

- `SKILL.md`
- `README.md` / `README.en.md`
- `references/`
- `assets/`
- `agents/`
- `validate-social-deck.mjs`
- `package.json` / `package-lock.json`
- 授权、产品说明、交接、CHANGELOG 等项目级文档

不要把一次性的生成案例、渲染输出、临时素材、调试脚本或下载图片直接放在 Skill 根目录。

## 测试产物放置规则

所有测试生成的产物都放到:

```text
rvj-local-tests/
```

(注意:`local-tests/` 是上游 Guizang 的目录名,Rare Visual fork 使用 `rvj-local-tests/` 以避免与上游习惯冲突,也方便 `git pull upstream` 时不冲突。)

推荐按一次任务或一个测试案例建独立子目录:

```text
rvj-local-tests/<case-name>/
```

每个测试目录可以包含自己的 `index.html`、`render.cjs` / `render.mjs`、`assets/`、`output/`、`SOURCES.md` 等文件。例如:

```text
rvj-local-tests/social-card-example/
rvj-local-tests/social-card-example/index.html
rvj-local-tests/social-card-example/render.cjs
rvj-local-tests/social-card-example/assets/
rvj-local-tests/social-card-example/output/
```

原则:

- 试跑 HTML 放在 `rvj-local-tests/<case-name>/`。
- 渲染出来的 PNG/JPEG/WebP 放在 `rvj-local-tests/<case-name>/output/`。
- 下载或临时使用的图片、截图、素材放在 `rvj-local-tests/<case-name>/assets/`。
- 一次性调试脚本放在对应测试目录里;只有通用校验或 Skill 本体需要的脚本才放根目录。
- 如果要把某个测试案例升级为正式示例,先明确它属于项目文档、参考资料还是发布资产,再移动到合适位置;不要默认留在根目录。
- **从上游 upgrade 同步时**:`local-tests/` 目录名要保持独立。如果你已经按上游命名建了 `local-tests/`,通过 `git mv local-tests rvj-local-tests` 重命名一次即可,后续 PR / commit 历史会保留。
- 如果你有从上游 fork 之前就存在的 `local-tests/`,保留即可(自己用),不需要重命名 —— `rvj-local-tests/` 只用于本 fork 改造后的新测试。
