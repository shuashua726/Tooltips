## URL编码与解码

``` python
# 编码
import urllib
url = 'http://test.com/s?wd=哈哈'
url = url.decode('gbk', 'replace')
print urllib.quote(url.encode('utf-8', 'replace'))

#结果: http%3a%2f%2ftest.com%2fs%3fwd%3d%e5%93%88%e5%93%88


# 解码
import urllib
encoded_url = 'http%3a%2f%2ftest.com%2fs%3fwd%3d%e5%93%88%e5%93%88'
print urllib.unquote(encoded_url).decode('utf-8', 'replace').encode('gbk', 'replace')
```
