##### PD-Action is an automation created by Project Discovery to Run throguh Github Actions. But Gituhb Restricted Access on the Repo
##### Note: Don't use this to Run on Github Actions since Gituhb will Ban your account due to heavy traffic load

#### 1. Clone this to your VPS
        git clone https://github.com/supunhalangodaa/BugBounty-Automation/
#### 2. Install Below Tools
        go get -v github.com/projectdiscovery/subfinder/v2/cmd/subfinder
        go get -v github.com/projectdiscovery/dnsx/cmd/dnsx
        go get -v github.com/projectdiscovery/naabu/v2/cmd/naabu
        go get -v github.com/projectdiscovery/httpx/cmd/httpx
        go get -v github.com/projectdiscovery/nuclei/v2/cmd/nuclei
        go get -v github.com/projectdiscovery/notify/cmd/notify
#### 3. Now Schedule the Recon.sh with Cron Job or Tmux
#### 4. To use Run Background sessions after logging off use below steps 
#### Start Tmux in the shell type below command
        Tmux
#### Now Run Bash Recon.sh script
        bash Recon.sh
#### Detach the tmux session by doing below
        Ctrl+b and then d
#### You can now safely log off from the remote machine, your process will keep running inside tmux
#### To check the session after logging Type 
        "tmux attach" 
#### And you will get the tmux session
