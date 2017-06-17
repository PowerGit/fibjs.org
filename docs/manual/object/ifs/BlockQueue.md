# 对象 BlockQueue
阻塞 FIFO（先进先出）队列对象

用以创建和管理阻塞先进先出数据队列，创建方法：
```JavaScript
var coroutine = require("coroutine");
var q = new coroutine.BlockQueue(100);
```
## 构造函数
        
### BlockQueue
队列对象构造函数
```JavaScript
 new BlockQueue(Integer size);
```

调用参数:
* size - 指定队列尺寸

## 函数
        
### put
插入一个新的元素到队列，成功返回 True，队列满则等待
```JavaScript
BlockQueue.put(Value e);
```

调用参数:
* e - 要插入的元素

### take
从队列中移除一个元素并返回，如果队列为空则等待
```JavaScript
Value BlockQueue.take();
```

返回结果:
* 返回取出的元素

### add
插入一个新的元素到队列，成功返回 True，队列满则抛出错误
```JavaScript
Boolean BlockQueue.add(Value e);
```

调用参数:
* e - 要插入的元素

返回结果:
* 成功返回 True

### offer
插入一个新的元素到队列，成功返回 True，队列满则返回 False
```JavaScript
Boolean BlockQueue.offer(Value e);
```

调用参数:
* e - 要插入的元素

返回结果:
* 成功返回 True

### remove
从队列中移除一个元素并返回，如果队列为空则抛出错误
```JavaScript
Value BlockQueue.remove();
```

返回结果:
* 返回取出的元素

### poll
从队列中移除一个元素并返回
```JavaScript
Value BlockQueue.poll();
```

返回结果:
* 返回取出的元素，队列为空则返回 Null

### element
从队列中返回一个元素，但不移除，队列为空则抛出错误
```JavaScript
Value BlockQueue.element();
```

返回结果:
* 返回取出的元素

### peek
从队列中返回一个元素，但不移除
```JavaScript
Value BlockQueue.peek();
```

返回结果:
* 返回取出的元素，队列为空则返回 Null

### clear
清除当前队列
```JavaScript
BlockQueue.clear();
```

### toArray
返回队列的 js 数组
```JavaScript
Array BlockQueue.toArray();
```

返回结果:
* 包含数据的 js 数组

### dispose
强制回收对象，调用此方法后，对象资源将立即释放
```JavaScript
BlockQueue.dispose();
```

### equals
比较当前对象与给定的对象是否相等
```JavaScript
Boolean BlockQueue.equals(object expected);
```

调用参数:
* expected - 制定比较的目标对象

返回结果:
* 返回对象比较的结果

### toString
返回对象的字符串表示，一般返回 &#34;[Native Object]&#34;，对象可以根据自己的特性重新实现
```JavaScript
String BlockQueue.toString();
```

返回结果:
* 返回对象的字符串表示

### toJSON
返回对象的 JSON 格式表示，一般返回对象定义的可读属性集合
```JavaScript
Value BlockQueue.toJSON(String key = "");
```

调用参数:
* key - 未使用

返回结果:
* 返回包含可 JSON 序列化的值

### valueOf
返回对象本身的数值
```JavaScript
Value BlockQueue.valueOf();
```

返回结果:
* 返回对象本身的数值

## 属性
        
### length
返回当前队列尺寸
```JavaScript
readonly Integer BlockQueue.length;
```
