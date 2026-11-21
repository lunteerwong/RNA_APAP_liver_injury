# RNA_APAP_liver_injury

# APAP肝损伤，时间序列转录组分析
Time-series transcriptomics analysis of APAP-induced liver injury

## 项目简介
对APAP（对乙酰氨基酚）诱导肝损伤的时间序列转录组数据进行系统分析，识别动态差异表达基因，筛选核心marker。

## 数据来源
- 数据库：GEO
- 数据集编号：GSEXXXXX（跑完后填）
- 样本信息：多个时间点（0h/2h/6h/12h/24h等）

## 分析流程
1. **数据质控**：FASTQ质量评估（FastQC）、过滤（Trimmomatic）
2. **比对定量**：STAR比对 + featureCounts定量
3. **差异分析**：DESeq2，各时间点 vs 对照
4. **时间聚类**：mFuzz，识别动态表达模式
5. **功能富集**：clusterProfiler，GO/KEGG分析
6. **特征筛选**：LASSO + 随机森林，筛选核心基因

## 技术栈
- 语言：R / Python / Bash
- 核心包：DESeq2, mFuzz, clusterProfiler, glmnet, randomForest
- 可视化：ggplot2, pheatmap

## 项目状态
- [x] 分析框架设计
- [ ] 数据下载与质控
- [ ] 差异分析
- [ ] 时间聚类
- [ ] 特征筛选
- [ ] 结果整理

## 作者
lunteer Wong
