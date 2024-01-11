
|                              **DOCUMENT - 2**![](https://lh7-us.googleusercontent.com/rJGHjBDcudv_cH82n4DBL0i4JakFj_mzDq3rss2IgqsUHvrEVVAfg2N6BUBHTE2UteEXsvkgShNZABs7hRTNPPiaDyCrG_2JfuY5YAI73GL-u2qw5vAvwmgQWBVArMqCI2sP2SDUrs6SuIRR2DhdTVk)                **Elastic Block Store**                      **By: Vinus Beniwal**                               **(Dec. Intern)** |

**CONTENT**

[INTRODUCTION ](#introduction)

[Features of Amazon EBS ](#features-of-amazon-ebs)

[1. Block Storage: ](#block-storage)

[2. Snapshots for Backup: ](#snapshots-for-backup)

[3. Elasticity: ](#elasticity)

[4. Encryption: ](#encryption)

[Points to be covered in EBS ](#points-to-be-covered-in-ebs)

[1. Volumes ](#volumes)

[Function: ](#function)

[Use Cases: ](#use-cases)

[2. Snapshots ](#snapshots)

[Function: ](#function-1)

[Use Cases: ](#use-cases-1)

[3. Lifecycle Manager ](#lifecycle-manager)

[**Steps to connect Snapshot and Volume ****6**](#steps-to-connect-snapshot-and-volume)

[ Reference Links ](https://docs.google.com/document/d/169RwX8mxG6m0NeVpV2lYFTqZOCAGXBEFdVj9j_u2Sfs/edit#heading=h.i4bywjb89x1z)


# INTRODUCTION<a id="introduction"></a>

                              EBS stands for Elastic Block Store

Amazon Elastic Block Store (EBS) in AWS is like a virtual hard drive for your virtual computer (EC2 instance). It's a way to store your data in the cloud.

**Think of it as a Virtual Hard Drive:**

When you create a virtual computer in AWS (an EC2 instance), you need a place to store your files and data. EBS is like a virtual hard drive that you can attach to your virtual computer.

So, in simple words, EBS is like a flexible, virtual hard drive that you can attach to your virtual computer in AWS, and it helps you store and manage your data in the cloud.

![](https://lh7-us.googleusercontent.com/9edT5ww_9tIsvz7dUBhRL7yGuEdH7Jvf2s2m2kDkgUKfloq_IlpYTlccX6ZL9xCPh6LQZR4s-z3ad_SfGLGX5arzuQQ4bdK-ZOBN7ggHuGrHcTCg_SldjvbIV_xBPGWvAiVYrvU0LuEfsOrlaT32AUc)


#   Features of Amazon EBS<a id="features-of-amazon-ebs"></a>

1. ## **Block Storage:** <a id="block-storage"></a>

EBS provides block-level storage volumes that you can attach to EC2 instances. These volumes behave like raw, unformatted block devices, and you can install a file system on them as you would with a physical hard drive.

2. ## **Snapshots for Backup:**<a id="snapshots-for-backup"></a>

 You can take snapshots of your virtual hard drive at specific points in time. It's like taking a picture of all your files so that if something goes wrong, you can go back to that picture and recover everything.

3. ## **Elasticity:**<a id="elasticity"></a>

 EBS volumes can be easily attached to or detached from EC2 instances. This flexibility allows you to scale your storage needs up or down based on your application requirements.

4. ## **Encryption:** <a id="encryption"></a>

EBS volumes can be encrypted using AWS Key Management Service (KMS) keys, providing an additional layer of security for sensitive data.

**\*** It's important to note that the features and capabilities of AWS services, including EBS, may evolve over time as AWS continues to enhance its offerings.


#   Points to be covered in EBS<a id="points-to-be-covered-in-ebs"></a>

1. **Volumes**

2. **Snapshots**

3. **Lifecycle Manager**

1) ## **Volumes**<a id="volumes"></a>

In Amazon Elastic Block Store (EBS), volumes and snapshots serve important functions related to storage management and data protection. Let's explore the functions of volumes and snapshots in EBS:


### Function: <a id="function"></a>

An EBS volume is a block-level storage device that can be attached to an Amazon EC2 instance. It provides a persistent and durable storage solution, independent of the lifecycle of the associated EC2 instance.


### Use Cases:<a id="use-cases"></a>

- Primary storage for EC2 instances.

- Stores the operating system, applications, and data.

- Used for various workloads, including databases, file systems, and application storage.

2. ## **Snapshots**<a id="snapshots"></a>


### Function: <a id="function-1"></a>

An EBS snapshot is a copy of an EBS volume. It captures the entire state of the volume, including all data, configuration, and settings.


### Use Cases:<a id="use-cases-1"></a>

- Backup and Data Protection: Snapshots provide a backup mechanism for EBS volumes, allowing you to restore data in case of data loss or corruption.

* Copying Volumes: Snapshots can be used to create new volumes.

- Migrating Data: Useful for migrating data across AWS accounts or regions.

3. ## **Lifecycle Manager**<a id="lifecycle-manager"></a>

      

With Amazon EBS Lifecycle Manager, you can automate the creation, deletion, and retention of EBS snapshots, making it easier to manage your backup and retention policies.

It provides flexibility in defining policies and integrates with other AWS services to enhance overall data protection and management capabilities.


# Steps to connect Snapshot and Volume<a id="steps-to-connect-snapshot-and-volume"></a>

- Snapshots are often used in conjunction with volumes for backup and recovery purposes.

* To create a backup, you typically initiate a snapshot of the EBS volume. This snapshot can then be used to restore the volume or create new volumes.

**Step1:** Launch an Instance of any Linux machine(Refer to document 1 - EC2 Instance). Copy the storage address or “public IP address” and “root device name” separately.

![](https://lh7-us.googleusercontent.com/wLH97A-PRunfbdAFpnZk1okMD53hKjbT-JiE6cIOFK21kxfAeSfk8VHBT2Ck4S93x-3c0NhNA-PS6mWkrUXElJlsq2NJutqrPBs5SXoOfz4O2ky3pLjiTeXmmTPVx86JkygXiajrA4rIlPSLwT6K-xU)

****![](https://lh7-us.googleusercontent.com/KNB3AgUhtpE5xmWmooJHOJ1biLJH1cNHSsrIMDvk9OgiRIwBCJ6PGshbeJQ1OuXpwda_CT4CFh5QItTpXHmw2480lT1gh2NSqe01p4cgQ54O8I_3dyLDo4Sojhiskcs3lqgefdzQKkl1irNqBSF2tDA)****

**Step2:** Connect this instance and add some information on this machine for testing purposes. Copy the password separately.

![](https://lh7-us.googleusercontent.com/tT5AAHU6xseGuKVM_n_PhFidbYMN8okQ78m8BUpuQW2YmTgjKo4P970qXrZRyBBk6kdHzXLyXtd2NIGdWebwhst8C7YPvQYjFAWSKn6_iGVp6uXLYfsWTB0UiXV1it5HkMWNhGV4f_oFKwa6926M9zs)

**Step3:** Now take a snapshot of this Linux Machine by following steps. 

- Go to Snapshot

- Click on create snapshot

![](https://lh7-us.googleusercontent.com/czx_lht4LiqVZqBdHTpAgQELuW89hEsXfjdkY_SSOPG1HUES6FO_xtxKHkFe75PsfABnSbsdo-g0fWakhcdD2p0PWN0Tn9k9BJp-s7gyjfZx4WhX8jGuAIAB2vh61p2giKtFDQRbmhJUCyU04uxGNL4)

![](https://lh7-us.googleusercontent.com/VNeoR8b0bX9q44RmyibosPK73DiiVYlVa_x-AA9_ZlbbGuO_TdqUMoXwOxuQIR0JvOxoaG__8rlaM0Fr18a1HQKS_oebF5GLScYYn9AjNV2jxpaY8kV3Z5dz0XE8ZqH4HDInvKs1COUw_G01l54A4DA)

- You will see Snapshot Setting on screen.

- Then choose Instance, because you are creating snap of an instance in which there is your data

- Then you find the Instance ID selection option below.

![](https://lh7-us.googleusercontent.com/oI8eX4jAafL7tloRJjbyihFfyGfdxsAq2C5WZr0ynIfCPkmZHrltRL6cPHl9m_aWRluhE3MwbpMPA7UryYtqysDSuywpJ8aB9CgD-nUKLoOoh-IDUERSCJ12UU-6EOD17Wb3zdDKORDO-M0aXIH2vNQ) ****

- Simply select the created instance.

- Then add any description related to your instance.

![](https://lh7-us.googleusercontent.com/uxotKmjBlC8fyRJKDkRoNXpsdLst1ui9XC7fMCX7r29qNh_MwN9CuH0kdq8y5cnGULC7ZHGZf1TqbqsSeMEpI1AWbdJ5FGD4-Z9lYJMYXx59Yw5OVmMoRrjTxF1i1G_TosIlXN2udR5A38vXCga7nvg)

- Now click on Create Snapshot.

![](https://lh7-us.googleusercontent.com/GzNbGwScTkoMw-YxPq6Aw9hO41odfB3aB1_OtgkGs3Ur-la92vUE51d0QdNuXpjp6gIELRPSEDZXajfBeQi_BfWUMfTKJXFwFmWSbzyMEGxhkgp07qknCwfqBpFbht7lI5FhscW8XbGzPstp1lwtX8E)

**Step4:** Now terminate your instance.

**Step5:** To restore the data, first of all convert your snapshot into volume.

- Select the snapshot.

- Go to actions and select “Create Volume from snapshot.

![](https://lh7-us.googleusercontent.com/jnrsmWy6LdyUVgB85EEd8n7-bV17Dx-x37nzI15ljRYYxKsiIlty9va94nahM3yo6kKWJubDf8tkfAID6nx_33GhyftctaC8Y2Au-q2AUBnlDVnR2tyE1w287cHu3a7ugY4Ggv4HyGxSvRdL9YkhU_w)

- Now simply click on create volume.

![](https://lh7-us.googleusercontent.com/zIdPkZy1g72kmJa1eCo84F3HZPWADcW4r0n747q9RdnTDVQM5qlJudxy-Z73ItXYLXaXSyMFZ27NCyY1e2_E7bprKs--rZrDAxXomBtFm_07d5nY8zUsxbx9kq3V2JRP_hVVaWzloHOtWQ3fQ9KEj7s)

**Step6:** Now launch a new instance of the same Linux image with a fresh key pair and simply stop the created Instance.

![](https://lh7-us.googleusercontent.com/VobOaczufevWT8s5_gKQO0E6Bw51MzZRibwLQ5wI1DNo-ZLxNtszKdaMHhCnNN5mlJqlxcJtlWaFcMp5_3SEIkS12Hkel6I-YoVuoZa94_N2bk3UX2tEdq_nQNf1mSLPFu46OBmtKC8-0w-P73ojrkY)

**Step7:** Remove the volume from this new Linux machine(instance). And then stop the instance.

- Go to Volume

- Select the Volume having the instance ID of the newly created machine.

-  Now go to the actions option and select “Detach Volume”.

![](https://lh7-us.googleusercontent.com/GGwy811BVgDoJT6qQppISW650vGAVr7N0HDhce18w8hLWJgws2_1NoVQmPfNI8AJU1cQ4B02qSCqa1xLkaWHZ8o2DeAdbvPKK9zSKdmheGP8BzBSdL9BvjR8BNc0MFkpJ7PCakwY8nbDHbZrnpocWKQ)

**Step8:**  

- Now attach the Volume of Previous Instance to the freshly created machine.

****![](https://lh7-us.googleusercontent.com/-Tooj7b6NZ5Zbezi_IF37jVtf2CtEZdgrY4f4_VzieK63omdOiBrbVYiGfSGerci-XUWF6ozZCsDUp1ibRqgPJV8TTGFHTEUZx4i6FXSNupV5Po7n1FqwPTh-iqNhK8pP8LBfWf7iHw0yFQkHTJpkwA)****

- You will find a new  page in which you have to select the newly created instance.

- Secondly you will find an option of Device name, where you have to enter the saved “Root device name” of the previous machine.

![](https://lh7-us.googleusercontent.com/QT0lNVoVFh08zkYp2YRNTn3YA2tQRb13hgUa0vs3VR54FO5XL5UhQ8iXB_63viDP0-HBmGQonxit_sTXAmwzC2rCy0Rvoyuds0D8ujQdKeaBqjNIkaDNpbHb6fmgdbx3ep0sWdHBq7_MKatB6XXw_8c)

- Now click on Attach volume.

**Step9:** Now restart the “Stopped” instance.

**Step10:** After restarting, connect the instance and you will find your data that was added to the previous instance.

![](https://lh7-us.googleusercontent.com/BF2bXdJa-sbXSPBwFm_oX9eyft2DqNBcWCJmeAm3TP5u0Vn1EFqj9TRBNTWJDAZ7tE0bOQdU4NfVeWClnHTYoSE3bHqtNda-N3Bg6L7330JhsRamSmanw8G0tNsQTXtYP1uoyvlp-ty1Iy4mDlVHUjs)


# Reference Links<a id="reference-links"></a>

<https://us-east-1.console.aws.amazon.com/ec2-instance-connect/ssh?region=us-east-1&connType=standard&instanceId=i-09ee79d702aa4163f&osUser=ec2-user&sshPort=22#/>

<https://us-east-1.console.aws.amazon.com/ec2/home?region=us-east-1#Instances>:

<https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-volumes-multi.html>
