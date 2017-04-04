## timestamp与datetime互转

```pyton
import time
import datetime

ts = time.time()
time = datetime.datetime.fromtimestamp(ts)

dt = datetime.datetime.now()
ts = time.mktime(dt.timetuple())

```
