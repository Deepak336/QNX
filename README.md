# QNX
QNX related Makefiles



CROSS COMPILATION:

qnx64.cmake:

At times open source modules dont support cross compilation for QNX.

Well most of the open source modules does have a cmake based build support, and cmake supports cross compilation using .cmake file,

wherein the compiler part, cflags, directives can be added.

I am adding a sample qnx64.cmake which is generic and can be used to cross compile for QNX 64bit arm arch based processors, for cmake based projects.

Feel free to modify as per need.



Once qnx64.cmake is added to open source checked out project, one can invoke cmake command to cross compile it.

Example:

        cmake -DCMAKE_TOOLCHAIN_FILE=<path_to_open_source_module>/qnx64.cmake ../
        make ;
       

