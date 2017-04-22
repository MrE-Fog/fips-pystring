#
# project: fips-pystring
#
if (NOT FIPS_IMPORT)
    cmake_minimum_required(VERSION 2.8)
    get_filename_component(FIPS_ROOT_DIR "../fips" ABSOLUTE)
    include("${FIPS_ROOT_DIR}/cmake/fips.cmake")
    fips_setup(PROJECT pystring)
endif()
fips_begin_lib(pystring)
    fips_dir(pystring)
    fips_files(pystring.h pystring.cpp)
fips_end_lib()
fips_finish()


