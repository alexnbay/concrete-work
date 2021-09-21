## <a name="uninstall"></a>Uninstall the Intel® Distribution of OpenVINO™ Toolkit in Linux
Choose one of the options provided below to uninstall the Intel® Distribution of OpenVINO™ Toolkit from your system.

### Uninstall with GUI
1. Run the uninstallation script from `<INSTALL_DIR>/openvino_toolkit_uninstaller`:
   ```sh
   sudo ./uninstall_GUI.sh
   ```
2. Follow the uninstallation wizard instructions.


### Uninstall with Command Line (Interactive Mode)
1. Run the uninstallation script from `<INSTALL_DIR>/openvino_toolkit_uninstaller`:
   ```sh
   sudo ./uninstall.sh
   ```
2. Follow the instructions on your screen.
4. When uninstallation is complete, press **Enter**.

### Uninstall with Command Line (Silent Mode)
1. Run the following command from `<INSTALL_DIR>/openvino_toolkit_uninstaller`:
   ```sh
   sudo ./uninstall.sh -s
   ```
2. Intel® Distribution of OpenVINO™ Toolkit is now uninstalled from your system.

## Troubleshooting

PRC developers might encounter pip installation related issues during OpenVINO™ installation. To resolve the issues, you may use one of the following options at your discretion:
* Add the download source with `-i` parameter in the `pip` command. For example: 
```
pip install numpy.py -i https://mirrors.aliyun.com/pypi/simple/
```
Use the `--trusted-host` parameter if the URL above is `http` instead of `https`.

* Modify or create `~/.pip/pip.conf` file to change the default download source with the content below:
```
[global]
index-url = http://mirrors.aliyun.com/pypi/simple/
[install]
trusted-host = mirrors.aliyun.com
```
