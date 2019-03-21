# CMakeLists.txt - fips-argagg

cmake_minimum_required(VERSION 3.10)

# use FIPS_ROOT from environment
get_filename_component(FIPS_ROOT_DIR "$ENV{FIPS_ROOT}" ABSOLUTE)
if(FIPS_ROOT_DIR)
    set(FIPS_ROOT_DIR "${FIPS_ROOT_DIR}/fips")
else(FIPS_ROOT_DIR)
    set(FIPS_ROOT_DIR "../fips")
endif(FIPS_ROOT_DIR)

# include the fips main cmake file
include("${FIPS_ROOT_DIR}/cmake/fips.cmake")

fips_add_subdirectory(argagg)

