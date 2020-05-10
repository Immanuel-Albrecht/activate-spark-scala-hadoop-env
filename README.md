# Requirements

This script requires `realpath` to be available from the command line. If your os/distribution does not come
with this command, you might want to install the corresponding package. (Some distros have it as `realpath` package, some provide it in `coreutils` or `gnu-coreutils`.)

## Setup

Extract your combination of choice of

 * a hadoop binary distribution (sub-dir should start with `hadoop`)
 * a spark binary distribution (probably without hadoop but with scala; sub-dir should start with `spark`)
 * a scala binary distributio (sub-dir should start with `scala`), and
 * a compatible jdk (probably openjdk8; sub-dir should start with `jdk`)

into a directory. Place `activate.env` in this directory. In a shell, run `source activate.env` in order to
setup PATH, CLASSPATH, and all the other environment variables in order to use the specified combination.
Now you may use `spark-shell`, `scala`, `hdfs`,... and all the other tools from your shell.

## Note for macOS

* You need to install a package that provides `realpath`. If you use homebrew, this can be done via `brew install coreutils`.
* If you download openjdk8, choose the .tar.gz-archive option. After extracting the archive, move all files and folders from the `Contents/Home` sub-subdirectory to the jdk subdirectory. (`mv jdk*/Contents/Home/* jdk*`).
