# Comparing `tmp/sdc11073-2.0.0a4.tar.gz` & `tmp/sdc11073-2.0.0a5.tar.gz`

## Comparing `sdc11073-2.0.0a4.tar` & `sdc11073-2.0.0a5.tar`

### file list

```diff
@@ -1,138 +1,138 @@
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/CHANGELOG.md
--rw-r--r--   0        0        0   347063 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/docs/sdc_social_preview.jpg
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/__init__.py
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/certloader.py
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/commlog.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/definitions_base.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/definitions_sdc.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/etc.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/exceptions.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/location.py
--rw-r--r--   0        0        0     8772 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/loghelper.py
--rw-r--r--   0        0        0     9314 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/multikey.py
--rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/namespaces.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/schema_resolver.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/dispatch/__init__.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/dispatch/dispatchkey.py
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/dispatch/messageconverter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/dispatch/pathelementregistry.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/dispatch/request.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/httpserver/__init__.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/httpserver/compression.py
--rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/httpserver/httpreader.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/httpserver/httprequesthandler.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/httpserver/httpserverimpl.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/__init__.py
--rw-r--r--   0        0        0    35169 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/clientmdib.py
--rw-r--r--   0        0        0    19227 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/clientmdibxtra.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/containerbase.py
--rw-r--r--   0        0        0    35160 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/descriptorcontainers.py
--rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/devicemdib.py
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/devicemdibxtra.py
--rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/devicewaveform.py
--rw-r--r--   0        0        0    25440 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/mdibbase.py
--rw-r--r--   0        0        0    24434 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/statecontainers.py
--rw-r--r--   0        0        0    36856 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/transactions.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/netconn/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/observableproperties/__init__.py
--rw-r--r--   0        0        0     8027 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/observableproperties/observables.py
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/observableproperties/valuecollector.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/__init__.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/msgfactory.py
--rw-r--r--   0        0        0    10118 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/msgreader.py
--rw-r--r--   0        0        0    15907 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclient.py
--rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclient_async.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclientpool.py
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/soapenvelope.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/__init__.py
--rw-r--r--   0        0        0    21440 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/alarmprovider.py
--rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/audiopauseprovider.py
--rw-r--r--   0        0        0     9426 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/clockprovider.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/contextprovider.py
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/metricprovider.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/nomenclature.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/operationprovider.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/patientcontextprovider.py
--rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/product.py
--rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/providerbase.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/__init__.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/components.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/manipulator.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/operations.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/request_handler_deferred.py
--rw-r--r--   0        0        0    32197 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/sdcclientimpl.py
--rw-r--r--   0        0        0    22009 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/subscription.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/__init__.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py
--rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/contextservice.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/descriptioneventservice.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/getservice.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/localizationservice.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py
--rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/setservice.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/stateeventservice.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/waveformservice.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/__init__.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/components.py
--rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/dpwshostedservice.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/intervaltimer.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/operations.py
--rw-r--r--   0        0        0    10632 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/periodicreports.py
--rw-r--r--   0        0        0    16697 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/sco.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/scopesfactory.py
--rw-r--r--   0        0        0    24480 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/sdcdeviceimpl.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/servicesfactory.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr.py
--rw-r--r--   0        0        0    14883 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr_async.py
--rw-r--r--   0        0        0    24606 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr_base.py
--rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/waveforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/__init__.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py
--rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py
--rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/localizationservice.py
--rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/porttypebase.py
--rw-r--r--   0        0        0    11710 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py
--rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/common.py
--rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/networkingthread.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/service.py
--rw-r--r--   0        0        0    30230 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/wsdimpl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/__init__.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/actions.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/addressing_types.py
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/basetypes.py
--rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/dataconverters.py
--rw-r--r--   0        0        0     6365 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/dpws_types.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/eventing_types.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/ext_qnames.py
--rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/isoduration.py
--rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/mex_types.py
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/msg_qnames.py
--rw-r--r--   0        0        0    27781 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/msg_types.py
--rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/pm_qnames.py
--rw-r--r--   0        0        0    58377 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/pm_types.py
--rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/wsd_types.py
--rw-r--r--   0        0        0    53115 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/xml_structure.py
--rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/BICEPS_MessageModel.xsd
--rw-r--r--   0        0        0   205547 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/ExtensionPoint.xsd
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/MetadataExchange.xsd
--rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/SafetyInformation.xsd
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/addressing.xsd
--rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/eventing.xsd
--rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/soap-envelope.xsd
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/ws-addr.xsd
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd
--rw-r--r--   0        0        0     9881 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/wsdl.xsd
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/xml.xsd
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/tutorial/README.rst
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/LICENSE
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/README.rst
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/CHANGELOG.md
+-rw-r--r--   0        0        0   347063 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/docs/sdc_social_preview.jpg
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/__init__.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/certloader.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/commlog.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/definitions_base.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/definitions_sdc.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/etc.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/exceptions.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/location.py
+-rw-r--r--   0        0        0     8772 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/loghelper.py
+-rw-r--r--   0        0        0     9314 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/multikey.py
+-rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/namespaces.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/schema_resolver.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/dispatch/__init__.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/dispatch/dispatchkey.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/dispatch/messageconverter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/dispatch/pathelementregistry.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/dispatch/request.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/httpserver/__init__.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/httpserver/compression.py
+-rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/httpserver/httpreader.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/httpserver/httprequesthandler.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/httpserver/httpserverimpl.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/mdib/__init__.py
+-rw-r--r--   0        0        0    35169 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/mdib/clientmdib.py
+-rw-r--r--   0        0        0    19165 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/mdib/clientmdibxtra.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/mdib/containerbase.py
+-rw-r--r--   0        0        0    35160 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/mdib/descriptorcontainers.py
+-rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/mdib/devicemdib.py
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/mdib/devicemdibxtra.py
+-rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/mdib/devicewaveform.py
+-rw-r--r--   0        0        0    25440 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/mdib/mdibbase.py
+-rw-r--r--   0        0        0    24434 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/mdib/statecontainers.py
+-rw-r--r--   0        0        0    36856 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/mdib/transactions.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/netconn/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/observableproperties/__init__.py
+-rw-r--r--   0        0        0     8027 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/observableproperties/observables.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/observableproperties/valuecollector.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/pysoap/__init__.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/pysoap/msgfactory.py
+-rw-r--r--   0        0        0    10118 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/pysoap/msgreader.py
+-rw-r--r--   0        0        0    15907 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/pysoap/soapclient.py
+-rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/pysoap/soapclient_async.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/pysoap/soapclientpool.py
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/pysoap/soapenvelope.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/roles/__init__.py
+-rw-r--r--   0        0        0    21440 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/roles/alarmprovider.py
+-rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/roles/audiopauseprovider.py
+-rw-r--r--   0        0        0     9426 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/roles/clockprovider.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/roles/contextprovider.py
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/roles/metricprovider.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/roles/nomenclature.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/roles/operationprovider.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/roles/patientcontextprovider.py
+-rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/roles/product.py
+-rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/roles/providerbase.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/__init__.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/components.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/manipulator.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/operations.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/request_handler_deferred.py
+-rw-r--r--   0        0        0    32197 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/sdcclientimpl.py
+-rw-r--r--   0        0        0    22009 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/subscription.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/__init__.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/contextservice.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/descriptioneventservice.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/getservice.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/localizationservice.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py
+-rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/setservice.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/stateeventservice.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/waveformservice.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/__init__.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/components.py
+-rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/dpwshostedservice.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/intervaltimer.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/operations.py
+-rw-r--r--   0        0        0    10632 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/periodicreports.py
+-rw-r--r--   0        0        0    16697 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/sco.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/scopesfactory.py
+-rw-r--r--   0        0        0    24480 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/sdcdeviceimpl.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/servicesfactory.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/subscriptionmgr.py
+-rw-r--r--   0        0        0    14883 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/subscriptionmgr_async.py
+-rw-r--r--   0        0        0    24606 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/subscriptionmgr_base.py
+-rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/waveforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/__init__.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py
+-rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py
+-rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/localizationservice.py
+-rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/porttypebase.py
+-rw-r--r--   0        0        0    11710 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py
+-rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/wsdiscovery/__init__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/wsdiscovery/common.py
+-rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/wsdiscovery/networkingthread.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/wsdiscovery/service.py
+-rw-r--r--   0        0        0    31651 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/wsdiscovery/wsdimpl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/__init__.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/actions.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/addressing_types.py
+-rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/basetypes.py
+-rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/dataconverters.py
+-rw-r--r--   0        0        0     6365 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/dpws_types.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/eventing_types.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/ext_qnames.py
+-rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/isoduration.py
+-rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/mex_types.py
+-rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/msg_qnames.py
+-rw-r--r--   0        0        0    27781 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/msg_types.py
+-rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/pm_qnames.py
+-rw-r--r--   0        0        0    59239 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/pm_types.py
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/wsd_types.py
+-rw-r--r--   0        0        0    59699 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xml_types/xml_structure.py
+-rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/BICEPS_MessageModel.xsd
+-rw-r--r--   0        0        0   205547 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/ExtensionPoint.xsd
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/MetadataExchange.xsd
+-rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/SafetyInformation.xsd
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/addressing.xsd
+-rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/eventing.xsd
+-rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/soap-envelope.xsd
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/ws-addr.xsd
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd
+-rw-r--r--   0        0        0     9881 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/wsdl.xsd
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/src/sdc11073/xsd/xml.xsd
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/tutorial/README.rst
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/LICENSE
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/README.rst
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 sdc11073-2.0.0a5/PKG-INFO
```

### Comparing `sdc11073-2.0.0a4/CHANGELOG.md` & `sdc11073-2.0.0a5/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 
 All notable changes to the sdc11073 module will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [master]
+## [2.0.0a5] - 2023-06-27
+
+### Fixed
+- improved error handling when reading attribute values from xml element
+- fixed possible exception in calculation of waveform age
+- fixed some places where default_py_value should be implied_py_value
+- fixed incomplete modeling of ClinicalInfo class
+
+### Added
+- added switch to allow disabling strict checking for AppSequence.
 
 ## [2.0.0a4] - 2023-06-16
 
 ### Changed
 - reworked wsdiscovery. Wsdiscovery can now only bind to a single ip address. 
   The only available classes are "WsDiscovery" and "WsDiscoverySingleAdapter".
