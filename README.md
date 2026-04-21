# Interview Assistant Skill

面试助手 Claude Code Skill，帮助用户高效备战面试。

## 功能特性

- **简历与JD匹配** - 深入挖掘简历亮点，匹配岗位需求
- **面经搜索** - 联网搜索最新面试经验（必须联网！）
- **自我介绍定制** - 根据简历和JD定制化设计
- **问题模拟** - 基于真实面经生成面试问题
- **两种模式** - 模拟面试模式 / 知识库备考模式

## 安装使用

### 方式一：本地 Skills 目录

1. 克隆此仓库
2. 将 `skills/interview-assistant` 文件夹复制到你的 Claude Code 本地 skills 目录
3. 在 `settings.json` 中添加配置：

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

### 方式二：分享给朋友

直接将 `skills/interview-assistant` 文件夹分享即可。

## 使用前提

- Claude Code 中已开启 WebSearch 权限（用于搜索最新面经）

## 使用示例

```
用户: 我要面试腾讯产品经理岗位
助手: 好的！请上传你的简历和目标岗位的JD，我来帮你准备。
```

## 项目结构

```
interviw_assistant_skill/
├── README.md
├── skills/
│   └── interview-assistant/
│       └── SKILL.md          # 核心skill文件
└── .gitignore
```

## License

MIT
