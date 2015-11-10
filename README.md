ServalHelper README

ServalHelper is a helperscript written in Python to support new users with their first serval steps. It provides help for downloading and building serval.

First the usage:

```
usage: ServalHelper [-h] [-c | -d | -w | -r] [-m interface | -a interface] [-p PATH]

Serval Helper Script

optional arguments:
  -h, --help                        show this help message and exit
  -c, --check                       check if all requirements are met
  -d, --download                    download Serval from Github
  -w, --wipe                        wipe all data in Rhizome Store
  -r, --remove                      remove every occurrence of Serval
  -m interface, --make interface    make Serval
  -a interface, --all interface     check and make in one go
  -p PATH, --path PATH              install path

  ```

  With the `-c` option you can Check all Dependencies for serval. Note: it only checks the dependencies you absolutely need. But there is a configure, which checks more dependencies.

  With the `-d` option serval will be downloaded per default to your home directory from GitHub.

  With the `-m` interface option serval will be build and all configurations and required folders are per default created in $HOME/serval-conf/. The interface is the networkinterface where serval will communicate with other serval clients.

  With the `-a` interface is the same as `-c` `-d` and `-m` interface.

  The `-w` option wipes your Rhizome store. But be careful. If you really want to wipe everything from Rhizome, you have to stop your serval and all other serval clients in the network otherwise your serval will immediately be a mess again.

  Finally there is the `-r` option, which will remove every occurrence of serval on your machine.

  You can change the installationpath with the `-p` option. It has to be a absolute path. If not, ServalHelper will change it to an absolute path.

  If you have questions or you find a bug please contact me: Sterz@students.uni-marburg.de
