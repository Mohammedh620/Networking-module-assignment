# Networking-module-assignment
For this assignment, I purchased a domain on Cloudfare. 
<img width="1477" height="367" alt="image" src="https://github.com/user-attachments/assets/07070eea-6f10-4310-908f-3cf1350d71eb" />
After buying the domain, I deployed an EC2 instance and SSH'ed it into the Ubuntu terminal to connect it. The security group on the instance must allow HTTP (80) for it to work. 
Then I installed NGINX using these commands in the terminal.
- sudo apt update
- sudo apt install nginx -y
- sudo systemctl enable nginx
- sudo systemctl start nginx

After, I createed an A record on my domain and used the public IPv4 address from my EC2 instance to point my record the instance.
<img width="1465" height="406" alt="Screenshot 2025-12-23 191521" src="https://github.com/user-attachments/assets/1fb3046f-6c8c-4553-aec2-a7d7159a8f73" />
After the DNS propagated, the NGINX default page loaded and I was complete.
<img width="893" height="305" alt="Screenshot 2025-12-23 191723" src="https://github.com/user-attachments/assets/999d9f1f-a071-4fd8-984a-c7c42148ffd4" />

