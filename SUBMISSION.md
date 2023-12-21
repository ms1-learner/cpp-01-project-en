# MS1 Project Guide
A project is a crucial part of the MS1 learning experience that allows you to strengthen your understanding of the content covered in a module by giving you the chance to apply what you've learned to a problem that closely simulates a real-world situation. Some projects are completed individually, giving you a chance to create a complex program start to finish on your own. Other projects are completed as a group, providing you with a collaborative experience that is similar to working in a real development team.

## Accessing Projects
At the end of each module, you’ll find an instructions page for that module's project. The instructions page will contain a link to the project repository on GitHub. The repository may be a blank placeholder, or it may contain some resources you will need to complete the project.

The general link structure will be something like the following:

`https://github.com/ms1-learner/[learning path]-[module number]-project-[locale version]`

For instance:

`https://github.com/ms1-learner/cpp-01-project-en`

## Setting Up the Project Repository
First clone the project repository, and navigate into it:

```bash
cd cpp-01-project-en
```

Then run the following git command:

```bash
git remote rename origin ms1
```

We will come back to this repository, so don't close the terminal just yet.

Next we need to make a new, empty repository on your enterprise GitHub account.

Navigate to your **repositories** page from your profile icon on the top right:

<img width="1840" alt="Screenshot 2023-12-21 at 12 55 54" src="https://github.com/ms1-learner/cpp-01-en/assets/5623716/15a2fc85-ac92-41a6-9179-cbc9c55818b4">

Select the green button labeled `New`.

On the "Create a new repository" page, select yourself as the owner, and give the repository the same name as the repository you cloned earlier. In this case, `cpp-01-project-en`. Leave all the other settings in their default state.

<img width="1840" alt="Screenshot 2023-12-21 at 15 21 10" src="https://github.com/ms1-learner/cpp-01-project-en/assets/5623716/df9e1cc7-9d32-4206-b5be-c980314b9ae7">

On the next screen, select HTTPS, then copy the git commands from the bottom box.

<img width="1840" alt="Screenshot 2023-12-21 at 15 22 11" src="https://github.com/ms1-learner/cpp-01-project-en/assets/5623716/c3bdf720-901d-40a1-975c-9a3bf2d57881">

Paste these commands in the same terminal from before, from inside the previously cloned repository.

```bash
git remote add origin https://github.tmc-stargate.com/alexander-bolinsky/cpp-01-project-en.git
git branch -M main
git push -u origin main
```

Once these commands finish running, if you return to your newly created repository on GitHub, it should now be populated with the content from the original cloned repository.

## Working on the Project
Proceed to work on the project locally in the same way you work on challenges.

### Pulling Changes
If some content was changed on the original repository and an instructor informs you to "pull" the latest changes, you can do so by running the following git command from inside your repository:

```bash
git pull ms1 main
```

## Submitting your Project
If you are working in a group, everyone needs to submit the same URL of the project repository. Make sure each group member is added as a collaborator to this repository. Coordinate with your group to decide whose GitHub account will host the project and who will submit the project on your group's behalf.

When you are done with your project, make sure the `main` branch is updated with the latest version of your project.

Copy the URL from your pull request in GitHub, navigate to the project page on MS1, paste the link, and click `Submit`.

<img width="841" alt="Screenshot 2023-12-21 at 15 56 27" src="https://github.com/ms1-learner/cpp-01-project-en/assets/5623716/51f5729a-e4cc-4911-9f89-07d15966f244">

That's it, all finished! You will be notified on MS1 when your project has been graded. If you do not pass the project, you will receive comments from your instructor detailing what you need to change in order to pass.
