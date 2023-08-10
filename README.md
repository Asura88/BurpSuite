<p align="center"><img src="https://portswigger.net/burp/communitydownload/images/burp-pro-logo.svg" alt="Burp Suite Professional logo" width="360" height="260"></p>

<h1 align="center">Welcome to Burp Suite loader👋</h1>

<div align="center">
  <!-- Platform -->
  <a href="Platform">
    <img src="https://img.shields.io/badge/Platform-Windows%E3%80%81Linux%E3%80%81macOS-green?color=gerrn&style=flat-square" alt="Platform">
  </a>
  <!-- License -->
  <a href="LICENSE">
    <img src="https://img.shields.io/github/license/x-Ai/BurpSuite?color=gerrn&style=flat-square" alt="LICENSE">
  </a>
  <!-- ❤︎ -->
  <a href="❤︎">
    <img src="https://img.shields.io/badge/❤︎-致敬永远好奇的心-green?color=gerrn&style=flat-square" alt="❤︎">
  </a>
</div>
<br>
<div align="center">
  ⚡️Burp Suite Professional 2023.*.* Loader已更新，祝玩的愉快...⚡️<br><br>
  商业使用请购买正版软件 - https://portswigger.net/buy/pro<br>
  ！<a href="https://github.com/x-Ai/BurpSuiteLoader">旧项目</a>已被PortSwigger投诉导致DMCA ！*未混淆，请自行围观jar包*
</div>

#### **<p align="center">✨如果本项目对您有帮助，点一下Star吧🥰✨</p>**


<h1 align="center"></h1>
<br><p align="center">时隔两年再次建立此项目是因为看到了SCZ师傅的<a href="https://mp.weixin.qq.com/s/4KXxKdnPeWqsEsylObhg8w">公众号文章</a>，想了想还是写一篇更加详细的文档来帮助需要的同学</p>
<h1 align="center"></h1>


### BurpSuitePro 下载地址

&ensp;&ensp;&ensp;&ensp;https://portswigger.net/burp/releases

### Loader

&ensp;&ensp;&ensp;&ensp;<a href="https://raw.githubusercontent.com/x-Ai/BurpSuite/main/BurpSuiteLoader.jar">BurpSuiteLoader.jar(5.93KB)</a>
- SHA256: 23499F88ED11FA69E6A9BF5B17594B326EF71C631D28DA804F02C3EF08C68150
- MD5: 694738870DB8D69A6F1BEB6D05CD0999

### Windows 启动器源码
&ensp;&ensp;&ensp;&ensp;<a href="https://raw.githubusercontent.com/x-Ai/BurpSuite/main/BurpSuiteLoadSources.zip">BurpSuiteLoadSources.zip(19.3KB)</a>
- SHA256: BDF5FAC98B8709532E721A75A6EFD491BFC54E09739436119BDBFCBCA12A82B5
- MD5: 91231D19E6EB35CCA959252EF01ECEA9

## 🚀 使用方式

<div align="center">
  <sub>！强烈建议下载安装包进行安装后使用 ！</sub>
</div>

### 命令行
> java -noverify -Dsun.java2d.d3d=false -Dsun.java2d.noddraw=true --add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED --add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED -javaagent:BurpSuiteLoader.jar  -jar burpsuite_pro.jar
### Windows
1. 下载：https://portswigger-cdn.net/burp/releases/download?product=pro&version=2022.3.1&type=WindowsX64
2. 放置进安装目录

<p align="center"><img src="/static/Launch.png" alt="Burp启动器"></p>
&ensp;&ensp;&ensp;&ensp;<a href="https://raw.githubusercontent.com/x-Ai/BurpSuite/main/BurpSuite.zip">BurpSuite.zip(9.15KB)</a>

- SHA256: 897AD7E16EC063EEAFAB9AEF4913851474B70594C0252354B2E69A09CA74C809
- MD5: 9C02C757FBE0163B54A7633D0BB91226

&ensp;&ensp;3. 使用编译好的启动器

### macOS

<br><p align="center">！全新安装后启动一次，防止出现 "安装包损坏" 问题 ！</p>

1. 下载macOS (Intel/M1)
2. 放置Loader至如下路径
> /Applications/Burp Suite Professional.app/Contents/Resources/app
<p align="center"><img src="https://github.com/x-Ai/BurpSuite/assets/5061489/aabbd918-e8d9-4b72-a572-54a61e560584" alt="macOSLoader路径"></p>



&ensp;&ensp;3. 修改如下路径文件内容

> /Applications/Burp Suite Professional.app/Contents/Info.plist
<p align="center"><img src="https://github.com/x-Ai/BurpSuite/assets/5061489/f6558e04-6667-453b-bebe-9e660dc29b42" alt="Info.plist路径"></p>


&ensp;&ensp;4. 修改Info.plist文件，`<string>-Dexe4j.moduleName=$APP_PACKAGE</string>` 后插入如下语句

```
......
<string>-noverify</string>
<string>--add-opens</string>
<string>java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED</string>
<string>--add-opens</string>
<string>java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED</string>
<string>-javaagent:$APP_PACKAGE/Contents/Resources/app/BurpSuiteLoader.jar</string>
```
<p align="center"><img src="https://github.com/x-Ai/BurpSuite/assets/5061489/29dc2e12-f815-4d18-8128-e37674d0c393" alt="Info.plist内容"></p>

&ensp;&ensp;5. 使用启动台中的BurpSuite快捷方式
## 💻展示

<p align="center"><img src="/static/Main.png" alt="BurpSuitePro"></p>


## 📝讨论

如果您在使用过程中存在疑问或更好的建议，可以提出 [issue](https://github.com/x-Ai/BurpSuite/issues)。

## ❤️致谢

- **surferxyz** && **scz** 二位大拿
- <a href="https://github.com/Hywell">Hywell</a> 
