# VSCode C++环境配置

#### 1.基本环境配置

- 选一个C++文本编译程序，这里选用[MinGW-w64](https://www.mingw-w64.org/)

  - 这里通过配置VScode使用，下载对应平台的编译器，这里使用[windows](https://sourceforge.net/projects/mingw-w64/files/)的下载资源，下载压缩包

    ![](../../../../resources/language_c++_compileInstaller.png)

  - 下载压缩包可以提供给vscode使用，只需要解压后，把文件bin目录配置到环境变量path位置
    <img src="../../../../resources/language_c++_compilePathSetup.png" alt="image-20221023163804354" style="zoom: 33%;" />

  - 通过cmd输入，g++ --version获得以下结果即可
    ![image-20221023164235448](../../../../resources/language_c++_compilecmdversion.png)
  
  - 在VScode中安装C++插件
    ![image-20221023162926833](../../../../resources/language_c++_vscodeCppAddOn.png)
    
  - 在vscode按shift+ctrl+p，进入C++插件配置
    <img src="../../../../resources/language_c++_vscodeC++ConfigUI.png" alt="image-20221023164638758" style="zoom:50%;" />
  
  - 在页面中设置以下配置即可
    ![image-20221023165614875](../../../../resources/language_c++_vscodeC++ConfigUIg++Setting.png)
  
  - 写入main.cpp文件，按F5配置Vscode的编译配置
    ![image-20221023170055093](../../../../resources/language_c++_vscodeC++BuildSettingSelect.png)
  
  - 配置自动设置完成，F5运行得到结果
    ![image-20221023183114091](../../../../resources/language_c++_compileHelloWorld.png)