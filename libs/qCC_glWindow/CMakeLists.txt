project( QCC_GL_LIB )

find_package(OpenCV REQUIRED)
include_directories( ${OpenCV_INCLUDE_DIRS} )  
#link_directories( ${OpenCV_LIBRARIES} )

add_library( ${PROJECT_NAME} SHARED )

add_subdirectory( include )
add_subdirectory( src )

target_compile_definitions( ${PROJECT_NAME} PRIVATE CCGLWINDOW_LIB_BUILD )

target_link_libraries( ${PROJECT_NAME}
	QCC_DB_LIB
	${OpenCV_LIBRARIES}
)

# Oculus support
include( cmake/OculusSupport.cmake )

if ( OPTION_USE_OCULUS_SDK )	
    target_link_OCULUS_SDK( ${PROJECT_NAME} )
endif()

InstallSharedLibrary( TARGET ${PROJECT_NAME} )
