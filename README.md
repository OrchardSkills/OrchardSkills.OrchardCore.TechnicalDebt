# Solving Technical Debt by Updating our Orchard Core Web Application to .NET Core 3.1

## Keeping up with Technology

# [YouTube Video](https://youtu.be/dkTz6W6zakg)

[![OrchardSkillsYouTubeThumbNailUpdate](https://user-images.githubusercontent.com/59172485/90587974-c767c780-e197-11ea-8c90-3abcce9c4b85.png)](https://youtu.be/dkTz6W6zakg)

# Introduction

In the realm of software development, every software project acquires technical debt. One of the areas a project can require technical dept is when a platform gets updated. Back on December 3, 2019, Microsoft released .NET Core 3.1. The most important feature is that .NET Core 3.1 is LTS meaning its a long-term supported release. It will be supported by Microsoft until December 3, 2022. On December 26, 2019, the Orchard Core team updated to their projects .NET 3.1.



![Technical-Debt-001](https://user-images.githubusercontent.com/59172485/90587880-a901cc00-e197-11ea-9ace-f769c14eb38f.png)

You can download the latest version of .NET Core at https://dotnet.microsoft.com/download.



![Technical-Debt-002](https://user-images.githubusercontent.com/59172485/90587884-aa32f900-e197-11ea-9dd3-6cfadbaa41f5.png)

Select the .NET Core 3.1 version.



![Technical-Debt-003](https://user-images.githubusercontent.com/59172485/90587885-aa32f900-e197-11ea-88bb-61154741d558.png)

Click on the Windows x46 version.



![Technical-Debt-004](https://user-images.githubusercontent.com/59172485/90587889-ab642600-e197-11ea-85aa-85545046d57a.png)

Load the MyOrchardCoreCMS solution. Most of the time Visual Studio will update .NET Core for you. Just make sure you have the latest version. You ca click on Help and the About to display the version.



![Technical-Debt-005](https://user-images.githubusercontent.com/59172485/90587892-ab642600-e197-11ea-85d7-bf62e90da322.png)

In order to update the .NET platform to the latest, right click on the "MyOrchardCoreCMS" project and select "Properties".



![Technical-Debt-006](https://user-images.githubusercontent.com/59172485/90587895-abfcbc80-e197-11ea-8edf-af90414959e3.png)

Now let's update to the latest NuGet packages. Right click on the "MyOrchardCoreCMS" project and select "Manage NuGet Packages...".



![Technical-Debt-007](https://user-images.githubusercontent.com/59172485/90587896-abfcbc80-e197-11ea-8289-adf969ffd635.png)

Click on the "Updated" tab, you can "Select all packages" and the press the "Update" button.



![Technical-Debt-008](https://user-images.githubusercontent.com/59172485/90587899-ac955300-e197-11ea-8d3b-f03c4357c3c3.png)

Click on the "OK" button to confirm.



![Technical-Debt-009](https://user-images.githubusercontent.com/59172485/90587903-ad2de980-e197-11ea-86c9-55182ccbaa2c.png)

Select the "MyOrchardCoreCMS.Web" from the drop down combo box and press the green play button.



![Technical-Debt-010](https://user-images.githubusercontent.com/59172485/90587905-adc68000-e197-11ea-8e77-411bb549d271.png)

Enter your site name, select the Blog recipe, your credentials and press the "Finish Setup" button.



![Technical-Debt-011](https://user-images.githubusercontent.com/59172485/90587906-adc68000-e197-11ea-9a74-5a45716d6795.png)

Your Orchard Core CMS Application is up and running with the latest software.



![Technical-Debt-012](https://user-images.githubusercontent.com/59172485/90587907-ae5f1680-e197-11ea-80fa-50477acb71ec.png)

Go to the Admin Dashboard by appending "/admin" on the URL.



![Technical-Debt-013](https://user-images.githubusercontent.com/59172485/90587908-ae5f1680-e197-11ea-9047-fd4c4836933b.png)

The Admin Dashboard is up and running as well.



![Technical-Debt-014](https://user-images.githubusercontent.com/59172485/90587909-aef7ad00-e197-11ea-8393-180c0c04972f.png)

With your favorite browser, browse to your DevOps site and select the project.



![Technical-Debt-015](https://user-images.githubusercontent.com/59172485/90587910-aef7ad00-e197-11ea-91bb-a13c6d51cd1c.png)

Select the Pipelines.



![Technical-Debt-016](https://user-images.githubusercontent.com/59172485/90587911-af904380-e197-11ea-80e4-0f5f5d7770ab.png)

Click on your CI pipeline.



![Technical-Debt-017](https://user-images.githubusercontent.com/59172485/90587912-af904380-e197-11ea-982f-1f2898fcfb89.png)

Click on Edit.



![Technical-Debt-018](https://user-images.githubusercontent.com/59172485/90587914-af904380-e197-11ea-95f6-a2f61ca10257.png)

Add a new task by pressing the "+".



![Technical-Debt-019](https://user-images.githubusercontent.com/59172485/90587915-b028da00-e197-11ea-8f93-98e147d1bcc0.png)

Search for :Use .NET Core" task and then add the task. Select "3.1.x" for the version. Save the changes.



![Technical-Debt-020-1](https://user-images.githubusercontent.com/59172485/90587916-b0c17080-e197-11ea-8354-122a79b42cc5.png)

Click on the CD Pipeline  and select the "Edit" button".



![Technical-Debt-020-2](https://user-images.githubusercontent.com/59172485/90587918-b0c17080-e197-11ea-9cc6-41b8728c0f0d.png)

Click on the "View stage tasks".



![Technical-Debt-020-3](https://user-images.githubusercontent.com/59172485/90587919-b15a0700-e197-11ea-99ec-adb0ee04c049.png)

Modify the Runtime Stack to "dotnetcore|3.1".



![Technical-Debt-023](https://user-images.githubusercontent.com/59172485/90587920-b15a0700-e197-11ea-86ff-afb0492f7e6d.png)

Go back to Visual Studio select the "Teams Explorer" tab and then the "Changes" button.

![Technical-Debt-024](https://user-images.githubusercontent.com/59172485/90587921-b1f29d80-e197-11ea-9105-30e7d86dad5c.png)

Enter you description and then press the "Commit All" button.



![Technical-Debt-025](https://user-images.githubusercontent.com/59172485/90587922-b28b3400-e197-11ea-9f62-67538f3d27a8.png)

Click on the "house" icon.



![Technical-Debt-026](https://user-images.githubusercontent.com/59172485/90587925-b28b3400-e197-11ea-8425-76c4a9cdcd5e.png)

Press the "Sync" button.



![Technical-Debt-027](https://user-images.githubusercontent.com/59172485/90587927-b323ca80-e197-11ea-8672-7b4e0b139c39.png)

Click the "Push" to push your changes to your repository.



![Technical-Debt-028](https://user-images.githubusercontent.com/59172485/90587929-b323ca80-e197-11ea-8d43-de1d90b56fcb.png)

Everything was pushed successfully.



![Technical-Debt-029-1](https://user-images.githubusercontent.com/59172485/90587932-b3bc6100-e197-11ea-87c5-347462cf6ed5.png)

Go back to the CI edit page select "Save and queue".



![Technical-Debt-029-2](https://user-images.githubusercontent.com/59172485/90587933-b3bc6100-e197-11ea-93c0-9552c2b6fb92.png)

Click the "Save and Run"



![Technical-Debt-030](https://user-images.githubusercontent.com/59172485/90587936-b454f780-e197-11ea-8a94-75d4fca50f00.png)

Once the build task has been queued, click on the "Agent job 1" link.



![Technical-Debt-031](https://user-images.githubusercontent.com/59172485/90587937-b4ed8e00-e197-11ea-9ce6-058bddd79ba7.png)

Build is now successful.



![Technical-Debt-032](https://user-images.githubusercontent.com/59172485/90587938-b4ed8e00-e197-11ea-8be0-0e90aadfd1a8.png)

Select the CD pipeline and select the latest release queued.



![Technical-Debt-033](https://user-images.githubusercontent.com/59172485/90587941-b5862480-e197-11ea-9596-14f271902a4f.png)

The delivery was successful.



![Technical-Debt-034](https://user-images.githubusercontent.com/59172485/90587944-b5862480-e197-11ea-9eea-043b7a6f1b71.png)

With your favorite browser, browse to your site. Congratulations you got rid of some of your technical debt. Everything is working with the latest software.

 

![Technical-Debt-035](https://user-images.githubusercontent.com/59172485/90587945-b61ebb00-e197-11ea-91e0-f869bd56096c.png)

Append "/admin" to your URL and enter your credentials to access the Admin Dashboard.



![Technical-Debt-036](https://user-images.githubusercontent.com/59172485/90587946-b61ebb00-e197-11ea-9764-5c905710304c.png)

Admin Dashboard has been updated and working as well.



# Conslusion

Technical Debt can be seen as a shortcut, which saves teams’ time, effort and/or money today, but might lead to increased costs in the future. Technical Debt cannot really be avoided in software projects.  If the team and the customer handle the risk of Technical Debt properly, it should remain manageable. Any repayment should be a business decision. Even if the repayment is so small that a consultation with the customer does not make sense, the developer must always ask himself whether an improvement of the code really justifies the invested time and effort.



# GitHub

The complete source code is located [here](hhttps://github.com/OrchardSkills/OrchardSkills.OrchardCore.VisualStudioOnline).

