cmake_minimum_required(VERSION 3.5)

set(COMPONENT_SRCDIRS
        ./
        )

set(COMPONENT_ADD_INCLUDEDIRS
        ./
        )

set(COMPONENT_REQUIRES
        freertos
        driver
        )

idf_component_register(
        SRC_DIRS ${COMPONENT_SRCDIRS}
        REQUIRES ${COMPONENT_REQUIRES}
        INCLUDE_DIRS ${COMPONENT_ADD_INCLUDEDIRS}
)