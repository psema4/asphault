# Asphault

A Hello, World repository to test [Concrete](https://github.com/ryankee/concrete) features.

## Usage

Assuming an Ubuntu environment, this should get you up and running:

1. Fork this repo to your github account
1. `md ~/devel/`
1. `cd ~/devel/`
1. `git clone git@github.com:*{Your-Github-ID}*/asphault.git`
1. `cd asphault`
1. `git config --add concrete.runner "bash t/runner.sh"`
1. Edit/add `runner.sh` and tests under `t/`
1. `git commit -am "*{Your Message}*"`
1. `git push origin master`
1. Run the ci server, or daemonize it
 * `concrete .`
 * `nohup concrete -p 8080 ~/devel/asphault &`
1. Open a web browser to
 * http://localhost:4567
 * or if your specified a port number with -p, http://localhost:{Port}

## Scheduling builds

1. Run concrete as a daemon
1. Add a cron entry to build sometime through the night (3AM, replace port number if necessary):
    `0 3 * * * curl -d "" http://localhost:4567`

## Requires

In addition to concrete and it's requirements (node + npm), the sample git hooks require the `mail` tool - see `git-hooks/README.md`