```

### Comparing `sdc11073-2.0.0a4/docs/sdc_social_preview.jpg` & `sdc11073-2.0.0a5/docs/sdc_social_preview.jpg`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/certloader.py` & `sdc11073-2.0.0a5/src/sdc11073/certloader.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/commlog.py` & `sdc11073-2.0.0a5/src/sdc11073/commlog.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/definitions_base.py` & `sdc11073-2.0.0a5/src/sdc11073/definitions_base.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/definitions_sdc.py` & `sdc11073-2.0.0a5/src/sdc11073/definitions_sdc.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/etc.py` & `sdc11073-2.0.0a5/src/sdc11073/etc.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/exceptions.py` & `sdc11073-2.0.0a5/src/sdc11073/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/location.py` & `sdc11073-2.0.0a5/src/sdc11073/location.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/loghelper.py` & `sdc11073-2.0.0a5/src/sdc11073/loghelper.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/multikey.py` & `sdc11073-2.0.0a5/src/sdc11073/multikey.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/namespaces.py` & `sdc11073-2.0.0a5/src/sdc11073/namespaces.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/schema_resolver.py` & `sdc11073-2.0.0a5/src/sdc11073/schema_resolver.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/dispatch/dispatchkey.py` & `sdc11073-2.0.0a5/src/sdc11073/dispatch/dispatchkey.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/dispatch/messageconverter.py` & `sdc11073-2.0.0a5/src/sdc11073/dispatch/messageconverter.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/dispatch/pathelementregistry.py` & `sdc11073-2.0.0a5/src/sdc11073/dispatch/pathelementregistry.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/dispatch/request.py` & `sdc11073-2.0.0a5/src/sdc11073/dispatch/request.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/httpserver/compression.py` & `sdc11073-2.0.0a5/src/sdc11073/httpserver/compression.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/httpserver/httpreader.py` & `sdc11073-2.0.0a5/src/sdc11073/httpserver/httpreader.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/httpserver/httprequesthandler.py` & `sdc11073-2.0.0a5/src/sdc11073/httpserver/httprequesthandler.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/httpserver/httpserverimpl.py` & `sdc11073-2.0.0a5/src/sdc11073/httpserver/httpserverimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/mdib/clientmdib.py` & `sdc11073-2.0.0a5/src/sdc11073/mdib/clientmdib.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/mdib/clientmdibxtra.py` & `sdc11073-2.0.0a5/src/sdc11073/mdib/clientmdibxtra.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,44 +306,45 @@
         if accepted_states is None or len(accepted_states) == 0 or not self._mdib.is_initialized:
             return
 
         waveform_age = {}  # collect age of all waveforms in this report, and make one report if age is above warn limit (instead of multiple)
         now = time.time()
         for state_container in accepted_states.values():
             rt_sample_containers = self._mdib.rt_buffers[state_container.DescriptorHandle].rt_data
-            waveform_age[state_container.DescriptorHandle] = now - rt_sample_containers[-1].determination_time
+            if len(rt_sample_containers) > 0:
+                waveform_age[state_container.DescriptorHandle] = now - rt_sample_containers[-1].determination_time
 
-            if len(waveform_age) > 0:
-                min_age = min(waveform_age.values())
-                max_age = max(waveform_age.values())
-                shall_log = self.waveform_time_warner.get_out_of_determination_time_log_state(
-                    min_age, max_age, self.DETERMINATIONTIME_WARN_LIMIT)
-                if shall_log != A_NO_LOG:
-                    tmp = ', '.join(f'"{k}": {v:.3f}sec.' for k, v in waveform_age.items())
-                    if shall_log == A_OUT_OF_RANGE:
-                        self._logger.warning(
-                            '_on_waveform_report mdib_version {}: age of samples outside limit of {} sec.: {}',
-                            self._mdib.mdib_version, self.DETERMINATIONTIME_WARN_LIMIT, tmp)
-                    elif shall_log == A_STILL_OUT_OF_RANGE:
-                        self._logger.warning(
-                            '_on_waveform_report mdib_version {}: age of samples still outside limit of {} sec.: {}',
-                            self._mdib.mdib_version, self.DETERMINATIONTIME_WARN_LIMIT, tmp)
-                    elif shall_log == A_BACK_IN_RANGE:
-                        self._logger.info(
-                            '_on_waveform_report mdib_version {}: age of samples back in limit of {} sec.: {}',
-                            self._mdib.mdib_version, self.DETERMINATIONTIME_WARN_LIMIT, tmp)
-            if LOG_WF_AGE_INTERVAL:
-                now = time.time()
-                if now - self._last_wf_age_log >= LOG_WF_AGE_INTERVAL:
-                    age_data = self.get_wf_age_stdev()
-                    if age_data is not None:
-                        self._logger.info('waveform mean age={:.1f}ms., stdev={:.2f}ms. min={:.1f}ms., max={}',
-                                          age_data.mean_age * 1000., age_data.stdev * 1000.,
-                                          age_data.min_age * 1000., age_data.max_age * 1000.)
-                    self._last_wf_age_log = now
+        if len(waveform_age) > 0:
+            min_age = min(waveform_age.values())
+            max_age = max(waveform_age.values())
+            shall_log = self.waveform_time_warner.get_out_of_determination_time_log_state(
+                min_age, max_age, self.DETERMINATIONTIME_WARN_LIMIT)
+            if shall_log != A_NO_LOG:
+                tmp = ', '.join(f'"{k}": {v:.3f}sec.' for k, v in waveform_age.items())
+                if shall_log == A_OUT_OF_RANGE:
+                    self._logger.warning(
+                        '_on_waveform_report mdib_version {}: age of samples outside limit of {} sec.: {}',
+                        self._mdib.mdib_version, self.DETERMINATIONTIME_WARN_LIMIT, tmp)
+                elif shall_log == A_STILL_OUT_OF_RANGE:
+                    self._logger.warning(
+                        '_on_waveform_report mdib_version {}: age of samples still outside limit of {} sec.: {}',
+                        self._mdib.mdib_version, self.DETERMINATIONTIME_WARN_LIMIT, tmp)
+                elif shall_log == A_BACK_IN_RANGE:
+                    self._logger.info(
+                        '_on_waveform_report mdib_version {}: age of samples back in limit of {} sec.: {}',
+                        self._mdib.mdib_version, self.DETERMINATIONTIME_WARN_LIMIT, tmp)
+        if LOG_WF_AGE_INTERVAL:
+            now = time.time()
+            if now - self._last_wf_age_log >= LOG_WF_AGE_INTERVAL:
+                age_data = self.get_wf_age_stdev()
+                if age_data is not None:
+                    self._logger.info('waveform mean age={:.1f}ms., stdev={:.2f}ms. min={:.1f}ms., max={}',
+                                      age_data.mean_age * 1000., age_data.stdev * 1000.,
+                                      age_data.min_age * 1000., age_data.max_age * 1000.)
+                self._last_wf_age_log = now
 
     def _on_episodic_context_report(self, received_message_data):
         cls = self._mdib.data_model.msg_types.EpisodicContextReport
         report = cls.from_node(received_message_data.p_msg.msg_node)
         self._mdib.process_incoming_context_states_report(received_message_data.mdib_version_group, report)
 
     def _on_episodic_component_report(self, received_message_data):
```

### Comparing `sdc11073-2.0.0a4/src/sdc11073/mdib/containerbase.py` & `sdc11073-2.0.0a5/src/sdc11073/mdib/containerbase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/mdib/descriptorcontainers.py` & `sdc11073-2.0.0a5/src/sdc11073/mdib/descriptorcontainers.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     is_leaf = True  # determines if children can be added
 
     node = properties.ObservableProperty()  # the etree node
 
     Handle = cp.HandleAttributeProperty('Handle', is_optional=False)
     Extension = cp.ExtensionNodeProperty(ext.Extension)
     DescriptorVersion = cp.VersionCounterAttributeProperty('DescriptorVersion',
-                                                           default_py_value=0)
+                                                           implied_py_value=0)
     SafetyClassification = cp.EnumAttributeProperty('SafetyClassification',
                                                     implied_py_value=pm_types.SafetyClassification.INF,
                                                     enum_cls=pm_types.SafetyClassification)
     Type = cp.SubElementProperty(pm_qnames.Type, value_class=pm_types.CodedValue, is_optional=True)
     # pylint: enable=invalid-name
     _props = ('Handle', 'DescriptorVersion', 'SafetyClassification', 'Extension', 'Type')
     _child_elements_order = (ext.Extension, pm_qnames.Type)  # child elements in BICEPS order
```

### Comparing `sdc11073-2.0.0a4/src/sdc11073/mdib/devicemdib.py` & `sdc11073-2.0.0a5/src/sdc11073/mdib/devicemdib.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/mdib/devicemdibxtra.py` & `sdc11073-2.0.0a5/src/sdc11073/mdib/devicemdibxtra.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/mdib/devicewaveform.py` & `sdc11073-2.0.0a5/src/sdc11073/mdib/devicewaveform.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/mdib/mdibbase.py` & `sdc11073-2.0.0a5/src/sdc11073/mdib/mdibbase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/mdib/statecontainers.py` & `sdc11073-2.0.0a5/src/sdc11073/mdib/statecontainers.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     is_alert_signal = False
     is_alert_condition = False
     is_multi_state = False
     is_context_state = False
 
     Extension = cp.ExtensionNodeProperty(ext.Extension)
     DescriptorHandle = cp.HandleRefAttributeProperty('DescriptorHandle', is_optional=False)
-    DescriptorVersion = cp.ReferencedVersionAttributeProperty('DescriptorVersion', default_py_value=0)
-    StateVersion = cp.VersionCounterAttributeProperty('StateVersion', default_py_value=0)
+    DescriptorVersion = cp.ReferencedVersionAttributeProperty('DescriptorVersion', implied_py_value=0)
+    StateVersion = cp.VersionCounterAttributeProperty('StateVersion', implied_py_value=0)
     _props = ('Extension', 'DescriptorHandle', 'DescriptorVersion', 'StateVersion')
 
     def __init__(self, descriptor_container):
         super().__init__()
         self.descriptor_container = descriptor_container
         if descriptor_container is not None:
             # pylint: disable=invalid-name
@@ -223,15 +223,15 @@
 
 class MdsStateContainer(AbstractComplexDeviceComponentStateContainer):
     NODETYPE = pm.MdsState
     OperatingJurisdiction = cp.SubElementProperty(pm.OperatingJurisdiction,
                                                   value_class=pm_types.OperatingJurisdiction,
                                                   is_optional=True)
     OperatingMode = cp.EnumAttributeProperty('OperatingMode',
-                                             default_py_value=pm_types.MdsOperatingMode.NORMAL,
+                                             implied_py_value=pm_types.MdsOperatingMode.NORMAL,
                                              enum_cls=pm_types.MdsOperatingMode)
     Lang = cp.StringAttributeProperty('Lang', default_py_value='en')
     _props = ('OperatingJurisdiction', 'OperatingMode', 'Lang')
 
 
 class ScoStateContainer(AbstractDeviceComponentStateContainer):
     NODETYPE = pm.ScoState
```

### Comparing `sdc11073-2.0.0a4/src/sdc11073/mdib/transactions.py` & `sdc11073-2.0.0a5/src/sdc11073/mdib/transactions.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/netconn/__init__.py` & `sdc11073-2.0.0a5/src/sdc11073/netconn/__init__.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/observableproperties/observables.py` & `sdc11073-2.0.0a5/src/sdc11073/observableproperties/observables.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/observableproperties/valuecollector.py` & `sdc11073-2.0.0a5/src/sdc11073/observableproperties/valuecollector.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/pysoap/msgfactory.py` & `sdc11073-2.0.0a5/src/sdc11073/pysoap/msgfactory.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/pysoap/msgreader.py` & `sdc11073-2.0.0a5/src/sdc11073/pysoap/msgreader.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclient.py` & `sdc11073-2.0.0a5/src/sdc11073/pysoap/soapclient.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclient_async.py` & `sdc11073-2.0.0a5/src/sdc11073/pysoap/soapclient_async.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclientpool.py` & `sdc11073-2.0.0a5/src/sdc11073/pysoap/soapclientpool.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/pysoap/soapenvelope.py` & `sdc11073-2.0.0a5/src/sdc11073/pysoap/soapenvelope.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/roles/alarmprovider.py` & `sdc11073-2.0.0a5/src/sdc11073/roles/alarmprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/roles/audiopauseprovider.py` & `sdc11073-2.0.0a5/src/sdc11073/roles/audiopauseprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/roles/clockprovider.py` & `sdc11073-2.0.0a5/src/sdc11073/roles/clockprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/roles/contextprovider.py` & `sdc11073-2.0.0a5/src/sdc11073/roles/contextprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/roles/metricprovider.py` & `sdc11073-2.0.0a5/src/sdc11073/roles/metricprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/roles/nomenclature.py` & `sdc11073-2.0.0a5/src/sdc11073/roles/nomenclature.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/roles/patientcontextprovider.py` & `sdc11073-2.0.0a5/src/sdc11073/roles/patientcontextprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/roles/product.py` & `sdc11073-2.0.0a5/src/sdc11073/roles/product.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/roles/providerbase.py` & `sdc11073-2.0.0a5/src/sdc11073/roles/providerbase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/components.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/components.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/manipulator.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/manipulator.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/operations.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/operations.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/request_handler_deferred.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/request_handler_deferred.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/sdcclientimpl.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/sdcclientimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/subscription.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/subscription.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/contextservice.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/contextservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/getservice.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/getservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/localizationservice.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/localizationservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/setservice.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/setservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/stateeventservice.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcclient/serviceclients/stateeventservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/components.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/components.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/dpwshostedservice.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/dpwshostedservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/intervaltimer.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/intervaltimer.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/operations.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/operations.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/periodicreports.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/periodicreports.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/sco.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/sco.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/scopesfactory.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/scopesfactory.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/sdcdeviceimpl.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/sdcdeviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/servicesfactory.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/servicesfactory.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/subscriptionmgr.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr_async.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/subscriptionmgr_async.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr_base.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/subscriptionmgr_base.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/waveforms.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/waveforms.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/localizationservice.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/localizationservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/porttypebase.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/porttypebase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py` & `sdc11073-2.0.0a5/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/common.py` & `sdc11073-2.0.0a5/src/sdc11073/wsdiscovery/common.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/networkingthread.py` & `sdc11073-2.0.0a5/src/sdc11073/wsdiscovery/networkingthread.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/service.py` & `sdc11073-2.0.0a5/src/sdc11073/wsdiscovery/service.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/wsdimpl.py` & `sdc11073-2.0.0a5/src/sdc11073/wsdiscovery/wsdimpl.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,19 @@
     from sdc11073.xml_types.msg_types import MessageType
 
 WSA_ANONYMOUS = nsh.WSA.namespace + '/anonymous'
 ADDRESS_ALL = "urn:docs-oasis-open-org:ws-dd:ns:discovery:2009:01"  # format acc to RFC 2141
 
 NS_D = nsh.WSD.namespace
 
