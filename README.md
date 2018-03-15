# zuora_restful_python
A python class for accessing the Zuora API via REST

# install
```
pip install  git+https://github.com/procore/zuora_restful_python.git
 -- or --
pip install --upgrade git+https://github.com/procore/zuora_restful_python
```

# sample use

```
import sys
from zuora_restful_python.zuora import Zuora

(username, password) = sys.argv[1:3]
zuora = Zuora(username, password)

for record in zuora.query_all('select Name from Account'):
    print(record['Name'])
```

## References

* [Zuora Developer Center](https://www.zuora.com/developer/)

## Note

if you are looking for the command line tool zoql, it has moved to https://github.com/bolaurent/python-cmdline-zoql.
