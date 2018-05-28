1、**n2nguien.exe**为安装文件，支持原始V1和V2，所有连接点不能混用，版本必须统一；<br>
2、此项目中的`edge2.exe`为**n2n_v21**版本或者称为**n2n_v2s**版，若需使用，需要将`edge2.exe`文件覆盖原安装文件中的`edge2.exe`；<br>
# 参考
[CentOS下交叉编译Windows N2N服务端及客户端](https://bugxia.com/327.html)<br>
# 编译
1、编译时主要先安装mingw32，然后修改cmake/CMakeToolchainFileMingw32.cmake<br>
2、编译
```vim
mkdir build
cd build
cmake -DCMAKE_TOOLCHAIN_FILE=../cmake/CMakeToolchainFileMingw32.cmake --build ./ ../
make
```

