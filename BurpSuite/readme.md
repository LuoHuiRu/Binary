# Windows

1. 将BurpLoaderKeygen.jar、burpsuite_pro_v20**.*.jar 放到同一目录下
2. java -jar BurpLoaderKeygen.jar
3. 点击 `Run`，输入许可证选择 【手动激活】
4. 激活后勾选 `Auto Run`,打开BurpLoaderKeygen.jar即可自动启动BurpSuite

# MacOS

1. 安装BurpSuite
2. 将BurpLoaderKeygen.jar放到`/Applications/Burp Suite Professional.app/Contents/Resources/app`目录下
3. 进入app目录，执行命令
  ```bash
  "/Applications/Burp Suite Professional.app/Contents/Resources/jre.bundle/Contents/Home/bin/java" -jar BurpLoaderKeygen.jar
  ```
  点击[Run]启动BurpSuite,激活后关闭注册机
4. 修改`/Applications/Burp Suite Professional.app/Contents/vmoptions.txt`,增加以下参数
  ```txt
  --add-opens=java.base/java.lang=ALL-UNNAMED
  --add-opens=java.base/java.lang=ALL-UNNAMED
  --add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED
  --add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED
  --add-opens=java.base/jdk.internal.org.objectweb.asm.Opcodes=ALL-UNNAMED
  -javaagent:BurpLoaderKeygen.jar
  -noverify
  ```
5. 如果出现“已损坏，无法打开”的错误，运行以下命令
  ```bash
  sudo xattr -r -d com.apple.quarantine /Applications/Burp\ Suite\ Professional.app
  ```