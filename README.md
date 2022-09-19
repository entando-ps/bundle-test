#SME-TEMPLATE-BUNDLE installation process

----- READ CAREFULLY ----

1. BEFORE installing SME-TEMPLATE-BUNDLE:

- project-namespace-server-deployment yaml must be edited adding:

- name: JACMS_IMAGERESOURCE_ALLOWEDEXTENSIONS <br>
  value: 'jpg,jpeg,png,svg,svg+xml,gif'

If you want to enable the Admin Console add this env var:

- name: APPBUILDER_INTEGRATION_ENABLED <br>
- value: false

2. After installing SME-TEMPLATE-BUNDLE:

- Be sure to have access to server-namePort DB
- Modify scripts accordingly to DB type and settings
- Execute inserts on update.sql files directly to server-namePort DB
- Reload configuration from AppBuilder

3. Updated SME-TEMPLATE-BUNDLE to version 2.0.0:

- New Content Types added:
  - glr-descriptor.yaml
  - gud-descriptor.yaml
  - tst-descriptor.yaml
- Modified Content Types:
  - contentTypes/log-descriptor.yaml
  - contentTypes/med-descriptor.yaml
  - contentTypes/txt-descriptor.yaml
- New Content Models added:
  - contentModels/sme-card-attenzione-(tst)-descriptor.yaml
  - contentModels/sme-card-immagine-singola-per-galleria-(glr)-descriptor.yaml
  - contentModels/sme-card-singole-link-guide-(gud)-descriptor.yaml
  - contentModels/sme-dettaglio-guide-(gud)-descriptor.yaml
  - contentModels/sme-esempi-attributi-corso-(aaa)-descriptor.yaml
  - contentModels/sme-galleria-con-zoom-e-slider-(glr)-descriptor.yaml
  - contentModels/sme-risultato-per-lista-(glr)-descriptor.yaml
  - contentModels/sme-risultato-per-lista-(gud)-descriptor.yaml
  - contentModels/sme-risultato-per-lista-(tst)-descriptor.yaml
  - contentModels/sme-scheda-descrittiva-complessa-(tst)-descriptor.yaml
  - contentModels/sme-scheda-descrittiva-generica-(tst)-descriptor.yaml
# bundle-test
