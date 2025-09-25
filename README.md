# Sync Source:-

```bash
repo init -u https://github.com/Superior13-NEXT/manifest.git -b QPR3
```

```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

# Start the build:-

```bash
. build/envsetup.sh
```

```bash
lunch superior_<devicecodename>-userdebug
```

```bash
m bacon -j$(nproc --all)
```
