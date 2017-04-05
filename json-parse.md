eval 不安全，有注入风险，
应该对数据用json2.js (www.json.org)解析，确保是json格式的数据
```
var itemDetails = JSON.parse(request.responseText);
```
