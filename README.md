## IAMGroupProject
AWS Identiy and Access management(IAM) is an AWS Service securely control access to your AWS resources in your organization. It ensures the right people in an organization can only access the service that they need to perform their tasks. It enhances security of your resource in the cloud, and it is part of the best security Practice.

## Project Overview
In this project, I am going to create IAM groups with  specific access policies aligned with each group's functions.There would be three groups: Admin, Developer and Tester. Each group has three or more users. There would be one user like DevaOps exists in two groups based on his function. 
### AdminGroup: John, Mahamat, and Sara
### DeveloperGroup: Ahmed, Christopher, Mary and Antony(DevOps).
### TesterGroup: Alber, Hamzam Patel and Antony(DevOps).

# Project Achitecture

![image](https://github.com/user-attachments/assets/d608a96c-344f-400d-a557-0150d0fa6dd2)
## Step by step implimentation of the project
Login in your AWS account and seach for IAM
![image](https://github.com/user-attachments/assets/48a02a04-4586-46fb-a823-48bade311ab9)
After opening the IAM dashboard, click on user groups on left side.

![image](https://github.com/user-attachments/assets/7191d6ae-6666-45a9-ab11-9f21d3fa0ec6)
Click on create group button on the top right corner.
![image](https://github.com/user-attachments/assets/55977926-8b3b-4378-9111-7473af811bbd)
Name the group as Admin and the user Mahamat is already created and I added him in the group Admin. Don't worry if you don't have users, you can add them later.
Check and attach the policy name AdminstratorAccess to the group which can give a complete access to AWS resource in my account.
![image](https://github.com/user-attachments/assets/d85ba5f3-651a-4f0c-a244-d51ad2a5f930)

