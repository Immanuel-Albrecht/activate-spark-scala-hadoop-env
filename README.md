## Setup

Extract your combination of choice of

 * a hadoop binary distribution (sub-dir should start with `hadoop`)
 * a spark binary distribution (probably without hadoop but with scala; sub-dir should start with `spark`)
 * a scala binary distributio (sub-dir should start with `scala`), and
 * a compatible jdk (probably openjdk8; sub-dir should start with `jdk`)

into a directory. Place `activate.env` in this directory. In a shell, run `source activate.env` in order to
setup PATH, CLASSPATH, and all the other environment variables in order to use the specified combination.
Now you may use `spark-shell`, `scala`, `hdfs`,... and all the other tools from your shell.

