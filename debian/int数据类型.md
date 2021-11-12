<!--
 * @Author: zhanghao
 * @Date: 2021-11-03 10:12:17
 * @LastEditTime: 2021-11-03 10:13:21
 * @Description: Do not edit
 * @Email: 
 * Copyright (C) 2021 zhanghao. All rights reserved.
-->


```c
/*
 * @Author: zhanghao
 * @Date: 2021-11-02 18:56:58
 * @LastEditTime: 2021-11-03 10:11:04
 * @Description:
 * 测试
 * int
 * char
 * short
 * long
 * long long
 * long long int
 * @Email:
 * Copyright (C) 2021 zhanghao. All rights reserved.
 */


#include <stdio.h>
/*
    short 、long、long long 分别是
    short int
    long int
    long long int
    的缩写
 */

int main(){
    int a1;
    long a2;
    long int a3;    //  == long

    long long b1;
    long long int b2;   //  ==  long long

    short c1;
    short int c2;   //  ==  short

    char d1;

    __int8_t  e1;
    __int16_t e2;
    __int32_t e3;
    __int64_t e4;   //  typedef signed long int __int64_t;


    // int ptr
    // __intptr_t 是为了跨平台
    // 其长度就是所在平台的 os 操作系统的位数
    // 所以用来存放地址
    // 64 bit 上 : typedef long int __intptr_t;
    // 32 bit 上 : typedef      int __intptr_t;

    __intptr_t f1;

    ssize_t f2;
    size_t  f3;

    printf("int           : %d""\r\n", sizeof(a1));
    printf("long          : %ld""\r\n",sizeof(a2));
    printf("long int      : %ld""\r\n",sizeof(a3));
    printf("long long     : %ld""\r\n",sizeof(b1));
    printf("long long int : %ld""\r\n",sizeof(b2));
    printf("short         : %d""\r\n",sizeof(c1));
    printf("short int     : %d""\r\n",sizeof(c2));
    printf("char          : %d""\r\n",sizeof(d1));

    printf("__int8_t      : %d""\r\n",sizeof(e1));
    printf("__int16_t     : %d""\r\n",sizeof(e2));
    printf("__int32_t     : %d""\r\n",sizeof(e3));
    printf("__int64_t     : %d""\r\n",sizeof(e4));
    printf("__intptr_t    : %d""\r\n",sizeof(f1));
    printf("ssize_t       : %d""\r\n",sizeof(f2));
    printf("size_t        : %d""\r\n",sizeof(f3));
    return 0;
}
/* $ gcc test_int.c
$ ./a.out
int           : 4
long          : 8
long int      : 8
long long     : 8
long long int : 8
short         : 2
short int     : 2
char          : 1
__int8_t      : 1
__int16_t     : 2
__int32_t     : 4
__int64_t     : 8
__intptr_t    : 8 
ssize_t       : 8
size_t        : 8*/



```
