# bash-scripts

`s`
```
#!/bin/bash
scala $1.scala ${@:2}
```

` ${@:2}` will pass any args to your script.

Make sure to `chmod +x s` and that `export PATH=$PATH:$HOME/bin` is in your bash profile and sourced.
