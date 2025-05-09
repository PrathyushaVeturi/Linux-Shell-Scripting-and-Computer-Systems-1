#Printing the Greeting message while login to the shell of a user, Vedant.

**Adding the User**
`sudo useradd -m Vedant -s /bin/bash`

**Adding a group**
`sudo groupadd Developers`

**Adding the user to the group**
`sudo usermod -aG Developers Vedant`

Now, you need to switch the user using the command, `sudo su <username>`.
`sudo su Vedant`

Now, execute the below command to add `echo "Welcome Vedant!"` to .bashrc file in the home directory of the user, Vedant.
`echo ' echo "Welcome Vedant!" ' >> /home/Vedant/.bashrc

**If you want to execute the above echo command without switching to the user, Vedant, you can use the below command**
`echo ' echo "Welcome Vedant!" ' | sudo tee -a /home/Vedant/.bashrc`

At the end, switch the user and check whether you receive the greeting or not.
