# Deploying a Standardized Desktop Wallpaper Using Group Policy
![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=flat&logo=youtube&logoColor=white)

https://youtu.be/hzmznYfqa34

## Short Summary
![Active Directory](https://img.shields.io/badge/Active_Directory-5E5E5E?style=for-the-badge&logo=microsoft&logoColor=white)

In this lab, I demonstrated how to deploy a desktop wallpaper to users within a specific Organizational Unit (OU) using Group Policy. The wallpaper file was stored on a shared network location, appropriate read permissions were configured, and a Group Policy Object (GPO) was created to apply the wallpaper to client systems. I then verified network access to the shared folder and confirmed successful deployment on a client workstation.

## Project Overview

This lab focused on using Active Directory Group Policy to centrally manage desktop wallpaper settings for domain users. The goal was to ensure that users within a designated OU received a consistent desktop wallpaper from a centrally managed network location.

## Goal

To deploy a desktop wallpaper to users in a specific OU through Group Policy while ensuring clients could access the wallpaper file from a shared network location.

## What I Did

1. Created or used a network shared partition to store the desktop wallpaper image.
2. Stored the wallpaper file in the shared location.
3. Configured read permissions on both the wallpaper file and the folder containing it.
4. Verified that client systems could access the shared folder and wallpaper file.
5. Created a Group Policy Object to configure the desktop wallpaper setting.
6. Configured the wallpaper policy to use the shared network path of the image.
7. Linked the GPO to the target users' Organizational Unit.
8. Forced a Group Policy update on the client system.
9. Restarted the client workstation.
10. Confirmed that the desktop wallpaper was successfully applied after policy processing.

## Tools and Technologies

* Windows Server
* Active Directory
* Group Policy Management
* Organizational Units (OUs)
* Shared Network Folders
* NTFS and Share Permissions
* Windows Client Workstation

## Technical Decisions

* Stored the wallpaper on a shared network location so it could be centrally managed.
* Configured read permissions to allow client systems to retrieve the wallpaper file.
* Used a UNC network path within the Group Policy setting to ensure clients could locate the image.
* Verified client access before applying the policy to help ensure successful deployment.

## Validation

To verify the configuration:

* Confirmed that the client could access the shared folder containing the wallpaper.
* Forced a Group Policy update.
* Restarted the client workstation.
* Verified that the configured wallpaper was applied successfully.

## Outcome

The desktop wallpaper was successfully deployed to the target client through Group Policy after policy updates and system restart.

## Skills Demonstrated

* Active Directory administration
* Group Policy configuration
* Organizational Unit management
* Shared folder configuration
* Permission management
* Client access verification
* Group Policy troubleshooting and validation
* Windows Server administration
