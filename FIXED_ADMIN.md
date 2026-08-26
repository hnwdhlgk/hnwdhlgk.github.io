# 后台连接修复版

修复 `admin/index.html` 点击“连接”无反应的问题：
- 使用明确的 addEventListener 事件绑定，不再依赖 inline onclick
- 点击后显示“验证中”
- 验证 GitHub 仓库与 data/categories.json、data/jobs.json
- 401/403/404 与网络错误给出明确提示
- 使用 sessionStorage 保存当前会话
- Token 不写入仓库
