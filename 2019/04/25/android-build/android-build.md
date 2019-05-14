---
title: android-build 
date: 2019-04-25 03:38:28
tags:
- Android

categories:
- 技术文章

---
示例Android Build类

#### Android Build类

> Build类提供了硬件厂商、编号、序列号、SDK版本等重要信息。 
> 类名：android.os.Build

| **常量名**   | **说明**                       |
| ------------ | ------------------------------ |
| BOARD        | 底层板名称                     |
| BOOTLOADER   | Bootloader版本号               |
| BRAND        | 品牌                           |
| CPU_ABI      | CPU指令集                      |
| CPU_ABI2     | CPU第二指令集                  |
| DEVICE       | 工业设计名称                   |
| DISPLAY      | 显示给用户的构建ID字符串       |
| FINGERPRINT  | 构建的唯一标识符               |
| HARDWARE     | 硬件的名称 比如高通            |
| HOST         | 主机                           |
| ID           | ID标签                         |
| MANUFACTURER | 产品生产商                     |
| MODEL        | 手机型号                       |
| PRODUCT      | 产品名称                       |
| RADIO        | 无线电固件版本号               |
| SERIAL       | 硬件序列号（如果可用）         |
| TAGS         | 逗号分隔标签描述构建，如”调试” |
| TIME         | 出场时间                       |
| TYPE         | 构建类型                       |
| USER         | 构建用户名称                   |

2.Build.VERSION类

> Build.VERSION类提供了开发代号、内部版本、SDK版本等信息      
> 类名：android.os.Build.VEISION

| **常量名**  | **说明**                                 |
| ----------- | ---------------------------------------- |
| CODENAME    | 当前的开发代号                           |
| INCREMENTAL | 使用的内部值表示这个构建底层的源代码控制 |
| RELEASE     | 用户可见版本字符串                       |
| SDK_INT     | 用户可见的SDK版本的框架                  |

3.Build.VERSION_CODES类

> android.os.Build.VERSION_CODES枚举当前已知的SDK版本代号

| **常量名**             | **说明**                             |
| ---------------------- | ------------------------------------ |
| BASE                   | 2008-10：第一个版本的android         |
| BASE_1_1               | 2009-02：第一个安卓更新，官方称为1.1 |
| CUPCAKE                | 2009-05：android1.5                  |
| CUR_DEVELOPMENT        | 发展过程中构建的版本，但是未正式发布 |
| DONUT                  | 2009-09：android1.6                  |
| ECLAIR                 | 2009-11：android2.0                  |
| ECLAIR_0_1             | 2009-12：android2.0.1                |
| ECLAIR_MR1             | 2010-01：android2.1                  |
| FROYO                  | 2010-06：android2.2                  |
| GINGERBREAD            | 2010-11：android2.3                  |
| GINGERBREAD_MR1        | 2011-02：android2.3.3                |
| HONEYCOMB              | 2011-02：android3.0                  |
| HONEYCOMB_MR1          | 2011-05：android3.1                  |
| HONEYCOMB_MR2          | 2011-06：android3.2                  |
| ICE_CREAM_SANDWICH     | 2011-10：android4.0                  |
| ICE_CREAM_SANDWICH_MR1 | 2011-12android4.0.3                  |
| JELLY_BEAN             | 2012-06：android4.1                  |
| JELLY_BEAN_MR1         | android4.2                           |
| JELLY_BEAN_MR2         | android4.3                           |
| KITKAT                 | android4.4                           |

```java
public void testDemo1(){
    //Build类
    System.out.println("Build:"+Build.BOARD);
    System.out.println("Build:"+Build.BOOTLOADER);
    System.out.println("Build:"+Build.CPU_ABI);
    System.out.println("Build:"+Build.CPU_ABI2);
    System.out.println("Build:"+Build.DEVICE);
    System.out.println("Build:"+Build.DISPLAY);
    System.out.println("Build:"+Build.FINGERPRINT);
    System.out.println("Build:"+Build.HARDWARE);
    System.out.println("Build:"+Build.HOST);
    System.out.println("Build:"+Build.ID);
    System.out.println("Build:"+Build.MANUFACTURER);
    System.out.println("Build:"+Build.MODEL);
    System.out.println("Build:"+Build.PRODUCT);
    System.out.println("Build:"+Build.RADIO);
    System.out.println("Build:"+Build.SERIAL);
    System.out.println("Build:"+Build.TAGS);
    System.out.println("Build:"+Build.TIME);
    System.out.println("Build:"+Build.TYPE);
    System.out.println("Build:"+Build.USER);
    System.out.println("Build:"+Build.BOARD);
    //Build.VERSION类
    System.out.println("Build.VERSION:"+Build.VERSION.CODENAME);
    System.out.println("Build.VERSION:"+Build.VERSION.INCREMENTAL);
    System.out.println("Build.VERSION:"+Build.VERSION.RELEASE);
    System.out.println("Build.VERSION:"+Build.VERSION.SDK_INT);
    //Build.VERSION_CODES类
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.BASE);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.BASE_1_1);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.CUPCAKE);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.CUR_DEVELOPMENT);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.ECLAIR);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.ECLAIR_0_1);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.ECLAIR_MR1);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.FROYO);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.GINGERBREAD);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.GINGERBREAD_MR1);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.HONEYCOMB);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.HONEYCOMB_MR1);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.HONEYCOMB_MR2);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.ICE_CREAM_SANDWICH);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.ICE_CREAM_SANDWICH_MR1);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.JELLY_BEAN);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.JELLY_BEAN_MR1);
    System.out.println("Build.VERSION_CODES:"+Build.VERSION_CODES.JELLY_BEAN_MR2);
}
```

