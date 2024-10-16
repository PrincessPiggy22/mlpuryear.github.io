
# ChickFilA ERD Graph

Add documentatipm

```mermaid
erDiagram
PRODUCT}o--||CUSTOMER: consumes
PRODUCT {
    int ProdID PK
    string ProdName
    string ProdCat
}
CUSTOMER||--||SALE: place
CUSTOMER {
    int CustmID PK
    string CustmFName
    string CustmLName
    string MembershipStat
    int CustmPhoneNum
    
}
SALE||--o{PRODUCT: contain
SALE {
    int SaleID PK
    money SaleTotal 
    time SaleTime
    date SaleDate
}
INVENTORY ||--o{ PRODUCT: StoresAndSupplies
INVENTORY {
    int InvenID PK
    int ProdID FK
    int ProdCat FK
    strng ProdName FK

}
```