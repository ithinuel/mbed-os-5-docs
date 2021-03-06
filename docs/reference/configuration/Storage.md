<h2 id="configuration-storage">Storage</h2>

The following is the complete list of storage configuration parameters, as generated by `mbed compile --config -v`. Please see [the configuration system documentation](/docs/development/reference/configuration.html) for details on how you may use or override these settings.

```
Configuration parameters
------------------------

Name: filesystem.present
    Defined by: library:filesystem
    Macro name: MBED_CONF_FILESYSTEM_PRESENT
    Value: 1 (set by library:filesystem)

Name: littlefs.read_size
    Description:
        Minimum size of a block read. This determines the size of read buffers.
        This may be larger than the physical read size to improve performance
        by caching more of the block device.

        By default, this is set to 64 bytes, which we determined experimentally.
        Note that the LittleFS uses the block device's read size if it is
        larger.
    Defined by: library:littlefs
    Macro name: MBED_LFS_READ_SIZE
    Value: 64 (set by library:littlefs)
Name: littlefs.prog_size
    Description:
        Minimum size of a block program. This determines the size of the program
        buffers. This may be larger than the physical program size to improve
        performance by caching more of the block device.

        By default, this is set to 64 bytes, which we determined experimentally.
        Note that the LittleFS uses the block device's program size if it is
        larger.
    Defined by: library:littlefs
    Macro name: MBED_LFS_PROG_SIZE
    Value: 64 (set by library:littlefs)
Name: littlefs.block_size
    Description:
        Minimum size of an erasable block. This does not affect RAM consumption
        and may be larger than the physical erase size. However, this needs to
        be small because each file takes up an entire block.

        By default, this is set to 512 bytes. Note that the LittleFS uses the
        block device's erase size if it is larger.
    Defined by: library:littlefs
    Macro name: MBED_LFS_BLOCK_SIZE
    Value: 512 (set by library:littlefs)
Name: littlefs.lookahead
    Description:
        Number of blocks to lookahead during block allocation. A larger
        lookahead reduces the number of passes required to allocate a block.
        The lookahead buffer requires only 1 bit per block, so it can be large
        with little effect on RAM. This is a multiple of 32.

        By default, this is set to 512 blocks (which use 64 bytes of RAM),
        which we determined experimentally.
    Defined by: library:littlefs
    Macro name: MBED_LFS_LOOKAHEAD
    Value: 512 (set by library:littlefs)
Name: littlefs.enable_info
    Description:
        Enables information logging (true = enabled, false = disabled,
        null = disabled) in release builds.

        By default, information logging is disabled.
    Defined by: library:littlefs
    Macro name: MBED_LFS_ENABLE_INFO
    Value: false (set by library:littlefs)
Name: littlefs.enable_debug
    Description:
        Enables debug logging (true = enabled, false = disabled,
        null = disabled) in release builds.

        By default, debug logging is enabled unless you are using a release
        build.
    Defined by: library:littlefs
    Macro name: MBED_LFS_ENABLE_DEBUG
    Value: null (set by library:littlefs)
Name: littlefs.enable_warn
    Description:
        Enables warn logging (true = enabled, false = disabled,
        null = disabled) in release builds.

        By default, warn logging is enabled unless you are using a release
        build.
    Defined by: library:littlefs
    Macro name: MBED_LFS_ENABLE_WARN
    Value: null (set by library:littlefs)
Name: littlefs.enable_error
    Description:
        Enables error logging (true = enabled, false = disabled,
        null = disabled) in release builds.

        By default, error logging is enabled unless you are using a release
        build.
    Defined by: library:littlefs
    Macro name: MBED_LFS_ENABLE_ERROR
    Value: null (set by library:littlefs)

Name: nvstore.max_keys
    Description:
        Maximal number of allowed NVStore keys.
    Defined by: library:nvstore
    Macro name: NVSTORE_MAX_KEYS
    Value: 16 (set by library:nvstore)
Name: nvstore.area_1_address
    Description:
        Address of the first NVStore area in flash.
    Defined by: library:nvstore
    Macro name: NVSTORE_AREA_1_ADDRESS
    Value: null (set by library:nvstore)
Name: nvstore.area_1_size
    Description:
        Size of the first NVStore area in flash.
    Defined by: library:nvstore
    Macro name: NVSTORE_AREA_1_SIZE
    Value: null (set by library:nvstore)
Name: nvstore.area_2_address
    Description:
        Address of the second NVStore area in flash.
    Defined by: library:nvstore
    Macro name: NVSTORE_AREA_2_ADDRESS
    Value: null (set by library:nvstore)
Name: nvstore.area_2_size
    Description:
        Size of the second NVStore area in flash.
    Defined by: library:nvstore
    Macro name: NVSTORE_AREA_2_SIZE
    Value: null (set by library:nvstore)

```
