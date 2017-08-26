# **BulkInsertQuestionChoices**

### Description: 

**Do you agree that it is a pain when you are trying to insert multiple question choices to a select variable on catalog?** You have to ensure a consistent Choice label and value style, maintain ordering while inserting the choices, etc. 

Wouldn't it be nice to do a bulk insertion of choices and save some time to do the actual development?

### Installation:
- Install the updateset found in dist folder.
- The update set will create a record producer, related variables and scripts. It adds a button that will be visible for Select type variable and is used to access the utility.

### Usage:

On clicking the newly added button * Add Choices *, you will get a record producer where you can fill the required details.

- There are two insertion mode - Alphabetical and As-Is, which inserts the choices in the given order.
- The variable is auto populated if you had opened the record producer via the Add option button.
- Enter the options separated by Newline and Click Submit.

#### Note:
- This does clean up of the choices and allows only (,),-, space and alphanumeric characters for choice label. You can change the Regex as per your need.
- Capitalizes each word of choice label to maintain consistency.
- Converts the choice value to lower text separated by '_'

Additionally, the following concepts are used and can be understood reading the source components.

* Regex usage.
* Record producer and Producer script usage
* Autopopulating catalog variable using URL.
* Reference qualifier of variables.
* UI action and redirection.
* Gliderecord query and insertion.
