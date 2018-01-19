cmake_minimum_required(VERSION 2.6)
project(ffmpegsdlvideoplayer)

include_directories("/home/geyu/app/ffmpeg-dev/include")

link_directories("/home/geyu/app/ffmpeg-dev/lib")

add_executable(ffmpegsdlvideoplayer main.cpp)

target_link_libraries(ffmpegsdlvideoplayer "avcodec" "avformat" "swscale" "avutil" "SDL2")
#install(TARGETS ffmpegsdlvideoplayer RUNTIME DESTINATION bin)
