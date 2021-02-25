# bash-scripts

### Execute Scala scripts leaving off file extension, eg `s script` will run `scala script.scala`

`s`
```
#!/bin/bash
scala $1.scala ${@:2}
```

` ${@:2}` will pass any args to your script.

Make sure to `chmod +x s` and that `export PATH=$PATH:$HOME/bin` is in your bash profile and sourced.
