# Leveraging Pangolin and Alibaba Cloud DNS for Secure and Cost-Effective Exposure of Home Network Applications to the Public Internet
Integrating Pangolin with Alibaba Cloud DNS to expose your home network applications to the public internet offers several advantages:

**Advantages:**

1. **Cost-Effective Deployment:** By utilizing a lightweight server as a reverse proxy, you can efficiently expose your home server applications to the internet without the need for complex infrastructure.

2. **Simplified Access:** With internal network penetration, your home server applications can be accessed via a public domain name using HTTPS, ensuring secure and straightforward access.

3. **Enhanced Security:** Leveraging Pangolin's security features alongside Alibaba Cloud DNS provides robust protection for your applications, safeguarding them from potential threats.

**Implementation Steps:**

To integrate Pangolin with Alibaba Cloud DNS and expose your home network applications to the public internet, follow these steps:

1. **Prepare Your Environment:**
   - **VPS:** Set up a Virtual Private Server (VPS) with a public IP address to act as the reverse proxy.
   - **DNS:** Configure your domain's DNS settings to point to the VPS's IP address.
   - **Networking:** Ensure that the necessary ports are open on your VPS to allow traffic to your home network applications.

2. **Clone the Repository:**
   - Clone the [Pangolin repository](https://github.com/neozhu/pangolin.git) to your VPS:
     ```bash
     git clone https://github.com/neozhu/pangolin.git
     ```

3. **Modify Configuration Files:**
   - Navigate to the cloned repository directory:
     ```bash
     cd pangolin
     ```
   - Edit the configuration files to replace placeholders (`<>`) with your specific parameters, such as domain names, internal IP addresses, and other relevant settings.

4. **Deploy Using Docker Compose:**
   - Run the following command to start the services in detached mode:
     ```bash
     sudo docker-compose up -d
     ```
   - This command will build and start the containers as defined in your `docker-compose.yml` file.


