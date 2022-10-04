add_library(stm_lib SHARED
	stmlib.h
	dsp/dsp.h
	dsp/parameter_interpolator.h
	system/bootloader_utils.h
	system/system_clock.h
	utils/random.cc
	utils/random.h
)

target_include_directories(stm_lib
PUBLIC
    $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>
)
