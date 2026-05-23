# Project Overview

As a security professional at a large organization. I am mainly working with their research team. Part of my job is to ensure users on this team are authorized with the appropriate permissions. This helps keep the system secure. 
my task is to examine existing permissions on the file system. I need to determine if the permissions match the authorization that should be given. If they do not match, I will modify the permissions to authorize the appropriate users and remove any unauthorized access.

### Procedures followed
In this project, I used the Linux command prompt to ensure users on the team are authorized with the appropriate permissions. **using the following steps:**

**1. Check file and directory details**

Using the linux command prompt, I checked the permissions set for files and subdirectories in the project's directory. Including hidden files.Then, I use the output of this command in the lab as a screenshot added to the Project file

```
pwd
cd /home/research2/projects
ls -la
````

**2. Describe the permissions string**

In this step i choose one example from the output in the previous step, then I write a short description that explains the 10-character string in the example describing what the 10-character string is for and what each character represents.A 10 character permission string tells you what type of file it is and who can do what with it.

**3. Change file permissions**

The organization provides a set of rules related to users' permissions; it does not allow others to have write access to any files. In this step I checked which file needs to have its permissions modified. Using a Linux command, I modify these permissions.

```
chmod o-w project_k.txt file
```
**4. Change file permissions on a hidden file**
 
In this step I modified permissions for a hidden file, the research team has archived the file, this file should not have write permissions for anyone, but the user and group should be able to read the file.I use a Linux command to assign the appropriate authorization.

```
chmod u-w,g-w,g+r .project_x.txt
```

**5. Change directory permissions**

This step requires modification of a directory permissions. The files and directories in the project's directory belong to the researcher2 user. Only researcher2 should be allowed to access the drafts directory and its contents. I used a Linux command to modify the permissions accordingly.

```
chmod g-x drafts
```

### Project Impact

The Project makes the organization safer and more organized. By checking who has access to files and fixing any incorrect permissions, you help:

- **Protect sensitive research data** from people who shouldn’t see it.
- **Make sure only the right users have the right access** so the system stays secure.
- **Prevent mistakes or misuse**, which reduces the chance of security problems.
- **Support the research team**, because they get the access they need without delays.
- **Keep the system clean and easy to manage** in the future.

