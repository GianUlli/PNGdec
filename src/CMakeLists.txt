add_library(
  PNGdec STATIC
  adler32.c
  crc32.c
  infback.c
  inffast.c
  inflate.c
  inftrees.c
  PNGdec.cpp
  zutil.c)
target_include_directories(PNGdec PUBLIC .)
target_compile_definitions(PNGdec PUBLIC NO_ARDUINO)
target_compile_options(PNGdec PRIVATE "-Wno-implicit-fallthrough")
