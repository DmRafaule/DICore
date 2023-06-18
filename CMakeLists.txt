cmake_minimum_required(VERSION 3.5)
project(DICore DESCRIPTION "Core 'essential' elements of DI" LANGUAGES CXX)

file( GLOB SOURCES **.cpp )

SetFlags()
SetLibraries( DIDebuger DITime DIMemory DIUtils )
CreateLibrary( ${PROJECT_NAME} )