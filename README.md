# DFT 測試筆記

## 一、DFT (Design For Testability) 概述
- 目的：提升晶片可測試性，方便製造巡檢與缺陷偵測。
- 主要技術：
  - 掃描鏈（Scan Chain）
  - 內建自我測試（BIST）
  - 邊界掃描（Boundary Scan / JTAG）
  - 測試點插入

## 二、ATE (Automatic Test Equipment) 使用
- 功能：自動執行測試向量，收集並分析測試結果。
- 工作流程：
  1. 載入測試程式
  2. 施加測試向量
  3. 收集輸出訊號
  4. 缺陷分析與報告
- 注意事項：
  - 優化測試時間
  - 確保覆蓋率
  - 硬體/軟體同步更新


