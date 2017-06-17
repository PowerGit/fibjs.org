# 模块 encoding
编码与解码模块，用于处理不同的数据编码格式与二进制之间的转换

引用方式：
```JavaScript
var encoding = require('encoding');
```
## 对象
        
### base32
base32 编码与解码模块
```JavaScript
base32 encoding.base32;
```

### base64
base64 编码与解码模块
```JavaScript
base64 encoding.base64;
```

### base64vlq
base64vlq 编码与解码模块
```JavaScript
base64vlq encoding.base64vlq;
```

### hex
hex 编码与解码模块
```JavaScript
hex encoding.hex;
```

### iconv
iconv 编码与解码模块
```JavaScript
iconv encoding.iconv;
```

### json
json 编码与解码模块
```JavaScript
json encoding.json;
```

### bson
bson 编码与解码模块
```JavaScript
bson encoding.bson;
```

## 函数
        
### jsstr
将字符串编码为 javascript 转义字符串，用以在 javascript 代码中包含文本
```JavaScript
static String encoding.jsstr(String str,
                Boolean json = false);
```

调用参数:
* str - 要编码的字符串
* json - 是否生成json兼容字符串

返回结果:
* 返回编码的字符串

### encodeURI
url 字符串安全编码
```JavaScript
static String encoding.encodeURI(String url);
```

调用参数:
* url - 要编码的 url

返回结果:
* 返回编码的字符串

### encodeURIComponent
url 部件字符串安全编码
```JavaScript
static String encoding.encodeURIComponent(String url);
```

调用参数:
* url - 要编码的 url

返回结果:
* 返回编码的字符串

### decodeURI
url 安全字符串解码
```JavaScript
static String encoding.decodeURI(String url);
```

调用参数:
* url - 要解码的 url

返回结果:
* 返回解码的字符串
