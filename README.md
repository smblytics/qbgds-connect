# qbgds-connect

## Welcome to QBGDS Connect

Google Data Studio "is a free tool that turns your data into informative, easy to read, easy to share, and fully customizable dashboards and reports." Learn more about it [here](https://support.google.com/datastudio/answer/6283323?hl=en).

"Quick Base is an application development platform that unites business and IT teams by enabling problem solvers of any technical background to work together to safely, securely and sustainably create an ecosystem of applications. Quick Base helps businesses accelerate the continuous innovation of unique processes by enabling citizen development at scale across one common platform." Learn more about it [here](https://www.quickbase.com/product/product-overview).

Now you can use both together with QBGDS Connect, which stands for Quick Base Google Data Studio Connect.

### Features
The QBGDS Conenctor provides similar functionality as the [Quick Base Power BI connector](https://help.quickbase.com/user-assistance/power_bi_with_quick_base.html) supported by Quick Base, just into a different business inteligence tool:
```
- Authenticates with specified Quick Base applications by using user tokens
- Quickly refreshes both large and small data sets from Quick Base
- Automatically updates both data and report columns.
```
And, supports a lot of the same use cases.
```
For example, you can use these features to add power to the following Quick Base use cases:

- Create and share report and chart types that are not supported by native Quick Base
- Merge data from multiple sources to analyze processes that span across multiple systems
- Convert timestamps to dates and times that are easy to read

Note: For Quick Base reports that are being used by Power BI, we recommend caution when making changes to the reports' configuration because changes may inadvertently break the Power BI features dependent on those reports.
```

### How to Use

To use QBGDS Connect:
1. Use the link you were provided to create a new data source in Google Data Studio with the connector
2. Provide the connector a [user token](https://help.quickbase.com/user-assistance/create_user_tokens.html) as the "key" for authentication -- note this _must_ have access to the application and table you expect to use in Google Data Studio
3. QBGDS will then prompt for more information -- (A) Enter a [realm](https://help.quickbase.com/user-assistance/what_is_a_realm.html) hostname for your Quick Base account (enter the full URL including quickbase.com), and (B) Enter a table ID (the [dbid](https://community.quickbase.com/browse/blogs/blogviewer?BlogKey=ad94a056-f327-4576-9dc5-fa79fcf79bbd&CommunityKey=d860b0f8-6a48-487b-b346-44c47a19a804&tab=blogviewer) of a table).  
4. Use as a normal Google Data Studio [data connector](https://support.google.com/datastudio/answer/6268208?hl=en).  Certain field types are not supported (like multi-text, vCard, etc.) and will not be returned in Data Studio.

### Defintions
**Realm**
```
A Quick Base realm is a logical slice of Quick Base dedicated to your organization that you control. Realms are defined using a DNS sub-domain with the format: https://customername.quickbase.com.
```
**Table ID / DBID**
```
Quick Base uses an alphanumeric database ID, or DBID, to uniquely identify each app and each table on our platform. You can find the DBID of a table in the address bar of your browser when you're looking at any page of the table. The home page of all Quick Base applications has a DBID that does not refer to any of the tables in the application. You can view a record or a report on one of your tables, then look in your browser's address bar to see that table's DBID. The DBID is after the "https://mycompany.quickbase.com/db/"; and before the first question mark "?" if there is one. For example the dbid in the following URL:

https://login.quickbase.com/db/6ewwzuuj?a=dr&r=ej&rl=bjd

is

6ewwzuuj
```

### Support or Contact

Having trouble with QBGDS Connect? Post an issue [here](https://github.com/smblytics/qbgds-connect/issues), and we’ll help you sort it out.


### Copyright

Copyright 2020 smblytics LLC
