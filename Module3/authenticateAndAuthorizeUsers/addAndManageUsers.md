# Add and Manage Users

## Task 1. Add a new user
`sudo useradd -g research_team researcher9`

## Task 2. Assign file ownership
`sudo chown researcher9 project_r.txt`

## Task 3. Add the user to a secondary group
`sudo usermod -aG sales_team researcher9`

## Task 4. Delete a usersudo 
`sudo userdel researcher9`
> when a new user is created, a group of the same name is created and the user is the only member of that group. after removing the user, it is a good practice to clean up any such empty groups that may remain behind. 

Delete the *researcher9* group that is no longer required

`groupdel researcher9`

