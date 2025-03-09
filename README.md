# test
this is only a test
flowchart TD
    A[客户提交工单] --> B[存入数据库: Tickets表]
    B --> C[模型分类预测]
    C --> D[更新预测分类字段]
    D --> E{学生工处理}
    E -->|简单工单| F[解决并关闭]
    E -->|复杂工单| G[修正分类]
    G --> H[更新实际分类字段]
    H --> I[转交产品经理]
    I --> J[产品经理处理]
    J --> K[更新状态为Resolved]
    K --> L[PPI仪表盘]
    F --> L
    L --> M[End]
