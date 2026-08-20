# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name** : V Kamalesh Vijayakumar
* **Register Number**: 212224110028
* **Date of Submission**: 20/8/2026

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

(Write the steps you followed in your own words)

1.  I logged into the AWS Management Console, opened the EC2 Dashboard, and explored the Elastic Block Store (EBS) section to understand different volume types such as gp2, gp3, and HDD volumes.
2. I created a new EBS volume by selecting the required size and volume type and ensured that the volume was created in the same Availability Zone as my EC2 instance.
3. After creating the volume, I attached the EBS volume to the running EC2 instance as an additional storage device using the EC2 console.
4. Then I connected to the EC2 instance using SSH, formatted the new volume using the ext4 file system, and mounted it to a directory (such as /mnt/ebs). I created sample files to store data in the mounted volume.
5. Finally, I rebooted the EC2 instance and verified that the files stored in the EBS volume were still available, confirming data persistence in Amazon EBS.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created

<img width="1263" height="528" alt="image" src="https://github.com/user-attachments/assets/8ec06354-3ac4-449c-b59d-947a3c02c52d" />


---

### Screenshot 2: EBS Volume Attached to EC2

<img width="1261" height="535" alt="image" src="https://github.com/user-attachments/assets/6a60ecbf-4a06-49b0-a6b6-2eba2a27658a" />

---

### Screenshot 3: Mounted Volume with Data

<img width="1254" height="429" alt="image" src="https://github.com/user-attachments/assets/cc2b0921-6a36-4e58-9571-8cf297d4c06f" />

---

## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.
