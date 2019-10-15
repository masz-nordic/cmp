if(CONFIG_CMP)
	zephyr_interface_library_named(CMP)

zephyr_include_directories(MPACK INTERFACE ./)

zephyr_library()
zephyr_library_sources(
    cmp.c
)

zephyr_library_link_libraries(CMP)
zephyr_link_libraries(CMP INTERFACE zephyr_interface)
endif()
