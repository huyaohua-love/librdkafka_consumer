cmake_minimum_required(VERSION 3.13)
project(librdkafka_consumer)

set(CMAKE_CXX_STANDARD 11)

#库根目录
#librdkafka
set(LIBRDKAFKA "/home/obsidian/Downloads/faceDetect/librdkafka_consumer/librdkafka")

#头文件
include_directories(${LIBRDKAFKA}/include)

add_executable(librdkafka_consumer main.cpp CKafkaConsumer.cpp CKafkaConsumer.h)

#链接库
target_link_libraries(
        librdkafka_consumer
        ${LIBRDKAFKA}/lib/librdkafka.so
        ${LIBRDKAFKA}/lib/librdkafka++.so
)