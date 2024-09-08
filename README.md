# #Kernel_gki_android12-9 #

##### Create a directory #####
```bash
 mkdir -p ~/gki_android12-9
 cd ~/gki_android12-9

```

##### Sync #####
##### Initialize local repository #####
```bash
repo init -u https://github.com/DVWorkspaces/kernel_gki_android12-9 -b main
```

##### Sync #####
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

##### Build #####
```bash
BUILD_CONFIG=common/build.config.gki.aarch64 build/build.sh
```
