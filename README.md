```

Shell 的使用
使用转义字符使命令行字符高亮
例如 '[\033[1;33m%s\033[0;0m@%s \033[1;36m%s\033[0;0m] $ ' 这串转义字符实现的效果如下：

__init__.py

from .cd import cd
from .exit import exit
from .getenv import getenv
from .history import history
from .constants import *
最后为了方便调用，我们将该目录下所有模块都导入到了 __init__.py 文件之中。


# 使用 os.path.expanduser('~') 获取当前操作系统平台的当前用户根目录
HISTORY_PATH = os.path.expanduser('~') + os.sep + '.shell_history'


Python 官方文档
https://docs.python.org/3/

```