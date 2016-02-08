# XXTEA 加密算法的 ActionScript 3 实现

<a href="https://github.com/xxtea/">
    <img src="https://avatars1.githubusercontent.com/u/6683159?v=3&s=86" alt="XXTEA logo" title="XXTEA" align="right" />
</a>

## 简介

XXTEA 是一个快速安全的加密算法。本项目是 XXTEA 加密算法的 HTML5 实现。

它不同于原始的 XXTEA 加密算法。它是针对 ByteArray(String) 类型数据进行加密的，而不是针对 int 或 uint 数组。同样，密钥也是 ByteArray(String) 类型。

## 使用

```actionscript
import org.xxtea.XXTEA;

var str:String = "Hello World! 你好，中国🇨🇳！";
var key:String = "1234567890";
var encrypt_data:String = XXTEA.encryptToString(str, key);
trace(encrypt_data);
var decrypt_data:String = XXTEA.decryptToString(encrypt_data, key);
trace(str == decrypt_data);
```
