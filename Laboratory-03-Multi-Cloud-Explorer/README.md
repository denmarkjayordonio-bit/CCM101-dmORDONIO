## Operating System

I used the `cat /etc/os-release` command to check what operating system the Linux server is using. Based on the result, the server is running **Ubuntu 24.04.4 LTS (Noble Numbat)**.

<img width="1440" height="852" alt="image" src="https://github.com/user-attachments/assets/0d4c9d89-19ae-497a-883a-7830c638f38b" />


## CPU Information

I used the `lscpu` command to check the CPU details. The result shows that the server has **1 CPU**, uses **x86_64 architecture**, and has an **Intel Xeon E312xx** processor. It is also using **KVM virtualization**, which means the Linux server is running in a virtual machine.

<img width="1440" height="852" alt="image" src="https://github.com/user-attachments/assets/d765838f-1d92-45df-877e-4378e11f9c86" />


## Memory

For the memory, I used the `free -h` command. The server has **1.9 GiB of total memory**, and about **1.4 GiB was still available** when I checked it.

<img width="1440" height="852" alt="image" src="https://github.com/user-attachments/assets/f4191bef-548c-4d4d-9689-b554524a9bb5" />


### Disk Space

I used the `df -h` command to check how much storage the server has. The main filesystem has **19 GB of total space**, with about **5.4 GB already used** and around **13 GB still available**. This means that only about **30% of the disk space is currently being used**.

<img width="1440" height="852" alt="image" src="https://github.com/user-attachments/assets/cd52e8f2-a13c-49a6-92dc-c2877a4ea7d9" />


### Cloud Migration

Based on the information I gathered, I think this Linux server can be moved to any of the three major cloud platforms: **AWS, Azure, or Google Cloud Platform (GCP)**. All three platforms support Linux virtual machines, including Ubuntu. The server's current CPU, memory, and storage requirements can be matched with a suitable virtual machine configuration in any of these cloud platforms.
