# XXTEA for ActionScript 3

<a href="https://github.com/xxtea/">
    <img src="https://avatars1.githubusercontent.com/u/6683159?v=3&s=86" alt="XXTEA logo" title="XXTEA" align="right" />
</a>

## Introduction

XXTEA is a fast and secure encryption algorithm. This is a XXTEA library for ActionScript 3.

It is different from the original XXTEA encryption algorithm. It encrypts and decrypts ByteArray(String) instead of int or uint Array, and the key is also ByteArray(String).

## Usage

```actionscript
import org.xxtea.XXTEA;

var str:String = "Hello World! 你好，中国🇨🇳！";
var key:String = "1234567890";
var encrypt_data:String = XXTEA.encryptToString(str, key);
trace(encrypt_data);
var decrypt_data:String = XXTEA.decryptToString(encrypt_data, key);
trace(str == decrypt_data);
```
