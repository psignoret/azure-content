<properties 
   pageTitle="Azure Active Directory Audit Report Events" 
   description="Audited events that are available for viewing and downloading from your Azure Active Directory" 
   services="active-directory" 
   documentationCenter="" 
   authors="kenhoff" 
   manager="?" 
   editor=""/>

<tags
   ms.service="active-directory"
   ms.devlang="na"
   ms.topic="article"
   ms.tgt_pltfrm="na"
   ms.workload="identity" 
   ms.date="03/23/2015"
   ms.author="kenhoff"/>

# Azure Active Directory Audit Report Events

The Azure Active Directory Audit Report helps customers identify privileged actions that occurred in their Azure Active Directory. Privileged actions include elevation changes (for example, role creation or password resets), changing policy configurations (for example password policies), or changes to directory configuration (for example, changes to domain federation settings). The reports provide the audit record for the event name, the actor who performed the action, the target resource affected by the change, and the date and time (in UTC). Customers are able to retrieve the list of audit events for their Azure Active Directory via the [Azure Management Portal](https://manage.windowsazure.com/).  

## Audit Report Events

<!--- audit event descriptions should be in the past tense --->

|	Events 					| 	Event Description								|
|	------------------------------		|	-------									|
|	Add User				|	Added a user to the directory.						|
|	Delete User				|	Deleted a user from the directory.					|
|	Set license properties			|										|
|	Reset user password			|	Reset the password for a user in the directory.				|
|	Change user password			|	Changed the password for a user in the directory.			|
|	Change user license			|	Changed the license assigned to a user in the directory.		|
|	Update user				|	Updated a user in the directory.					|
|	Add role member to Role			|			|
|	Remove role member from Role		|			|
|	Set Company contact information		|			|
|	Add partner to company			|			|
|	Remove Partner from company		|			|
|	Add service principal			|	Added a service principal to the directory.				|
|	Remove service principal		|	Removed a service principal from the directory.				|
|	Add service principal credentials	|	Added credentials to a service principal.		|
|	Remove service principal credentials	|	Removed credentials from a service principal.		|
|	Add domain to company			|	Added a domain to the directory.		|
|	Remove domain from company		|	Removed a domain from the directory.		|
|	Update domain				|	Updated a domain on the directory.		|
|	Set domain authentication		|			|
|	Set federation settings on domain	|			|
|	Verify domain				|	Verified a domain on the directory.		|
|	Verify email verified domain		|	Verified a domain on the directory using email verification.		|
|	Add delegation entry			|			|
|	Set delegation entry			|			|
|	Remove delegation entry			|			|
|	Set DirSyncEnabled flag on company	|	Set the property that enables a directory for Azure AD Sync.		|
|	Set Password Policy			|			|
|	Restore Application			|			|
|	Set Company Information			|			|
|	Set String Auth Policy			|			|
|	Promote tenant to partner		|			|
|	Set force change user password		|	Set the property that forces a user to change their password on login.	|

### Properties included with each audit event

| Property	| Description								|
| ------	| ------								|		
| Date and Time	| The date and time that the audit event occured			|
| Actor		| The user or service principal that performed the action		|
| Action	| The action that was performed						|
| Target	| The user or service principal that the action was performed on	|

### User attributes included in the Update User audit event

| Attribute 				| Description	|
| ---------------------------------	| ---------	|
| AccountEnabled			| The user is not blocked from signing into Azure AD.														|
| AssignedLicense			| All licenses that have been assigned to the user.														|
| AssignedPlan				| Service plans resulting from the licenses assigned to the user.												|
| LicenseAssignmentDetail		| Details on licenses assigned to the user. For instance, if group-based licensing was involved, this would include the group that granted the license.		|
| Mobile				| The user's mobile phone.																	|
| OtherMail				| The user's alternate email address.																|
| OtherMobile				| The user's alternate mobile phone.																|
| StrongAuthenticationMethod		| Default method of verification used for Multi-Factor Authentication, such as Voice Call, SMS, or Verification code from a mobile app.				|
| StrongAuthenticationPhoneAppDetail	| Contains the device token for the user's registered mobile app.												|
| StrongAuthenticationRequirement	| If Multi-Factor Authentication is enforced, enabled, or disabled for this user.										|
| StrongAuthenticationUserDetails	| The user’s phone number, alternative phone number and email address used for Multi-Factor Authentication and password reset verification.					|
| TelephoneNumber			| The user's telephone number.																	|

Audit records are a required control for many compliance regulations. For customers using the Azure Active Directory Audit Report to meet their compliance regulations, it is recommended that the customer submit a copy of this help topic with the copy of the customer’s exported audit report to help explain the report details. If the auditor would like to understand the compliance regulations that Azure currently meets, direct the auditor to the [Compliance page](http://azure.microsoft.com/en-us/support/trust-center/compliance/) of the Microsoft Azure Trust Center.
