  Software Engineering - Framgang – Surefire Bericht 

* * *

Zuletzt veröffentlicht: 2023-06-07 | Version: 1.0-SNAPSHOT

* * *

[![Erstellt von Maven](./images/logos/maven-feather.png)](http://maven.apache.org/ "Erstellt von Maven")

//&lt;!\[CDATA\[ function toggleDisplay(elementId) { var elm = document.getElementById(elementId + '-error'); if (elm == null) { elm = document.getElementById(elementId + '-failure'); } if (elm && typeof elm.style != "undefined") { if (elm.style.display == "none") { elm.style.display = ""; document.getElementById(elementId + '-off').style.display = "none"; document.getElementById(elementId + '-on').style.display = "inline"; } else if (elm.style.display == "") { elm.style.display = "none"; document.getElementById(elementId + '-off').style.display = "inline"; document.getElementById(elementId + '-on').style.display = "none"; } } } //\]\]&gt;

Surefire Bericht
----------------

Zusammenfassung
---------------

\[[Zusammenfassung](#Summary)\] \[[Pakete](#Package_List)\] \[[Testfälle](#Test_Cases)\]

  

| Tests | Fehler | Fehlschläge | Ausgelassen | Erfolgsrate | Zeit |
| --- | --- | --- | --- | --- | --- |
| 192 | 0   | 0   | 20  | 89,583% | 73,592 |

  

Hinweis: Fehlschläge werden erwartet und durch Behauptungen überprüft während Fehler unerwartet sind.

  

Pakete
------

\[[Zusammenfassung](#Summary)\] \[[Pakete](#Package_List)\] \[[Testfälle](#Test_Cases)\]

  

| Paket | Tests | Fehler | Fehlschläge | Ausgelassen | Erfolgsrate | Zeit |
| --- | --- | --- | --- | --- | --- | --- |
| [controller](#controller) | 22  | 0   | 0   | 2   | 90,909% | 3,238 |
| [database](#database) | 34  | 0   | 0   | 2   | 94,118% | 15,43 |
| [product](#product) | 48  | 0   | 0   | 4   | 91,667% | 0,045 |
| [ui.controller](#ui.controller) | 16  | 0   | 0   | 0   | 100% | 40,034 |
| [ui](#ui) | 4   | 0   | 0   | 0   | 100% | 5,227 |
| [model](#model) | 22  | 0   | 0   | 8   | 63,636% | 8,262 |
| [sampledatagenerator](#sampledatagenerator) | 6   | 0   | 0   | 4   | 33,333% | 0,012 |
| [config](#config) | 4   | 0   | 0   | 0   | 100% | 1,248 |
| [customer](#customer) | 36  | 0   | 0   | 0   | 100% | 0,096 |

  

Hinweis: Die Paketstatistiken werden nicht rekursiv berechnet, es werden lediglich die Ergebnisse aller enthaltenen Tests aufsummiert.

### controller

|     | Klasse | Tests | Fehler | Fehlschläge | Ausgelassen | Erfolgsrate | Zeit |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [![](images/icon_success_sml.gif)](#controller.CSVControllerTest) | [CSVControllerTest](#controller.CSVControllerTest) | 4   | 0   | 0   | 0   | 100% | 1,526 |
| [![](images/icon_warning_sml.gif)](#controller.CSVImportModelTest) | [CSVImportModelTest](#controller.CSVImportModelTest) | 3   | 0   | 0   | 1   | 66,667% | 0,013 |
| [![](images/icon_success_sml.gif)](#controller.DatabaseControllerTest) | [DatabaseControllerTest](#controller.DatabaseControllerTest) | 4   | 0   | 0   | 0   | 100% | 0,062 |
| [![](images/icon_success_sml.gif)](#controller.CSVControllerTest) | [CSVControllerTest](#controller.CSVControllerTest) | 4   | 0   | 0   | 0   | 100% | 1,557 |
| [![](images/icon_warning_sml.gif)](#controller.CSVImportModelTest) | [CSVImportModelTest](#controller.CSVImportModelTest) | 3   | 0   | 0   | 1   | 66,667% | 0,01 |
| [![](images/icon_success_sml.gif)](#controller.DatabaseControllerTest) | [DatabaseControllerTest](#controller.DatabaseControllerTest) | 4   | 0   | 0   | 0   | 100% | 0,07 |

### database

|     | Klasse | Tests | Fehler | Fehlschläge | Ausgelassen | Erfolgsrate | Zeit |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#database.DbTest) | [DbTest](#database.DbTest) | 17  | 0   | 0   | 1   | 94,118% | 7,523 |
| [![](images/icon_warning_sml.gif)](#database.DbTest) | [DbTest](#database.DbTest) | 17  | 0   | 0   | 1   | 94,118% | 7,907 |

### product

|     | Klasse | Tests | Fehler | Fehlschläge | Ausgelassen | Erfolgsrate | Zeit |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [![](images/icon_success_sml.gif)](#product.ControllerProductTest) | [ControllerProductTest](#product.ControllerProductTest) | 1   | 0   | 0   | 0   | 100% | 0,005 |
| [![](images/icon_warning_sml.gif)](#product.GoodsEntranceTest) | [GoodsEntranceTest](#product.GoodsEntranceTest) | 2   | 0   | 0   | 2   | 0%  | 0,001 |
| [![](images/icon_success_sml.gif)](#product.GoodsOutgoingTest) | [GoodsOutgoingTest](#product.GoodsOutgoingTest) | 3   | 0   | 0   | 0   | 100% | 0,004 |
| [![](images/icon_success_sml.gif)](#product.ProductTest) | [ProductTest](#product.ProductTest) | 16  | 0   | 0   | 0   | 100% | 0,011 |
| [![](images/icon_success_sml.gif)](#product.SupplierTest) | [SupplierTest](#product.SupplierTest) | 2   | 0   | 0   | 0   | 100% | 0,002 |
| [![](images/icon_success_sml.gif)](#product.ControllerProductTest) | [ControllerProductTest](#product.ControllerProductTest) | 1   | 0   | 0   | 0   | 100% | 0,003 |
| [![](images/icon_warning_sml.gif)](#product.GoodsEntranceTest) | [GoodsEntranceTest](#product.GoodsEntranceTest) | 2   | 0   | 0   | 2   | 0%  | 0,001 |
| [![](images/icon_success_sml.gif)](#product.GoodsOutgoingTest) | [GoodsOutgoingTest](#product.GoodsOutgoingTest) | 3   | 0   | 0   | 0   | 100% | 0,002 |
| [![](images/icon_success_sml.gif)](#product.ProductTest) | [ProductTest](#product.ProductTest) | 16  | 0   | 0   | 0   | 100% | 0,013 |
| [![](images/icon_success_sml.gif)](#product.SupplierTest) | [SupplierTest](#product.SupplierTest) | 2   | 0   | 0   | 0   | 100% | 0,003 |

### ui.controller

|     | Klasse | Tests | Fehler | Fehlschläge | Ausgelassen | Erfolgsrate | Zeit |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [![](images/icon_success_sml.gif)](#ui.controller.IMSESceneControllerTest) | [IMSESceneControllerTest](#ui.controller.IMSESceneControllerTest) | 8   | 0   | 0   | 0   | 100% | 20,237 |
| [![](images/icon_success_sml.gif)](#ui.controller.IMSESceneControllerTest) | [IMSESceneControllerTest](#ui.controller.IMSESceneControllerTest) | 8   | 0   | 0   | 0   | 100% | 19,797 |

### ui

|     | Klasse | Tests | Fehler | Fehlschläge | Ausgelassen | Erfolgsrate | Zeit |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [![](images/icon_success_sml.gif)](#ui.MainFXTest) | [MainFXTest](#ui.MainFXTest) | 2   | 0   | 0   | 0   | 100% | 2,64 |
| [![](images/icon_success_sml.gif)](#ui.MainFXTest) | [MainFXTest](#ui.MainFXTest) | 2   | 0   | 0   | 0   | 100% | 2,587 |

### model

|     | Klasse | Tests | Fehler | Fehlschläge | Ausgelassen | Erfolgsrate | Zeit |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [![](images/icon_success_sml.gif)](#model.CorporateDesignTest) | [CorporateDesignTest](#model.CorporateDesignTest) | 1   | 0   | 0   | 0   | 100% | 0,001 |
| [![](images/icon_warning_sml.gif)](#model.CSVExportModelTest) | [CSVExportModelTest](#model.CSVExportModelTest) | 1   | 0   | 0   | 1   | 0%  | 0,001 |
| [![](images/icon_warning_sml.gif)](#model.DatabaseModelTest) | [DatabaseModelTest](#model.DatabaseModelTest) | 9   | 0   | 0   | 3   | 66,667% | 4,284 |
| [![](images/icon_success_sml.gif)](#model.CorporateDesignTest) | [CorporateDesignTest](#model.CorporateDesignTest) | 1   | 0   | 0   | 0   | 100% | 0,003 |
| [![](images/icon_warning_sml.gif)](#model.CSVExportModelTest) | [CSVExportModelTest](#model.CSVExportModelTest) | 1   | 0   | 0   | 1   | 0%  | 0,001 |
| [![](images/icon_warning_sml.gif)](#model.DatabaseModelTest) | [DatabaseModelTest](#model.DatabaseModelTest) | 9   | 0   | 0   | 3   | 66,667% | 3,972 |

### sampledatagenerator

|     | Klasse | Tests | Fehler | Fehlschläge | Ausgelassen | Erfolgsrate | Zeit |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#sampledatagenerator.DatabaseControllerIntegrationTest) | [DatabaseControllerIntegrationTest](#sampledatagenerator.DatabaseControllerIntegrationTest) | 1   | 0   | 0   | 1   | 0%  | 0,001 |
| [![](images/icon_warning_sml.gif)](#sampledatagenerator.MainTest) | [MainTest](#sampledatagenerator.MainTest) | 1   | 0   | 0   | 1   | 0%  | 0,001 |
| [![](images/icon_success_sml.gif)](#sampledatagenerator.ProductGeneratorTest) | [ProductGeneratorTest](#sampledatagenerator.ProductGeneratorTest) | 1   | 0   | 0   | 0   | 100% | 0,004 |
| [![](images/icon_warning_sml.gif)](#sampledatagenerator.DatabaseControllerIntegrationTest) | [DatabaseControllerIntegrationTest](#sampledatagenerator.DatabaseControllerIntegrationTest) | 1   | 0   | 0   | 1   | 0%  | 0,001 |
| [![](images/icon_warning_sml.gif)](#sampledatagenerator.MainTest) | [MainTest](#sampledatagenerator.MainTest) | 1   | 0   | 0   | 1   | 0%  | 0,001 |
| [![](images/icon_success_sml.gif)](#sampledatagenerator.ProductGeneratorTest) | [ProductGeneratorTest](#sampledatagenerator.ProductGeneratorTest) | 1   | 0   | 0   | 0   | 100% | 0,004 |

### config

|     | Klasse | Tests | Fehler | Fehlschläge | Ausgelassen | Erfolgsrate | Zeit |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [![](images/icon_success_sml.gif)](#config.ConfigTest) | [ConfigTest](#config.ConfigTest) | 2   | 0   | 0   | 0   | 100% | 0,637 |
| [![](images/icon_success_sml.gif)](#config.ConfigTest) | [ConfigTest](#config.ConfigTest) | 2   | 0   | 0   | 0   | 100% | 0,611 |

### customer

|     | Klasse | Tests | Fehler | Fehlschläge | Ausgelassen | Erfolgsrate | Zeit |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [![](images/icon_success_sml.gif)](#customer.AddressTest) | [AddressTest](#customer.AddressTest) | 13  | 0   | 0   | 0   | 100% | 0,014 |
| [![](images/icon_success_sml.gif)](#customer.ControllerCustomerTest) | [ControllerCustomerTest](#customer.ControllerCustomerTest) | 1   | 0   | 0   | 0   | 100% | 0,025 |
| [![](images/icon_success_sml.gif)](#customer.CustomerTest) | [CustomerTest](#customer.CustomerTest) | 4   | 0   | 0   | 0   | 100% | 0,006 |
| [![](images/icon_success_sml.gif)](#customer.AddressTest) | [AddressTest](#customer.AddressTest) | 13  | 0   | 0   | 0   | 100% | 0,021 |
| [![](images/icon_success_sml.gif)](#customer.ControllerCustomerTest) | [ControllerCustomerTest](#customer.ControllerCustomerTest) | 1   | 0   | 0   | 0   | 100% | 0,026 |
| [![](images/icon_success_sml.gif)](#customer.CustomerTest) | [CustomerTest](#customer.CustomerTest) | 4   | 0   | 0   | 0   | 100% | 0,004 |

  

Testfälle
---------

\[[Zusammenfassung](#Summary)\] \[[Pakete](#Package_List)\] \[[Testfälle](#Test_Cases)\]

### ConfigTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testPrivateConstructor | 0,606 |
| ![](images/icon_success_sml.gif) | testConfigProperties | 0,004 |

### CSVControllerTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testReadListOfProducts | 1,504 |
| ![](images/icon_success_sml.gif) | testWriteToCsv | 0,004 |
| ![](images/icon_success_sml.gif) | testWriteToCsvWithProductList | 0,002 |
| ![](images/icon_success_sml.gif) | testImportProductsInDatabase | 0,008 |

### CSVImportModelTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#controller.CSVImportModelTest.buildAProduct) | [buildAProduct](#controller.CSVImportModelTest.buildAProduct)<br><br>\+ \- \[ Detail \] | 0   |
|     | csv.buildAProduct Methode nicht vollständig!! |     |
| ![](images/icon_success_sml.gif) | testReadListOfProducts | 0,002 |
| ![](images/icon_success_sml.gif) | testBuildAProduct | 0,001 |

### DatabaseControllerTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testAddUser_UserDoesNotHaveRights | 0,053 |
| ![](images/icon_success_sml.gif) | testDeleteUser_UserDoesNotHaveRights | 0,001 |
| ![](images/icon_success_sml.gif) | testGetCorporateDesign | 0,002 |
| ![](images/icon_success_sml.gif) | testGetUserRights | 0,002 |

### AddressTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testSetCountry | 0,001 |
| ![](images/icon_success_sml.gif) | testGetPostalcode | 0,001 |
| ![](images/icon_success_sml.gif) | testGetCity | 0,001 |
| ![](images/icon_success_sml.gif) | testSetPostalcode | 0,001 |
| ![](images/icon_success_sml.gif) | testSetHousNo | 0,001 |
| ![](images/icon_success_sml.gif) | testSetOthers | 0   |
| ![](images/icon_success_sml.gif) | testGetHousNo | 0   |
| ![](images/icon_success_sml.gif) | testSetStreet | 0   |
| ![](images/icon_success_sml.gif) | testGetCountry | 0   |
| ![](images/icon_success_sml.gif) | testGetOthers | 0   |
| ![](images/icon_success_sml.gif) | testGetStreet | 0   |
| ![](images/icon_success_sml.gif) | testSetCity | 0,001 |
| ![](images/icon_success_sml.gif) | testAddressConstructor | 0,002 |

### ControllerCustomerTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testAddCustomer | 0,024 |

### CustomerTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testGetAddress | 0,001 |
| ![](images/icon_success_sml.gif) | testGetName | 0   |
| ![](images/icon_success_sml.gif) | testSetAddress | 0   |
| ![](images/icon_success_sml.gif) | testSetName | 0   |

### DbTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | validateUserIncorrectUsername | 1,148 |
| ![](images/icon_success_sml.gif) | getCustomer | 0   |
| ![](images/icon_success_sml.gif) | validateUserCorrectInput | 0,301 |
| ![](images/icon_success_sml.gif) | getDataForProductOverview | 0,313 |
| ![](images/icon_success_sml.gif) | CSVExport | 0,001 |
| ![](images/icon_success_sml.gif) | UpdateCorporateDesign | 0,489 |
| ![](images/icon_success_sml.gif) | readCSVFile | 0,001 |
| ![](images/icon_success_sml.gif) | validateUserIncorrectPassword | 0,215 |
| ![](images/icon_success_sml.gif) | updateColorScheme | 0,945 |
| ![](images/icon_success_sml.gif) | getUser | 0,259 |
| ![](images/icon_success_sml.gif) | testGetDatabaseData | 0,372 |
| [![](images/icon_warning_sml.gif)](#database.DbTest.importCSVInDatabase) | [importCSVInDatabase](#database.DbTest.importCSVInDatabase)<br><br>\+ \- \[ Detail \] | 0   |
|     | Mika muss die csv als Resource implementieren \| erledigt |     |
| ![](images/icon_success_sml.gif) | testAddUserNew | 0,986 |
| ![](images/icon_success_sml.gif) | testAddUserOld | 1,236 |
| ![](images/icon_success_sml.gif) | getUserRights | 0,001 |
| ![](images/icon_success_sml.gif) | testDeleteUserNew | 0,266 |
| ![](images/icon_success_sml.gif) | testDeleteUserOld | 0,975 |

### CorporateDesignTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testCorporateDesign | 0   |

### CSVExportModelTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#model.CSVExportModelTest.testWriteToCsv) | [testWriteToCsv](#model.CSVExportModelTest.testWriteToCsv)<br><br>\+ \- \[ Detail \] | 0   |
|     | nicht fertig |     |

### DatabaseModelTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#model.DatabaseModelTest.testGetCorporateDesign) | [testGetCorporateDesign](#model.DatabaseModelTest.testGetCorporateDesign)<br><br>\+ \- \[ Detail \] | 0   |
|     | fix assertions |     |
| ![](images/icon_success_sml.gif) | testAddUserExisting | 1,383 |
| ![](images/icon_success_sml.gif) | testGetUser | 0,22 |
| ![](images/icon_success_sml.gif) | testDeletUserNew | 0,267 |
| ![](images/icon_success_sml.gif) | testDeletUserOld | 1,131 |
| ![](images/icon_success_sml.gif) | testInsertNewProducts | 0,259 |
| [![](images/icon_warning_sml.gif)](#model.DatabaseModelTest.testGetDatabaseData) | [testGetDatabaseData](#model.DatabaseModelTest.testGetDatabaseData)<br><br>\+ \- \[ Detail \] | 0   |
|     | fix assertions |     |
| ![](images/icon_success_sml.gif) | testAddUserNew | 1,015 |
| [![](images/icon_warning_sml.gif)](#model.DatabaseModelTest.testUpdateCorporateDesign) | [testUpdateCorporateDesign](#model.DatabaseModelTest.testUpdateCorporateDesign)<br><br>\+ \- \[ Detail \] | 0   |
|     | fix assertions |     |

### ControllerProductTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testConstructor | 0,003 |

### GoodsEntranceTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#product.GoodsEntranceTest.testRemoveProduct) | [testRemoveProduct](#product.GoodsEntranceTest.testRemoveProduct)<br><br>\+ \- \[ Detail \] | 0   |
|     | method under construction |     |
| [![](images/icon_warning_sml.gif)](#product.GoodsEntranceTest.testAddProduct) | [testAddProduct](#product.GoodsEntranceTest.testAddProduct)<br><br>\+ \- \[ Detail \] | 0   |
|     | method under construction |     |

### GoodsOutgoingTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testGettersAndSetters | 0,001 |
| ![](images/icon_success_sml.gif) | testRemoveProduct | 0,001 |
| ![](images/icon_success_sml.gif) | testAddProduct | 0   |

### ProductTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testGetPrice | 0   |
| ![](images/icon_success_sml.gif) | testParseProductToDocument | 0   |
| ![](images/icon_success_sml.gif) | testToString_WithoutAdditionalInformationMap | 0,001 |
| ![](images/icon_success_sml.gif) | testGetAdditionalInformationMap | 0   |
| ![](images/icon_success_sml.gif) | testGetId | 0   |
| ![](images/icon_success_sml.gif) | testToString_WithEmptyAdditionalInformationMap | 0   |
| ![](images/icon_success_sml.gif) | testParseProductToDocument_WithAdditionalInformation | 0,001 |
| ![](images/icon_success_sml.gif) | testParseProductToDocument_WithEmptyAdditionalInformationMap | 0   |
| ![](images/icon_success_sml.gif) | testProductToCSVString | 0   |
| ![](images/icon_success_sml.gif) | testToDocument | 0   |
| ![](images/icon_success_sml.gif) | testGetQuantity | 0   |
| ![](images/icon_success_sml.gif) | testParseProductToDocument_WithNullAdditionalInformationMap | 0   |
| ![](images/icon_success_sml.gif) | testParseProductToDocument_WithoutAdditionalInformationMap | 0   |
| ![](images/icon_success_sml.gif) | testToString_WithAdditionalInformation | 0   |
| ![](images/icon_success_sml.gif) | testGetDescription | 0   |
| ![](images/icon_success_sml.gif) | testToString_WithNullAdditionalInformationMap | 0,001 |

### SupplierTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testConstructorAndGetters | 0,001 |
| ![](images/icon_success_sml.gif) | testSetters | 0   |

### DatabaseControllerIntegrationTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#sampledatagenerator.DatabaseControllerIntegrationTest.testInsertNewProducts) | [testInsertNewProducts](#sampledatagenerator.DatabaseControllerIntegrationTest.testInsertNewProducts)<br><br>\+ \- \[ Detail \] | 0   |
|     | void sampledatagenerator.DatabaseControllerIntegrationTest.testInsertNewProducts() is @Disabled |     |

### MainTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#sampledatagenerator.MainTest.testInsertRandomProducts) | [testInsertRandomProducts](#sampledatagenerator.MainTest.testInsertRandomProducts)<br><br>\+ \- \[ Detail \] | 0   |
|     | funktioniert nicht |     |

### ProductGeneratorTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testGenerateRandomProduct | 0,002 |

### IMSESceneControllerTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testLoginWithValidCredentials | 5,325 |
| ![](images/icon_success_sml.gif) | testLoadPane(String, String, String)\[1\] | 2,717 |
| ![](images/icon_success_sml.gif) | testLoadMenuBar | 0,599 |
| ![](images/icon_success_sml.gif) | showCorporateDesignSettingPane(String, String, String, String)\[1\] | 3,002 |
| ![](images/icon_success_sml.gif) | testShowAddProductScene | 3,276 |
| ![](images/icon_success_sml.gif) | testSidebarForDashboardIsNull | 1,328 |
| ![](images/icon_success_sml.gif) | testLoadTabForSidebars(String, String)\[1\] | 1,036 |
| ![](images/icon_success_sml.gif) | testLoginWithInvalidCredentialsShowsErrorMessage | 2,878 |

### MainFXTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testApplicationExit | 1,353 |
| ![](images/icon_success_sml.gif) | testIconSetup | 1,287 |

### ConfigTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testPrivateConstructor | 0,584 |
| ![](images/icon_success_sml.gif) | testConfigProperties | 0,003 |

### CSVControllerTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testReadListOfProducts | 1,535 |
| ![](images/icon_success_sml.gif) | testWriteToCsv | 0,004 |
| ![](images/icon_success_sml.gif) | testWriteToCsvWithProductList | 0,003 |
| ![](images/icon_success_sml.gif) | testImportProductsInDatabase | 0,008 |

### CSVImportModelTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#controller.CSVImportModelTest.buildAProduct) | [buildAProduct](#controller.CSVImportModelTest.buildAProduct)<br><br>\+ \- \[ Detail \] | 0   |
|     | csv.buildAProduct Methode nicht vollständig!! |     |
| ![](images/icon_success_sml.gif) | testReadListOfProducts | 0,003 |
| ![](images/icon_success_sml.gif) | testBuildAProduct | 0,001 |

### DatabaseControllerTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testAddUser_UserDoesNotHaveRights | 0,061 |
| ![](images/icon_success_sml.gif) | testDeleteUser_UserDoesNotHaveRights | 0,001 |
| ![](images/icon_success_sml.gif) | testGetCorporateDesign | 0,002 |
| ![](images/icon_success_sml.gif) | testGetUserRights | 0,002 |

### AddressTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testSetCountry | 0,001 |
| ![](images/icon_success_sml.gif) | testGetPostalcode | 0,001 |
| ![](images/icon_success_sml.gif) | testGetCity | 0,001 |
| ![](images/icon_success_sml.gif) | testSetPostalcode | 0   |
| ![](images/icon_success_sml.gif) | testSetHousNo | 0,001 |
| ![](images/icon_success_sml.gif) | testSetOthers | 0   |
| ![](images/icon_success_sml.gif) | testGetHousNo | 0,001 |
| ![](images/icon_success_sml.gif) | testSetStreet | 0,001 |
| ![](images/icon_success_sml.gif) | testGetCountry | 0,001 |
| ![](images/icon_success_sml.gif) | testGetOthers | 0,001 |
| ![](images/icon_success_sml.gif) | testGetStreet | 0,001 |
| ![](images/icon_success_sml.gif) | testSetCity | 0,001 |
| ![](images/icon_success_sml.gif) | testAddressConstructor | 0,002 |

### ControllerCustomerTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testAddCustomer | 0,026 |

### CustomerTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testGetAddress | 0   |
| ![](images/icon_success_sml.gif) | testGetName | 0   |
| ![](images/icon_success_sml.gif) | testSetAddress | 0   |
| ![](images/icon_success_sml.gif) | testSetName | 0,001 |

### DbTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | validateUserIncorrectUsername | 1,33 |
| ![](images/icon_success_sml.gif) | getCustomer | 0,001 |
| ![](images/icon_success_sml.gif) | validateUserCorrectInput | 0,347 |
| ![](images/icon_success_sml.gif) | getDataForProductOverview | 0,396 |
| ![](images/icon_success_sml.gif) | CSVExport | 0,001 |
| ![](images/icon_success_sml.gif) | UpdateCorporateDesign | 0,589 |
| ![](images/icon_success_sml.gif) | readCSVFile | 0,003 |
| ![](images/icon_success_sml.gif) | validateUserIncorrectPassword | 0,289 |
| ![](images/icon_success_sml.gif) | updateColorScheme | 0,971 |
| ![](images/icon_success_sml.gif) | getUser | 0,234 |
| ![](images/icon_success_sml.gif) | testGetDatabaseData | 0,308 |
| [![](images/icon_warning_sml.gif)](#database.DbTest.importCSVInDatabase) | [importCSVInDatabase](#database.DbTest.importCSVInDatabase)<br><br>\+ \- \[ Detail \] | 0   |
|     | Mika muss die csv als Resource implementieren \| erledigt |     |
| ![](images/icon_success_sml.gif) | testAddUserNew | 0,992 |
| ![](images/icon_success_sml.gif) | testAddUserOld | 1,186 |
| ![](images/icon_success_sml.gif) | getUserRights | 0   |
| ![](images/icon_success_sml.gif) | testDeleteUserNew | 0,304 |
| ![](images/icon_success_sml.gif) | testDeleteUserOld | 0,94 |

### CorporateDesignTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testCorporateDesign | 0,001 |

### CSVExportModelTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#model.CSVExportModelTest.testWriteToCsv) | [testWriteToCsv](#model.CSVExportModelTest.testWriteToCsv)<br><br>\+ \- \[ Detail \] | 0   |
|     | nicht fertig |     |

### DatabaseModelTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#model.DatabaseModelTest.testGetCorporateDesign) | [testGetCorporateDesign](#model.DatabaseModelTest.testGetCorporateDesign)<br><br>\+ \- \[ Detail \] | 0   |
|     | fix assertions |     |
| ![](images/icon_success_sml.gif) | testAddUserExisting | 1,307 |
| ![](images/icon_success_sml.gif) | testGetUser | 0,238 |
| ![](images/icon_success_sml.gif) | testDeletUserNew | 0,269 |
| ![](images/icon_success_sml.gif) | testDeletUserOld | 0,981 |
| ![](images/icon_success_sml.gif) | testInsertNewProducts | 0,247 |
| [![](images/icon_warning_sml.gif)](#model.DatabaseModelTest.testGetDatabaseData) | [testGetDatabaseData](#model.DatabaseModelTest.testGetDatabaseData)<br><br>\+ \- \[ Detail \] | 0   |
|     | fix assertions |     |
| ![](images/icon_success_sml.gif) | testAddUserNew | 0,926 |
| [![](images/icon_warning_sml.gif)](#model.DatabaseModelTest.testUpdateCorporateDesign) | [testUpdateCorporateDesign](#model.DatabaseModelTest.testUpdateCorporateDesign)<br><br>\+ \- \[ Detail \] | 0   |
|     | fix assertions |     |

### ControllerProductTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testConstructor | 0,002 |

### GoodsEntranceTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#product.GoodsEntranceTest.testRemoveProduct) | [testRemoveProduct](#product.GoodsEntranceTest.testRemoveProduct)<br><br>\+ \- \[ Detail \] | 0   |
|     | method under construction |     |
| [![](images/icon_warning_sml.gif)](#product.GoodsEntranceTest.testAddProduct) | [testAddProduct](#product.GoodsEntranceTest.testAddProduct)<br><br>\+ \- \[ Detail \] | 0   |
|     | method under construction |     |

### GoodsOutgoingTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testGettersAndSetters | 0,001 |
| ![](images/icon_success_sml.gif) | testRemoveProduct | 0   |
| ![](images/icon_success_sml.gif) | testAddProduct | 0   |

### ProductTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testGetPrice | 0,001 |
| ![](images/icon_success_sml.gif) | testParseProductToDocument | 0,001 |
| ![](images/icon_success_sml.gif) | testToString_WithoutAdditionalInformationMap | 0   |
| ![](images/icon_success_sml.gif) | testGetAdditionalInformationMap | 0   |
| ![](images/icon_success_sml.gif) | testGetId | 0,001 |
| ![](images/icon_success_sml.gif) | testToString_WithEmptyAdditionalInformationMap | 0   |
| ![](images/icon_success_sml.gif) | testParseProductToDocument_WithAdditionalInformation | 0,001 |
| ![](images/icon_success_sml.gif) | testParseProductToDocument_WithEmptyAdditionalInformationMap | 0,001 |
| ![](images/icon_success_sml.gif) | testProductToCSVString | 0,001 |
| ![](images/icon_success_sml.gif) | testToDocument | 0   |
| ![](images/icon_success_sml.gif) | testGetQuantity | 0   |
| ![](images/icon_success_sml.gif) | testParseProductToDocument_WithNullAdditionalInformationMap | 0   |
| ![](images/icon_success_sml.gif) | testParseProductToDocument_WithoutAdditionalInformationMap | 0   |
| ![](images/icon_success_sml.gif) | testToString_WithAdditionalInformation | 0,001 |
| ![](images/icon_success_sml.gif) | testGetDescription | 0,001 |
| ![](images/icon_success_sml.gif) | testToString_WithNullAdditionalInformationMap | 0   |

### SupplierTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testConstructorAndGetters | 0,001 |
| ![](images/icon_success_sml.gif) | testSetters | 0   |

### DatabaseControllerIntegrationTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#sampledatagenerator.DatabaseControllerIntegrationTest.testInsertNewProducts) | [testInsertNewProducts](#sampledatagenerator.DatabaseControllerIntegrationTest.testInsertNewProducts)<br><br>\+ \- \[ Detail \] | 0   |
|     | void sampledatagenerator.DatabaseControllerIntegrationTest.testInsertNewProducts() is @Disabled |     |

### MainTest

|     |     |     |
| --- | --- | --- |
| [![](images/icon_warning_sml.gif)](#sampledatagenerator.MainTest.testInsertRandomProducts) | [testInsertRandomProducts](#sampledatagenerator.MainTest.testInsertRandomProducts)<br><br>\+ \- \[ Detail \] | 0   |
|     | funktioniert nicht |     |

### ProductGeneratorTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testGenerateRandomProduct | 0,003 |

### IMSESceneControllerTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testLoginWithValidCredentials | 5,163 |
| ![](images/icon_success_sml.gif) | testLoadPane(String, String, String)\[1\] | 2,721 |
| ![](images/icon_success_sml.gif) | testLoadMenuBar | 0,593 |
| ![](images/icon_success_sml.gif) | showCorporateDesignSettingPane(String, String, String, String)\[1\] | 3,065 |
| ![](images/icon_success_sml.gif) | testShowAddProductScene | 3,182 |
| ![](images/icon_success_sml.gif) | testSidebarForDashboardIsNull | 1,315 |
| ![](images/icon_success_sml.gif) | testLoadTabForSidebars(String, String)\[1\] | 0,974 |
| ![](images/icon_success_sml.gif) | testLoginWithInvalidCredentialsShowsErrorMessage | 2,703 |

### MainFXTest

|     |     |     |
| --- | --- | --- |
| ![](images/icon_success_sml.gif) | testApplicationExit | 1,325 |
| ![](images/icon_success_sml.gif) | testIconSetup | 1,26 |

  

Details der Fehlschläge
-----------------------

\[[Zusammenfassung](#Summary)\] \[[Pakete](#Package_List)\] \[[Testfälle](#Test_Cases)\]

  

|     |     |
| --- | --- |
| ![](images/icon_warning_sml.gif) | buildAProduct |
|     | skipped: csv.buildAProduct Methode nicht vollständig!! |
| ![](images/icon_warning_sml.gif) | importCSVInDatabase |
|     | skipped: Mika muss die csv als Resource implementieren \| erledigt |
| ![](images/icon_warning_sml.gif) | testWriteToCsv |
|     | skipped: nicht fertig |
| ![](images/icon_warning_sml.gif) | testGetCorporateDesign |
|     | skipped: fix assertions |
| ![](images/icon_warning_sml.gif) | testGetDatabaseData |
|     | skipped: fix assertions |
| ![](images/icon_warning_sml.gif) | testUpdateCorporateDesign |
|     | skipped: fix assertions |
| ![](images/icon_warning_sml.gif) | testRemoveProduct |
|     | skipped: method under construction |
| ![](images/icon_warning_sml.gif) | testAddProduct |
|     | skipped: method under construction |
| ![](images/icon_warning_sml.gif) | testInsertNewProducts |
|     | skipped: void sampledatagenerator.DatabaseControllerIntegrationTest.testInsertNewProducts() is @Disabled |
| ![](images/icon_warning_sml.gif) | testInsertRandomProducts |
|     | skipped: funktioniert nicht |
| ![](images/icon_warning_sml.gif) | buildAProduct |
|     | skipped: csv.buildAProduct Methode nicht vollständig!! |
| ![](images/icon_warning_sml.gif) | importCSVInDatabase |
|     | skipped: Mika muss die csv als Resource implementieren \| erledigt |
| ![](images/icon_warning_sml.gif) | testWriteToCsv |
|     | skipped: nicht fertig |
| ![](images/icon_warning_sml.gif) | testGetCorporateDesign |
|     | skipped: fix assertions |
| ![](images/icon_warning_sml.gif) | testGetDatabaseData |
|     | skipped: fix assertions |
| ![](images/icon_warning_sml.gif) | testUpdateCorporateDesign |
|     | skipped: fix assertions |
| ![](images/icon_warning_sml.gif) | testRemoveProduct |
|     | skipped: method under construction |
| ![](images/icon_warning_sml.gif) | testAddProduct |
|     | skipped: method under construction |
| ![](images/icon_warning_sml.gif) | testInsertNewProducts |
|     | skipped: void sampledatagenerator.DatabaseControllerIntegrationTest.testInsertNewProducts() is @Disabled |
| ![](images/icon_warning_sml.gif) | testInsertRandomProducts |
|     | skipped: funktioniert nicht |

  

* * *

Copyright © 2023[DHBW](www.dhbw.de). .

* * *