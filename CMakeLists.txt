cmake_minimum_required(VERSION 3.7)
set(VERSION 4.0)
project(hw-cloud-config)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_INCLUDE_CURRENT_DIR ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_CXX_FLAGS "-g -Wall")

install(FILES dde-session-ui.conf DESTINATION /etc/deepin/)

install(FILES com.deepin.dde.auth.gschema.xml DESTINATION /usr/share/glib-2.0/schemas/)

install(FILES hw.cloud.config.gschema.override DESTINATION /usr/share/glib-2.0/schemas/)
