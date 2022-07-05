### Testing CI / CD using AWS Code Deploy and Jenkins on Ubuntu 18.04###
1.  Prepare Jenkins Server
2.  Install Deploy-Agent on Target Server and Its Dependencies
        sudo apt install ruby-full wget -y
        cd /home/ubuntu
        wget https://bucket-name.s3.region-identifier.amazonaws.com/latest/install
        chmod +x ./install
        sudo ./install auto
        sudo service codedeploy-agent start
        sudo service codedeploy-agent status
3.  Create Code Deploy Application
4.  Create Code Pipeline