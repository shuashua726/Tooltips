
## 'geckodriver' executable needs to be in PATH

**ERROR**: 

selenium.common.exceptions.WebDriverException: Message: 'geckodriver' executable needs to be in PATH

**SOLVED**:

1. selenium 3.x��ʼ��webdriver/firefox/webdriver.py��`__init__`�У�`executable_path="geckodriver"`����2.x��`executable_path="wires"`
2. firefox 47���ϰ汾����Ҫ���ص�����driver����geckodriver����http://docs.seleniumhq.org/download/��Third Party Drivers, Bindings, and Plugins�����ҵ�Mozilla GeckoDriver�����ص������������Ŀ¼����ѹ�󽫸�·�����뵽PC��path�����windows�����ɡ�

**LINK**:

https://www.zhihu.com/question/49568096