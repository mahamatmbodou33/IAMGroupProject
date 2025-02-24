## IAMGroupProject
AWS Identity and Access Management (IAM) is an AWS Service that securely controls access to your organization's AWS resources. It ensures the right people in an organization can only access the service needed to perform their tasks. It enhances the security of your resources in the cloud, and it is part of the best security Practice.

## Project Overview
In this project, I am going to create IAM groups with specific access policies aligned with each group's functions. There would be three groups: Admin, Developer, and Tester. Each group has three or more users. Also, there would be one user like DevaOps who exists in two groups based on his function. Implementing and managing individual security credentials to enhance security best practices.
### AdminGroup: John, Mahamat, and Sara
### DeveloperGroup: Ahmed, Christopher, Mary, and Antony(DevOps).
### TesterGroup: Alber, Hamzam Patel and Antony(DevOps).

# Project Architecture

![image](https://github.com/user-attachments/assets/d608a96c-344f-400d-a557-0150d0fa6dd2)
## Step-by-step implementation of the project
Login to your AWS account and search for IAM
![image](https://github.com/user-attachments/assets/48a02a04-4586-46fb-a823-48bade311ab9)
After opening the IAM dashboard, click on user groups on the left side.

![image](https://github.com/user-attachments/assets/7191d6ae-6666-45a9-ab11-9f21d3fa0ec6)
Click on the Create Group button in the top right corner.
![image](https://github.com/user-attachments/assets/55977926-8b3b-4378-9111-7473af811bbd)
Name the group as Admin and the user Mahamat is already created and I added him in the group Admin. Don't worry if you don't have users, you can add them later.
Check and attach the policy name AdminstratorAccess to the group which can give complete access to AWS resources in my account.
![image](https://github.com/user-attachments/assets/d85ba5f3-651a-4f0c-a244-d51ad2a5f930)

Scroll down and click Create Group

![image](https://github.com/user-attachments/assets/f2911079-fce8-4c2d-a9d5-bb4ab0349338)
Admin group successfully created, click view group to view group details.
![image](https://github.com/user-attachments/assets/f6a2ecee-5eb3-4570-a569-0ea6b3196341)
Now it's time to create a user. Click on the user and then create a user
![image](https://github.com/user-attachments/assets/7e351e68-0448-4f30-9503-feac18445aee)
Choose a user name and click next.
![image](https://github.com/user-attachments/assets/e5223289-11af-49b4-80ea-5d5e9f0abb6e)

Choose the first option and don't forget to select Admin.
![image](https://github.com/user-attachments/assets/76b024bd-8d8a-4cf5-a72b-fe315e959c1a)
Click next
![image](https://github.com/user-attachments/assets/edbfd36f-c038-41c0-b042-32120ef9da0e)

Click on Create user
![image](https://github.com/user-attachments/assets/6d59d022-24be-4ef3-ad7f-101ec36ea7c6)
Successfully created user Sara. Repeat the same process to create the remaining.
![image](https://github.com/user-attachments/assets/02b2af41-9d5a-48ac-aaad-97d87de704e1)
Now, it's time to create the Developer group. Navigate to the user group and click on Create group
![image](https://github.com/user-attachments/assets/1db84c02-3004-4213-9bb2-606aa2246a06)
Name the group as Developer
![image](https://github.com/user-attachments/assets/abc6aca9-48c6-4c17-9bae-ce4ca9b5da11)
Attach the following policies to the group Developer:
#### AmazonEC2FullAccess, AmazonS3FullAccess and AmazonRDSFullAccess
Click a User group. 
![image](https://github.com/user-attachments/assets/a0f14159-5092-4201-a0fe-b41a6854c415)
The developer group is successfully created.
![image](https://github.com/user-attachments/assets/6e58e529-55e0-4885-9c19-9e42170e2e3c)
Let's add a user to Developer. Click on the Create user button.
![image](https://github.com/user-attachments/assets/0f8fa78f-64a0-4256-9afc-245bd58d90d6)

Name the user as Mary and click Next.
![Screenshot 2025-02-20 221458](https://github.com/user-attachments/assets/836d84f3-0019-4109-a61c-7adc6d346523)
![Screenshot 2025-02-20 221458](https://github.com/user-attachments/assets/ebb0155e-8c12-4a5f-bc55-9edf39c46918)

![Screenshot 2025-02-20 230329](https://github.com/user-attachments/assets/f193e273-38f7-46e7-9ea4-4ac1e2e059d4)
Now, Let's create the last UserGroup which is Tester. Click on Create Group.
![Screenshot 2025-02-20 231148](https://github.com/user-attachments/assets/5be3d8d8-1b15-4dba-904d-721b36a78b66)
Name the group as Tester.

![Screenshot 2025-02-20 231854](https://github.com/user-attachments/assets/bbe8c259-3b0f-48df-992e-edcfb0ae1312)
Attach the AmazonS3ReadOnly policy to the group and click on Create Group.
![Screenshot 2025-02-20 231940](https://github.com/user-attachments/assets/c3215ab8-0ca4-4c7c-8019-fb14f025692c)

![Screenshot 2025-02-20 232111](https://github.com/user-attachments/assets/7268c716-7bf5-4038-b698-32b94545d6d1)
Tester Group was successfully created. Now, let's add a user to the group. 

![Screenshot 2025-02-20 233923](https://github.com/user-attachments/assets/18a7efed-b683-4450-a1fe-901ae3b3135e)
Name the user as Alber and click Next.

![Screenshot 2025-02-20 234132](https://github.com/user-attachments/assets/bc87507a-271c-4832-b319-fcb85984d955)
Select the first option and check the Tester group to add the user to the group.
![Screenshot 2025-02-20 234220](https://github.com/user-attachments/assets/99648e16-63d7-4c5c-93ec-a4a4127dcd9c)
Click Next and create a user.
![Screenshot 2025-02-20 234302](https://github.com/user-attachments/assets/ea265797-6124-4ba0-bd80-bab231592160)
![Screenshot 2025-02-20 234333](https://github.com/user-attachments/assets/5ab73914-2846-4918-9d46-423f808fbda3)
Repeat the same process to add the remaining users to the group.
![Screenshot 2025-02-20 234705](https://github.com/user-attachments/assets/9d2be483-c54d-4153-aa3c-ca23ab3f2345)
the last user Antony_DevOps exits in both groups Developer and Tester. Let's add him to the groups. Click Create user.
![Screenshot 2025-02-20 235532](https://github.com/user-attachments/assets/5272100e-bffd-41ef-906e-305874dc6e1c)
Name the user as Antony_DevOps and click next.

![Screenshot 2025-02-20 235658](https://github.com/user-attachments/assets/bcd43579-1065-4bfe-be93-c2e1cee62d08)
Select Add User to the group and check to select both groups Developer and Tester.
![Screenshot 2025-02-20 235823](https://github.com/user-attachments/assets/be569d33-8bdf-4a17-b302-f380ab5176c4)
Click Next.
![Screenshot 2025-02-20 235859](https://github.com/user-attachments/assets/79df9c00-28c4-43d5-9501-3c1da6730f55)
Review the details and click Create user
![Screenshot 2025-02-21 000048](https://github.com/user-attachments/assets/eb4c8d4e-3d4b-466a-88f4-088d4e81e7ef)
Successfully added Antony_DevOps to both groups.
![Screenshot 2025-02-21 000237](https://github.com/user-attachments/assets/1111cb6d-4d47-46c3-8b10-9b9248fcf82d)
Now, we finished the first part of the project. Let's begin with the last part, which is about implementing and managing which user's security credentials. Security is very crucial in the cloud, it is best practice to assign security credentials and Multifactor authentication (MFA) to verify and authenticate the identity of every user that is accessing your resources in your AWS account. So with further due, let's assign credentials to the user. click on the user Sara.
![Screenshot 2025-02-21 082316](https://github.com/user-attachments/assets/3137395d-41ce-4557-ae93-b2a4323683ce)
Click on security credentials and Enable console access
![Screenshot 2025-02-21 082432](https://github.com/user-attachments/assets/0551978e-3929-4462-b1b4-6ebc584d6f0d)
You have to create a password. If you choose an Autogenerated password, AWS will generate the password for you. The second option is a custom password where you can create your own password. So it's up to you the choose, I'll go with the custom password.
![Screenshot 2025-02-21 082531](https://github.com/user-attachments/assets/2d947c71-c3eb-44d3-adc4-9e99d416531c)
Click on Download .csv file and close the window.
![Screenshot 2025-02-21 082603](https://github.com/user-attachments/assets/b7007ae8-a785-416a-96c4-9a6ceeda88c4)
Repeat the same process to create credentials for the remaining users.


