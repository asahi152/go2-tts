# go2文字转语音

## 功能特点

可以将用户输入的文本转化为语音并且播放。

## 环境要求

- Python 3.x
- 操作系统 Ubuntu20.04
- 相关库：
  - `websocket-client` - 用于 WebSocket 连接
  - `pydub` - 用于音频处理
  - `unitree_sdk2py` - Unitree 机器人 SDK

## 安装依赖

手动安装以下依赖库：

```bash
pip install websocket-client pydub 
```
## 使用方法

1. **克隆仓库**

   ```bash
   git clone https://github.com/asahi152/go2-tts.git
   cd go2-tts
   ```
2. **运行程序**

   执行主程序：

   ```bash
   python3 tts.py <网络接口名>
   ```

   本程序调用API生成的文件格式为pcm并保存在工程文件夹中，代码中将其转换为wav格式进行播放。在提示符后输入想要转化为语音的文本并按下回车即可。
