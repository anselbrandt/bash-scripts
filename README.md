# bash-scripts

### Execute Scala scripts without file extension

E.g. `s script` will run `scala script.scala`. Any args will also be passed.

`s`
```
#!/bin/bash
scala $1.scala ${@:2}
```

` ${@:2}` will pass any args to your script.

Make sure to `chmod +x s` and that `export PATH=$PATH:$HOME/bin` is in your bash profile and sourced.
