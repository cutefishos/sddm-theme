cmake_minimum_required(VERSION 3.5)

project(cutefish-sddm-theme)

set(CMAKE_INCLUDE_CURRENT_DIR ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTORCC ON)

install(FILES Main.qml DESTINATION ${CMAKE_INSTALL_PREFIX}/usr/share/sddm/themes/cutefish)
install(FILES SessionMenu.qml DESTINATION ${CMAKE_INSTALL_PREFIX}/usr/share/sddm/themes/cutefish)
install(FILES UserView.qml DESTINATION ${CMAKE_INSTALL_PREFIX}/usr/share/sddm/themes/cutefish)
install(FILES FishUIMenu.qml DESTINATION ${CMAKE_INSTALL_PREFIX}/usr/share/sddm/themes/cutefish)
install(FILES FishUIMenuItem.qml DESTINATION ${CMAKE_INSTALL_PREFIX}/usr/share/sddm/themes/cutefish)
install(FILES system-shutdown-symbolic.svg DESTINATION ${CMAKE_INSTALL_PREFIX}/usr/share/sddm/themes/cutefish)

install(FILES theme.conf DESTINATION ${CMAKE_INSTALL_PREFIX}/usr/share/sddm/themes/cutefish)
install(FILES hidpi.conf DESTINATION ${CMAKE_INSTALL_PREFIX}/etc/sddm.conf.d/)
install(FILES sddm.conf DESTINATION ${CMAKE_INSTALL_PREFIX}/etc/)

# install(FILES "faces/.face.icon" DESTINATION /usr/share/sddm/faces/)
