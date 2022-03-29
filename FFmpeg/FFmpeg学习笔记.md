[TOC]



# 下载及环境配置

## 下载

需要下载` ffmpeg-x.x.x-full_build-shared.7z`，解压后才有`.h`和`.dll`文件。

## VS2019环境配置

1. 修改include
2. 修改dependency
3. 复制dll到工作目录

## 测试代码

```C++
#include <stdio.h>

extern "C" {
#include  <libavcodec\avcodec.h>
}
#pragma comment(lib, "avcodec.lib")

int main() {
    printf("%s\n", avcodec_configuration());
    return 0;
}
```

![image-20220330000301257](E:\学习\FFmpeg\img\image-20220330000301257.png)

# YUV格式

[YUV格式详解](https://blog.csdn.net/xkuzhang/article/details/115423061)