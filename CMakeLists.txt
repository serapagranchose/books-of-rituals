cmake_minimum_required(VERSION 3.17)

project(books-of-rituals
    VERSION 0.1
    DESCRIPTION "A game that makes you control a sorcerer who fights his own with a book of spells"
)

find_package(SFML 2.4 COMPONENTS audio graphics window system REQUIRED)

file(GLOB SRCS "src/*.cpp")

add_executable(books-of-rituals ${SRCS})

target_link_libraries(books-of-rituals sfml-audio sfml-graphics sfml-window sfml-system)
