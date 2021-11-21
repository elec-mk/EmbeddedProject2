cmake_minimum_required(VERSION 3.15)

project(EmbeddedProject2 LANGUAGES C CXX ASM)

find_bsp(ID com.sysprogs.project_importers.stm32.cubemx SOURCE_PROJECT EmbeddedProject2.ioc)

add_bsp_based_executable(NAME EmbeddedProject2
	GENERATE_BIN
	GENERATE_MAP)

