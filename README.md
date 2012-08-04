Simple test repository for [Concrete](https://github.com/ryankee/concrete).

Usage:

1. Fork the repo to your github account
2. `md ~/devel/`
3. `cd ~/devel/`
4. `git clone git://github.com/`{Your-Github-ID}`/asphault.git`
5. Edit/add `runner.sh` and tests under `t/`
6. Run concrete server: `concrete .`
7. Daemonize on port 8080: `nohup concrete -p 8080 ~/devel/asphault &`
