# Project Overview

I am a security professional working at a health care company. As part of my job, I am required to regularly update a file that identifies the employees who can access restricted content. The contents of the file are based on who is working with personal patient records. Employees are restricted access based on their IP address. There is an allow list for IP addresses permitted to sign into the restricted subnetwork. There's also a remove list that identifies which employees I must remove from this allow list. My task is to create an algorithm that uses Python code to check whether the allow list contains any IP addresses identified on the remove list. If so, I should remove those IP addresses from the file containing the allow list.

#### Project Scop
The project's primary objectives were as follows:

**1.Open the file that contains the allow list**
For the first part of the algorithm, I opened the "allow_list.txt" file. First, I assigned this file name as a string to the import_file variable
```
# Assign `import_file` to the name of the file 
import_file = "allow_list.txt"
```
Then, I used a with statement to open the file:
```
# Build `with` statement to read in the initial contents of the file

with open(import_file, "r") as file:
```
**2.Read the file contents**

In order to read the file contents, I used the .read() method to convert it into the string.
```
with open(import_file, "r") as file:
  # Use `.read()` to read the imported file and store it in a variable named `ip_addresses`
  ip_addresses = file.read()
```
**3.Convert the string into a list**

In order to remove individual IP addresses from the allow list, I needed it to be in list format. Therefore, I next used the .split() method to convert the ip_addresses string into a list:
```
# Use `.split()` to convert `ip_addresses` from a string to a list

ip_addresses = ip_addresses.split()
```

**4.Iterate through the remove list**

A key part of my algorithm involves iterating through the IP addresses that are elements in the remove_list. To do this, I incorporated a for loop:
```
# Build iterative statement
# Name loop variable `element`
# Loop through `ip_addresses`

for element in remove_list:
```
**5.Remove IP addresses that are on the remove list**
```
for element in remove_list:

    #create condetional statment to evaluate if `element` is in `ip_addresses `

if element in ip_addresses:

       # use the`remove()` method to remove
       # elements from `ip_addresses`

         ip_addresses.remove(element)
```
**6.Update the file with the revised list of IP addresses**

As a final step in my algorithm, I needed to update the allow list file with the revised list of IP addresses. To do so, I first needed to convert the list back into a string. I used the .join() method for this:
```
    # Convert `ip_addresses` back to a string so that it can be written into the text file 

    ip_addresses = " \n".join(ip_addresses)    
```
Then, I used another with statement and the .write() method to update the file:
```
 # Build `with` statement to rewrite the original file

    with open(import_file, "w") as file:

        # Rewrite the file, replacing its contents with `ip_addresses`

        file.write(ip_addresses)
```

### Project Impact

This project improved the security and efficiency of access control management by automating the process of identifying and removing unauthorized IP addresses from an allow list. By eliminating manual verification, the Python algorithm reduced the risk of human error, ensured that only authorized employees retained access to restricted patient records, and supported the organization's access control policies. The project demonstrates practical experience in Python scripting, automation, file handling, conditional logic, and implementing cybersecurity principles such as the principle of least privilege and secure access management. It also highlights my ability to develop efficient solutions that enhance operational security and protect sensitive healthcare information.
