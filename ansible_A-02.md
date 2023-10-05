## Ansible Assignment-2

Install nginx in your servers(more then 2) and make sure the log files of nginx should not be granted more than 1 GB space on the nodes

Create equal number of websites as per your team  members and every members website should be hosted for only 2 hours and after every 2 hours another website should start displaying.

    - First 2 hours <team>.opstree.com should display content of tanya website
    
    - Next 2 hours <team>.opstree.com should display content of Heena website

Install Apache

Also Configure nginx to run as reverse proxy to apache after completing first point individually.


- Run the ansible commands in such a way that workers nodes are updated one by one and not altogether and also make sure using all type of strategies.

### Steps followed:

#### created host file and tested it

  ![image](https://github.com/HarshitSingh-Codes/Practice-/assets/67234531/edacff34-3aab-4a8b-a1c6-eb529e13bf88)

#### install nginx in all server and check it
ansible -m apt -a "name=nginx state=present update_cache=yes" -b all

![image](https://github.com/HarshitSingh-Codes/Practice-/assets/67234531/d9dc1219-a3cb-4694-b76e-4f5565565b97)

#### set size of nginx log file to 1GB

![image](https://github.com/HarshitSingh-Codes/Practice-/assets/67234531/754381a9-9257-4648-87e2-01f605c434c4)

make team members website 

![image](https://github.com/HarshitSingh-Codes/Practice-/assets/67234531/e604c627-d61c-4121-8fcf-19df2edf7947)

![image](https://github.com/HarshitSingh-Codes/Practice-/assets/67234531/da3811dd-ffda-4439-95a4-284958e74978)

![image](https://github.com/HarshitSingh-Codes/Practice-/assets/67234531/cd4dc969-2504-4312-99e7-045213ae2aa4)

#### restart NGINX and test it

![image](https://github.com/HarshitSingh-Codes/Practice-/assets/67234531/f21d513a-5597-4018-9111-1324b8860f8a)




