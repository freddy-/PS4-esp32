idf_component_register(SRCS "src/ps4.c"
                            "src/ps4_l2cap.c"
                            "src/ps4_parser.c"
                            "src/ps4_spp.c"
                    REQUIRES nvs_flash bt
                    PRIV_REQUIRES bt
                    INCLUDE_DIRS src
                    PRIV_INCLUDE_DIRS $ENV{IDF_PATH}/components/bt/common/include
                                      $ENV{IDF_PATH}/components/bt/host/bluedroid/common/include
                                      $ENV{IDF_PATH}/components/bt/host/bluedroid/stack/include
                                      $ENV{IDF_PATH}/components/bt/host/bluedroid/stack/gap/include
                                      $ENV{IDF_PATH}/components/bt/host/bluedroid/stack/l2cap/include)