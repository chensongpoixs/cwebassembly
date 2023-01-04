# 安装emscripten


## 1、下载

```
# Get the emsdk repo
git clone https://github.com/emscripten-core/emsdk.git

# Enter that directory
cd emsdk
```

## 2、配置emsk的平台环境

```
# Fetch the latest version of the emsdk (not needed the first time you clone)
git pull

# Download and install the latest SDK tools.
./emsdk install latest

# Make the "latest" SDK "active" for the current user. (writes .emscripten file)
./emsdk activate latest

# Activate PATH and other environment variables in the current terminal
source ./emsdk_env.sh

#####################################################################
On Windows, run emsdk instead of ./emsdk, and emsdk_env.bat instead of source ./emsdk_env.sh.

Note

On Windows, if you use the activate command, the step of emsdk_env.bat is optional. If you want to know more, see activate SDK version.

Note

git pull will fetch the current list of tags, but very recent ones may not yet be present there. You can run ./emsdk update-tags to update the list of tags directly.

If you change the location of the SDK (e.g. take it to another computer on an USB), re-run the ./emsdk activate latest and source ./emsdk_env.sh commands.



```

