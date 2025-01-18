# The Install of Batfish on Linux

1. install maven 3.6.1

2. install jdk17

3. install vpn [v2ray](./v2ray.md)
When the dns has the problem, we could reset dns as the following.
```
sudo systemctl restart NetworkManager
```

4. git clone 
```
$ git config --global http.version HTTP/1.1

$ https://github.com/batfish/batfish.git
```

5. install [bazel](https://github.com/batfish/batfish/blob/master/docs/building_and_running/README.md)

Note that, we first install the bazelisk, which the manager tools of bazel. But bazelisk installing bazel, needs the vpn.

```
$ export GODEBUG="http2client=0"
```

6. install [idea environment](https://github.com/batfish/batfish/wiki/IntelliJ-setup-for-developers)

7. install [pybatfish](https://github.com/batfish/pybatfish)
```
https://github.com/batfish/pybatfish.git
```