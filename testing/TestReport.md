# Software Engineering - Framgång - Test Report

Last published: 2023-06-13 | Version: 1.0-SNAPSHOT

</br> 
</br> 


## Summary


| Tests | Errors | Failures | Skipped | Success rate | Time |
| --- | --- | --- | --- | --- | --- |
| 129 | 0   | 0   | 0   | 100% | 101,734 |

</br> 
</br> 
</br> 
</br> 


  

## Packages

\[[Summary](#summary)\] \[[Packages](#packages)\] \[[Test Cases](#test-cases)\]

  

| Package | Tests | Errors | Failures | Skipped | Success rate | Time |
| --- | --- | --- | --- | --- | --- | --- |
| [controller](#controller) | 11  | 0   | 0   | 0   | 100% | 3,353 |
| [database](#database) | 19  | 0   | 0   | 0   | 100% | 12,729 |
| [product](#product) | 51  | 0   | 0   | 0   | 100% | 5,332 |
| [ui.controller](#uicontroller) | 16  | 0   | 0   | 0   | 100% | 66,253 |
| [ui](#ui) | 2   | 0   | 0   | 0   | 100% | 3,091 |
| [model](#model) | 9   | 0   | 0   | 0   | 100% | 9,557 |
| [sampledatagenerator](#sampledatagenerator) | 1   | 0   | 0   | 0   | 100% | 0,008 |
| [config](#config) | 2   | 0   | 0   | 0   | 100% | 1,314 |
| [customer](#customer) | 18  | 0   | 0   | 0   | 100% | 0,097 |

</br> 
</br> 



### controller

|     | Class | Tests | Errors | Failures | Skipped | Success rate | Time |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ![](icon_success.gif) | [CSVControllerTest](#csvcontrollertest) | 4   | 0   | 0   | 0   | 100% | 3,181 |
| ![](icon_success.gif) | [CSVImportModelTest](#csvimportmodeltest) | 2   | 0   | 0   | 0   | 100% | 0,018 |
| ![](icon_success.gif) | [DatabaseControllerTest](#databasecontrollertest) | 5   | 0   | 0   | 0   | 100% | 0,154 |

</br> 
</br> 

### database

|     | Class | Tests | Errors | Failures | Skipped | Success rate | Time |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ![](icon_success.gif) | [DbTest](#dbtest) | 19  | 0   | 0   | 0   | 100% | 12,729 |

</br> 
</br> 

### product

|     | Class | Tests | Errors | Failures | Skipped | Success rate | Time |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ![](icon_success.gif) | [ControllerProductTest](#controllerproducttest) | 1   | 0   | 0   | 0   | 100% | 0,008 |
| ![](icon_success.gif) | [GoodsEntranceTest](#goodsentrancetest) | 16  | 0   | 0   | 0   | 100% | 1,624 |
| ![](icon_success.gif) | [GoodsOutgoingTest](#goodsoutgoingtest) | 9   | 0   | 0   | 0   | 100% | 1,699 |
| ![](icon_success.gif) | [ProductTest](#producttest) | 23  | 0   | 0   | 0   | 100% | 1,996 |
| ![](icon_success.gif) | [SupplierTest](#suppliertest) | 2   | 0   | 0   | 0   | 100% | 0,005 |

</br> 
</br> 

### ui.controller

|     | Class | Tests | Errors | Failures | Skipped | Success rate | Time |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ![](icon_success.gif) | [IMSESceneControllerTest](#imsescenecontrollertest) | 16  | 0   | 0   | 0   | 100% | 66,253 |

</br> 
</br> 

### ui

|     | Class | Tests | Errors | Failures | Skipped | Success rate | Time |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ![](icon_success.gif) | [MainFXTest](#mainfxtest) | 2   | 0   | 0   | 0   | 100% | 3,091 |

</br> 
</br> 

### model

|     | Class | Tests | Errors | Failures | Skipped | Success rate | Time |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ![](icon_success.gif) | [CorporateDesignTest](#corporatedesigntest) | 1   | 0   | 0   | 0   | 100% | 0,002 |
| ![](icon_success.gif) | [DatabaseModelTest](#databasemodeltest) | 8   | 0   | 0   | 0   | 100% | 9,555 |

</br> 
</br> 

### sampledatagenerator

|     | Class | Tests | Errors | Failures | Skipped | Success rate | Time |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ![](icon_success.gif) | [ProductGeneratorTest](#productgeneratortest) | 1   | 0   | 0   | 0   | 100% | 0,008 |

</br> 
</br> 

### config

|     | Class | Tests | Errors | Failures | Skipped | Success rate | Time |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ![](icon_success.gif) | [ConfigTest](#configtest) | 2   | 0   | 0   | 0   | 100% | 1,314 |

</br> 
</br> 

### customer

|     | Class | Tests | Errors | Failures | Skipped | Success rate | Time |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ![](icon_success.gif) | [AddressTest](#addresstest) | 13  | 0   | 0   | 0   | 100% | 0,044 |
| ![](icon_success.gif) | [ControllerCustomerTest](#controllercustomertest) | 1   | 0   | 0   | 0   | 100% | 0,043 |
| ![](icon_success.gif) | [CustomerTest](#customertest) | 4   | 0   | 0   | 0   | 100% | 0,01 |

</br> 
</br> 
</br> 
</br> 


## Test Cases

\[[Summary](#summary)\] \[[Packages](#packages)\] \[[Test Cases](#test-cases)\]

### ConfigTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testPrivateConstructor | 1,25 |
| ![](icon_success.gif) | testConfigProperties | 0,006 |

</br> 
</br> 

### CSVControllerTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testReadListOfProducts | 3,131 |
| ![](icon_success.gif) | testWriteToCsv | 0,009 |
| ![](icon_success.gif) | testWriteToCsvWithProductList | 0,004 |
| ![](icon_success.gif) | testImportProductsInDatabase | 0,019 |

</br> 
</br> 

### CSVImportModelTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testReadListOfProducts | 0,008 |
| ![](icon_success.gif) | testBuildAProduct | 0,002 |

</br> 
</br> 

### DatabaseControllerTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testAddUser_UserDoesNotHaveRights | 0,133 |
| ![](icon_success.gif) | testDeleteUser_UserDoesNotHaveRights | 0,003 |
| ![](icon_success.gif) | testGetCorporateDesign | 0,005 |
| ![](icon_success.gif) | testGetUserRights | 0,004 |
| ![](icon_success.gif) | testGetUser | 0,001 |

</br> 
</br> 

### AddressTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testSetCountry | 0,003 |
| ![](icon_success.gif) | testGetPostalcode | 0,001 |
| ![](icon_success.gif) | testGetCity | 0,001 |
| ![](icon_success.gif) | testSetPostalcode | 0,001 |
| ![](icon_success.gif) | testSetHousNo | 0,001 |
| ![](icon_success.gif) | testSetOthers | 0,005 |
| ![](icon_success.gif) | testGetHousNo | 0,002 |
| ![](icon_success.gif) | testSetStreet | 0,001 |
| ![](icon_success.gif) | testGetCountry | 0,001 |
| ![](icon_success.gif) | testGetOthers | 0,001 |
| ![](icon_success.gif) | testGetStreet | 0,001 |
| ![](icon_success.gif) | testSetCity | 0,004 |
| ![](icon_success.gif) | testAddressConstructor | 0,003 |

</br> 
</br> 

### ControllerCustomerTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testAddCustomer | 0,042 |

</br> 
</br> 

### CustomerTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testGetAddress | 0,001 |
| ![](icon_success.gif) | testGetName | 0,001 |
| ![](icon_success.gif) | testSetAddress | 0,001 |
| ![](icon_success.gif) | testSetName | 0,001 |

</br> 
</br> 

### DbTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | validateUserIncorrectUsername | 2,191 |
| ![](icon_success.gif) | getCustomer | 0,001 |
| ![](icon_success.gif) | validateUserCorrectInput | 0,394 |
| ![](icon_success.gif) | getDataForProductOverview | 0,426 |
| ![](icon_success.gif) | CSVExport | 0,002 |
| ![](icon_success.gif) | testEditUserRight | 1,744 |
| ![](icon_success.gif) | testEditUserWrong | 0,631 |
| ![](icon_success.gif) | UpdateCorporateDesign | 0,591 |
| ![](icon_success.gif) | readCSVFile | 0,002 |
| ![](icon_success.gif) | testGetAllUser | 1,424 |
| ![](icon_success.gif) | validateUserIncorrectPassword | 0,246 |
| ![](icon_success.gif) | updateColorScheme | 1,083 |
| ![](icon_success.gif) | getUser | 0,236 |
| ![](icon_success.gif) | testGetDatabaseData | 0,272 |
| ![](icon_success.gif) | testAddUserNew | 0,941 |
| ![](icon_success.gif) | testAddUserOld | 1,227 |
| ![](icon_success.gif) | getUserRights | 0,001 |
| ![](icon_success.gif) | testDeleteUserNew | 0,243 |
| ![](icon_success.gif) | testDeleteUserOld | 1,054 |

</br> 
</br> 

### CorporateDesignTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testCorporateDesign | 0,001 |

</br> 
</br> 

### DatabaseModelTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testAddUserExisting | 1,29 |
| ![](icon_success.gif) | testGetAllUser | 1,387 |
| ![](icon_success.gif) | testGetUser | 0,237 |
| ![](icon_success.gif) | testDeletUserNew | 0,224 |
| ![](icon_success.gif) | testDeletUserOld | 1,943 |
| ![](icon_success.gif) | testInsertNewProducts | 0,255 |
| ![](icon_success.gif) | testAddUserNew | 2,97 |
| ![](icon_success.gif) | testUserEditRight | 1,245 |

</br> 
</br> 

### ControllerProductTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testConstructor | 0,007 |

</br> 
</br> 

### GoodsEntranceTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testDatabaseNameSetter | 0,001 |
| ![](icon_success.gif) | testChangedProductsGetter | 0   |
| ![](icon_success.gif) | testChangedProductsSetter | 0,004 |
| ![](icon_success.gif) | testVolumeGetter | 0,001 |
| ![](icon_success.gif) | testDatabaseControllerSetter | 0,001 |
| ![](icon_success.gif) | testVolumeSetter | 0,001 |
| ![](icon_success.gif) | testParseToDocument | 0,087 |
| ![](icon_success.gif) | testIdGetter | 0,001 |
| ![](icon_success.gif) | testIdSetter | 0,001 |
| ![](icon_success.gif) | testGetterSetter | 0,001 |
| ![](icon_success.gif) | testWeightGetter | 0,001 |
| ![](icon_success.gif) | testWriteEntranceInDatabase | 1,509 |
| ![](icon_success.gif) | testPriceGetter | 0   |
| ![](icon_success.gif) | testWeightSetter | 0   |
| ![](icon_success.gif) | testPriceSetter | 0,001 |
| ![](icon_success.gif) | testDatabaseNameGetter | 0,001 |

</br> 
</br> 

### GoodsOutgoingTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testChangedProductsGetterAndSetter | 0,002 |
| ![](icon_success.gif) | testVolumeGetterAndSetter | 0,001 |
| ![](icon_success.gif) | testParseToDocument | 0,003 |
| ![](icon_success.gif) | testPriceGetterAndSetter | 0   |
| ![](icon_success.gif) | testWriteSellingInDatabase | 1,68 |
| ![](icon_success.gif) | testDatabaseNameGetterAndSetter | 0,001 |
| ![](icon_success.gif) | testIdGetterAndSetter | 0,001 |
| ![](icon_success.gif) | testDatabaseControllerGetterAndSetter | 0   |
| ![](icon_success.gif) | testWeightGetterAndSetter | 0,001 |

</br> 
</br> 

### ProductTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testGetPrice | 0,001 |
| ![](icon_success.gif) | testParseProductToDocument | 0   |
| ![](icon_success.gif) | testToString_WithoutAdditionalInformationMap | 0,007 |
| ![](icon_success.gif) | testGetAdditionalInformationMap | 0,001 |
| ![](icon_success.gif) | testGetId | 0,002 |
| ![](icon_success.gif) | updateAProductCompleteWorkflowForSelling | 1,029 |
| ![](icon_success.gif) | testToString_WithEmptyAdditionalInformationMap | 0,001 |
| ![](icon_success.gif) | testParseProductToDocument_WithAdditionalInformation | 0   |
| ![](icon_success.gif) | testParseProductToDocument_WithEmptyAdditionalInformationMap | 0   |
| ![](icon_success.gif) | testAdditionalInformationMapGetterAndSetter | 0,001 |
| ![](icon_success.gif) | testProductToCSVString | 0,001 |
| ![](icon_success.gif) | testPriceGetterAndSetter | 0,001 |
| ![](icon_success.gif) | testToDocument | 0   |
| ![](icon_success.gif) | testGetQuantity | 0   |
| ![](icon_success.gif) | testDescriptionGetterAndSetter | 0   |
| ![](icon_success.gif) | testParseProductToDocument_WithNullAdditionalInformationMap | 0,001 |
| ![](icon_success.gif) | updateAProductInModelForSelling | 0,93 |
| ![](icon_success.gif) | testParseProductToDocument_WithoutAdditionalInformationMap | 0   |
| ![](icon_success.gif) | testToString_WithAdditionalInformation | 0,001 |
| ![](icon_success.gif) | testGetDescription | 0,002 |
| ![](icon_success.gif) | testQuantityGetterAndSetter | 0,001 |
| ![](icon_success.gif) | testToString_WithNullAdditionalInformationMap | 0,001 |
| ![](icon_success.gif) | testIdGetterAndSetter | 0   |

</br> 
</br> 

### SupplierTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testConstructorAndGetters | 0,002 |
| ![](icon_success.gif) | testSetters | 0   |

</br> 
</br> 

### ProductGeneratorTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testGenerateRandomProduct | 0,004 |

</br> 
</br> 

### IMSESceneControllerTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testPurchase | 11,414 |
| ![](icon_success.gif) | testLoginWithValidCredentials | 3,755 |
| ![](icon_success.gif) | testLoadPane(String, String, String)\[1\] | 2,885 |
| ![](icon_success.gif) | addAndDeleteUser | 8,511 |
| ![](icon_success.gif) | testSale | 6,707 |
| ![](icon_success.gif) | testLoadMenuBar | 0,686 |
| ![](icon_success.gif) | testGetGrayscale | 3,525 |
| ![](icon_success.gif) | showCorporateDesignSettingPane(String, String, String)\[1\] | 2,367 |
| ![](icon_success.gif) | testShowAddProductScene | 2,93 |
| ![](icon_success.gif) | testSidebarForDashboardIsNull | 1,388 |
| ![](icon_success.gif) | testLoadTabForSidebars(String, String)\[1\] | 0,998 |
| ![](icon_success.gif) | refresh | 1,601 |
| ![](icon_success.gif) | editProduct | 6,041 |
| ![](icon_success.gif) | addProduct | 6,297 |
| ![](icon_success.gif) | editUser | 4,098 |
| ![](icon_success.gif) | testLoginWithInvalidCredentialsShowsErrorMessage | 2,873 |

</br> 
</br> 

### MainFXTest

|     |     |     |
| --- | --- | --- |
| ![](icon_success.gif) | testApplicationExit | 1,731 |
| ![](icon_success.gif) | testIconSetup | 1,355 |

</br> 
</br> 

## Coverage
<img src="coverage.png" alt="unit test coverage" width="750">  
The figure above shows the progress of the code base during the entire duration of the project, as well as the test coverage. At the end of the project, we had 1.142 lines to cover, of which we covered 939 lines with unit tests. This results in a test coverage of 81.0%.  
</br>  
</br>  

<img src="coverage-eclipse.png" alt="unit test coverage" width="750">  

The figure above shows the test coverage of the unit tests in Eclipse. As can be seen, all packages were covered by tests and the coverage is between 75% and 100% per package. The test coverage was calculated in Eclipse and therefore differs slightly from the calculated metric from Sonarqube, as the lines to be covered are defined differently.  
</br>  
The detailed view of the coverage of the individual methods was compiled as a [JaCoCo report](coverage.zip). This can be downloaded, unzipped and the included index.html file opened in any browser. From this, it is possible to navigate to the individual packages and methods.  
</br>  
</br>  


