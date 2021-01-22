# Initial Installation

If you have completed the Moodle deployment on Cloud Platform, the following steps is for you to start use it quikly

## Preparation

1. Get the **Internet IP** on your Cloud Platform
2. Check you **[Inbound of Security Group Rule](https://support.websoft9.com/docs/faq/tech-instance.html)** of Cloud Console to ensure the TCP:80 is allowed
3. Make a domain resolution on your DNS Console if you want to use domain for Moodle

## Moodle Installation Wizard

1. Using local Chrome or Firefox to visit the URL *https://domain name* or *https://Internet IP*, enter to Moodle installation page

2. Choose a language, then go to next step
   ![Moodle-install-language](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/md01.png)

3. Set the Moodle source code and data directory
   ![Moodle set directory](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/md02.png)

4. Choose the database type
   ![Moodle Choose database](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/md03.png)

5. Fill in your database connection information ([Don't know password?](/stack-accounts.html#mysql))
   ![Moodle set database connection](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/md04.png)

6. Confirm the Copyright
   ![Moodle Confirm the Copyright](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/md05.png)

7. Installing
   ![Moodle start install](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/md06.png)
   ![Moodle start install](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/md07.png)

8. Set administrator account
   ![Moodle set administrator account](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/md08.png)

   > Email is your system ID, not collected by anyone because it stored in your Cloud Server

9. Set site name, short name, front page summary...
   ![Moodle set site information](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/md09.png)

10. Installed successfully.
   ![Moodle installation successfully](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/md10.png)

11. [Register a Moodle account](/solution-more.html#moodle-register) to connect Moodle official website for more extension

> More useful Moodle guide, please refer to [Moodle Documentation](https://docs.moodle.org)

## Moodle Setup Wizard

## Q&A

#### I can't visit the start page of Moodle?

Your TCP:80 of Security Group Rules is not allowed so there no response from Chrome or Firefox

#### Which database does this Moodle package use?

MySQL

#### Can I use Cloud database for Moodle?

Yes
