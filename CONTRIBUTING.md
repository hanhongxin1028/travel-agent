# 团队 Git 协作流程说明文档

## 1. 分支管理规范

- 主分支：`main`（最终代码）
- 开发分支：`dev`（集成所有功能，稳定后合并到 `main`）
- 功能分支：以 `feature/模块名称` 命名，例如：
  - `feature/intent-recognition`
  - `feature/itinerary-planner`

---

## 2. 克隆仓库
```bash
git clone https://github.com/hanhongxin1028/travel-agent.git
cd travel-agent
```
---

## 3. 拉取最新代码
切换到 dev 分支并拉取最新代码：
```bash
git checkout dev
git pull origin dev
```
---

## 4. 创建功能分支
```bash
git checkout -b feature/your-module-name
```
---

## 5. 本地开发和提交代码
```bash
git add .
git commit -m "简洁描述本次修改内容"
git push origin feature/your-module-name
```
---

## 6. 创建 Pull Request（PR）
* 登录 GitHub，打开项目仓库

* 找到刚推送的分支，点击 “Compare & pull request”

* 填写标题和描述，关联 Issue（示例：Closes #5）

* 指派 Review 人，等待审核

