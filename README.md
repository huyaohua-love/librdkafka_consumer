# librdkafka_consumer
librdkafka是kafka消息系统的C/C++跨平台开源库。该项目用C++对librdkafka(librdkafka-0.11.6)进行简单封装，之前项目开发中使用，测试通过的测试代码，留备后用。

生产者：https://github.com/huyaohua-love/librdkafka_producer.git

运行修改:（注意librdkafka需要的库，参考官网。）
修改：CMakeLists.txt第8行 set(LIBRDKAFKA "/home/obsidian/Downloads/faceDetect/librdkafka_consumer/librdkafka") 的路径。
