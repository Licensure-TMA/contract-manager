# TACT Compilation Report
Contract: Main
BOC Size: 2867 bytes

# Types
Total Types: 12

## StateInit
TLB: `_ code:^cell data:^cell = StateInit`
Signature: `StateInit{code:^cell,data:^cell}`

## Context
TLB: `_ bounced:bool sender:address value:int257 raw:^slice = Context`
Signature: `Context{bounced:bool,sender:address,value:int257,raw:^slice}`

## SendParameters
TLB: `_ bounce:bool to:address value:int257 mode:int257 body:Maybe ^cell code:Maybe ^cell data:Maybe ^cell = SendParameters`
Signature: `SendParameters{bounce:bool,to:address,value:int257,mode:int257,body:Maybe ^cell,code:Maybe ^cell,data:Maybe ^cell}`

## Deploy
TLB: `deploy#946a98b6 queryId:uint64 = Deploy`
Signature: `Deploy{queryId:uint64}`

## DeployOk
TLB: `deploy_ok#aff90f57 queryId:uint64 = DeployOk`
Signature: `DeployOk{queryId:uint64}`

## FactoryDeploy
TLB: `factory_deploy#6d0ff13b queryId:uint64 cashback:address = FactoryDeploy`
Signature: `FactoryDeploy{queryId:uint64,cashback:address}`

## LicenseCreate
TLB: `license_create#94c07f2b sellerAddress:address contentName:^string contentDescription:^string contentUrls:^string licenseType:^string contentCategory:^string contentSubcategory:^string price:coins allRestrictions:^string additionalTerms:^string = LicenseCreate`
Signature: `LicenseCreate{sellerAddress:address,contentName:^string,contentDescription:^string,contentUrls:^string,licenseType:^string,contentCategory:^string,contentSubcategory:^string,price:coins,allRestrictions:^string,additionalTerms:^string}`

## License
TLB: `_ licenseId:int257 sellerAddress:address buyerAddress:address createdAt:uint32 contentName:^string contentDescription:^string contentUrls:^string licenseType:^string contentCategory:^string contentSubcategory:^string price:coins currency:^string allRestrictions:^string additionalTerms:^string status:^string = License`
Signature: `License{licenseId:int257,sellerAddress:address,buyerAddress:address,createdAt:uint32,contentName:^string,contentDescription:^string,contentUrls:^string,licenseType:^string,contentCategory:^string,contentSubcategory:^string,price:coins,currency:^string,allRestrictions:^string,additionalTerms:^string,status:^string}`

## LicenseArray
TLB: `_ map:dict<int, ^License{licenseId:int257,sellerAddress:address,buyerAddress:address,createdAt:uint32,contentName:^string,contentDescription:^string,contentUrls:^string,licenseType:^string,contentCategory:^string,contentSubcategory:^string,price:coins,currency:^string,allRestrictions:^string,additionalTerms:^string,status:^string}> length:uint64 = LicenseArray`
Signature: `LicenseArray{map:dict<int, ^License{licenseId:int257,sellerAddress:address,buyerAddress:address,createdAt:uint32,contentName:^string,contentDescription:^string,contentUrls:^string,licenseType:^string,contentCategory:^string,contentSubcategory:^string,price:coins,currency:^string,allRestrictions:^string,additionalTerms:^string,status:^string}>,length:uint64}`

## LicenseDelete
TLB: `license_delete#2c5294ac licenseId:int257 sellerAddress:address = LicenseDelete`
Signature: `LicenseDelete{licenseId:int257,sellerAddress:address}`

## LicenseBuy
TLB: `license_buy#863c797b licenseId:int257 buyerAddress:address = LicenseBuy`
Signature: `LicenseBuy{licenseId:int257,buyerAddress:address}`

## LicenseBuyV2
TLB: `license_buy_v2#00ee7ecd licenseId:int257 buyerAddress:address cost:coins = LicenseBuyV2`
Signature: `LicenseBuyV2{licenseId:int257,buyerAddress:address,cost:coins}`

# Get Methods
Total Get Methods: 6

## balance

## resultOfCreate
Argument: sellerAddress

## resultOfDelete
Argument: sellerAddress

## resultOfBuy
Argument: buyerAddress

## arrayOfLicenses

## oneLicensebyId
Argument: licenseId

# Error Codes
2: Stack undeflow
3: Stack overflow
4: Integer overflow
5: Integer out of expected range
6: Invalid opcode
7: Type check error
8: Cell overflow
9: Cell underflow
10: Dictionary error
13: Out of gas error
32: Method ID not found
34: Action is invalid or not supported
37: Not enough TON
38: Not enough extra-currencies
128: Null reference exception
129: Invalid serialization prefix
130: Invalid incoming message
131: Constraints error
132: Access denied
133: Contract stopped
134: Invalid argument
135: Code of a contract was not found
136: Invalid address
137: Masterchain support is not enabled for this contract
6108: No permission to buy
15509: Only deployer is allowed to withdraw
23004: No permission to delete
46050: No license exists
48618: Insufficient funds for transfer
50625: License is already purchased