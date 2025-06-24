ADD_SUBDIRECTORY( src )
# Define libusb as an IMPORTED static library  
add_library(libusb_imported STATIC IMPORTED)  
set_target_properties(libusb_imported PROPERTIES  
    IMPORTED_LOCATION "C:/Program Files/libfreenect/lib/libusb-1.0.lib"  
    INTERFACE_INCLUDE_DIRECTORIES "C:/Program Files/libfreenect/include"  
)
