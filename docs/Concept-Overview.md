The purpose of this tool is to assist with monthly financial reporting to the accountant and insurance company
I am on income protection insurance
Due to my health issues, I am finding it very difficult to do the montly work
Many of the expenses can be seen through emails
They could be accessed via my Outlook 365 account (various) and my Apple Mail app with various accounts.

There are two parts to this, and I am hoping that this can be undertaken without too much duplication

**Usual Operations**

Copy the last periods excel document and create a new one for the period (monthly)
Download files from
    American Express (two major accounts)
    ANZ Visa
    Nab Visa
    St George Bank (business accounts - various)
Reformat the data of each and then save as an Xlsx file
For Visa transaction amounts are usually displayed as negatives, change all the negative amounts to positives
Delete payments (not credits) from the credit card files
For Bank files, it is important to understand the use of codes for credits and debits and how they interact with processing later.
Add a column for the Source, eg, AMEX Charge, AMEX Credit, ANZ Visa, NAB Visa, STG Bank (last 4 digits of the account number)

Format each file into the standardised format, retaining all additional information
There needs to be three additional columns (best placed to the right of the amount)
    GST Indicator
        G - Australian GST Paid
        E - Exempt from GST
        P - Personal Tax Item (potential)
        Z - Personal - not needed for business reporting
    Category of Spend
        See examples in the example spreadsheets
    Certainty of Allocations (which columns) and why
    Specific Notes for the accountant (which would be copied to another sheet in the workbook)

How is the various additional information added?
    There may be emails:
        1. May have the organisation's name or the billing entity
        2. The amount and currency (noting that on the credit card statements, both the AUD and foreign currency plus exchange fees)
        3. There may be an email for the initial subscription, but there may or may not be any for the subsequent monthly or annual payments
        4. There may be manual receipts that somehow need to be scanned.
        5. There may be the occasional cash payments with receipts that somehow need to be scanned.
    The general rules for the GST indicator
        Z - obvious personal items, such as supermarkets, clothing shops, etc., when in my own local area.  However, a supermarket outside of my local area is likely to be a business trip, so an expense with a status of G
        P - Would usually be limited to health expenses, such as health insurance, pharmacy, doctors, physiotherapists, speech therapists, CPAP, etc.
        G - These are directly business-related items that are billed in Australia, and some overseas companies where they had collected GST on behalf of the Australian government because I forgot to provide my ABN number to have the GST excused. Note that some items from Apple, Amazon etc might be E (excepmt), G or Z.  Some might be able to be automatically determined from past experience, such as on Apple Invoices, Netflix would be a Z where as YouTube would be a G. They can be reliabily replicated, however, from Amazon, there might be Kindle books, some are Z others G (work related) or material for the office (G) or for the bathroom (z)
        E - Exempt from GST, usually international payments, where no GST has been charged (see G above)
    Category of Spend
        These may be determined from the invoice or the history of prior purchases of the same items.
    Certainty of Allocations
        Green with works both - the system is very confident of the GST Indicator and Category of Spend.
        Yellow with one or both columns - the system has had a best guess, but needs human review
        Red with one or both columns - the system has not been able or unwilling to allocate codes and requires human input.

**Copies of Receipts**
    1. I am currently using Squirrel to maintain copies of the invoices/receipts to meet the ATO requirements.  However, this is becoming an expensive solution. So ideally I would like to have the receipts recorded in the data base some how (may use Notion for working on the data before extraction into Excel)
    2. For many expenses, it may be either an attachment (PDF) to an email or an email itself
    3. For manual documents, maybe there is a way to scan into Slack which might ask some questions, particularly the GST Indicator.  It may be too much to enter the Category of Spend

**Processing for Credit Cards - A New Sheet in the Workbook**
    1. There needs to be a process to allocate the GST Indicator, Category of Spend, Certainty of Allocations, and any notes.
    2. There needs to be a process to seek input from me where the Certainty of Allocation is not Green for both columns. This might be a daily push from the database via email, Slack or the like that easily allows for the data to be updated and corrected
    3. Once a month is fully allocated, then
        3.1 for that month
            Sort the months' data by GST Indicator, then by date
        3.2 Total the amounts for each GST Indicator
        3.3 for the GST Amount, divide the total by 1/11, providing the total GST paid (double check the formula)

**Processing for Bank Transactions - A new Sheet in the Workbook**
    1. 
        
