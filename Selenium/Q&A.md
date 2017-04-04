
## 'geckodriver' executable needs to be in PATH

**ERROR**: 

selenium.common.exceptions.WebDriverException: Message: 'geckodriver' executable needs to be in PATH

**SOLVED**:

1. selenium 3.x开始，webdriver/firefox/webdriver.py的`__init__`中，`executable_path="geckodriver"`；而2.x是`executable_path="wires"`
2. firefox 47以上版本，需要下载第三方driver，即geckodriver；在http://docs.seleniumhq.org/download/的Third Party Drivers, Bindings, and Plugins下面找到Mozilla GeckoDriver，下载到任意电脑任意目录，解压后将该路径加入到PC的path（针对windows）即可。

**LINK**:

https://www.zhihu.com/question/49568096