+# AppSequence node is mandatory acc. to text is wsdicovery spec, but in reality this is sometimes missing.
+# An application can decide to modify this value if it seems appropriate.
+# If allow_missing_app_sequence is True, the message is accepted and an InstanceId of 0 is used.
+# If allow_missing_app_sequence is False and the element is missing, the whole message will be ignored.
+allow_missing_app_sequence = False
 
 class MatchBy(str, Enum):
     """Different Match Options."""
 
     ldap = NS_D + '/ldap'  # "http://docs.oasis-open.org/ws-dd/ns/discovery/2009/01/ldap"
     uri = NS_D + '/rfc3986'  # "http://docs.oasis-open.org/ws-dd/ns/discovery/2009/01/rfc3986"
     uuid = NS_D + '/uuid'  # "http://docs.oasis-open.org/ws-dd/ns/discovery/2009/01/uuid"
@@ -263,15 +268,15 @@
 
         if x_addrs contains item, which includes {ip} pattern, one item per IP address will be sent
         """
         if not self._server_started:
             raise ApiUsageError("Server not started")
 
         metadata_version = self._local_services[epr].metadata_version + 1 if epr in self._local_services else 1
-        instance_id = str(random.randint(1, 0xFFFFFFFF))
+        instance_id = str(random.randint(1, 0xFFFFFFFF))  # Noqa: S311
         service = Service(types, scopes, x_addrs, epr, instance_id, metadata_version=metadata_version)
         self._logger.info('publishing %r', service)
         self._local_services[epr] = service
         self._send_hello(service)
 
     def clear_remote_services(self):
         """Clear remotely discovered services."""
@@ -361,20 +366,28 @@
 
     def _remove_remote_service(self, epr: str):
         if epr in self._remote_services:
             del self._remote_services[epr]
 
     def _handle_received_hello(self, received_message: ReceivedMessage, addr_from: str):
         app_sequence_node = received_message.p_msg.header_node.find(nsh.WSD.tag('AppSequence'))
-        app_sequence = wsd_types.AppSequenceType.from_node(app_sequence_node)
+        if app_sequence_node is None:
+            if allow_missing_app_sequence:
+                instance_id = 0
+            else:
+                self._logger.debug('received Hello from %r without AppSequence, ignoring it', addr_from)
+                return
+        else:
+            app_sequence = wsd_types.AppSequenceType.from_node(app_sequence_node)
+            instance_id = app_sequence.InstanceId
         hello = wsd_types.HelloType.from_node(received_message.p_msg.msg_node)
         epr = hello.EndpointReference.Address
         scopes = hello.Scopes
         service = Service(hello.Types, scopes, hello.XAddrs, epr,
-                          app_sequence.InstanceId, metadata_version=hello.MetadataVersion)
+                          instance_id, metadata_version=hello.MetadataVersion)
         self._add_remote_service(service)
         if not hello.XAddrs:  # B.D.
             self._logger.debug('%s(%s) has no Xaddr, sending resolve message', epr, addr_from)
             self._send_resolve(epr)
         if self._remote_service_hello_callback is not None:
             if matches_filter(service,
                               self._remote_service_hello_callback_types_filter,
@@ -388,22 +401,30 @@
         if services:
             self._send_probe_match(services, received_message.p_msg.header_info_block.MessageID, addr_from)
         if self._on_probe_callback is not None:
             self._on_probe_callback(addr_from, probe)
 
     def _handle_received_probe_matches(self, received_message: ReceivedMessage, addr_from: str):
         app_sequence_node = received_message.p_msg.header_node.find(nsh.WSD.tag('AppSequence'))
-        app_sequence = wsd_types.AppSequenceType.from_node(app_sequence_node)
+        if app_sequence_node is None:
+            if allow_missing_app_sequence:
+                instance_id = 0
+            else:
+                self._logger.debug('received ProbeMatches from %r without AppSequence, ignoring it', addr_from)
+                return
+        else:
+            app_sequence = wsd_types.AppSequenceType.from_node(app_sequence_node)
+            instance_id = app_sequence.InstanceId
         probe_matches = wsd_types.ProbeMatchesType.from_node(received_message.p_msg.msg_node)
         self._logger.debug('handle_received_message: len(ProbeMatch) = %d', len(probe_matches.ProbeMatch))
         for match in probe_matches.ProbeMatch:
             epr = match.EndpointReference.Address
             scopes = match.Scopes
             service = Service(match.Types, scopes, match.XAddrs, epr,
-                              app_sequence.InstanceId, metadata_version=match.MetadataVersion)
+                              instance_id, metadata_version=match.MetadataVersion)
             self._add_remote_service(service)
             if match.XAddrs is None or len(match.XAddrs) == 0:
                 self._logger.info('%s(%s) has no Xaddr, sending resolve message', epr, addr_from)
                 self._send_resolve(epr)
             elif not match.Types:
                 self._logger.info('%s(%s) has no Types, sending resolve message', epr, addr_from)
                 self._send_resolve(epr)
@@ -416,21 +437,29 @@
         epr = resolve.EndpointReference.Address
         if epr in self._local_services:
             service = self._local_services[epr]
             self._send_resolve_match(service, received_message.p_msg.header_info_block.MessageID, addr_from)
 
     def _handle_received_resolve_matches(self, received_message: ReceivedMessage, addr_from: str): # noqa ARG002
         app_sequence_node = received_message.p_msg.header_node.find(nsh.WSD.tag('AppSequence'))
-        app_sequence = wsd_types.AppSequenceType.from_node(app_sequence_node)
+        if app_sequence_node is None:
+            if allow_missing_app_sequence:
+                instance_id = 0
+            else:
+                self._logger.debug('received ResolveMatches from %r without AppSequence, ignoring it', addr_from)
+                return
+        else:
+            app_sequence = wsd_types.AppSequenceType.from_node(app_sequence_node)
+            instance_id = app_sequence.InstanceId
         resolve_matches = wsd_types.ResolveMatchesType.from_node(received_message.p_msg.msg_node)
         match = resolve_matches.ResolveMatch
         epr = match.EndpointReference.Address
         scopes = match.Scopes
         service = Service(match.Types, scopes, match.XAddrs, epr,
-                          app_sequence.InstanceId, metadata_version=match.MetadataVersion)
+                          instance_id, metadata_version=match.MetadataVersion)
         self._add_remote_service(service)
         if self._remote_service_resolve_match_callback is not None:
             self._remote_service_resolve_match_callback(service)
 
     def _handle_received_bye(self, received_message: ReceivedMessage, addr_from: str):
         bye = wsd_types.ByeType.from_node(received_message.p_msg.msg_node)
         epr = bye.EndpointReference.Address
```

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/actions.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/actions.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/addressing_types.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/addressing_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/basetypes.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/basetypes.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/dataconverters.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/dataconverters.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/dpws_types.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/dpws_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/eventing_types.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/eventing_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/isoduration.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/isoduration.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/mex_types.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/mex_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/msg_qnames.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/msg_qnames.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/msg_types.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/msg_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/pm_qnames.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/pm_qnames.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/pm_types.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/pm_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """ Implementation of data types used in Participant Model"""
+from __future__ import annotations
+
 import inspect
 import sys
 from dataclasses import dataclass
 from decimal import Decimal
 from typing import Optional, Union
 
 from lxml import etree as etree_
-from .basetypes import StringEnum, XMLTypeBase
+
+from ..namespaces import QN_TYPE, text_to_qname
 from . import ext_qnames as ext
 from . import msg_qnames as msg
 from . import pm_qnames as pm
 from . import xml_structure as cp
-from ..namespaces import QN_TYPE, text_to_qname
+from .basetypes import StringEnum, XMLTypeBase
 
 
 class SafetyClassification(StringEnum):
     INF = 'Inf'
     MED_A = 'MedA'
     MED_B = 'MedB'
     MED_C = 'MedC'
@@ -1068,32 +1071,49 @@
         # pylint: disable=invalid-name
         self.Value = value
         if reference_range is not None:
             self.ReferenceRange = reference_range
         # pylint: enable=invalid-name
 
 
+class CriticalityEnum(StringEnum):
+    Low = 'Lo'
+    High = 'Hi'
+
+
 class ClinicalInfo(PropertyBasedPMType):
     # pylint: disable=invalid-name
     NODETYPE = pm.ClinicalInfo
-    Type = cp.SubElementProperty(pm.Type, value_class=CodedValue)  # optional
+    Type = cp.SubElementProperty(pm.Type, value_class=CodedValue, is_optional=True)
+    Code = cp.SubElementProperty(pm.Type, value_class=CodedValue, is_optional=True)
+    Criticality = cp.NodeEnumTextProperty(pm.Criticality, CriticalityEnum,
+                                          is_optional=True, implied_py_value=CriticalityEnum.Low)
     Description = cp.SubElementListProperty(pm.Description, value_class=LocalizedText)  # 0...n
     RelatedMeasurement = cp.SubElementListProperty(pm.RelatedMeasurement, value_class=Measurement)  # 0...n
     # pylint: enable=invalid-name
-    _props = ['Type', 'Description', 'RelatedMeasurement']
+    _props = ['Type', 'Code', 'Criticality', 'Description', 'RelatedMeasurement']
 
-    def __init__(self, type_code=None, descriptions=None, related_measurements=None):
-        """
-        :param type_code: a CodedValue Instance
+    def __init__(self, type_: CodedValue | None = None,
+                 code: CodedValue | None = None,
+                 criticality: CriticalityEnum | None = None,
+                 descriptions: list[LocalizedText] | None=None,
+                 related_measurements: list[Measurement] | None = None):
+        """Potential clinical harm if this clinical information is not considered while treating the patient.
+
+        :param type_: a CodedValue instance
+        :param code: a CodedValue instance
+        :param criticality: a CriticalityEnum iInstance
         :param descriptions: a list of LocalizedText objects
         :param related_measurements: a list of Measurement objects
         """
         super().__init__()
         # pylint: disable=invalid-name
-        self.Type = type_code
+        self.Type = type_
+        self.Code = code
+        self.Criticality = criticality
         if descriptions:
             self.Description = descriptions
         if related_measurements:
             self.RelatedMeasurement = related_measurements
         # pylint: enable=invalid-name
