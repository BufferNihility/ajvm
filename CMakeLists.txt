cmake_minimum_required(VERSION 3.15)
project(ajvm C)

set(CMAKE_C_STANDARD 11)

include_directories(.)

add_executable(ajvm
        bytecode.h
        classloader.c
        garbage_collect.c
        garbage_collect.h
        interp_engine.c
        libelf.c
        libelf.h
        list.h
        log.c
        log.h
        safe_printf.c
        safe_printf.h
        slab.c
        slab.h
        trace.c
        trace.h
        type.h
        vm_error.c
        vm_error.h
        wvm.c
        wvm.h)

add_definitions("-g -D_GNU_SOURCE")