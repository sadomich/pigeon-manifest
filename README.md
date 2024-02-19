# PigeonOS Repo Manifest

## Download the 'repo' utility:

```shell
$ curl http://commondatastorage.googleapis.com/git-repo-downloads/repo sudo | tee /usr/bin/repo > /dev/null
$ sudo chmod a+x /usr/bin/repo
```

## Fetch Pigeon Project Manifest:

Make sure the git is set up properly:
```shell
git config --global user.name "Your Name"
git config --global user.email "Your Email"
```

To store git account credential use:
```shell
git config --global credential.helper store
```

Create new folder for the project <project folder>, and navigate to it.
Fetch the project manifest:
```shell
$ repo init -u https://github.com/sadomich/pigeon-manifest.git -b <branch>
```

## Download/Update the project sources:
```shell
$ repo sync --no-clone-bundle
```
