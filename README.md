Use Case:
Prepare a .csv file of 1k records with column headers PAN, Date, Time, Transaction Amount DeviceID, ProcCode STAN, ActionCode, FinancialInstitution, MerchantCategory, MerchantName, Address, City, Country Status

[MANDATORY] PAN should contain 16-digits of Random number fix first 7-digits unchanged create for both Visa and MasterCard for General Merchant Category codes, T & E, Payment Brands, Agricuultural Services, Utility Sevices, Miscellaneous Stores, Government Sevices and Gaming & Gambling MCCs 
[MANDATORY] populate real time values for Date, Time, Amount (in USD) and STAN must be unique, use ProcCode 000000, 090000 for retailer merchants and populate relevant values in MerchantCategory and other fields
[MANDATORY] validate each and every financial transaction in .csv file  
[MANDATORY] populate ActionCode 000 and Status Non-Fraud for transaction Amount anything < 100$ from non-gambling, gaming MCCs but set ActionCode A50 and Status 'Suspected Fraud' for anything from Gambling, Gaming Fraud transactions from High-Risk Jurisdictions (Black List) and OFAC sanctioned, EU sanctioned, UN sanctioned countries 
[Critical] Classify Non-fraud and Fraudulent transactions and prepare graphical representation
