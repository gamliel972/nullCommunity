# Setup VyAPI - A Modern (as per 2019) Cloud Based Vulnerable Android App

## Software Prerequisites 

Follow the `Prerequisites` section of [VyAPI GitHub repository](https://github.com/appsecco/VyAPI) to ensure all required softwares are installed in your laptop. You should be ready to use the following 

1. Amplify CLI
2. AWS CLI
3. Android Studio

## Configure the Amplify CLI

1. Run following command in a terminal window

        amplify configure

    ![amplify configure](image/1-amplify-configure.png)

2. Enter *AWS admin credentials* when prompted

    ![AWS admin login](image/1b-aws-admin-account-sign-in.png)

3. Ensure successful login into the `AWS Management Console`

    ![AWS Management Console](image/1c-aws-management-console.png)

4. Press `Enter` in your terminal window

    ![Press Enter](image/1d-press-enter.png)

5. Follow on-screen instructions
   1. Select a `region`
   2. Provide a `username` for the new IAM user

        ![Enter username](image/2-enter-username.png)

   3. Complete the user creation using the AWS console

        ![User creation using AWS console](image/2b-add-user-using-aws-console.png)

        ![Set permissions](image/2c-set-permissions.png)

        ![User Security Credentials](image/2d-user-security-credentials.png)

6. Press `Enter` in your terminal window

    ![Press Enter](image/2e-press-enter.png)

7. Enter the user security credentials as obtained in step #7.3 (see above)
8.  Enter a name for your new AWS Profile

    ![AWS Profile Name](image/2f-aws-profile-name.png)

9.  You should see your new IAM user in the AWS console (`Identity and Access Management (IAM)` > `Users`)

    ![](image/2g-check-user-in-iam-home.png)


## Build VyAPI using Amplify Framework

1. Clone the VyAPI GitHub repository

        git clone git@github.com:appsecco/VyAPI.git

2. Enter `VyAPI` folder

        cd VyAPI/

3. 