# Issues

## CLI docker command missing:

Installed Docker desktop on the M1 Mac Big Sur, the GUI runs smoothly without any issues after providing permissions

However the terminal was not able to find the docker commands be it `docker` or `docker-compose`

### Fix

- Open terminal and find out what is your `$HOME` path

```sh
echo $HOME
```

```sh
sudo vim /etc/paths
```

- Add `<<$HOME>>/.docker/run` to the end of the file
- Save and quit the file

Now on restarting the terminal you should be able to access the `docker` and `docker-compose` commands.

---
