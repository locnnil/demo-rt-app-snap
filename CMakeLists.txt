cmake_minimum_required(VERSION 3.5)
project(rt-app C)

add_executable(cfs cfs.c)
install(TARGETS cfs RUNTIME DESTINATION bin)

add_executable(edf edf.c)
install(TARGETS edf RUNTIME DESTINATION bin)

add_executable(fifo fifo.c)
install(TARGETS fifo RUNTIME DESTINATION bin)

add_executable(lock lock.c)
install(TARGETS lock RUNTIME DESTINATION bin)

add_executable(thread-affinity thread-affinity.c)
install(TARGETS thread-affinity RUNTIME DESTINATION bin)
