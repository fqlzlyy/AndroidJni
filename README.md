# AndroidJni
基于 Android JNI学习的例子，Java 调用 C/C++, C/C++ 回调 Java 

## JNI 调用步骤

1. 创建一个 android 工程
2. JAVA 代码中写声明 native 方法 public native String helloFromJNI();
3. 通过 javah 命令生成 .h 文件
4. 创建jni目录,编写c/c++代码,方法名字要对应(一般从.h文件拷贝过来)
5. 编写Android.mk文件
6. Ndk编译生成动态库(ndk-build)
7. Java代码 load 动态库.调用native代码
