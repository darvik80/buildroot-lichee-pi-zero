cmake_minimum_required(VERSION 3.0)

project(ESP-hosted)

# Reset Git repository
#execute_process(
#    COMMAND git reset --hard
#)

# Initialize submodules for esp-idf
execute_process(
    COMMAND git submodule update --init --depth=1
    WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}
)

# Output message
message("###### Setup Done ######")
