# 枭熊 · D&D 怪物 URL 库

为枭熊插件提供 `data/bestiary/bestiary-TOWER.json` 怪物数据。

## 插件导入地址（方式一 · 单文件 URL）

在枭熊插件「+ 添加库」填入：

```
https://morenxcq.github.io/dnd-bestiary/data/bestiary/bestiary-TOWER.json
```

## 目录结构

```
data/bestiary/bestiary-TOWER.json   ← 怪物聚合文件（顶层单键 "monster"，source=TOWER）
search/index.json                   ← 可选总索引（为方式二预留）
```

## 维护方式（D:\ds工作区）

1. 把要上线的怪物 JSON（顶层为 `"monster"` 数组）放进 `枭熊库\` 文件夹。
2. 运行一键更新：
   ```
   python -X utf8 _工具\url_lib_update.py push
   ```
3. 推送后插件里点 🔄 刷新即可看到更新。

> `枭熊库\` 是唯一手动纳入口；此处 `data/`、`search/` 由脚本自动生成，不要手改。
