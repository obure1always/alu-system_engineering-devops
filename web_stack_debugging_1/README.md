Nginx likes port 80 mandatory Using your debugging skills, find out what’s keeping your Ubuntu container’s Nginx installation from listening on port 80. Feel free to install whatever tool you need, start and destroy as many containers as you need to debug the issue. Then, write a Bash script with the minimum number of commands to automate your fix.
Requirements:

Nginx must be running, and listening on port 80 of all the server’s active IPv4 IPs Write a Bash script that configures a server to the above requirements root@966c5664b21f:/# curl 0:80 curl: (7) Failed to connect to 0 port 80: Connection refused root@966c5664b21f:/# root@966c5664b21f:/# ./0-nginx_likes_port_80 > /dev/null 2&>1 root@966c5664b21f:/# root@966c5664b21f:/# curl 0:80

<title>Welcome to nginx!</title> <style> body { width: 35em; margin: 0 auto; font-family: Tahoma, Verdana, Arial, sans-serif; } </style>
Welcome to nginx!
If you see this page, the nginx web server is successfully installed and working. Further configuration is required.

For online documentation and support please refer to nginx.org.
Commercial support is available at nginx.com.

Thank you for using nginx.

root@966c5664b21f:/# Repo:
GitHub repository: alu-system_engineering-devops Directory: web_stack_debugging_1 File: 0-nginx_likes_port_80

0/3 pts Score Project badge Your score will be updated as you progress.

Please review all the tasks before you start the peer review.
