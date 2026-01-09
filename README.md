# book-recommendation-system
书籍推荐系统（课程期末项目）：基于召回-排序-重排流程的轻量级推荐系统，包含用户注册、书籍评分、个性化推荐等功能。
book-recommendation-system/
├── .gitattributes
├── README.md          # 项目说明文档
├── requirements.txt   # 依赖库列表
├── src/               # 核心代码目录
│   ├── 01_data_explore.py        # 数据探索
│   ├── 02_data_clean.py          # 数据清洗
│   ├── 03_feature_engineering.py # 特征工程
│   ├── 04_recall_model.py        # 召回模型（双塔模型）
│   ├── 05_ranking_model.py       # 排序模型（LightGBM）
│   ├── 06_recommend_core.py      # 推荐核心逻辑（召回-排序-重排）
│   ├── 07_recommend_service.py   # 推荐服务接口（Flask）
│   ├── 08_evaluate.py            # 模型评估
│   ├── 09_item_cf.py             # Item-CF协同过滤召回
│   └── 10_add_book_categories.py # 书籍分类特征处理
├── models/            # 模型文件
│   └── ranking_model.pkl         # 排序模型保存
├── templates/         # 前端页面模板
│   ├── index.html     # 首页（推荐结果+评分提交）
│   └── register.html  # 用户注册页面
├── data/              # 数据目录
│   ├── features/      # 特征数据（用户/书籍嵌入、特征工程结果）
│   ├── processed/     # 清洗后的数据
│   └── raw/           # 原始数据
└── static/            # 静态资源
    └── style.css      # 前端样式

    依次运行01到10，然后在08打开前端