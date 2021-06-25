# FontSchPayMaster
Flow solution for various adjustment to a single or multiple Scheduled Payments related to a single Sales Order

Pre-requisites:
1) Fonteva Installed
2) Datatable installed from UnofficialSF: https://unofficialsf.com/datatable-lightning-web-component-for-flow-screens-2/

Outline:
1) A set of screenflows to allow backend staff to adjust Scheduled Payments related to a single Sales Order in a number of ways using a guided UI
2) A single Master flow is responsible for providing access to the appropriate sub-flow functions
3) Current sub-flow functionality:
    - Change Payment Dates: Adjust payment dates for one or more unprocessed Scheduled Payments
    - Reallocate Scheduled Payments: Reallocate funds from one or more unpaid Scheduled Payments to one or more other Scheduled Payments (useful to collect missed payments on subsequent Scheduled Payments
    - Change Payment Methods: Adjust the Payment Method for one or more unprocessed Scheduled Payments
    - DD Retry Payment: Retry one or more qualifying Direct Debit Scheduled Payments
    - Clean Up SPLs: As aparet of the reallocate functionlaity some "duplicate" Scheduled Payment Lines are created, this process comibines "duplicates" to keep the data efficient

Installation:
1) Ensure all pre-requisites are met
2) Install the contents of this Repo
3) Ensure the 6 Flows have been activated
4) Add a new button to the Page Layout for Sales Order - to launch the Master flow
5) On  a Sales Order that has one or more Scheduled Payments click the Button
6) Explore and test the functions provided
7) If specific business logic is required for the client, adjust or add new sub-flows as required

Documentation:
https://docs.google.com/document/d/1KWQ6ukMxAHGnbKWJqCGHghKD3pCLOpXX7XAUQ5Ab9Ks/edit?usp=sharing
