file(GLOB SOURCES *.c)

idf_component_register(SRCS ${SOURCES}
                       INCLUDE_DIRS . ../cmd ../clock ../i2c ../lepton ../../main
                       REQUIRES clock i2c cmd
                       PRIV_REQUIRES nvs_flash)
