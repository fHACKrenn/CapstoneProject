# Vainglory draft simulator with WebSocket

Make sure you install requirements before you use/run the application by doing
```
pip install -r requirements.txt
```
in terminal/console

## MutableMapping error
If you encounter MutableMapping import error from collections,
### For python version 3.10 or above
```
from collections.abc import MutableMapping
```
### For python version 3.9 or lower
```
from collections import MutableMapping
```
