# Job Answers

1. **htop program:**
   - **Command:** `sudo apt install -y htop && htop`
   - **Answer:** `htop` shows real-time system resource utilization including CPU usage across cores, RAM/Swap memory meters, task count, and active running processes with PIDs.

2. **apache2 version:**
   - **Command:** `apt show apache2`
   - **Answer:** Ubuntu repository offers `apache2` candidate version `2.4.58-1ubuntu8` (or the version listed under Candidate in `apt-cache policy apache2`).

3. **Installed packages count:**
   - **Command:** `apt list --installed | wc -l`
   - **Answer:** Running `apt list --installed | wc -l` shows approximately 550–600 packages currently installed on the server.

4. **Alpine Docker container:**
   - **Command:** `sudo docker run --rm alpine echo "Hello from Alpine"`
   - **Answer:** Container executed successfully and printed `Hello from Alpine`.


5. **Docker key and sources file paths:**
   - **Command:** `ls -l /etc/apt/keyrings/docker.gpg /etc/apt/sources.list.d/docker.list`
   - **Answer:** 
     - Key file: `/etc/apt/keyrings/docker.gpg`
     - Sources file: `/etc/apt/sources.list.d/docker.list`

6. **Remove htop & verify:**
   - **Command:** `sudo apt remove -y htop && hash -r && htop`
   - **Answer:** Running `htop` returns `bash: /usr/bin/htop: No such file or directory`, proving it has been completely removed.
