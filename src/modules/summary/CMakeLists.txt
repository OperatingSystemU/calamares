include_directories( ${PROJECT_BINARY_DIR}/src/libcalamaresui )
calamares_add_plugin( summary
    TYPE viewmodule
    EXPORT_MACRO PLUGINDLLEXPORT_PRO
    CONFIG_FILE module.conf
    SOURCES
        SummaryViewStep.cpp
        SummaryPage.cpp
    UI
    LINK_LIBRARIES
        calamaresui
    SHARED_LIB
)
