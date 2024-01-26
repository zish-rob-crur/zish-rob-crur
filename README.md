```python
​
import json
from dataclasses import asdict, dataclass

@dataclass
class Stack:
    languages   : tuple = ("Python","Go","Javascript","Typescript","HTML","CSS",)
    databases   : tuple = ("PostgreSQL", "Mongo", "Redis","Elasticsearch","RabbitMQ",)
    misc        : tuple = ("Docker", "Celery",)
    ongoing     : tuple = ("Vue","Golang",)

    def serialize(self):
        return json.dumps(asdict(self), indent=4)


stack = Stack()
print(stack.serialize())
​
```

