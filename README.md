# Add-Domain-Shared-Contacts
Add Update Delete and Sync Domain Shared Contacts

This script will add, update, delete and sync domain shared contacts through batches of data directly into your domain.

In order to use this addon, you will have to perform the following:
1) Create a sheet with the name EXACTLY like this – “SHARED_CONTACTS”
2)Append the following values in the top cells (from A1 to M1):
- First Name
- Last Name
- Full Name
- Primary Email
- Secondary Email
- Primary Phone
- Secondary Phone
- City
- Street
- Region
- Post code
- Country
- Validation

You can also just use the spreadsheet that we created by making a copy of it and start uploading directly into it -> https://docs.google.com/spreadsheets/d/1_8pSrlFrutZ1ro-nmRdSMfWLvRywD7BPXhgC_GeNnA0/edit#gid=2048680943
 
Here’s what the script does :
* Goes through all the rows in the sheet called “SHARED_CONTACTS” (except its header)
* Builds an XML based on the info gathered from the row based on the operation you desire
* Sends the request to your Google Apps Domain
* Error reporting is provided in the "validation" field
 
Notes:
* You have to be an Administrator in your Google Apps Domain for this to work
* Keep in mind that it might take 24 hours for the contacts to be available while composing an email in GMail (as per Google’s specs)
* Follow https://support.google.com/a/answer/60218?hl=en to make sure your Domain Shared Contacts are shown in your “Directory” folder in https://contacts.google.com
