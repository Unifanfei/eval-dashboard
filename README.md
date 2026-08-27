# TrialGuard 评估看板（静态部署）

临床试验预测评估平台的只读静态版本，由 GitHub Pages 托管。

- 页面：`index.html`（与主仓库 `evaluation_dashboard.html` 同源，附加静态 fetch 适配器）
- 数据：`eval_api/` 下冻结 JSON，与只读评估接口（8103）响应结构一致
- 包含批次：`eval_batch_20260827_kimi_codex_review_v1`（75 条）、`eval_batch_20260827_deepseek_codex_review_v3`（75 条）
- 本站不包含控制平面（8092）面板；页面中相应入口会显示"静态部署未包含控制平面接口"
- 三轴独立展示（预测准确性/分析质量/搜索与证据质量），不生成综合总分；not_evaluable 不折算为 0

数据导出脚本与来源见主仓库 `clinical_agent`。
