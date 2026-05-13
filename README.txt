私人英语听写系统 - GitHub Pages 版

包含文件：
1. admin.html
   用于上传 txt 文稿和 mp3 音频，自动切分英文句子，手动标记每句 start/end 时间，并导出 dictation-data.js 或 JSON。

2. dictation.html
   私人听写练习页面。输入密码后进入，可以播放当前句子的音频片段、打字、检查答案、显示答案、下一句。

3. dictation-data.js
   示例数据文件。你用 admin.html 导出新数据后，用新的 dictation-data.js 替换它。

4. audio/
   放你的 mp3 音频文件。比如 audio/lesson1.mp3。

使用方法：
1. 把 admin.html、dictation.html、dictation-data.js、audio 文件夹上传到你现有 GitHub Pages 网站根目录。
2. 不要在 index.html 放入口，这样别人一般不知道页面地址。
3. 访问：
   https://你的用户名.github.io/你的仓库名/admin.html
   https://你的用户名.github.io/你的仓库名/dictation.html

修改密码：
打开 dictation.html，找到：
const PASSWORD = "123456";
把 123456 改成你自己的密码。

重要限制：
GitHub Pages 是静态网站。admin.html 里的上传只是在浏览器本地处理，不会自动永久保存到网站服务器。
你需要：
上传文稿和音频 → 标记时间 → 导出 dictation-data.js → 把新文件和 mp3 一起上传到 GitHub。
