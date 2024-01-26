```python
​
from pydantic import BaseModel


class zishRobCrur(BaseModel):
    languages: tuple = (
        "Python",
        "Go",
        "Javascript",
        "Typescript",
        "HTML",
        "CSS",
        "Vue",
    )
    databases: tuple = ("PostgreSQL", "Mongo", "Redis", "RabbitMQ", "MySQL")
    misc: tuple = ("Docker", "Celery")
    ongoing: tuple = ("Nothing",)
    editors: tuple = ("NeoVim", "VSCode", "PyCharm", "GoLand", "WebStorm")
    terminal: tuple = ("WezTerm", "oh-my-zsh", "tmux")
    themes: tuple = ("Flexoki Dark", "VsCode Dark+")


zishRobCrur = zishRobCrur()
print(
    zishRobCrur.model_dump_json(
        indent=4,
    )
)
​
```