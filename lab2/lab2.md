## Lab details
- Lab 2 week 3
- Course: **25F_CST8912_011 Cloud Solutions Architect**
- Name: **Anani Thierry Kassa**
- student ID: **041-140-713**


## Step-by-step documentation
1. Resource Group creation
![alt text](csa1.PNG)

2.	Virtual Networks
![alt text](csa2.PNG)

3. Peering configuration
    - vnet0
![alt text](csa3.PNG)
    - vnet1
![alt text](csa4.PNG)
    - vnet2
![alt text](csa5.PNG)

4. VM deployments
    - VM0
![alt text](csa6.PNG)
    - VM1
![alt text](csa7.PNG)
    - VM2
![alt text](csa8.PNG)

5. PowerShell Test-NetConnection results
    - From VM0 → VM1
![alt text](csa11.PNG)
    - From VM0 → VM2
![alt text](csa12.PNG)
    - From VM1 → VM2
![alt text](csa13.PNG)

6. Findings & Analysis:
- Why VNet peering is important

VNet peering is important because it offers private communication between VNets, low latency and high bandwith. Non-overlapping IP address spaces is crucial to maintain such a good communication between VNets.

- How private IP communication was established

Private IP communication was established by connecting virtual machine between each other. More precisely by running the **Test-NetConnection** command using the private IP address of the remote computer on the source computer.

- Benefits of global peering (performance & security)

Performance → Low latency, high bandwidth, no VPN gateway overhead.

Security → Private, encrypted backbone traffic with no internet exposure.
