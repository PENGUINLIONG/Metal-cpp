# Metal-cpp

An adapted copy of Apple's metal-cpp header-only library for easy integration
in CMake projects.

## Upgrade Metal-cpp

Remove everything existing in `third/metal-cpp` and copy the new distribution into it. Run the following script to generate the single header in `include/metal-cpp`.

```
python third/metal-cpp/SingleHeader/MakeSingleHeader.py \
    third/metal-cpp/Foundation/Foundation.hpp \
    third/metal-cpp/QuartzCore/QuartzCore.hpp \
    third/metal-cpp/Metal/Metal.hpp \
    -o include/metal-cpp/Metal.hpp
```

## License

Source codes in this repository not licensed by Apple is MIT-licensed.
