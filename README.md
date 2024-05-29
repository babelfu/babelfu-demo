# Demo repository for Babelfu

I am writing an introduction for Babelfu to clarify and guide its users. Although Babelfu is still a work in progress, its interface may seem obvious to me; it might not be as intuitive for the user. This introduction aims to bridge that gap and ensure a smoother user experience.

Users may encounter corner cases that I have not considered or deliberately avoided to expedite the development of a proof of concept. 
I hope to help users navigate Babelfu more effectively by outlining the key functionalities and potential limitations.

## Getting started

Before starting, I recommend forking this repository. It will increase its popularity 📈 and allow you to use it inside Babelfu.

Visit [babelfu.com](https://babelfu.com) and create an account. To keep it simple, I only ask for an email and a password. I will not even send you a confirmation email.

![image](screenshots/signup.png)

Once you are logged in, you can create a new "Project." This will redirect you to the "Connections" page, where you can connect your GitHub account.

![image](screenshots/connections.png)

On Github, authorize Babelfu to access some of your repositories. At least select the forked repository to continue with the guide.

![image](screenshots/authorize.png)
![image](screenshots/install.png)

Now you can create a new Project for real. You can leave the "name" empty, select the repository, leave the default locale and translations path with the default values, and click "Create Project".

![image](screenshots/new-project.ong)


You will be redirected to the "Project" page. The project will start syncing immediately, fetching the branches and opening pull requests.

Babelfu allows the exploration and modification of the translations by branch or pull request. While you can modify the translations for a branch directly, I recommend modifying the translations in an existing pull request as you would in a normal code change. In the future, I would like to:
    - Create a pull request from the UI.
    - Configure if we allow the modification of the translations directly in the branch.
    
Go to your repository and create a new pull request to add, modify, or remove translations in some languages.
Return to Babelfu and click "Sync translations" to fetch the changes. In the future it would listen to the GitHub events to sync automatically.

Check the "Locales" dropdown to select the languages you want to see.
You can filter the translations by using the "With proposals" and "With changes" toggles. I have to rethink the behaviour in conjunction with the "Locales" dropdown. Of course you can search the translations by key.
- You will see the changes on the "Translations" page. Now, you can modify the same translations or others. Once you are happy with the changes, click "Commit changes" to commit the changes to the pull request.
On the "Commits view," you will see a preview of the changes. If you are sure, you can click "Commit changes" to commit the changes to the pull request. Under the hood, it will sync the head and base branches.
