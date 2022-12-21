## 安装
```
npm install hui-day
```

## 导入
```js
const huiDay = require('hui-day');
```

## 格式化时间

```js
// 调用 dateFormat 对时间进行格式化
const dtStr = huiDay.dateFormat(new Date());
// 返回结果 2022-12-21 21:16:44
console.log(dtStr);
```

## 转义 HTML 中的特殊字符
```js
// 带转换的 HTML 字符串
const html = '<h1 title="abc">这是h1标签<span>123&nbsp;</span></h1>';
// 调用 htmlEscape 方法进行转换
const str = huiDay.htmlEscape(html);
//结果 &lt;h1 title=&quot;abc&quot;&gt;这是h1标签&lt;span&gt;123&amp;nbsp;&lt;/span&gt;&lt;/h1&gt;
console.log(str);
```

## 还原 HTML 中的特殊字符
```js
// 调用 htmlUnEscape 方法进行还原
const str2 = huiDay.htmlUnEscape(str);
// 输出结果 <h1 title="abc">这是h1标签<span>123&nbsp;</span></h1>
console.log(str2);
```

## 开源协议
ISC