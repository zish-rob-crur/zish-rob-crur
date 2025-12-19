<div align="center">

# The sunset is beautiful; farewell, sunset

<samp>
I prefer restraint and clarity.<br>
No noise. No over-explaining.<br>
Energy goes to what matters; boundaries stay with me.
</samp>


### `Default`

<kbd>Quiet, not weak</kbd> &nbsp; <kbd>Gentle, not pleasing</kbd>
<br>
<kbd>Slow to warm up, steady for the long run</kbd>
<br>
<kbd>Evidence-first, feelings acknowledged</kbd>
<br>
<kbd>Simple, durable, sustainable</kbd>


### `What I keep`

<kbd>Training and recovery</kbd> &nbsp; <kbd>A low-noise environment</kbd>
<br>
<kbd>Few, but good relationships</kbd> &nbsp; <kbd>Reusable personal “defaults”</kbd>
<br>
<kbd>Long-term thinking</kbd>


### `Taste`

> *Clean lines. White space. Minimal effort on display.*
> *Bright, not harsh. Sharp, not harmful.*


### `Toolbox`

</div>

```python
from pydantic import BaseModel


class zishRobCrur(BaseModel):
    temperament: tuple = ("Calm", "Reserved", "Clear boundaries", "Long-termism")
    taste: tuple = ("Clean", "Whitespace", "Low-noise", "Timeless")
    habits: tuple = ("Training", "Recovery", "Keep it simple")
    editors: tuple = ("VSCode", "Neovim")
    terminal: tuple = ("WezTerm", "oh-my-zsh", "tmux")
    themes: tuple = ("Flexoki Light", "Vscode Modern Light")


zishRobCrur = zishRobCrur()
print(zishRobCrur.model_dump_json(indent=4))
