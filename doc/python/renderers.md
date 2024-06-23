import matplotlib.pyplot as plt

# 用户建议内容及数量
suggestions = {
    "用户界面优化": 2,
    "智能报警逻辑优化": 3,
    "智能场景设置": 1,
    "用户反馈机制": 2,
    "设备兼容性增强": 2,
    "安全加固措施": 2,
    "智能语音交互优化": 2,
    "定期固件更新": 2
}

# 提取建议内容和数量
suggestion_labels = list(suggestions.keys())
suggestion_counts = list(suggestions.values())

# 绘制柱状图
plt.figure(figsize=(10, 6))
plt.barh(suggestion_labels, suggestion_counts, color='skyblue')
plt.xlabel('建议数量')
plt.ylabel('建议内容')
plt.title('智能家居系统功能优化建议数量')
plt.gca().invert_yaxis()  # 使y轴反向，让建议内容从上到下显示
plt.show()
