zephyr_library()

zephyr_library_sources_ifdef(CONFIG_LED_STRIP_COMPOSITE src/led_strip_composite.c)
zephyr_library_sources_ifdef(CONFIG_CKLED2001 src/ckled2001.c)

zephyr_include_directories(include)

zephyr_include_directories(${APPLICATION_SOURCE_DIR}/include)