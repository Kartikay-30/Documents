
**Amazon Simple Storage Service (S3)**![](https://lh7-us.googleusercontent.com/UA0ooxTO4n9Mc15rjYW3VqV1U7SDLwS21-CUheZzq7lfMg2nOXOD8Jt1Dfe8Mn_XDDUuodPHNXolJCt6DJLXyXMtD_p_-Y-a8PtbXsQaHeCy58pelam28_v_UpznSUtzWtPXVCzjnEvP9nlFdWc_cIU)![](https://lh7-us.googleusercontent.com/HLLNPR4m3n2yUYENZo8-4A_bx9gNUStrS0F9RIXQsvrnVTeO4MmTESINgjBeCg0ESD78ieCKCL0I70TavGZRKEnVPatca0ncG3hSeku6XqixmwSLrHPIi24GAZAgR4JIpsmfnO6g0UAjtwfRYwmrpSI)******By:- Kartikay****December Intern** 

Table of Content:-

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

![](https://lh7-us.googleusercontent.com/O-Wnr3vmt6xRxCTwZVWKltUy-rjdelLPX8XSxXi_1lUgMTihFJzbS5AMmhfarlRyakm5jqE2bt_HDkV2V59wfRw7BDxLKnIijU4KtCi7VtNQ4HVf60gOhmIZcWliWWB8TKSeu9fYpJ4azSQ89hOuuN8)


## Benefits of AWS:-<a id="benefits-of-aws-"></a>

- Flexibility

- Cost Effective

- Scalability

- Security

- User-friendly

- Data Encryption

2. #  What is Amazon S3 ?<a id="what-is-amazon-s3-"></a>

- Amazon S3 is an object storage service that offers industry-leading scalability, data availability, security, and performance.

- Store and protect any amount of data for a range of use cases, such as data lakes, websites, cloud-native applications, backups, archive, machine learning, and analytics.

![](https://lh7-us.googleusercontent.com/LMqcph9uJRja6PeZ7iFDh5RNGWbuQnV5l5mJMWQUNelAduMjShDLEHr2O7xw5m3OF3jkxWep0g_0e_aR8Rlt4hvjJxk1C3U0z2qJoUqYiJWoZEIJevUl5Gj0TAB1Yd7jQNYqGd7GpAONDdK9FU_S5cU)

- Amazon S3 is designed for **99.999999999% (11-9's)** of durability, and stores data for millions of customers all around the world.

3. #  Features of Amazon S3:-<a id="features-of-amazon-s3-"></a>

- ## **Storage Classes**<a id="storage-classes"></a>

Amazon S3 storage classes are designed to give customers flexibility when storing their data on AWS. Four storage classes are available: 

- **Standard:** the default storage class and is suitable for most workloads.

- **Standard – Infrequent Access (Standard – IA):** designed for data accessed less frequently but still needs to be quickly accessible.

- **Reduced Redundancy Storage (RRS):** designed for data that can be safely stored with lower levels of redundancy.

- **Glacier:** designed for infrequently accessed data and can be stored for long periods at a lower cost.

* ## **Storage Management**<a id="storage-management"></a>

Amazon S3 storage management lets you control how your data is stored and organized within your Amazon S3 buckets. With storage management, you can specify how Amazon S3 keeps your information, whether held in a standard storage or infrequent access (IA) storage class and stored in a bucket versioning-enabled or versioning-disabled bucket. You can also specify whether Amazon S3 encrypts your data at rest and whether your data is automatically compressed.

- ## **Access Management & Security**<a id="access-management--security"></a>

Amazon S3’s access management features allow you to control who has access to your data securely. You can manage access to your data using access control lists (ACLs) or Amazon S3 bucket policies. ACLs allow you to grant granular permissions to individual users or groups.

- ## **Data processing**<a id="data-processing"></a>

Data processing refers to taking data and manipulating it to extract valuable information. This can be done through various methods.

Amazon S3 offers a variety of features that make it an ideal platform for data processing, including:

- **Scalability:** Amazon S3 can scale to accommodate any amount of data, making it ideal for big data processing.

- **Flexibility:** Amazon S3 supports various data formats, making it easy to process data from multiple sources.

- **Durability:** Amazon S3 is designed to be highly durable, meaning that data is unlikely to be lost even if there are hardware failures.

- **Security:** Amazon S3 offers a variety of security features, making it a safe platform for storing and processing sensitive data.

* ## **Storage logging & Monitoring**<a id="storage-logging--monitoring"></a>

Amazon S3 storage logging and monitoring provide visibility into the requests made to your Amazon S3 bucket. Amazon S3 storage logs give you information about when each request was made, the request path, the request method, the request headers, and the request-response headers. Amazon S3 access logs also give you the identity of the requester:

- With Amazon S3 storage logging and monitoring, you can track the data access patterns in your Amazon S3 bucket and use the information to troubleshoot issues, audit compliance, or analyze data usage trends.

- Amazon S3 storage logging and monitoring are disabled by default. To enable storage logging and tracking, you must create an Amazon S3 bucket and then allow logging on the bucket.

![](https://lh7-us.googleusercontent.com/IgD4Rnewyljy0YX-4lrpCBZiaqgQB2EdosfKtDkX6kUIb4M7BVQyChw38F8jbl2nkEI90dPhKG34FoZBpOJeV6su_VGttJfvpjt-vYlR2C-ZE9CtBMiEXrYOgqLk-y1IFeC-GvHm9hCeNojtq1p6L_U)

4. # How Amazon S3 Works <a id="how-amazon-s3-works"></a>

![](https://lh7-us.googleusercontent.com/dj0b-L521LB91YAv7M7DsO-VdzbvYG-uu4xFFRn9xH8dQEpRRx2nOssUtsO1wl6yf3XFkjXFGYek6CzS7MX7vlc_Kka1TSbSqnk4NeW6BPufakpY2eSVIbO5-p3BA_y2KJaD9Xw56_BejWuzxsz0OtA)

1. Create a bucket with a unique name.

![](https://lh7-us.googleusercontent.com/IwbuRfe754M6MZi6YIvNDhYP4854-wnXUiUPorlK0bgCRxKosaCZ7BfDQI_JgPHyv4RL5IHMVBh3D-R1q6y51p5tl_zW7Rh4w-n3okWiYYg16FW7IwHj62Pse7hByXp_4o8xbds6L_FXcS6sks_i4Ng)

2. Block all public access.

![](https://lh7-us.googleusercontent.com/qTDeEU6epwKanwIP1ykLWsgyE1OC98vZKmnY47tvrYieIvvZZWbPDO6owchLHfUhanGX3QpsqRwallsBuLviUP8rc9cwUq9NlUD2oSj0hJUIlUIX0F-aN4ue1CqwwUVNrFVJfiPNmJmLfv3iO9ti3xI)

3. Then click on “Create Bucket”.

![](https://lh7-us.googleusercontent.com/EosfjKPXLqaVjM7WuPfLgg_-hqb3I0EAg9MpPdBcY3O8AjyQp0PsRPLZF2K1mj-1CH7Px42Zs2qOvX-EQl8Q9cHBPtSBTmuNNNbZFbDXgloX0mSlOJbQIBk7Vit350ffRjh7A04OQsSc1Qs_OXeWY5o)

4. After that upload (object) file in the bucket.

![](https://lh7-us.googleusercontent.com/LyojPf_5aufAWrUBtqcsKQhtAbYKIyicp_LWNyr8N9O9-hK7L6FR6O_QK6UCIE8alZV-xhD70gx640MaLBSvYNBYIRu97S85kdNAYYu-99GTyiCpQEYIFLH9JCnhOWXCL2YtcK6f2WPniUqkNPbTWCA)

![](https://lh7-us.googleusercontent.com/w5EPgYPBdjYGla_MDDXkd3ZaTmcO73SgBfMxtgAfqgSg8uiOviJklxDeb4MUEKO1LfInsEg7Pjsnhy0MO0IeFLY9PNI7c8PR6-N_PHeHR2DrT__Bp0fW2-SLyfZ1jH8IDF52F6z6LbrUyxOdn-HnYIU)

Here FOSTERING.webp is the object that is stored in the bucket (alphabucket2342).

5. Then go to “Permissions” in the object.

![](https://lh7-us.googleusercontent.com/kSA8oZCp9DE5qXtoyf1tf2m_8vh39mVwycvaFR4mxkR8Wh9rZubtJ5Ou8264DD9gFfkHohBWZwakPBh3UfNXtZJIksNduDn8DwwHsvpm0Yzn5mn46w_sCLou76uXGRoaNSrj30FF1Fmvho_NIRWISKk)

6. To access that object we need to unblock the permission of public access. We can do this earlier as well while creating a bucket.

![](https://lh7-us.googleusercontent.com/V7gJAtpvauQumqAUR9QJqpFqiH3gQzLtURGgm08yUgIa1eaoRxSAG1IrJZcrqH94oKBqEyG5ex4IT9A0FsQtFfUl11in6y3LMEki7h-cUTjnWNG2hJed5a2Z9cjc3VXiMbU_UJOBOiJofxwEp3xkku4)

7. Then go to “Permission” and click on edit in Bucket Policy then click on edit then click on “Policy Generator”.

![](https://lh7-us.googleusercontent.com/T7HjEkXEepoULZIAO5UnIYf76S3xlfo6hmIsAvh_GxZt1KS-7EQ9nMUc1NS728fA_pyEEwarLcc6RIBXtHDhAvggDLjVtU3REDAAhRcLYaUlgOMhJq0wB5VJbIqEpHwVTqHZyq7olQDBeqMdwz-C5G0)

![](https://lh7-us.googleusercontent.com/N_tQutEeaXlursbiIC4Wowaa62MFo_Kb7nheWSocZrhWsxIMuyYliaEykhlArsreiaN2HyRTJzkMDQLIZSHVrKGop0T1pEB1JWj69EQfyNMBSPicZRXJL6Ua8Fu85ZMfHkWKUr_Je3ZsbejlEYvphbY)

8. After this, complete the Step-1, Step-2 and Step-3.

![](https://lh7-us.googleusercontent.com/81CJOf-ye9afgmeHTLAkG_AKjuDhLCyjGHAK1HuwVLPJ19Szwm3UxgSV0JIAFwXRbbQFYL-M069zA1WofrHTBeqb1AEbPwYjSLeLzBxMvoVR12WSoyjPMje3B57Fivjy6Au5FTjMIzHDdehuNBl4Dtg)

9. Then go back to “Bucket Policy” and paste that code.

![](https://lh7-us.googleusercontent.com/HJhSO0Rv1RMqxmEqV3gWnRPQ-zeDxk12pdkSeYlSsmO8nO-h1s7MVVY2EWlENGKeSXm5fAax_5oPvHGuUgXXQ6MNjJOQ6OiEYI8_tXoxzu0ftOJzQd91hD68fGm98YssU1A8q9odEAjfIyJe-TMwZkI)

10. **Remember one thing write “/\*” after the bucket name in the code. Then click on save change.**

![](https://lh7-us.googleusercontent.com/LqB0cbUhOvn7fbkU3_hg5JcvTwZ9A8eBq8t6ib7i2W6jChdQmc0r0likfxn7ilJ3Rj7tUnshTdfcNyFuw3AlBs_DKWselDTBg4Y94Tvse-_AjIGBH0hwanGFf1cZjodxLEZBeWkPRiqqBmSev8qp9dY)

11. Then go to the bucket and click on the object and copy the URL of that object.

![](https://lh7-us.googleusercontent.com/sawok7HWdySEnRhmEHsbCeZTGhAmJlFTSgxn3dPfnfRLNKdQRlmrR7q141yaJJF9yL9oBODyrod7J1cfJPGehqb1rGRD2NPAiEa_jyJKgxMt2C5LP_EpZjCAieYcm5obpMvyrJWUKonV6p8_5twfAFI)

12. Lastly, open a new tab and paste that URL, if that URL runs properly then our data is successfully stored on cloud.

![](https://lh7-us.googleusercontent.com/VsljAygxUVprpwNM5nWMBPhnO7p5tLrvq8Fj6EWahHKUNZZhnRE47ou3Ev-J3LoQ_ru63U76RdjTY2sGq21Hl2K_bQOdRxffVxTGTwLs4pEAbFcgkW72E75kgO6EIRiUIntPHppuNibKOXeaGxCIqKY)


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

 
