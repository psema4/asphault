# Asphault

A Hello, World repository to test [Concrete](https://github.com/ryankee/concrete) features.

## Usage

1. Fork the repo to your github account
1. `md ~/devel/`
1. `cd ~/devel/`
1. `git clone git@github.com:`{Your-Github-ID}`/asphault.git`
1. `git config --add concrete.runner "bash t/runner.sh"`
1. Edit/add `runner.sh` and tests under `t/`
1. `git commit -am "`{Your Message}`"`
1. `git push origin master`
1. Run the ci server, or daemonize it
 * `concrete .`
 * `nohup concrete -p 8080 ~/devel/asphault &`
1. Open a web browser to
 * http://localhost:4567
 * or if your specified a port number with -p, http://localhost:{Port}

## Requires

Sample git hooks require mail, see `git-hooks/README.md`
