#
# ZPP is a header only library, so the only thing we do here is
# making sure the user can do #include <zpp/thread.hpp>
#

add_compile_definitions(OS_USE_SEMIHOSTING)
zephyr_include_directories(${ZEPHYR_BASE}/include/zephyr/portability)
zephyr_include_directories(include)
zephyr_library_sources(src/Chrono.cpp)
zephyr_library_sources(src/ConditionVariable.cpp)
zephyr_library_sources(src/EventFlag.cpp)
zephyr_library_sources(src/Memory.cpp)
zephyr_library_sources(src/MessageQueue.cpp)
zephyr_library_sources(src/Mutex.cpp)
zephyr_library_sources(src/OS.cpp)
zephyr_library_sources(src/OSException.cpp)
#zephyr_library_sources(src/rtx_os.cpp)
zephyr_library_sources(src/Semaphore.cpp)
zephyr_library_sources(src/Thread.cpp)
zephyr_library_sources(src/ThreadFlag.cpp)
zephyr_library_sources(src/Threads.cpp)
zephyr_library_sources(src/Timer.cpp)