```

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/wsd_types.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/wsd_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xml_types/xml_structure.py` & `sdc11073-2.0.0a5/src/sdc11073/xml_types/xml_structure.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,87 @@
-""" Classes in this module are used to declare the place where a xml value is located inside a document.
+"""Classes in this module are used to declare the place where a xml value is located inside a document.
+
 They also provide a mapping between XML data types (which are always stings in specific formats) and
 python types. By doing so these classes completely hide the XML nature of data.
 The basic offered types are Element, list of elements, attribute, and list of attributes.
 They are the buildings blocks that are needed to declare XML data types.
 Container properties represent values in xml nodes.
 """
-
 from __future__ import annotations
+
 import copy
 import time
+from abc import ABC, abstractmethod
 from collections import OrderedDict
-from datetime import datetime, date
-from typing import Union
+from datetime import date, datetime
+from typing import TYPE_CHECKING, Any, Callable
+
 from lxml import etree as etree_
 
+from sdc11073.exceptions import ApiUsageError
+from sdc11073.namespaces import QN_TYPE, docname_from_qname, text_to_qname
+
 from . import isoduration
-from .dataconverters import DataConverterProtocol
-from .dataconverters import DurationConverter, ClassCheckConverter, ListConverter, EnumConverter
-from .dataconverters import StringConverter, NullConverter
-from .dataconverters import TimestampConverter, DecimalConverter, IntegerConverter, BooleanConverter
-from ..exceptions import ApiUsageError
-from ..namespaces import QN_TYPE, docname_from_qname, text_to_qname
+from .dataconverters import (
+    BooleanConverter,
+    ClassCheckConverter,
+    DecimalConverter,
+    DurationConverter,
+    EnumConverter,
+    IntegerConverter,
+    ListConverter,
+    NullConverter,
+    StringConverter,
+    TimestampConverter,
+)
+
+if TYPE_CHECKING:
+    from decimal import Decimal
+    from .dataconverters import DataConverterProtocol
 
+    from sdc11073.namespaces import NamespaceHelper
 
 STRICT_TYPES = True  # if True, only the expected types are excepted.
 MANDATORY_VALUE_CHECKING = True  # checks if mandatory values are present when xml is generated
 
 
-class ElementNotFoundException(Exception):
+class ElementNotFoundError(Exception):  # Noqa: D101
     pass
 
+
 class _NumberStack:
     # uses as a part of _local_var_name in _XmlStructureBaseProperty.
     # This makes duplicate names impossible
     _value = 0
+
     @classmethod
     def unique_number(cls) -> str:
         cls._value += 1
         return str(cls._value)
 
 
-class _XmlStructureBaseProperty:
-    """ This defines a python property that converts between Python Data Types and XML data types.
+class _XmlStructureBaseProperty(ABC):
+    """_XmlStructureBaseProperty defines a python property that converts between Python Data Types and XML data types.
+
     It has knowledge about two things:
     - how to covert data from xml to python type and vice versa
     - name/ location of the xml data in a node.
 
     All derived Properties have the same interface:
     __get__ and __set__ : read and write access, using Python data types.
     get_py_value_from_node: reads the value from XML data and converts it to Python data type.
     update_xml_value: convert the Python data type to XML type and write it to XML node.
-     """
+    """
 
-    def __init__(self, local_var_name: str, value_converter: DataConverterProtocol,
-                 default_py_value=None, implied_py_value=None, is_optional=False):
-        """
+    def __init__(self, local_var_name: str,  # Noqa: PLR0913
+                 value_converter: DataConverterProtocol,
+                 default_py_value: Any | None = None,
+                 implied_py_value: Any | None = None,
+                 is_optional: bool = False):
+        """Construct an instance.
 
         :param local_var_name: a member with this same is added to instance
         :param value_converter: DataConverterProtocol
         :param default_py_value: initial value when initialized
                                  (should be set for mandatory elements, otherwise created xml might violate schema)
                                  and if the xml element does not exist.
         :param implied_py_value: for optional elements, this is the value that shall be implied if
@@ -85,652 +108,743 @@
         if implied_py_value is not None:
             self._implied_py_value = implied_py_value
         self._is_optional = is_optional
         self._local_var_name = local_var_name
         self._is_default_value_set = False
 
     @property
-    def is_optional(self):
+    def is_optional(self) -> bool:
         return self._is_optional
 
-    def __get__(self, instance, owner):
-        """ returns a python value, uses the locally stored value"""
+    def __get__(self, instance, owner) -> Any:  # Noqa ANN001
+        """Return a python value, use the locally stored value."""
         if instance is None:  # if called via class
             return self
         try:
             value = getattr(instance, self._local_var_name)
         except AttributeError:
             value = None
         if value is None:
             value = self._implied_py_value
         return value
 
-    def get_actual_value(self, instance):
-        """ Returns the actual value without considering default value and implied value,
-        e.g. returns None if no value in xml exists.
-        :param instance: the instance that has the property as member"""
+    def get_actual_value(self, instance: Any) -> Any | None:
+        """Return the actual value without considering default value and implied value.
+
+        E.g. return None if no value in xml exists.
+        :param instance: the instance that has the property as member
+        """
         try:
             return getattr(instance, self._local_var_name)
         except AttributeError:
             return None
 
-    def __set__(self, instance, py_value):
-        """value is the representation on the program side, e.g a float. """
+    def __set__(self, instance, py_value):  # Noqa ANN001
+        """Value is the representation on the program side, e.g a float."""
         if STRICT_TYPES:
             self._converter.check_valid(py_value)
         setattr(instance, self._local_var_name, py_value)
 
-    def init_instance_data(self, instance):
-        """
-        Sets initial values to default_py_value.
+    def init_instance_data(self, instance: Any):
+        """Set initial values to default_py_value.
+
         This method is used internally and should not be called by application.
         :param instance: the instance that has the property as member
         :return: None
         """
         if self._default_py_value is not None:
             setattr(instance, self._local_var_name, copy.deepcopy(self._default_py_value))
 
-    def update_xml_value(self, instance, node: etree_.Element):
-        """
-        Updates node with current data from instance.
+    @abstractmethod
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Update node with current data from instance.
+
         This method is used internally and should not be called by application.
         :param instance: the instance that has the property as member
         :param node: the etree node that shall be updated
         :return: None
         """
-        # to be defined in derived classes
-        raise NotImplementedError
 
-    def get_py_value_from_node(self, instance, node: etree_.Element):
-        """
-        Reads data from node.
+    @abstractmethod
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element):
+        """Read data from node.
+
         This method is used internally and should not be called by application.
         :param instance: the instance that has the property as member
         :param node: the etree node that provides the value
         :return: value
         """
-        # to be defined in derived classes
-        raise NotImplementedError
 
-    def update_from_node(self, instance, node: etree_.Element):
-        """
-        Updates instance data with data from node.
+    def update_from_node(self, instance: Any, node: etree_.Element):
+        """Update instance data with data from node.
+
         This method is used internally and should not be called by application.
         :param instance:the instance that has the property as member
         :param node:the etree node that provides the value
         :return: value
         :return:
         """
         value = self.get_py_value_from_node(instance, node)
         setattr(instance, self._local_var_name, value)
 
 
 class _AttributeBase(_XmlStructureBaseProperty):
-    """ Base class that represents an XML Attribute.
-    XML Representation is a string, Python representation is determined by value_converter."""
+    """Base class that represents an XML Attribute.
+
+    The XML Representation is a string.
+    The python representation is determined by value_converter.
+    """
+
+    def __init__(self, attribute_name: str,  # Noqa: PLR0913
+                 value_converter: DataConverterProtocol | None = None,
+                 default_py_value: Any = None,
+                 implied_py_value: Any = None,
+                 is_optional: bool = True):
+        """Construct an instance.
 
-    def __init__(self, attribute_name: str, value_converter=None,
-                 default_py_value=None, implied_py_value=None, is_optional=True):
-        """
-        Represents an attribute in xml.
         :param attribute_name: name of the attribute in xml node
         :param value_converter: converter between xml value and python value
         :param default_py_value: see base class doc.
         :param implied_py_value: see base class doc.
         :param is_optional: see base class doc.
         """
         if isinstance(attribute_name, etree_.QName):
             local_var_name = f'_a_{attribute_name.localname}_{_NumberStack.unique_number()}'
         else:
             local_var_name = f'_a_{attribute_name.lower()}_{_NumberStack.unique_number()}'
         super().__init__(local_var_name, value_converter, default_py_value, implied_py_value, is_optional)
         self._attribute_name = attribute_name
 
-    def get_py_value_from_node(self, instance, node):
-        value = self._default_py_value
-        try:
-            xml_value = node.attrib.get(self._attribute_name)
-            if xml_value is not None:
-                value = self._converter.to_py(xml_value)
-        except ElementNotFoundException:
-            pass
-        return value
+    def get_py_value_from_node(self, instance: Any,  # Noqa: ARG002
+                               node: etree_.Element | None) -> Any:
+        xml_value = None if node is None else node.attrib.get(self._attribute_name)
+        return None if xml_value is None else self._converter.to_py(xml_value)
 
-    def update_xml_value(self, instance, node: etree_.Element):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:
             # this can only happen if there is no default value defined and __set__ has never been called
             py_value = None
         if py_value is None:
             if MANDATORY_VALUE_CHECKING and not self.is_optional:
                 raise ValueError(f'mandatory value {self._attribute_name} missing')
             try:
-                if self._attribute_name in node.attrib.keys():
+                if self._attribute_name in node.attrib:
                     del node.attrib[self._attribute_name]
-            except ElementNotFoundException:
+            except ElementNotFoundError:
                 return
         else:
             xml_value = self._converter.to_xml(py_value)
             node.set(self._attribute_name, xml_value)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f'{self.__class__.__name__} attribute {self._attribute_name}'
 
 
-class _ElementBase(_XmlStructureBaseProperty):
-    """ Base class that represents an XML Element."""
+class _ElementBase(_XmlStructureBaseProperty, ABC):
+    """_ElementBase represents an XML Element."""
 
-    def __init__(self, sub_element_name: Union[etree_.QName, None], value_converter, default_py_value=None, implied_py_value=None,
-                 is_optional=False):
-        """
-        Represents a (sub) element in xml.
-        :param sub_element_name: a QName or None
-                                if None, the property represents the node itself, otherwise the sub node with given name.
+    def __init__(self, sub_element_name: etree_.QName | None, # Noqa: PLR0913
+                 value_converter: DataConverterProtocol,
+                 default_py_value: Any = None,
+                 implied_py_value: Any = None,
+                 is_optional: bool = False):
+        """Construct the representation of a (sub) element in xml.
+
+        :param sub_element_name: a QName or None. If None, the property represents the node itself,
+                                 otherwise the sub node with given name.
+        :param value_converter: see base class doc.
         :param default_py_value: see base class doc.
         :param implied_py_value: see base class doc.
         :param is_optional: see base class doc.
         """
         if sub_element_name is None:
             local_var_name = f'_e_{_NumberStack.unique_number()}'
         else:
             local_var_name = f'_e_{sub_element_name.localname.lower()}_{_NumberStack.unique_number()}'
         super().__init__(local_var_name, value_converter, default_py_value, implied_py_value, is_optional)
         self._sub_element_name = sub_element_name
 
     @staticmethod
-    def _get_element_by_child_name(node, sub_element_name, create_missing_nodes: bool):
+    def _get_element_by_child_name(node: etree_.Element,
+                                   sub_element_name: etree_.QName | None,
+                                   create_missing_nodes: bool) -> etree_.Element:
         if sub_element_name is None:
             return node
         sub_node = node.find(sub_element_name)
         if sub_node is None:
             if not create_missing_nodes:
-                raise ElementNotFoundException(f'Element {sub_element_name} not found in {node.tag}')
+                raise ElementNotFoundError(f'Element {sub_element_name} not found in {node.tag}')
             sub_node = etree_.SubElement(node, sub_element_name)  # create this node
         return sub_node
 
-    def remove_sub_element(self, node):
+    def remove_sub_element(self, node: etree_.Element):
         if self._sub_element_name is None:
             return
         sub_node = node.find(self._sub_element_name)
         if sub_node is not None:
             node.remove(sub_node)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f'{self.__class__.__name__} in sub element {self._sub_element_name}'
 
 
 class StringAttributeProperty(_AttributeBase):
     """Python representation is a string."""
 
-    def __init__(self, attribute_name: str, default_py_value=None, implied_py_value=None, is_optional=True):
+    def __init__(self, attribute_name: str,
+                 default_py_value: Any = None,
+                 implied_py_value: Any = None, is_optional: bool = True):
         super().__init__(attribute_name, StringConverter, default_py_value, implied_py_value, is_optional)
 
 
 class AnyURIAttributeProperty(StringAttributeProperty):
-    pass
+    """Represents an AnyURIAttribute."""
 
 
 class CodeIdentifierAttributeProperty(StringAttributeProperty):
-    pass
+    """Represents a CodeIdentifier attribute."""
 
 
 class HandleAttributeProperty(StringAttributeProperty):
-    pass
+    """Represents a Handle attribute."""
 
 
 class HandleRefAttributeProperty(StringAttributeProperty):
-    pass
+    """Represents a HandleRef attribute."""
 
 
 class SymbolicCodeNameAttributeProperty(StringAttributeProperty):
-    pass
+    """Represents a SymbolicCodeName attribute."""
 
 
 class ExtensionAttributeProperty(StringAttributeProperty):
-    pass
+    """Represents an Extension attribute."""
 
 
 class LocalizedTextRefAttributeProperty(StringAttributeProperty):
-    pass
+    """Represents a LocalizedTextRef attribute."""
 
 
 class TimeZoneAttributeProperty(StringAttributeProperty):
-    pass
+    """Represents a TimeZone attribute."""
 
 
 class EnumAttributeProperty(_AttributeBase):
-    """ Python representation is an Enum."""
+    """Base class for enum attributes."""
 
-    def __init__(self, attribute_name: str, enum_cls,
-                 default_py_value=None, implied_py_value=None, is_optional=True):
+    def __init__(self, attribute_name: str, # Noqa: PLR0913
+                 enum_cls: Any,
+                 default_py_value: Any = None,
+                 implied_py_value: Any = None,
+                 is_optional: bool = True):
         super().__init__(attribute_name, EnumConverter(enum_cls), default_py_value, implied_py_value, is_optional)
 
 
 class TimestampAttributeProperty(_AttributeBase):
-    """ XML notation is integer in milliseconds.
-    Python is a float in seconds."""
+    """Represents a Timestamp attribute.
+
+    XML notation is integer in milliseconds.
+    Python is a float in seconds.
+    """
 
-    def __init__(self, attribute_name: str, default_py_value=None, implied_py_value=None, is_optional=True):
+    def __init__(self, attribute_name: str,
+                 default_py_value: Any = None,
+                 implied_py_value: Any = None,
+                 is_optional: bool = True):
         super().__init__(attribute_name, value_converter=TimestampConverter,
                          default_py_value=default_py_value, implied_py_value=implied_py_value, is_optional=is_optional)
 
 
 class CurrentTimestampAttributeProperty(_AttributeBase):
-    """ used for ClockState, it always writes current time to node.
-    Setting value from python is possible, but makes no sense.
+    """Represents a special Timestamp attribute used for ClockState, it always writes current time to node.
+
+    Setting the value from python is possible, but makes no sense.
     """
 
-    def __init__(self, attribute_name, is_optional=True):
+    def __init__(self, attribute_name: str,
+                 is_optional: bool = True):
         super().__init__(attribute_name, value_converter=TimestampConverter,
                          default_py_value=None, is_optional=is_optional)
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         setattr(instance, self._local_var_name, time.time())
         super().update_xml_value(instance, node)
 
 
 class DecimalAttributeProperty(_AttributeBase):
-    """Python representation is a Decimal. """
+    """Represents a Decimal attribute."""
 
-    def __init__(self, attribute_name, default_py_value=None, implied_py_value=None, is_optional=True):
+    def __init__(self, attribute_name: str,
+                 default_py_value: Decimal | None = None,
+                 implied_py_value: Decimal | None = None,
+                 is_optional: bool = True):
         super().__init__(attribute_name, value_converter=DecimalConverter,
                          default_py_value=default_py_value, implied_py_value=implied_py_value, is_optional=is_optional)
 
 
 class QualityIndicatorAttributeProperty(DecimalAttributeProperty):
-    """BICEPS: A value between 0 and 1 """
+    """Represents a QualityIndicator attribute, a value between 0 and 1."""
 
 
 class DurationAttributeProperty(_AttributeBase):
-    """ XML notation is integer in milliseconds.
-    Python is a float in seconds."""
+    """Represents a Duration attribute.
+
+    XML notation is integer in milliseconds.
+    Python is a float in seconds.
+    """
 
-    def __init__(self, attribute_name, default_py_value=None, implied_py_value=None, is_optional=True):
+    def __init__(self, attribute_name: str,
+                 default_py_value: float | None = None,
+                 implied_py_value: float | None = None,
+                 is_optional: bool = True):
         super().__init__(attribute_name, value_converter=DurationConverter,
                          default_py_value=default_py_value, implied_py_value=implied_py_value, is_optional=is_optional)
 
 
 class IntegerAttributeProperty(_AttributeBase):
-    """ XML notation is an integer, python is an integer."""
+    """Represents an Integer attribute.
+
+    XML notation is an integer, python is an integer.
+    """
 
-    def __init__(self, attribute_name, default_py_value=None, implied_py_value=None, is_optional=True):
+    def __init__(self, attribute_name: str,
+                 default_py_value: int | None = None,
+                 implied_py_value: int | None = None,
+                 is_optional: bool = True):
         super().__init__(attribute_name, value_converter=IntegerConverter,
                          default_py_value=default_py_value, implied_py_value=implied_py_value, is_optional=is_optional)
 
 
 class UnsignedIntAttributeProperty(IntegerAttributeProperty):
-    """Python has no unsigned int, therefore this is the same as IntegerAttributeProperty. """
-    pass
+    """Represents an UnsignedInt attribute.
+
+    Python has no unsigned int, therefore this is the same as IntegerAttributeProperty.
+    """
 
 
 class VersionCounterAttributeProperty(UnsignedIntAttributeProperty):
-    """VersionCounter in BICEPS is unsigned long.
-    Python has no unsigned int, therefore this is the same as IntegerAttributeProperty. """
-    pass
+    """Represents a VersionCounter attribute.
+
+    VersionCounter in BICEPS is unsigned long.
+    Python has no unsigned long, therefore this is the same as IntegerAttributeProperty.
+    """
 
 
 class ReferencedVersionAttributeProperty(VersionCounterAttributeProperty):
-    pass
+    """Represents an ReferencedVersion attribute."""
 
 
 class BooleanAttributeProperty(_AttributeBase):
-    """ XML notation is 'true' or 'false'.
-    Python is a boolean."""
+    """Represents a Boolean attribute.
 
-    def __init__(self, attribute_name, default_py_value=None, implied_py_value=None, is_optional=True):
+    XML notation is 'true' or 'false'.
+    Python is a bool.
+    """
+
+    def __init__(self, attribute_name: str,
+                 default_py_value: bool | None = None,
+                 implied_py_value: bool | None = None,
+                 is_optional: bool = True):
         super().__init__(attribute_name, value_converter=BooleanConverter,
                          default_py_value=default_py_value, implied_py_value=implied_py_value, is_optional=is_optional)
 
 
 class QNameAttributeProperty(_AttributeBase):
-    """ XML Representation is a prefix:name string, Python representation is a QName."""
+    """Represents a qualified name attribute.
+
+    XML Representation is a prefix:name string, Python representation is a QName.
+    """
 
-    def __init__(self, attribute_name, default_py_value=None, implied_py_value=None, is_optional=True):
+    def __init__(self, attribute_name: str,
+                 default_py_value: etree_.QName | None = None,
+                 implied_py_value: etree_.QName | None = None,
+                 is_optional: bool = True):
         super().__init__(attribute_name, value_converter=ClassCheckConverter(etree_.QName),
                          default_py_value=default_py_value, implied_py_value=implied_py_value, is_optional=is_optional)
 
-    def get_py_value_from_node(self, instance, node):
-        """
-        :return: None or a QName
-        """
-        value = self._default_py_value
-        try:
-            xml_value = node.attrib.get(self._attribute_name)
-            if xml_value is not None:
-                value = text_to_qname(xml_value, node.nsmap)
-        except ElementNotFoundException:
-            pass
-        return value
+    def get_py_value_from_node(self, instance: Any,  # Noqa: ARG002
+                               node: etree_.Element | None) -> Any:
+        xml_value = None if node is None else node.attrib.get(self._attribute_name)
+        return None if xml_value is None else text_to_qname(xml_value, node.nsmap)
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:  # set to None
             py_value = None
         if py_value is None:
             py_value = self._default_py_value
         if py_value is None:
             if MANDATORY_VALUE_CHECKING and not self.is_optional:
                 raise ValueError(f'mandatory value {self._attribute_name} missing')
             try:
-                if self._attribute_name in node.attrib.keys():
+                if self._attribute_name in node.attrib:
                     del node.attrib[self._attribute_name]
-            except ElementNotFoundException:
+            except ElementNotFoundError:
                 return
         else:
             xml_value = docname_from_qname(py_value, node.nsmap)
             node.set(self._attribute_name, xml_value)
 
 
 class _AttributeListBase(_AttributeBase):
-    """ XML Representation is a string which is a space separated list.
-    Python representation is a list of strings if value_converter is None,
-    else a list of converted values."""
+    """Base class for a list of values as attribute.
 
-    def __init__(self, attribute_name, value_converter, is_optional=True):
+    XML Representation is a string which is a space separated list.
+    Python representation is a list of Any (type depends on ListConverter),
+    else a list of converted values.
+    """
+
+    _converter: ListConverter
+    def __init__(self, attribute_name: str,
+                 value_converter: ListConverter,
+                 is_optional: bool = True):
         super().__init__(attribute_name, value_converter, is_optional=is_optional)
 
-    def __get__(self, instance, owner):
-        """ returns a python value, uses the locally stored value"""
+    def __get__(self, instance, owner):  # Noqa ANN001
+        """Return a python value, use the locally stored value."""
         if instance is None:  # if called via class
             return self
         try:
             return getattr(instance, self._local_var_name)
         except AttributeError:
             setattr(instance, self._local_var_name, [])
             return getattr(instance, self._local_var_name)
 
-    def init_instance_data(self, instance):
+    def init_instance_data(self, instance: Any):
         setattr(instance, self._local_var_name, [])
 
-    def get_py_value_from_node(self, instance, node):
-        values = self._default_py_value
-        try:
-            xml_value = node.attrib.get(self._attribute_name)
-            if xml_value is not None:
-                split_result = xml_value.split(' ')
-                values = [self._converter.elem_to_py(val) for val in split_result if val]
-        except ElementNotFoundException:
-            pass
-        return values
+    def get_py_value_from_node(self, instance: Any,  # Noqa: ARG002
+                               node: etree_.Element | None) -> list[Any]:
+        xml_value = None if node is None else node.attrib.get(self._attribute_name)
+        if xml_value is not None:
+            split_result = xml_value.split(' ')
+            return [self._converter.elem_to_py(val) for val in split_result if val]
+        return []
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:
             # set to None (it is in the responsibility of the called method to do the right thing)
             py_value = None
         if not py_value and self.is_optional:  # is None:
             try:
-                if self._attribute_name in node.attrib.keys():
+                if self._attribute_name in node.attrib:
                     del node.attrib[self._attribute_name]
-            except ElementNotFoundException:
+            except ElementNotFoundError:
                 return
         else:
             if py_value is None:
                 if MANDATORY_VALUE_CHECKING and not self.is_optional:
                     raise ValueError(f'mandatory value {self._attribute_name} missing')
                 xml_value = ''
             else:
                 xml_value = ' '.join([self._converter.elem_to_xml(v) for v in py_value])
             node.set(self._attribute_name, xml_value)
 
 
 class _StringAttributeListBase(_AttributeListBase):
-    def __init__(self, attribute_name, value_converter=None):
+    """Base class for a list of strings as attribute.
+
+    XML Representation is a string which is a space separated list.
+    Python representation is a list of strings.
+    """
+
+    def __init__(self, attribute_name: str, value_converter: DataConverterProtocol | None = None):
         converter = value_converter or ListConverter(ClassCheckConverter(str))
         super().__init__(attribute_name, converter)
 
 
 class HandleRefListAttributeProperty(_StringAttributeListBase):
-    pass
+    """Represents a list of HandleRef attribute."""
 
 
 class EntryRefListAttributeProperty(_StringAttributeListBase):
-    pass
+    """Represents a list of EntryRef attribute."""
 
 
 class OperationRefListAttributeProperty(_StringAttributeListBase):
-    pass
+    """Represents a list of OperationRef attribute."""
 
 
 class AlertConditionRefListAttributeProperty(_StringAttributeListBase):
-    pass
+    """Represents a list of AlertConditionRef attribute."""
 
 
 class DecimalListAttributeProperty(_AttributeListBase):
-    """ XML representation: an attribute string that represents 0...n decimals, separated with spaces.
-        Python representation: List of Decimal if attribute is set (can be an empty list!), otherwise None.
-        """
+    """Represents a list of Decimal attribute.
+
+    XML representation: an attribute string that represents 0...n decimals, separated with spaces.
+    Python representation: List of Decimal if attribute is set (can be an empty list!), otherwise None.
+    """
 
-    def __init__(self, attribute_name):
+    def __init__(self, attribute_name: str):
         super().__init__(attribute_name, ListConverter(DecimalConverter))
 
 
 class NodeTextProperty(_ElementBase):
-    """ The handled data is the text of an element.
-    Python representation is a string."""
+    """Represents the text of an XML Element.
+
+    Python representation depends on value converter.
+    """
 
-    def __init__(self, sub_element_name, value_converter, default_py_value=None, implied_py_value=None,
-                 is_optional=False, min_length=0):
+    def __init__(self, sub_element_name: etree_.QName | None, # Noqa: PLR0913
+                 value_converter: DataConverterProtocol,
+                 default_py_value: Any | None = None,
+                 implied_py_value: Any | None = None,
+                 is_optional: bool = False,
+                 min_length: int = 0):
         super().__init__(sub_element_name, value_converter, default_py_value, implied_py_value, is_optional)
         self._min_length = min_length
 
-    def get_py_value_from_node(self, instance, node):
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         try:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=False)
             return self._converter.to_py(sub_node.text)
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             return self._default_py_value
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:  # set to None (it is in the responsibility of the called method to do the right thing)
             py_value = None
         if py_value is None:
             if MANDATORY_VALUE_CHECKING and not self.is_optional and self._min_length:
                 raise ValueError(f'mandatory value {self._sub_element_name} missing')
 
             if not self._sub_element_name:
                 # update text of this element
                 node.text = ''
+            elif self.is_optional:
+                sub_node = node.find(self._sub_element_name)
+                if sub_node is not None:
+                    node.remove(sub_node)
             else:
-                if self.is_optional:
-                    sub_node = node.find(self._sub_element_name)
-                    if sub_node is not None:
-                        node.remove(sub_node)
-                else:
-                    sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
-                    sub_node.text = None
+                sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
+                sub_node.text = None
         else:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
             sub_node.text = self._converter.to_xml(py_value)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'{self.__class__.__name__} in sub-element {self._sub_element_name}'
 
 
 class NodeStringProperty(NodeTextProperty):
-    """Python representation is a string."""
+    """Represents the text of an XML Element.
+
+    Python representation is a string.
+    """
 
-    def __init__(self, sub_element_name=None, default_py_value=None, implied_py_value=None, is_optional=False,
-                 min_length=0):
+    def __init__(self, sub_element_name: etree_.QName | None = None, # Noqa: PLR0913
+                 default_py_value: str | None = None,
+                 implied_py_value: str | None = None,
+                 is_optional: bool = False,
+                 min_length: int = 0):
         super().__init__(sub_element_name, StringConverter, default_py_value, implied_py_value, is_optional, min_length)
 
 
 class AnyUriTextElement(NodeStringProperty):
-    # for now the same as NodeStringProperty ,but later it could be handy to add uri type checking
-    pass
+    """For now the same as NodeStringProperty ,but later it could be handy to add uri type checking."""
 
 
-class LocalizedTextContentProperty(NodeStringProperty):
-    pass
+# class LocalizedTextContentProperty(NodeStringProperty):
+#     pass
 
 
 class NodeEnumTextProperty(NodeTextProperty):
-    """Python representation is an Enum."""
+    """Represents the text of an XML Element.
 
-    def __init__(self, sub_element_name, enum_cls, default_py_value=None, implied_py_value=None, is_optional=False):
+    Python representation is an enum.
+    """
+
+    def __init__(self, sub_element_name: etree_.QName | None,  # Noqa: PLR0913
+                 enum_cls: Any,
+                 default_py_value: Any | None = None,
+                 implied_py_value: Any | None = None,
+                 is_optional: bool = False):
         super().__init__(sub_element_name, EnumConverter(enum_cls), default_py_value, implied_py_value,
                          is_optional, min_length=1)
         self.enum_cls = enum_cls
 
 
 class NodeEnumQNameProperty(NodeTextProperty):
-    """Python representation is an Enum of QName, XML is prefix:localname."""
+    """Represents a qualified name as text of an XML Element.
+
+    Python representation is an Enum of QName, XML is prefix:localname.
+    """
 
-    def __init__(self, sub_element_name, enum_cls, default_py_value=None, implied_py_value=None, is_optional=False):
+    def __init__(self, sub_element_name: etree_.QName | None,  # Noqa: PLR0913
+                 enum_cls: Any,
+                 default_py_value: Any | None = None,
+                 implied_py_value: Any | None = None,
+                 is_optional: bool = False):
         super().__init__(sub_element_name, EnumConverter(enum_cls), default_py_value, implied_py_value,
                          is_optional, min_length=1)
         self.enum_cls = enum_cls
 
-    def get_py_value_from_node(self, instance, node):
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         try:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=False)
             prefix, localname = sub_node.text.split(':')
             namespace = node.nsmap[prefix]
             q_name = etree_.QName(namespace, localname)
             return self._converter.to_py(q_name)
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             return self._default_py_value
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:  # set to None (it is in the responsibility of the called method to do the right thing)
             py_value = None
         if py_value is None:
             if MANDATORY_VALUE_CHECKING and not self.is_optional and self._min_length:
                 raise ValueError(f'mandatory value {self._sub_element_name} missing')
 
             if not self._sub_element_name:
                 # update text of this element
                 node.text = ''
+            elif self.is_optional:
+                sub_node = node.find(self._sub_element_name)
+                if sub_node is not None:
+                    node.remove(sub_node)
             else:
-                if self.is_optional:
-                    sub_node = node.find(self._sub_element_name)
-                    if sub_node is not None:
-                        node.remove(sub_node)
-                else:
-                    sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
-                    sub_node.text = None
+                sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
+                sub_node.text = None
         else:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
             for prefix, namespace in sub_node.nsmap.items():
                 if namespace == py_value.value.namespace:
                     value = f'{prefix}:{py_value.value.localname}'
                     sub_node.text = self._converter.to_xml(value)
                     return
-            raise ValueError(f'no prefix for namespace "{namespace}"')
+            raise ValueError(f'no prefix for namespace "{py_value.value.namespace}"')
 
 
 class NodeIntProperty(NodeTextProperty):
-    """Python representation is a string."""
+    """Python representation is an int."""
 
-    def __init__(self, sub_element_name=None, default_py_value=None, implied_py_value=None, is_optional=False,
-                 min_length=0):
+    def __init__(self, sub_element_name: etree_.QName | None = None,  # Noqa: PLR0913
+                 default_py_value: int | None = None,
+                 implied_py_value: int | None = None,
+                 is_optional: bool = False,
+                 min_length: int = 0):
         super().__init__(sub_element_name, IntegerConverter, default_py_value, implied_py_value, is_optional,
                          min_length)
 
 
 class NodeTextQNameProperty(_ElementBase):
-    """ The handled data is a single qualified name in the text of an element
-    in the form prefix:localname"""
+    """The handled data is a single qualified name in the text of an element in the form prefix:localname."""
 
-    def __init__(self, sub_element_name, default_py_value=None, is_optional=False):
+    def __init__(self, sub_element_name: etree_.QName | None,
+                 default_py_value: etree_.QName | None = None,
+                 is_optional: bool = False):
         super().__init__(sub_element_name, ClassCheckConverter(etree_.QName), default_py_value,
                          is_optional=is_optional)
 
-    def get_py_value_from_node(self, instance, node):
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         try:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=False)
             xml_value = sub_node.text
             if xml_value is not None:
                 value = text_to_qname(xml_value, sub_node.nsmap)
                 return value
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             pass
         return self._default_py_value
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:  # set to None (it is in the responsibility of the called method to do the right thing)
             py_value = None
 
         if py_value is None:
             if not self._sub_element_name:
                 # update text of this element
                 node.text = ''
+            elif self.is_optional:
+                sub_node = node.find(self._sub_element_name)
+                if sub_node is not None:
+                    node.remove(sub_node)
             else:
-                if self.is_optional:
-                    sub_node = node.find(self._sub_element_name)
-                    if sub_node is not None:
-                        node.remove(sub_node)
-                else:
-                    if MANDATORY_VALUE_CHECKING and not self.is_optional:
-                        raise ValueError(f'mandatory value {self._sub_element_name} missing')
-                    sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
-                    sub_node.text = None
+                if MANDATORY_VALUE_CHECKING and not self.is_optional:
+                    raise ValueError(f'mandatory value {self._sub_element_name} missing')
+                sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
+                sub_node.text = None
         else:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
             value = docname_from_qname(py_value, sub_node.nsmap)
             sub_node.text = value
 
 
 class _ExtensionLocalValue:
-    def __init__(self, value):
+    def __init__(self, value: Any):
         self.value = value or OrderedDict()
 
-    def __eq__(self, other):
+    def __eq__(self, other: _ExtensionLocalValue) -> bool:
         if other is None:
             return len(self.value) == 0
         return self.value == other.value
 
 
 class ExtensionNodeProperty(_ElementBase):
-    """ Represents an ext:Extension Element that contains xml tree of any kind."""
+    """Represents an ext:Extension Element that contains xml tree of any kind."""
 
-    def __init__(self, sub_element_name, default_py_value=None):
+    def __init__(self, sub_element_name: etree_.QName | None, default_py_value: Any | None = None):
         super().__init__(sub_element_name, ClassCheckConverter(_ExtensionLocalValue), default_py_value,
                          is_optional=True)
 
-    def __get__(self, instance, owner):
-        """ returns a python value, uses the locally stored value"""
+    def __get__(self, instance, owner):  # Noqa ANN001
+        """Return a python value, uses the locally stored value."""
         if instance is None:  # if called via class
             return self
         try:
             value = getattr(instance, self._local_var_name)
         except AttributeError:
             value = None
         if value is None:
             value = _ExtensionLocalValue(None)
             setattr(instance, self._local_var_name, value)
         return value
 
-    def get_py_value_from_node(self, instance, node):
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:
+        """Read value from node."""
         try:
             extension_nodes = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=False)
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             return None
         values = OrderedDict()
         for extension_node in extension_nodes:
             try:
                 cls = instance.extension_class_lookup.get(extension_node.tag)
             except AttributeError:
                 cls = None
             if cls:
                 values[extension_node.tag] = cls.from_node(extension_node)
             else:
                 values[extension_node.tag] = extension_node
         return _ExtensionLocalValue(values)
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             extension_local_value = getattr(instance, self._local_var_name)
         except AttributeError:
             extension_local_value = None
         if extension_local_value is None:
             sub_node = node.find(self._sub_element_name)
             if sub_node is not None:
@@ -741,77 +855,80 @@
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
 
             del sub_node[:]  # delete all children first
 
             for tag, val in extension_local_value.value.items():
                 if val is None:
                     continue
-                if hasattr(val, 'as_etree_node'):
-                    _node = val.as_etree_node(tag, node.nsmap)
-                else:
-                    _node = val
+                _node = val.as_etree_node(tag, node.nsmap) if hasattr(val, 'as_etree_node') else val
                 sub_node.append(copy.copy(_node))
 
+
 class AnyEtreeNodeProperty(_ElementBase):
-    """ Represents an Element that contains xml tree of any kind."""
+    """Represents an Element that contains xml tree of any kind."""
 
-    def __init__(self, sub_element_name, is_optional=False):
+    def __init__(self, sub_element_name: etree_.QName | None, is_optional: bool = False):
         super().__init__(sub_element_name, NullConverter, default_py_value=None,
                          is_optional=is_optional)
 
-    def get_py_value_from_node(self, instance, node):
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         try:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=False)
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             return None
         return sub_node[:]  # all children
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:  # set to None (it is in the responsibility of the called method to do the right thing)
             py_value = None
 
         if py_value is None:
             if self.is_optional:
                 sub_node = node.find(self._sub_element_name)
                 if sub_node is not None:
                     node.remove(sub_node)
-            else:
-                if MANDATORY_VALUE_CHECKING and not self.is_optional:
-                    raise ValueError(f'mandatory value {self._sub_element_name} missing')
-                sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
+            elif MANDATORY_VALUE_CHECKING:
+                raise ValueError(f'mandatory value {self._sub_element_name} missing')
         else:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
-            if isinstance(py_value, etree_._Element):
+            if isinstance(py_value, etree_._Element):  # Noqa: SLF001
                 sub_node.append(py_value)
             else:
                 sub_node.extend(py_value)
 
 
 class SubElementProperty(_ElementBase):
-    """ uses a value that has an "as_etree_node" method"""
+    """Uses a value that has an "as_etree_node" method."""
 
-    def __init__(self, sub_element_name, value_class, default_py_value=None,
-                 implied_py_value=None, is_optional=False):
+    def __init__(self, sub_element_name: etree_.QName | None,  # Noqa: PLR0913
+                 value_class: Any,
+                 default_py_value: Any | None = None,
+                 implied_py_value: Any | None = None,
+                 is_optional: bool = False):
         super().__init__(sub_element_name, ClassCheckConverter(value_class), default_py_value, implied_py_value,
                          is_optional)
         self.value_class = value_class
 
-    def get_py_value_from_node(self, instance, node):
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         value = self._default_py_value
         try:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=False)
             value_class = self.value_class.value_class_from_node(sub_node)
             value = value_class.from_node(sub_node)
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             pass
         return value
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:
             py_value = self._default_py_value
 
         if py_value is None:
             if not self.is_optional:
@@ -824,38 +941,52 @@
                     and py_value.NODETYPE != self.value_class.NODETYPE:
                 # set xsi type
                 sub_node.set(QN_TYPE, docname_from_qname(py_value.NODETYPE, node.nsmap))
             node.append(sub_node)
 
 
 class ContainerProperty(_ElementBase):
-    """ a value that has "mk_node" and cls.from_node methods"""
+    """ContainerProperty supports xsi:type information from xml and instantiates value accordingly."""
 
-    def __init__(self, sub_element_name, value_class, cls_getter, ns_helper, is_optional=False):
+    def __init__(self, sub_element_name: etree_.QName | None,  # Noqa: PLR0913
+                 value_class: Any,
+                 cls_getter: Callable[[etree_.QName], type],
+                 ns_helper: NamespaceHelper,
+                 is_optional: bool = False):
+        """Construct a ContainerProperty.
+
+        :param sub_element_name: see doc of base class
+        :param value_class: Default value class if no xsi:type is found
+        :param cls_getter: function that returns a class for xsi:type QName
+        :param ns_helper: name space helper that knows current prefixes
+        :param is_optional: see doc of base class
+        """
         super().__init__(sub_element_name, ClassCheckConverter(value_class), is_optional=is_optional)
         self.value_class = value_class
         self._cls_getter = cls_getter
         self._ns_helper = ns_helper
 
-    def get_py_value_from_node(self, instance, node):
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         value = self._default_py_value
         try:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=False)
             node_type_str = sub_node.get(QN_TYPE)
             if node_type_str is not None:
                 node_type = text_to_qname(node_type_str, node.nsmap)
                 value_class = self._cls_getter(node_type)
             else:
                 value_class = self.value_class
             value = value_class.from_node(sub_node)
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             pass
         return value
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:
             py_value = self._default_py_value
 
         if py_value is None:
             if not self.is_optional:
@@ -867,110 +998,118 @@
             sub_node = py_value.mk_node(self._sub_element_name, self._ns_helper)
             if py_value.NODETYPE != self.value_class.NODETYPE:
                 # set xsi type
                 sub_node.set(QN_TYPE, docname_from_qname(py_value.NODETYPE, node.nsmap))
             node.append(sub_node)
 
 
-class _ElementListProperty(_ElementBase):
-    def __get__(self, instance, owner):
-        """ returns a python value, uses the locally stored value"""
+class _ElementListProperty(_ElementBase, ABC):
+    def __get__(self, instance, owner):  # Noqa ANN001
+        """Return a python value, uses the locally stored value."""
         if instance is None:  # if called via class
             return self
         try:
             return getattr(instance, self._local_var_name)
         except AttributeError:
             setattr(instance, self._local_var_name, [])
             return getattr(instance, self._local_var_name)
 
-    def init_instance_data(self, instance):
+    def init_instance_data(self, instance: Any):
         setattr(instance, self._local_var_name, [])
 
-    def get_py_value_from_node(self, instance, node):
-        # still not implemented here, to be defined in derived classes
-        raise NotImplementedError
-
-    def update_xml_value(self, instance, node):
-        # still not implemented here, to be defined in derived classes
-        raise NotImplementedError
-
 
 class SubElementListProperty(_ElementListProperty):
-    """ a list of values that have an "as_etree_node" method. Used if maxOccurs="Unbounded" in BICEPS_ParticipantModel"""
+    """SubElementListProperty is  a list of values that have an "as_etree_node" method.
+
+    Used if maxOccurs="Unbounded" in BICEPS_ParticipantModel.
+    """
 
-    def __init__(self, sub_element_name, value_class, is_optional=True):
+    def __init__(self, sub_element_name: etree_.QName | None,
+                 value_class: Any,
+                 is_optional: bool = True):
         super().__init__(sub_element_name, ListConverter(ClassCheckConverter(value_class)), is_optional=is_optional)
         self.value_class = value_class
 
-    def get_py_value_from_node(self, instance, node):
-        """ get from node"""
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         objects = []
         try:
             nodes = node.findall(self._sub_element_name)
             for _node in nodes:
                 value_class = self.value_class.value_class_from_node(_node)
                 value = value_class.from_node(_node)
                 objects.append(value)
             return objects
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             return objects
 
-    def update_xml_value(self, instance, node):
-        """ value is a list of objects with "as_etree_node" method"""
-        # remove all existing nodes
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:  # set to None (it is in the responsibility of the called method to do the right thing)
             py_value = self._default_py_value
 
         if py_value is not None:
             for val in py_value:
-                #name = self._sub_element_name or val.NODETYPE
                 sub_node = val.as_etree_node(self._sub_element_name, node.nsmap)
                 if hasattr(val, 'NODETYPE') and hasattr(self.value_class, 'NODETYPE') \
                         and val.NODETYPE != self.value_class.NODETYPE:
                     # set xsi type
                     sub_node.set(QN_TYPE, docname_from_qname(val.NODETYPE, node.nsmap))
                 node.append(sub_node)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'{self.__class__.__name__} datatype {self.value_class.__name__} in subelement {self._sub_element_name}'
 
 
 class ContainerListProperty(_ElementListProperty):
-    """ a list of values that have "mk_node" and cls.from_node methods.
-    Used if maxOccurs="Unbounded" in BICEPS_ParticipantModel"""
+    """ContainerListProperty is a property with a list of elements, each supports xsi:type information.
 
-    def __init__(self, sub_element_name, value_class, cls_getter, ns_helper, is_optional=True):
+    Used if maxOccurs="Unbounded" in BICEPS_ParticipantModel.
+    """
+
+    def __init__(self, sub_element_name: etree_.QName | None,  # Noqa: PLR0913
+                 value_class: Any,
+                 cls_getter: Callable[[etree_.QName], type],
+                 ns_helper: NamespaceHelper,
+                 is_optional: bool = True):
+        """Construct a list of Containers.
+
+        :param sub_element_name: see doc of base class
+        :param value_class: Default value class if no xsi:type is found
+        :param cls_getter: function that returns a class for xsi:type QName
+        :param ns_helper: name space helper that knows current prefixes
+        :param is_optional: see doc of base class
+        """
         super().__init__(sub_element_name, ListConverter(ClassCheckConverter(value_class)), is_optional=is_optional)
         self.value_class = value_class
         self._cls_getter = cls_getter
         self._ns_helper = ns_helper
 
-    def get_py_value_from_node(self, instance, node):
-        """ get from node"""
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         objects = []
         try:
             nodes = node.findall(self._sub_element_name)
             for _node in nodes:
                 node_type_str = _node.get(QN_TYPE)
                 if node_type_str is not None:
                     node_type = text_to_qname(node_type_str, _node.nsmap)
                     value_class = self._cls_getter(node_type)
                 else:
                     value_class = self.value_class
                 value = value_class.from_node(_node)
                 objects.append(value)
             return objects
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             return objects
 
-    def update_xml_value(self, instance, node):
-        """ value is a list of objects with "mk_node" method"""
-        # remove all existing nodes
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:  # set to None (it is in the responsibility of the called method to do the right thing)
             py_value = self._default_py_value
 
         nodes = node.findall(self._sub_element_name)
         for _node in nodes:
@@ -980,38 +1119,42 @@
             for val in py_value:
                 sub_node = val.mk_node(self._sub_element_name, self._ns_helper)
                 if val.NODETYPE != self.value_class.NODETYPE:
                     # set xsi type
                     sub_node.set(QN_TYPE, docname_from_qname(val.NODETYPE, node.nsmap))
                 node.append(sub_node)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'{self.__class__.__name__} datatype {self.value_class.__name__} in subelement {self._sub_element_name}'
 
 
 class SubElementTextListProperty(_ElementListProperty):
-    """ represents a list of strings. on xml side every string is a text of a sub element"""
+    """SubElementTextListProperty represents a list of strings.
+
+    On xml side every string is a text of a sub element.
+    """
 
-    def __init__(self, sub_element_name, value_class, is_optional=True):
+    def __init__(self, sub_element_name: etree_.QName | None,
+                 value_class: Any,
+                 is_optional: bool = True):
         super().__init__(sub_element_name, ListConverter(ClassCheckConverter(value_class)), is_optional=is_optional)
 
-    def get_py_value_from_node(self, instance, node):
-        """ get from node"""
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         objects = []
         try:
             nodes = node.findall(self._sub_element_name)
             for _node in nodes:
                 objects.append(_node.text)
             return objects
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             return objects
 
-    def update_xml_value(self, instance, node):
-        """ value is a list of strings"""
-        # remove all existing nodes
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:
             py_value = self._default_py_value
 
         if py_value is None or len(py_value) == 0:
             return
@@ -1024,192 +1167,207 @@
             child = etree_.SubElement(node, self._sub_element_name)
             try:
                 child.text = val
             except TypeError as ex:
                 # re-raise with better info about data
                 raise TypeError(f'{ex} in {self}') from ex
 
-    def __str__(self):
-        return f'{self.__class__.__name__} in subelement {self._sub_element_name}'
+    def __str__(self) -> str:
+        return f'{self.__class__.__name__} in sub-element {self._sub_element_name}'
 
 
 class SubElementStringListProperty(SubElementTextListProperty):
-    """ represents a list of strings. on xml side every string is a text of a sub element"""
+    """SubElementStringListProperty represents a list of strings.
 
-    def __init__(self, sub_element_name, is_optional=True):
+    On xml side every string is a text of a sub element.
+    """
+
+    def __init__(self, sub_element_name: etree_.QName | None,
+                 is_optional: bool = True):
         super().__init__(sub_element_name, str, is_optional=is_optional)
 
 
 class SubElementHandleRefListProperty(SubElementStringListProperty):
-    """ List of Handles"""
+    """Represents a list of Handles."""
 
 
 class SubElementWithSubElementListProperty(SubElementProperty):
-    """This Represents an Element that is optional and only present if its value class is not empty.
-    value_class must have an is_empty method
+    """Class represents an optional Element that is only present if its value class is not empty.
+
+    value_class must have an is_empty method.
     """
 
-    def __init__(self, sub_element_name, default_py_value, value_class):
+    def __init__(self, sub_element_name: etree_.QName | None,
+                 default_py_value: Any,
+                 value_class: Any):
         assert hasattr(value_class, 'is_empty')
         super().__init__(sub_element_name,
                          default_py_value=default_py_value,
                          value_class=value_class)
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:
             py_value = self._default_py_value
 
         if py_value is None or py_value.is_empty():
             return
         self.remove_sub_element(node)
         node.append(py_value.as_etree_node(self._sub_element_name, node.nsmap))
 
-    def __set__(self, instance, py_value):
+    def __set__(self, instance: Any, py_value: Any):
         if isinstance(py_value, self.value_class):
             super().__set__(instance, py_value)
         else:
             raise ApiUsageError(f'do not set {self._sub_element_name} directly, use child member!')
 
 
 class AnyEtreeNodeListProperty(_ElementListProperty):
-    """ Node < sub_element_name> has etree Element children."""
+    """class represents a list of etree_.Element."""
 
-    def __init__(self, sub_element_name, is_optional=True):
-        value_class = etree_._Element
+    def __init__(self, sub_element_name: etree_.QName | None,
+                 is_optional: bool = True):
+        value_class = etree_._Element  # Noqa: SLF001
         super().__init__(sub_element_name, ListConverter(ClassCheckConverter(value_class)), is_optional=is_optional)
 
-    def get_py_value_from_node(self, instance, node):
-        """ get from node"""
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         objects = []
         try:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=False)
             if sub_node is None:
                 return []
             return sub_node[:]
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             return objects
 
-    def update_xml_value(self, instance, node):
-        """ value is a list of etree nodes"""
-        # remove all existing nodes
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:
             py_value = None
 
         if py_value is None or len(py_value) == 0:
             if self.is_optional:
                 self.remove_sub_element(node)
             return
 
         sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
         sub_node.extend(py_value)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f'{self.__class__.__name__} in subelement {self._sub_element_name}'
 
 
 class NodeTextListProperty(_ElementListProperty):
-    """The handled data is a list of words (string without whitespace). The xml text is the joined list of words.
-    """
+    """The handled data is a list of words (string without whitespace). The xml text is the joined list of words."""
 
-    def __init__(self, sub_element_name, value_class, is_optional=False):
+    def __init__(self, sub_element_name: etree_.QName | None,
+                 value_class: Any,
+                 is_optional: bool = False):
         super().__init__(sub_element_name, ListConverter(ClassCheckConverter(value_class)),
                          is_optional=is_optional)
 
-    def get_py_value_from_node(self, instance, node):
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         try:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=False)
             if sub_node.text is not None:
                 return sub_node.text.split()
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             pass
         return self._default_py_value
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:  # set to None (it is in the responsibility of the called method to do the right thing)
             py_value = None
 
         if py_value is None:
             if not self._sub_element_name:
                 # update text of this element
                 node.text = ''
+            elif self.is_optional:
+                sub_node = node.find(self._sub_element_name)
+                if sub_node is not None:
+                    node.remove(sub_node)
             else:
-                if self.is_optional:
-                    sub_node = node.find(self._sub_element_name)
-                    if sub_node is not None:
-                        node.remove(sub_node)
-                else:
-                    if MANDATORY_VALUE_CHECKING and not self.is_optional:
-                        raise ValueError(f'mandatory value {self._sub_element_name} missing')
-                    sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
-                    sub_node.text = None
+                if MANDATORY_VALUE_CHECKING and not self.is_optional:
+                    raise ValueError(f'mandatory value {self._sub_element_name} missing')
+                sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
+                sub_node.text = None
         else:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
             sub_node.text = ' '.join(py_value)
 
 
 class NodeTextQNameListProperty(_ElementListProperty):
-    """ The handled data is a list of qualified names. The xml text is the joined list of qnames in the
-    form prefix:localname"""
+    """The handled data is a list of qualified names.
 
-    def __init__(self, sub_element_name, is_optional=False):
+    The xml text is the joined list of qnames in the form prefix:localname.
+    """
+
+    def __init__(self, sub_element_name: etree_.QName | None,
+                 is_optional: bool = False):
         super().__init__(sub_element_name, ListConverter(ClassCheckConverter(etree_.QName)),
                          is_optional=is_optional)
 
-    def get_py_value_from_node(self, instance, node):
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         result = []
         try:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=False)
             if sub_node is None:
                 return None
             if sub_node.text is not None:
                 for q_name_string in sub_node.text.split():
                     result.append(text_to_qname(q_name_string, sub_node.nsmap))
                 return result
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             pass
         return self._default_py_value or result
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:  # set to None (it is in the responsibility of the called method to do the right thing)
             py_value = None
 
         if py_value is None:
             if not self._sub_element_name:
                 # update text of this element
                 node.text = ''
+            elif self.is_optional:
+                sub_node = node.find(self._sub_element_name)
+                if sub_node is not None:
+                    node.remove(sub_node)
             else:
-                if self.is_optional:
-                    sub_node = node.find(self._sub_element_name)
-                    if sub_node is not None:
-                        node.remove(sub_node)
-                else:
-                    if MANDATORY_VALUE_CHECKING and not self.is_optional:
-                        raise ValueError(f'mandatory value {self._sub_element_name} missing')
-                    sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
-                    sub_node.text = None
+                if MANDATORY_VALUE_CHECKING and not self.is_optional:
+                    raise ValueError(f'mandatory value {self._sub_element_name} missing')
+                sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
+                sub_node.text = None
         else:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
             tmp = []
             for q_name in py_value:
                 # by setting each qname as text, namespace prefixes are generated automatically
                 sub_node.text = q_name
                 tmp.append(sub_node.text)
             sub_node.text = ' '.join(tmp)
 
 
 class DateOfBirthProperty(_ElementBase):
-    """ this represents the DateOfBirth type of BICEPS xml schema draft 10:
+    """DateOfBirthProperty represents the DateOfBirth type of BICEPS.
+
         <xsd:simpleType>
             <xsd:union memberTypes="xsd:dateTime xsd:date xsd:gYearMonth xsd:gYear"/>
         </xsd:simpleType>
     xsd:dateTime is YYYY-MM-DDThh:mm:ss.sss
     xsd:date is YYYY-MM-DD format. All components are required
     xsd:gYearMonth is YYYY-MM
     xsd:gYear is YYYY
@@ -1217,47 +1375,53 @@
 
     Time zone info can be provided:
        UTC can be specified by appending a Z character, e.g. 2002-09-24Z
        other timezones by adding a positive or negative time behind the date, e.g. 2002.09-24-06:00, 2002-09-24+06:00
     xsd:time is hh:mm:ss format, e.g. 9:30:10, 9:30:10.5. All components are required.
     Time zone handling is identical to date type
 
-    The corresponding Python types are datetime.Date (=> not time point available) or datetime.Datetime (with time point attribute)
+    The corresponding Python types are datetime.Date (=> not time point available)
+    or datetime.Datetime (with time point attribute).
     """
 
-    def __init__(self, sub_element_name, default_py_value=None, implied_py_value=None, is_optional=True):
+    def __init__(self, sub_element_name: etree_.QName | None,
+                 default_py_value: Any = None,
+                 implied_py_value: Any = None,
+                 is_optional: bool = True):
         super().__init__(sub_element_name, ClassCheckConverter(datetime, date),
                          default_py_value, implied_py_value, is_optional)
 
-    def get_py_value_from_node(self, instance, node):
+    def get_py_value_from_node(self, instance: Any, node: etree_.Element) -> Any:  # Noqa: ARG002
+        """Read value from node."""
         try:
             sub_node = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=False)
             if sub_node is not None:
                 date_string = sub_node.text
                 return isoduration.parse_date_time(date_string)
-        except ElementNotFoundException:
+        except ElementNotFoundError:
             pass
         return None
 
-    def update_xml_value(self, instance, node):
+    def update_xml_value(self, instance: Any, node: etree_.Element):
+        """Write value to node."""
         try:
             py_value = getattr(instance, self._local_var_name)
         except AttributeError:  # set to None (it is in the responsibility of the called method to do the right thing)
             py_value = self._default_py_value
 
         if py_value is None:
             self.remove_sub_element(node)
-        else:
-            if isinstance(py_value, str):
-                datestring = py_value  # use strings as they are
-            else:
-                datestring = self._mk_datestring(py_value)
-            sub_element = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
-            sub_element.text = datestring
+            return
+
+        date_string = py_value if isinstance(py_value, str) else self._mk_datestring(py_value)
+        sub_element = self._get_element_by_child_name(node, self._sub_element_name, create_missing_nodes=True)
+        sub_element.text = date_string
 
     @staticmethod
-    def mk_value_object(date_string):
+    def mk_value_object(date_string: str) -> date | datetime | isoduration.GYear | isoduration.GYearMonth | None:
+        """Parse isoduration string."""
         return isoduration.parse_date_time(date_string)
 
     @staticmethod
-    def _mk_datestring(date_object):
+    def _mk_datestring(date_object: date | datetime | isoduration.GYear | isoduration.GYearMonth | None) -> str:
+        """Create isoduration string."""
         return isoduration.date_time_string(date_object)
```

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/BICEPS_MessageModel.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/BICEPS_MessageModel.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/ExtensionPoint.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/ExtensionPoint.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/MetadataExchange.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/MetadataExchange.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/SafetyInformation.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/SafetyInformation.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/addressing.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/addressing.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/eventing.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/eventing.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/soap-envelope.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/soap-envelope.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/ws-addr.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/wsdl.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/wsdl.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/src/sdc11073/xsd/xml.xsd` & `sdc11073-2.0.0a5/src/sdc11073/xsd/xml.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/tutorial/README.rst` & `sdc11073-2.0.0a5/tutorial/README.rst`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/.gitignore` & `sdc11073-2.0.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/LICENSE` & `sdc11073-2.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/README.rst` & `sdc11073-2.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/pyproject.toml` & `sdc11073-2.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a4/PKG-INFO` & `sdc11073-2.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdc11073
-Version: 2.0.0a4
+Version: 2.0.0a5
 Summary: Pure python implementation of IEEE11073 SDC protocol
 Project-URL: Homepage, https://github.com/Draegerwerk/sdc11073
 Project-URL: Bug Tracker, https://github.com/Draegerwerk/sdc11073/issues
 Author-email: Bernd Deichmann <bernd.deichmann@draeger.com>, Leon Budnick <leon.budnick@draeger.com>
 License-File: LICENSE
 Keywords: IEEE11073,SDC
 Classifier: Development Status :: 5 - Production/Stable
```

