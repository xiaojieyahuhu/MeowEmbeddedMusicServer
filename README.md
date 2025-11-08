# Meow 为嵌入式设备制作的音乐串流服务
[English](README.md) | [简体中文](README_zh-CN.md)

MeowEmbeddedMusicServer 是一个为嵌入式设备制作的音乐串流服务。
它可以播放来自你的服务器的音乐，也可以为你的嵌入式设备提供音乐流媒体服务。
它还可以管理音乐库，并且可以搜索和下载音乐。

## 特性
- 🎵 在线听音乐
- 📱 为嵌入式设备提供音乐串流服务
- 📚 管理音乐库
- 🔍 搜索和缓存音乐
- ⬇️ 支持直接下载音频文件
- 🎼 自动获取歌词和封面
- 💾 智能缓存机制

## 最新更新

### ✨ 新增功能
- **音频直接下载**: 支持通过 `url=true` 参数直接下载音频文件
- **静态文件服务**: 支持通过 HTTP 访问缓存的音乐、封面、歌词文件
- **自动文件命名**: 下载的音频文件自动命名为"歌手名 - 歌曲名.mp3"格式

### 🐛 修复问题
- 修复了静态资源访问404的问题
- 修复了文件路径不一致的问题
- 统一了资源URL路径前缀为 `/files/`
- 完善了依赖管理，添加了 `go.sum` 文件

## 快速开始

### 1. 配置音乐源
确保 `sources.json` 文件已正确配置

### 2. 运行服务器
```bash
./app
```

### 3. 使用API
- **搜索并获取音乐信息**:
  ```
  http://localhost:2233/stream_pcm?song=歌曲名&singer=歌手名
  ```
- **直接下载音频文件**:
  ```
  http://localhost:2233/stream_pcm?song=歌曲名&singer=歌手名&url=true
  ```

## 技术特点
- 基于 Go 语言开发，性能优异
- 支持多个音乐源接入（酷我、网易云、咪咕、百度等）
- 自动缓存机制，减少重复请求
- RESTful API 设计，易于集成

# 教程文档
请参阅 [维基](https://github.com/IntelligentlyEverything/MeowEmbeddedMusicServer/wiki).


## Star 历史

<a href="https://star-history.com/#IntelligentlyEverything/MeowEmbeddedMusicServer&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=IntelligentlyEverything/MeowEmbeddedMusicServer&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=IntelligentlyEverything/MeowEmbeddedMusicServer&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=IntelligentlyEverything/MeowEmbeddedMusicServer&type=Date" />
 </picture>
</a>