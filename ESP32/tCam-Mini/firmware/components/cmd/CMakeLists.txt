file(GLOB SOURCES *.c)

idf_component_register(SRCS ${SOURCES}
                       INCLUDE_DIRS . ../lepton ../clock ../sys ../../main
                       PRIV_REQUIRES mbedtls nvs_flash app_update)
