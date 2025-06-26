# 🧪 104.1 Create Partitions and Filesystems

## 🛠️ What I Did in This Lab
I created disk partitions using tools like fdisk, gdisk, and parted. Then, I applied filesystems using commands like mkfs.ext4, mkfs.xfs, and mkswap. Finally, I reviewed how Btrfs can support advanced features like compression and subvolumes

I’ve included some helpful links to guide you through the lab and for studying afterward:

[EXAM OBJECTIVE 104.1](https://www.lpi.org/our-certifications/exam-101-102-objectives/#104.1_Create_partitions_and_filesystems)

[OBJ.104.1 NOTES]()

[OBJ.104.1 LAB]()

---

# 0️⃣ ⚠️ The Errors I Encountered
Value out of range.
No enough free sectors available.

![nQ4QlP9](https://github.com/user-attachments/assets/e574acfc-8c5b-4f57-96ab-680cedfc0db9)

## 1️⃣ Manage MBR and GPT Partition Tables
🔹 Use fdisk for MBR Partitioning

![1CMQ6y0](https://github.com/user-attachments/assets/cfe549c7-24ec-4e7f-9d51-c7f34fed9d3d)

![6fnOoea](https://github.com/user-attachments/assets/94724490-ea78-40ed-9838-437fc3471a11)

🔹 Use gdisk for GPT Partitioning

![ZsDFk3r](https://github.com/user-attachments/assets/bb62f15e-5257-4628-95a9-6d3a637c8fdf)

![9VwGWSe](https://github.com/user-attachments/assets/234f121e-c09e-4a32-a402-23b368d22102)

🔹 Use parted for Interactive Partitioning

![61TG0eB](https://github.com/user-attachments/assets/157bd36f-7a7b-481a-a985-f1d5b0d2adf5)

## 2️⃣ Create Filesystems Using mkfs
🔹 Format to ext4

![cgvywbK](https://github.com/user-attachments/assets/9c144be7-6aac-4504-ba7d-8067fdf9f13a)

🔹 Format to XFS

![ulz4sOS](https://github.com/user-attachments/assets/0694f27a-29a7-465a-a0b5-40615829f6e7)

🔹 Format to VFAT (FAT32)

![dvNdGxp](https://github.com/user-attachments/assets/29cd4aff-23fe-4ca2-b71b-345da89b7a65)

## 3️⃣ Create and Enable Swap Space
🔹 Create a Swap Partition

![lBw8Per](https://github.com/user-attachments/assets/b48f6380-dd74-4c6a-bb7b-31b6a9f3354d)

🔹 Verify Swap

![i4aYvBw](https://github.com/user-attachments/assets/ef105626-00f5-4c8c-a842-04331b00b44c)

---

## 🎯 What I Learned
In this lab, I learned how to manage both MBR and GPT partition tables using CLI tools. I practiced creating and formatting different filesystems and enabling swap. I also got a hands-on introduction to Btrfs and its advanced features like compression and subvolumes. This lab improved my confidence with disk preparation and partition management in a Linux environment. 
