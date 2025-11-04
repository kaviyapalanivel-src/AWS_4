Understood. Below is a **clean professional README** with no suggestions, no extra lines — only final task content.

---

# AWS EC2 and EBS Implementation

## Objective

Deploy an EC2 instance, install a web server, create and attach an EBS volume, create a snapshot, and provision a new volume from that snapshot.

---

## Steps Performed

### 1. EC2 Instance Launch

* AMI: Ubuntu
* Instance type: t2.micro
* Security group rules:

  * SSH (22)
  * HTTP (80)
* Instance launched in a public subnet with internet access

---

### 2. Web Server Installation (Apache)

Connected to the instance via EC2 Instance Connect and executed:

```
sudo apt update
sudo apt install apache2 -y
```

Verified by accessing the public IP of the instance in a browser — default Apache page displayed.

---

### 3. EBS Volume Creation

* Created a 5GB EBS volume
* Selected the same Availability Zone as the EC2 instance

---

### 4. EBS Volume Attachment

* Attached the 5GB volume to the EC2 instance through the AWS console
* Verified using:

```
lsblk
```

---

### 5. Snapshot Creation

* Created a snapshot from the attached EBS volume

---

### 6. New Volume Creation From Snapshot

* Created a new EBS volume using the snapshot
* Verified successful volume creation

---

## Evidence / Documentation

Screenshots provided for:

* EC2 instance running
* Apache web page
* EBS volume creation
* Volume attachment
* Snapshot
* New volume created from snapshot

---

## Conclusion

Tasks successfully completed:

* EC2 instance deployment
* Apache web server installation
* EBS lifecycle management: create, attach, snapshot, restore

---

Done.
