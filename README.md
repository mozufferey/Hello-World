# Hello-World
Just started with ESP32

28.07.2017 After hours spend on my PC trying to have the Hello world running with ESP 32 I deside to change course and start with GIT.
The main problem I face wast with the Free RTOS. It seems that GCC Xtensa is not fully compatible and the Hello world example will not run with it. It seam that some #define fonction are producing problem. I will use this project in the hope to fix it. MOZ

18.08.2017 After many trial and video watching I find a few think who let me use eclipse to run the esp. Here are a few hints.
  1)  Modify the file "profile" in "msys32/etc/" line 24 with the following value:
          MSYS2_PATH="/usr/local/bin:/usr/bin:/bin:/mingw32/bin"
  2)  Use template to start a project. (Template should be improved with include path and PATH and IDF_PATH already defined)
  3)  Open and empty c make project. 
  4)  The project is a "No-toolchain". Gnu make builder. No binary parser. Builder setting is "external" with use "default build command" 
  5)  Do not use relativ Path in include library. (Problem with eclipse)
  
  The rest is pretty the same as presented in the startup video.
  
  
  
