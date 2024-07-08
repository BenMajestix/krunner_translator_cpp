add_definitions(-DTRANSLATION_DOMAIN=\"plasma_runner_org.kde.krunner_translator_cpp\")

kcoreaddons_add_plugin(krunner_translator_cpp INSTALL_NAMESPACE "kf6/krunner")

target_sources(krunner_translator_cpp PRIVATE
    krunner_translator_cpp.cpp
)

target_link_libraries(krunner_translator_cpp
    Qt6::Gui # QAction
    KF6::Runner
    KF6::I18n
)
