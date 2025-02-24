## IAMGroupProject
AWS Identity and Access Management (IAM) is an AWS Service that securely controls access to your organization's AWS resources. It ensures the right people in an organization can only access the service needed to perform their tasks. It enhances the security of your resources in the cloud, and it is part of the best security Practice.

## Project Overview
In this project, I am going to create IAM groups with specific access policies aligned with each group's functions. There would be three groups: Admin, Developer, and Tester. Each group has three or more users. Also, there would be one user like DevaOps who exists in two groups based on his function. 
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
And click a User group
![image](https://github.com/user-attachments/assets/a0f14159-5092-4201-a0fe-b41a6854c415)
The developer group is successfully created.
![image](https://github.com/user-attachments/assets/6e58e529-55e0-4885-9c19-9e42170e2e3c)
Let's add user to Developer
![image](https://github.com/user-attachments/assets/0f8fa78f-64a0-4256-9afc-245bd58d90d6)


