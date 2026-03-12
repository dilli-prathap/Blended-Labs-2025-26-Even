# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name**: DILLI PRATHAP
* **Register Number**: 212224110014
* **Date of Submission**: 12-03-2026

---

## Objective

The objective of this experiment is to understand how Amazon Elastic Block Store (EBS) provides persistent block-level storage for EC2 instances. This lab focuses on creating and attaching an EBS volume, formatting and mounting it on an EC2 instance, storing data, and verifying data persistence after instance reboot.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing EC2 instance (Amazon Linux 2 preferred)
* Basic knowledge of Linux commands

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Amazon EBS
* SSH Client (Terminal / PuTTY)

---

## Tasks Performed

### Task 1: Explore Amazon EBS

Explore the Amazon EBS service through the EC2 dashboard. Observe different volume types such as General Purpose SSD (gp2/gp3), Provisioned IOPS SSD, Throughput Optimized HDD, and Cold HDD.

---

### Task 2: Create an EBS Volume

Create a new EBS volume in the same Availability Zone as the EC2 instance. Choose an appropriate size and volume type.

---

### Task 3: Attach EBS Volume to EC2 Instance

Attach the created EBS volume to the running EC2 instance as an additional block device.

---

### Task 4: Format the EBS Volume

Connect to the EC2 instance using SSH and format the attached volume with a file system (for example, ext4).

---

### Task 5: Mount the EBS Volume

Mount the formatted volume to a directory in the EC2 instance (for example, /data or /mnt/ebs).

---

### Task 6: Store Data in EBS Volume

Create files and directories inside the mounted EBS volume and store sample data.

---

### Task 7: Verify Data Persistence

Reboot the EC2 instance and verify that the data stored in the EBS volume is still available after reboot.

---

## Workflow (Student Explanation)

1. I logged in to the **AWS Management Console** and opened the **EC2 Dashboard**. Then I explored the **Elastic Block Store (EBS)** section to understand the different volume types available.

2. I created a new **EBS volume** by selecting the required size and volume type. While creating the volume, I made sure it was in the **same Availability Zone** as my running EC2 instance.

3. After the volume was created, I attached the EBS volume to the EC2 instance as an **additional block device** using the **Attach Volume** option.

4. I connected to the EC2 instance using **SSH**, identified the attached volume using the `lsblk` command, and formatted the volume with the **ext4 file system**.

5. I created a directory, mounted the EBS volume to that directory, stored sample files in it, and then rebooted the EC2 instance to verify that the **data persisted after the reboot**.


---

## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created

<img width="1101" height="1007" alt="Screenshot 2026-03-12 102151" src="https://github.com/user-attachments/assets/f7fbe1a3-f950-4e4c-91db-bdf064ba87b4" />

---

### Screenshot 2: EBS Volume Attached to EC2

<img width="1113" height="944" alt="Screenshot 2026-03-12 102600" src="https://github.com/user-attachments/assets/d134f8f0-0e58-4626-a2d7-9ba6e81e942f" />


---

### Screenshot 3: Mounted Volume with Data
<img width="1531" height="978" alt="Screenshot 2026-03-12 103046" src="https://github.com/user-attachments/assets/0e02d1e8-de71-40a2-aab2-316d1d70234e" />

<img width="1532" height="948" alt="Screenshot 2026-03-12 104100" src="https://github.com/user-attachments/assets/a32fc92f-7194-4759-a4a4-54fcb8140687" />

<img width="1529" height="956" alt="Screenshot 2026-03-12 105359" src="https://github.com/user-attachments/assets/b33b5489-f565-4f35-a722-aac14f61659f" />

---

## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.
