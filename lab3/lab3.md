# Assignment 3

1.	Create Storage Account- Create a storage account named labtest8912 under your student subscription.
![alt text](i1.PNG)

2.	Use the resource group CST8912-demo.
3.	Select Canada Central as the region.
4.	Choose Geo-redundant storage (GRS).
5.	Keep networking and data protection options as default.
6.	Modify Redundancy and Access Tier

7.	Go to your storage account → Data Management → Redundancy
8.	Change redundancy from Geo-redundant (GRS) to Local redundant (LRS).
9.	Under Configuration, set Blob access tier to Cool, then save.
![alt text](i9.PNG)
10.	Create Container and Upload Blob
![alt text](i10.PNG)
11.	Under Data Storage, click Containers → create a container named labtestcontainer8912.
12.	Upload a blob into folder sampletest8912.
![alt text](i12.PNG)
13.	Change Advanced Settings → Access Tier to Hot
![alt text](i13.PNG)

14.	Use the sample files link provided (ask instructor if not available).

15.	Test Private Access
16.	Click the uploaded file in the container.
17.	Copy the Blob URL.
https://labtestalg8912.blob.core.windows.net/labtestcontainer8912/sampletest8912/biostats.csv

18.	Open a private/incognito browser window, paste the URL.
19.	Verify that it does not work (public access is private → resource not found).
![alt text](i19.PNG)
20.	Generate Shared Access Signature (SAS)
21.	On the file blade, click Generate SAS.
22.	Copy the SAS Token URL.
https://labtestalg8912.blob.core.windows.net/labtestcontainer8912/sampletest8912/biostats.csv?sp=r&st=2025-09-25T21:52:17Z&se=2025-09-26T06:07:17Z&spr=https&sv=2024-11-04&sr=b&sig=Jmw1%2FL%2BOKVmbFmXxsy8UPTopSMm7yGpGrpkjI%2BOONW0%3D
23.	Paste it into the private browser window.
24.	Verify that you can now access the file.
![alt text](i24.PNG)

25.	Create Lifecycle Management Rule
26.	On the container blade, under Data Management → Lifecycle Management, create a new rule: Rule Name: myrule8912
27.	Scope: Limit blobs with filters -- Blob type/subtype: Default
![alt text](i27.PNG)
28.	Condition: Base blobs last modified more than 15 days ago → Move to Cool storage
![alt text](i28.PNG)
29.	Clean Up & Document--Delete all resources created during this lab.

30.	Submit a lab report with screenshots for each step.
    - Resource group deleted
![alt text](i30.PNG)

   - Storage account deleted
![alt text](i30-1.PNG)