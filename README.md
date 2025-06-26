# 🧪 Lab: Create Partitions and Filesystems

🛠️ What I Did in This Lab
I created disk partitions using tools like fdisk, gdisk, and parted. Then, I applied filesystems using commands like mkfs.ext4, mkfs.xfs, and mkswap. Finally, I reviewed how Btrfs can support advanced features like compression and subvolumes

1️⃣ Manage MBR and GPT Partition Tables
🔹 Use fdisk for MBR Partitioning
bash
Copy
Edit
sudo fdisk /dev/sdX
Create a new primary partition

Set the partition type if needed (e.g., Linux or swap)

Write and save changes

🔹 Use gdisk for GPT Partitioning
bash
Copy
Edit
sudo gdisk /dev/sdX
Create new partitions under GPT scheme

Review the partition table with p

Save with w

🔹 Use parted for Interactive Partitioning
bash
Copy
Edit
sudo parted /dev/sdX
Use commands like mklabel gpt and mkpart

Confirm with print to see partition layout

2️⃣ Create Filesystems Using mkfs
🔹 Format to ext4
bash
Copy
Edit
sudo mkfs.ext4 /dev/sdX1
🔹 Format to XFS
bash
Copy
Edit
sudo mkfs.xfs /dev/sdX2
🔹 Format to VFAT (FAT32)
bash
Copy
Edit
sudo mkfs.vfat /dev/sdX3
🔹 Format to exFAT
bash
Copy
Edit
sudo mkfs.exfat /dev/sdX4
3️⃣ Create and Enable Swap Space
🔹 Create a Swap Partition
bash
Copy
Edit
sudo mkswap /dev/sdX5
sudo swapon /dev/sdX5
🔹 Verify Swap
bash
Copy
Edit
swapon --show
free -h
4️⃣ Explore Btrfs (Basic Feature Knowledge)
🔹 Create a Btrfs Filesystem
bash
Copy
Edit
sudo mkfs.btrfs /dev/sdX6
🔹 Mount with Compression (zlib or lzo)
bash
Copy
Edit
sudo mount -o compress=zlib /dev/sdX6 /mnt
🔹 Create a Subvolume
bash
Copy
Edit
sudo btrfs subvolume create /mnt/myvol

## 🎯 What I Learned
In this lab, I learned how to manage both MBR and GPT partition tables using CLI tools. I practiced creating and formatting different filesystems and enabling swap. I also got a hands-on introduction to Btrfs and its advanced features like compression and subvolumes. This lab improved my confidence with disk preparation and partition management in a Linux environment. 
