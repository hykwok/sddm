set(TRANSLATION_FILES
    ar.ts
    cs.ts
    de.ts
    es.ts
    et.ts
    fi.ts
    fr.ts
    hu.ts
    it.ts
    ja.ts
    ko.ts
    lt.ts
    lv.ts
    pl.ts
    pt_BR.ts
    pt_PT.ts
    ro.ts
    ru.ts
    tr.ts
    zh_CN.ts
)

qt5_add_translation(QM_FILES ${TRANSLATION_FILES})

install(FILES ${QM_FILES} DESTINATION "${COMPONENTS_TRANSLATION_DIR}")

add_custom_target(components-translation DEPENDS ${QM_FILES})
