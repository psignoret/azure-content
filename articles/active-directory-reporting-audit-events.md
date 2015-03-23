<properties 
   pageTitle="Azure Active Directory Audit Report Events" 
   description="Audited events that are available for viewing and downloading from your Azure Active Directory" 
   services="active-directory" 
   documentationCenter="dev-center-name" 
   authors="kenhoff" 
   manager="ilanas" 
   editor=""/>

<tags
   ms.service="active-directory"
   ms.devlang="no"
   ms.topic="article"
   ms.tgt_pltfrm="na"
   ms.workload="required" 
   ms.date="03/23/2015"
   ms.author="kenhoff"/>

# Azure Active Directory Audit Report Events

## Header

## Audit Report Events

<!--- audit event descriptions should be in the past tense --->

|	Events 					| 	Description					|
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
|	Add service principal credentials	|			|
|	Remove service principal credentials	|			|
|	Add domain to company			|			|
|	Remove domain from company		|			|
|	Update domain				|			|
|	Set domain authentication		|			|
|	Set federation settings on domain	|			|
|	Verify domain				|			|
|	Verify email verified domain		|			|
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

### Audited Update User event properties

| Property				| Description	|
| ---------------------------------	| ---------	|
| AccountEnabled			|		|
| AlernativeSecurityId			|		|
| AssignedLicense			|		|
| AssignedPlan				|		|
| LicenseAssignmentDetail		|		|
| Mobile				|		|
| OtherMail				|		|
| OtherMobile				|		|
| StrongAuthenticationMethod		|		|
| StrongAuthenticationPhoneAppDetail	|		|
| StrongAuthenticationRequirement	|		|
| StrongAuthenticationUserDetails	|		|
| TelephoneNumber			|		|

## Footer
