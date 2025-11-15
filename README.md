# Yukkuri-audition

- 通过 Python 中的 selenium 库实现自动化批量生成**油库里**语音

- 源码为 main.py 文件，其运行需要 Chrome 浏览器和驱动器 ChromeDriver，放在项目里了

- Yukkuri_transformer.exe 是打包后的文件，点击可直接运行

# 使用方法

1. 首先需要电脑里面有 Chrome 浏览器，最好是最新版的

2. 将想要转化成语音的文字用 .txt 文件保存，两句不同的话用换行分开

3. 双击 Yukkuri_transformer.exe 文件，会跳出交互界面，将文本地址输入第一个框，下载地址输入第二个框

4. 点击“开始转化”，程序开始运行

5. 结束后，程序会在下载地址上创建一个叫做 Yukkuri_aud 的文件夹，其中保存了所有的语音

# 存在的问题

本地的 Chrome 浏览器版本和 repo 提供的 ChromeDriver 驱动版本可能出现不兼容，导致无法正常启动浏览器会话，需要手动下载对应版本的 ChromeDriver

具体步骤：

1. 在 Chrome 浏览器中打开 chrome://settings/help，确认版本号，比如 `142.0.7444.163`，版本号就是第一位数 `142`
2. 访问 [Chrome for Testing availability](https://googlechromelabs.github.io/chrome-for-testing/) ，根据你使用的操作系统，下载对应版本的 ChromeDriver
3. 将下载的新版 chromedriver.exe 替换掉 repo 中的 chromedriver.exe
4. 再次打开 Yukkuri_transformer.exe 即可

