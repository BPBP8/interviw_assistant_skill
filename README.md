# Interview Assistant - 面试助手

一个通用的AI面试准备助手提示词，适用于各种AI助手（Claude, GPT, Gemini等）。

## 功能特性

- **简历与JD匹配** - 深入挖掘简历亮点，匹配岗位需求
- **面经搜索** - 联网搜索最新面试经验（必须联网！）
- **自我介绍定制** - 根据简历和JD定制化设计
- **问题模拟** - 基于真实面经生成面试问题
- **两种模式** - 模拟面试模式 / 知识库备考模式

## 快速开始

### 在Claude Code中使用

1. 将 `skills/interview-assistant/SKILL.md` 内容复制到Claude Code的skill配置中
2. 或者配置本地skills目录：

```json
{
  "extraKnownMarketplaces": {
    "local-skills": {
      "source": {
        "source": "directory",
        "path": "你的skills路径"
      }
    }
  }
}
```

### 在其他AI助手使用

将 `skills/interview-assistant/SKILL.md` 中的内容作为系统提示词或开场白发送给AI即可。

## 工作流程

1. **收集信息** - 接收用户简历和目标岗位JD
2. **简历分析** - 挖掘简历亮点，输出亮点报告
3. **联网搜面经** - 搜索该岗位/公司的最新面试经验
4. **自我介绍** - 定制1-2分钟自我介绍稿
5. **模拟面试** - 选择模式进行面试练习
6. **复盘改进** - 总结表现，提供提升建议

## 项目结构

```
interviw_assistant_skill/
├── README.md
├── .gitignore
└── skills/
    └── interview-assistant/
        └── SKILL.md          # 面试助手提示词
```

## 使用前提

- AI助手需要具备联网搜索能力（用于搜索最新面经）
- 如果AI不支持联网，仍可使用通用面试题库进行准备

## License

MIT
