# frontend/ — 前端模块（成员 B）

Vue 3 + TypeScript + CesiumJS 三维可视化系统。

## 职责

- 历史轨迹、预测轨迹、强度变化、风圈/影响范围、预测走廊的三维展示
- 台风筛选、时间轴动画、点位查询、图层开关、数据面板
- 按成员 A 定义的字段和时间格式接入预测 JSON
- 离线历史回放 + 基本异常处理 + 演示稳定性

## 目录

```
frontend/
├── src/          # 源码
│   ├── main.ts
│   ├── App.vue
│   ├── components/   # Cesium 组件
│   └── views/        # 页面
├── public/       # 静态资源（含预测 JSON 数据）
├── index.html
├── package.json
└── vite.config.ts
```

## 技术栈

- Vue 3 / TypeScript / CesiumJS / Vite
- 包管理：npm 或 pnpm

## 运行

待补充（`npm install` → `npm run dev`）。

## 注意

- 历史 / 预测 / 范围图层分开管理，使用明确图例与颜色区分。
- 提交前清理 Cesium token、测试账号、调试日志、无关界面元素。
