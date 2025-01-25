# QuickAccess

## 项目介绍

这个项目是一个简单的网页应用，旨在帮助用户快速访问不同的环境地址。用户可以通过输入搜索内容，直接跳转到指定的搜索引擎结果页面。同时，用户可以查看和访问配置文件中定义的不同环境地址。

### 主要功能：
- **搜索功能**: 用户可以在搜索框中输入内容，按下 Enter 键后，应用会在新标签页中打开指定搜索引擎的搜索结果。
- **环境地址访问**: 用户可以查看配置文件中定义的不同环境地址，并通过点击环境配置块直接跳转到相应的地址。

## 如何使用？

1. **配置文件**:
   - 在项目目录下，确保存在一个名为 `config.txt` 的文件。该文件应包含以下格式的内容：
     ```
     search=https://www.baidu.com/
     [百度]
     dev=https://www.baidu1.com
     test=https://www.baidu-dev.com
     env1=https://www.example1.com
     env2=https://www.example2.com
     env3=https://www.example3.com

     [谷歌]
     dev=https://www.google123.com
     test=https://www.google-dev.com

     [BING]
     dev=https://www.bing.com
     test=https://www.bing-dev.com
     pre=https://www.bing-pre.com
     ```

2. **使用 Python 打开应用**:
   - 在项目目录下，打开终端或命令提示符，运行以下命令：
     ```
     python -m http.server 8000
     ```
   - 然后在浏览器中打开以下地址：
     ```
     http://localhost:8000/index.html
     ```

3. **使用搜索功能**:
   - 在搜索框中输入你想要搜索的内容，然后按下 Enter 键。应用会在新标签页中打开指定搜索引擎的搜索结果。

4. **访问环境地址**:
   - 点击弹窗中显示的环境配置块，应用会在新标签页中打开对应的环境地址。

## 注意事项
- 确保浏览器允许弹出窗口，以便正常使用搜索功能和环境地址访问。
- 配置文件中的 URL 必须是有效的，以确保能够成功跳转。

希望这个项目能帮助你更高效地访问所需的网页！
