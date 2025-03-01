# Full-stack ai tender document review system
![image](https://github.com/user-attachments/assets/3d88163a-45ed-4c1f-aac0-402650fca634)

该项目目前正在开发过程中…..

## ai标书审核系统

这是一个利用大模型自主规划和决策，调用工具，自动化完成标书审核各项细分任务的项目，意在帮助

- **效率提升**：减少人工逐条核对的时间成本。
- **准确性**：避免人为疏漏，尤其是复杂条款的语义理解。

预计实现功能包括但不限于：

### **1. 资质合规性审查**

- **任务内容**：验证投标方资质文件（如营业执照、资质证书、业绩证明等）是否符合招标要求。
- **大模型应用**：
    - 通过OCR识别文档关键信息，提取企业名称、资质等级、有效期等实体。
    - 与招标要求的资质标准进行语义匹配，标记不符合项。

### **2. 技术参数匹配**

- **任务内容**：检查投标文件中的技术方案、产品参数是否响应招标书的技术要求。
- **大模型应用**：
    - 对比招标技术参数与投标文件的描述，识别差异（如参数遗漏、数值不符）。
    - 使用语义相似度模型判断技术方案是否满足招标需求。

### **3. 报价分析与异常检测**

- **任务内容**：审核报价单的合理性，识别异常报价（如明显低于成本价）。
- **大模型应用**：
    - 提取报价数据，分析分项报价的逻辑性。
    - 结合历史数据或行业基准，预测合理报价范围并标记异常值。

### **4. 条款合规性检查**

- **任务内容**：审查合同条款、服务承诺等是否符合法律法规（如《招标投标法》）和招标文件要求。
- **大模型应用**：
    - 识别敏感条款（如排他性条款、霸王条款）。
    - 对比招标文件中的合同模板，检测条款偏离或遗漏。

### **5. 文档完整性核验**

- **任务内容**：确认投标文件是否包含所有必需材料（如授权书、保证金证明等）。
- **大模型应用**：
    - 根据招标清单生成文档完整性 checklist。
    - 通过文本分类或关键词提取判断材料是否齐全。
    
<img width="975" alt="截屏2025-03-01 17 10 56" src="https://github.com/user-attachments/assets/d252b94e-04d4-4de9-a522-0c8a28577ed6" />

系统架构：

后端 langchain + Django + faiss + deepseek api

前端 next.js + react + shadcn ui

