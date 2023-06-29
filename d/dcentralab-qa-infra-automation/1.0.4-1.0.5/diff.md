# Comparing `tmp/dcentralab_qa_infra_automation-1.0.4.tar.gz` & `tmp/dcentralab_qa_infra_automation-1.0.5.tar.gz`

## Comparing `dcentralab_qa_infra_automation-1.0.4.tar` & `dcentralab_qa_infra_automation-1.0.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/vcs.xml
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/BasePage.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
--rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/BasePage.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
+-rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-1.0.4/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-1.0.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     # Open the json file
     f = open(file_name)
 
     # Returns JSON object as a dictionary
     data_list = json.load(f)
 
     # Store the data driven in global param.
-    pytest.data_driven = data_list.get("farms")
+    pytest.data_driven = data_list
 
     vesting_types = pytest.data_driven.get("types")
 
     # Closing file
     f.close()
     return vesting_types
```

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/BasePage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/BasePage.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,14 +122,26 @@
         :param by_locator - current locator to click on
         :param file_path:
         """
         pytest.logger.info("upload file: " + file_path + " into " + element_name + " element")
         return WebDriverWait(self.driver, self.timeout).until(EC.visibility_of_element_located(by_locator)).send_keys(
             file_path)
 
+    def get_text_from_specific_index(self, element_name, by_locator, index):
+        """
+        Performs get text of web element whose locator is passed to it
+        :param by_locator - current locator
+        :param element_name: - current element
+        :param index - current index
+        :return current element text
+        """
+        pytest.logger.info("get the value from " + element_name + " element")
+        return WebDriverWait(self.driver, self.timeout).until(EC.visibility_of_all_elements_located(by_locator))[
+            index].text
+
     def get_text(self, element_name, by_locator):
         """
         Performs get text of web element whose locator is passed to it
         :param by_locator - current locator
         :param element_name: - current element
         :return current element text
         """
```

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,12 +23,15 @@
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
         return self.is_element_exist("TITLE", TITLE)
 
+    def is_button_exists(self):
+        return self.is_element_exist("GET_STARTED_BUTTON", GET_STARTED_BUTTON)
+
     def click_on_get_started(self):
         """
         click on get started button
         """
         self.click("GET_STARTED_BUTTON", GET_STARTED_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from dcentralab_qa_infra_automation.pages.metamaskPages.ImproveMetamaskPage import ImproveMetamaskPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.NewToMetamaskPage import NewToMetamaskPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.SwitchNetworkPage import SwitchNetworkPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.WalletConnectedHomePage import WalletConnectedHomePage
 from dcentralab_qa_infra_automation.pages.metamaskPages.WelcomeToMetamaskPage import WelcomeToMetamaskPage
 
 """
-MetaMask wallet actions
+coinbase wallet actions
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 
 class MetamaskActions(WalletsActionsInterface):
 
@@ -26,30 +26,32 @@
         self.driver = driver
 
     def import_wallet(self):
         """
         import wallet process
         """
         # Open new tab
-        self.driver.execute_script("window.open('');")
+        # self.driver.execute_script("window.open('');")
 
         # Focus on the new tab window
-        self.driver.switch_to.window(self.driver.window_handles[1])
+        self.driver.switch_to.window(self.driver.window_handles[2])
 
         # Open chrome extension
-        self.driver.get(pytest.properties.get("metamask.connect.url"))
+        # self.driver.get(pytest.properties.get("metamask.connect.url"))
 
         # Focus on the first tab window
-        self.driver.switch_to.window(self.driver.window_handles[1])
+        # self.driver.switch_to.window(self.driver.window_handles[1])
 
         welcomeToMetamaskPage = WelcomeToMetamaskPage(self.driver)
 
         # Check if metamask wallet page loaded
         assert welcomeToMetamaskPage.is_page_loaded(), "welcome to metamask page loaded"
 
+        assert welcomeToMetamaskPage.is_button_exists()
+
         # Click on get started button
         welcomeToMetamaskPage.click_on_get_started()
 
         improveMetamaskPage = ImproveMetamaskPage(self.driver)
 
         # Check if improve to metamask page loaded
         assert improveMetamaskPage.is_page_loaded(), "improve metamask page loaded"
```

### Comparing `dcentralab_qa_infra_automation-1.0.4/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py` & `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/LICENSE` & `dcentralab_qa_infra_automation-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.4/pyproject.toml` & `dcentralab_qa_infra_automation-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-1.0.4/PKG-INFO` & `dcentralab_qa_infra_automation-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 1.0.4
+Version: 1.0.5
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

