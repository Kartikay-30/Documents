# **Amazon Simple Storage Service (S3)**
 ![](https://lh7-us.googleusercontent.com/WOlJBvLCsKT12z00a5hQoX9j_WxoTnZScpnus8W-Mtun6aIH99F_2gNc8JD1Fj-olR9oxKiEyE3_HyM8Ej6TraOsej69x7A08X5H-hPH75AmaSdV7yOV5Z478qE1N0K7bGjycCrcxjjOoKHRu9iOko8)
 ![](https://lh7-us.googleusercontent.com/7e_z6E1UOJsdOk0-lBYKF36oM3x12OrGLogvQWg-m1Pn4xjpFOUiQbLw-w5xUuBhMelc8kJVPK4PWxZ2vPvG8p_Kj9DwW0BFv8sMeeYILqQzZBZsJPZQOtXGnLucDme3msej9y_iF9TNRaqrW__Ydnk)
 # **By:- Kartikay (December Intern)** 

**Table of Content:-**

[1. What is AWS ? ](#what-is-aws-)

[Benefits of AWS:- ](#benefits-of-aws-)

[2. What is Amazon S3 ? ](#what-is-amazon-s3-)

[3. Features of Amazon S3:- ](#features-of-amazon-s3-)

[➔ Storage Classes ](#storage-classes)

[➔ Storage Management ](#storage-management)

[➔ Access Management & Security ](#access-management--security)

[➔ Data processing ](#data-processing)

[➔ Storage logging & Monitoring ](#storage-logging--monitoring)

[4. How Amazon S3 Works ](#how-amazon-s3-works)

[Key Points :- ](#key-points--)

[(a) Bucket ](#bucket)

[(b) Objects ](#objects)

[(c) Key ](#key)

[(d) S3 Versioning ](#s3-versioning)

[(e) Version Id ](#version-id)

[(f) Bucket Policy ](#bucket-policy)

[(g) S3 Access Point ](#s3-access-point)

[(h) Access Control Lists (ACL) ](#access-control-lists-acl)

[(i) Region ](#region)

[# Reference Links ](#-reference-links)

1. #  What is AWS ?<a id="what-is-aws-"></a>

- Amazon Web Services (AWS) is a secure cloud services platform, offering compute power, database storage, content delivery and other functionality to help businesses scale and grow.

![](https://lh7-us.googleusercontent.com/A1F0KTFAFOcqnwmKC-COzqBSO6IwXp7p3GZb1Yxm2lcW_BjyLBgfEE5xkkByv7qt9rMemMEkEtSVxI4WjI4WghSdZan21SlPTHI1ob8I97fFSXVCynvY1EJew0LLKVssd1FE7i8w0FwAXsEVZeBjYl0)


## Benefits of AWS:-<a id="benefits-of-aws-"></a>

- Flexibility

- Cost Effective

- Scalability

- Security

- User-friendly

- Data Encryption

2. #  What is Amazon S3 ?<a id="what-is-amazon-s3-"></a>

-  Amazon S3 is like a virtual space on the internet where we can store and retrieve any amount of data at any time. It is like an online storage warehouse where we can keep your files, documents, images, videos, and more. 

- S3 is designed to be highly scalable, reliable, and easy to use, making it a popular choice for businesses and developers to store and manage their digital content in the cloud.

![](https://lh7-us.googleusercontent.com/QbxhVoxPeRRe_L2l8Fefj7xV9zFhGXElm_qu4Gk87WXsCvvQzhQX25O5nh5HQnNhHtfqew3Hasd0Z-d4qvN5MgyvhBjDE23ox0FlkWYPXbP6bROiurLxDFkENP5vLGEb5QmC4iqPwiuZPl_hpUxbKvU)

- Amazon S3 is designed for **99.999999999% (11-9's)** of durability, and stores data for millions of customers all around the world.

3. #  Features of Amazon S3:-<a id="features-of-amazon-s3-"></a>

- ## **Storage Classes**<a id="storage-classes"></a>

Amazon S3 storage classes are designed to give customers flexibility when storing their data on AWS. Four storage classes are available: 

- **Standard:** the default storage class and is suitable for most workloads.

- **Standard – Infrequent Access (Standard – IA):** designed for data accessed less frequently but still needs to be quickly accessible.

- **Reduced Redundancy Storage (RRS):** designed for data that can be safely stored with lower levels of redundancy.

- **Glacier:** designed for infrequently accessed data and can be stored for long periods at a lower cost.

* ## **Storage Management**<a id="storage-management"></a>

- Amazon S3 storage management lets us control how our data is stored and organized within our Amazon S3 buckets. With storage management, we can specify how Amazon S3 keeps our information, whether held in a standard storage or infrequent access (IA) storage class and stored in a bucket versioning-enabled or versioning-disabled bucket. We can also specify whether Amazon S3 encrypts our data at rest and whether our data is automatically compressed.

* ## **Access Management & Security**<a id="access-management--security"></a>

- Amazon S3’s access management features allow you to control who has access to your data securely. You can manage access to your data using access control lists (ACLs) or Amazon S3 bucket policies. ACLs allow you to grant granular permissions to individual users or groups.

* ## **Data processing**<a id="data-processing"></a>

- Data processing refers to taking data and manipulating it to extract valuable information. This can be done through various methods.

Amazon S3 offers a variety of features that make it an ideal platform for data processing, including:

- **Scalability:** Amazon S3 can scale to accommodate any amount of data, making it ideal for big data processing.

- **Flexibility:** Amazon S3 supports various data formats, making it easy to process data from multiple sources.

- **Durability:** Amazon S3 is designed to be highly durable, meaning that data is unlikely to be lost even if there are hardware failures.

- **Security:** Amazon S3 offers a variety of security features, making it a safe platform for storing and processing sensitive data.

* ## **Storage logging & Monitoring**<a id="storage-logging--monitoring"></a>

- Amazon S3 storage logging and monitoring provide visibility into the requests made to your Amazon S3 bucket. Amazon S3 storage logs give you information about when each request was made, the request path, the request method, the request headers, and the request-response headers. Amazon S3 access logs also give you the identity of the requester:

* With Amazon S3 storage logging and monitoring, you can track the data access patterns in your Amazon S3 bucket and use the information to troubleshoot issues, audit compliance, or analyze data usage trends.

* Amazon S3 storage logging and monitoring are disabled by default. To enable storage logging and tracking, you must create an Amazon S3 bucket and then allow logging on the bucket.

![](https://lh7-us.googleusercontent.com/aZBomhmjgCLsPW6svO89N_3Ctj9JeteakLlMkpmzZVVaZLeC9Bbg82O1_LBeF9NDJeWJbp4a8vGUvzT-wEPO-WRDOz9WWSZkyYcq8LpOTywpBSLqFukQcXWXq_K_oSmMUMmeHrrcdxMgniY0Wkc0_B8)

4. # How Amazon S3 Works <a id="how-amazon-s3-works"></a>

![](https://lh7-us.googleusercontent.com/thfaRJ1g0DP1eWm3eW8z3IhZZkdDAI5V9FnrtT4atc941XJ1MCnccLqAcyUGGlp-ucRlkhuapIJ5tjYDGT6vbfHbGiSdaT4-uK7FZCc-Fw2WAoc3NItimu1GkzhSAhRZ18GZSLMVPoUbEz6Ch3gyMRc)

1. Create a bucket with a unique name.

![](https://lh7-us.googleusercontent.com/voqD-_7ZKMO2BNUNNwYIarO86S7TKj1tzPc_gK-OvB8soSd_OcocoRJa7zidiOeaS7c36MKuyjiMFoOsfAdUalm27TutQBYy4HmVy1y0Zp15pSovpGx4dt6CxGXD0W4VuDBVk4nEDrxn4qYIfkunxZ0)


2. Block all public access.

![](https://lh7-us.googleusercontent.com/VSldrqKbycrG1kpdYYuW7mf2wF06ccm2wDgGSTSD9-mWPeRwYcbpmobqSjQ9jBPUxDMOsftkoH5sN4IOgXidc7YABwcaFPdbsU5b4-Bvld3Rhgg8kgmfQNVPaJc6JX_1uin7tYjltm9szYZt16g9Ufs)

3. Then click on “Create Bucket”.

![](https://lh7-us.googleusercontent.com/IX_u6djFZS_8En6WS_kaJCSQKa3zbdxGw4YNXOsw5vNdxuse-oq8cNC7K5Qh5olKPUwdQlTwUK0xCI-sq8iusnta0e08I0VRoboKKW8mPsCb4R53PfhQl1OLdksaGP_50p8StPbcDYi_WpbW5IM4pfc)

4. After that upload (object) file in the bucket.

![](https://lh7-us.googleusercontent.com/o7yRx-dmDNI_S850kaYAMFyryY0a-sAhDxVqBPGg2_lyRDpCNn3LMCIwKzdtqXt5qD62ZNGDMtmM4LS2rnGO5NJpIIW4wh_acqxjnFWK6je6TbXtHOKj9eO1DJIhnOKYi9k_dPPjk9_vNjBo_VbxsO4)

![](https://lh7-us.googleusercontent.com/ZO-tD4aL1dWHXTdmAetr1epISmqtnJWsmJtZ1iupPZzGY8jt5rgIfW4WYeoivfJUkQl8vy2C9_m2lIebaEyjpZe6zmnHcPdg8_TgwnP1_Lr2_GtEMYRqqdugbUDiQn7rfI_A6Ey_IUs8cXCpFWpNxOs)

Here FOSTERING.webp is the object that is stored in the bucket (alphabucket2342).

5. Then go to “Permissions” in the object.

![](https://lh7-us.googleusercontent.com/FcN87rxOaxIaQ9UEAgpGhVaIoWmZRhRNs_9DIagYKvUxtPsmz8w7oIiTy-3hTXzuvXcM6Oip-DHdkIdtMywnQho3dG2JEA_9T-bUJZc_PcUI3fFML0uYrAInLY7ghOj78DhjAFqc03JS5AGdquMAXNU)

6. To access that object we need to unblock the permission of public access. We can do this earlier as well while creating a bucket.

![](https://lh7-us.googleusercontent.com/vmR_-5ZVzc5QFfVZrXxw5fwE8gxcQeibevAdWelP28BWKgeZ1eKjyeyAE_dlpP4P16w9MPxVfP8E8SnLczY2omGKOCbjZI8fz3m2KLz1RlbCaMrAPpE5b5WUtNr5_qN-eB9KQtOXkP9X_iRyf51FQTY)

7. Then go to “Permission” and click on edit in Bucket Policy then click on edit then click on “Policy Generator”.

![](https://lh7-us.googleusercontent.com/P9GvWCJdRTO4H1qsOhB_fxPkkVLdJ6wKhOSCuAAsPowS2aHAXmJbI2Rz5tDqpZEzLMk2Dx7Dx9vRmu450oben-Xu_vK2_SWtqc84b4a-EiH86GTq6ILRRA414fRyJINxaJjs13yojyVSGQ2J73VOhns)

![](https://lh7-us.googleusercontent.com/5XcLFU2o-K0gS_TR1Yw2x3sp7ltBOF3LbljbdbdajoE6t70UBA4v2ZQXSD6aRePCBZXp9yUkV94O3rlHwUgAeVqJjZ1v4WgWEEjGvlc5yykKDmKVZ8hxsG3ASnUSpLTeM2S90tItArc8iNZuCxNx_tQ)

8. After this, complete the Step-1, Step-2 and Step-3.

![](https://lh7-us.googleusercontent.com/HDGDEPkSvY1LbJmQXJE9JCNFaZt-sUNnpAuBXieUIa1_NSzDtK2uMxLkbFPAlpdU5phzJYlaIRSZTX-YQoDZXPC66w0SswPUWmx5QFw9Cdd1iaSXW47ff7LJ4g4z3huhptjB3CCf3WO_7UXi-J_bE4c)

9. Then go back to “Bucket Policy” and paste that code.

![](https://lh7-us.googleusercontent.com/YPx63RYDcUGFvt3ydrDjEGKhCAmDsbn7qkSKVtZiNNUWmtLuBv8-qHunHK1jTorKLsxwYdMwOzBqppCG6xVC2ZtTLZ18AcHgDfxknA7WHz7pMV-O46dDLbEUgVadQvja_RyL62SD36Z1vSOYRM1G9wg)

10. **Remember one thing write “/\*” after the bucket name in the code. Then click on save change.**

![](https://lh7-us.googleusercontent.com/SgMcxshHu1K9YFN2R5XHAZVk9TdqfBUekUGqe0l9QlgvrhEwjLvcJyOfS-ymw9UjqUTo_hLFad8fgO6WzrZLxr2eHTl_ovdkZ8lo3TakbUOne9Y4RokNzpFAXHIDAnluiWnK6GLpCSf2mYyHkuD8sNU)

11. Then go to the bucket and click on the object and copy the URL of that object.

![](https://lh7-us.googleusercontent.com/5S5U1l5U6yh5PhG6A4eQC0RrEcLJrIR0d48Uo01NQ0YsuhRDlqHCL-QRFKZVIXKnD9KFSyxQhojm0OcN3gIboMGg56D7vFwebsQ9NZ8ygR-6Bj6MUQdNTU7B5NamOH61CyqUmdIyLZmWHat6XCcANQA)

12. Lastly, open a new tab and paste that URL, if that URL runs properly then our data is successfully stored on cloud.

![](https://lh7-us.googleusercontent.com/T9Zv13hy1lXQCKrGyy6UxIkhGuTERZElxI8z_f2aoUTUL8_ntL09Yhf45h4iKl0nFq5tDxVgHPwslE5z_Qp9igGKxzYEWPsWa3IozjDmsm5IoAO7E3rkgJZ7vbSYXaeiVZ1pCwnui2bDX5jnYOC7qXI)


## Key Points :-<a id="key-points--"></a>

1. ## Bucket <a id="bucket"></a>

- It is a container to store objects in Amazon S3.

- It also organize the Amazon S3 namespace at the highest level

        

      Buckets also:

- Organize the Amazon S3 namespace at the highest level.

* Identify the account responsible for storage and data transfer charges.

- Provide access control options, such as bucket policies, access control lists (ACLs), and S3 Access Points, that you can use to manage access to your Amazon S3 resources.

* Serve as the unit of aggregation for usage reporting.

2. ## Objects<a id="objects"></a>

- Fundamental entities stored in amazon s3.

- Objects consist of object data and metadata.

- Metadata :- It is a set of name - value pairs that describe the object.

- An object is uniquely identified within a bucket by a key (name) and a version ID.

3. ## Key<a id="key"></a>

- An object key is the unique identifier for an object within a bucket.

- Every object in a bucket has exactly one key.

4. ## S3 Versioning<a id="s3-versioning"></a>

- S3 versioning means to keep multiple variants of an object in the same bucket we use S3 versioning.

- We can preserve, retrieve and restore every version of every object stored in a bucket.

 

5. ## Version Id<a id="version-id"></a>

- When we enable S3 Versioning in the bucket, amazon s3 generates a unique version id for each object added to the bucket.

6. ## Bucket Policy<a id="bucket-policy"></a>

- It is a resource based AWS IAM (Identity & Access Management) policy that is used to grant access permission to the bucket and the object.

- Only bucket owners can associate a policy with a  bucket.

- Bucket policies are limited to 20 kb in size.

7. ## S3 Access Point<a id="s3-access-point"></a>

- These are named network end points with dedicated access policies that describe how data can be accessed using endpoints.

- It simplifies managing data access at scale for shared dataset in Amazon S3.

- Each access point has its own access point policy.

8. ## Access Control Lists (ACL)<a id="access-control-lists-acl"></a>

- We use ACL to grant read and write permissions to authorized users for individual buckets/objects.

- In modern use cases in Amazon S3 no longer require the use of ACLs.

9. ## Region<a id="region"></a>

- Choose a geographical AWS region for storing.

- We might choose a region to optimize latency, minimize cost.

- Objects stored in an AWS region never leave the region unless you transfer or replicate.


# # Reference Links <a id="-reference-links"></a>

- <https://docs.aws.amazon.com/s3/?nc2=h_ql_doc_s3>

* <https://youtu.be/sWOkwp4Kd_I?si=RTez-oGOIjFGGcVu>

- <https://youtu.be/k1RI5locZE4?si=E6F_VZJkZUBrO8fO>

* <https://youtu.be/HTb_VYOE4WM?si=NU6JOY8F13G1wzzb>

- <https://youtu.be/_I14_sXHO8U>

 
