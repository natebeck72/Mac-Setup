macos-config
Install

The easiest way to install is to follow the following steps:

    Make sure you have signed into the Mac App Store. This makes mas easier to deal with
    Install Apples's command line tools: xcode-select --install
    Upgrade Pip to 20.3 or later: sudo pip3 install --upgrade pip
    Install Ansible: sudo pip install ansible
    Create the mac-ansible directory mkdir mac-ansible
    Change directory to mac-ansible cd mac-ansible
    Clone the Repository: git clone https://github.com/natebeck72/Mac-Setup
    Change Directories into the repo: cd Mac-Setup
    Update the requirements file: ansible-galaxy install -r requirements.yml
    Run the osascript command to account for sandboxing  osascript -e 'tell application "Finder"' -e 'set _b to bounds of window of desktop' -e 'end tell'
    Run the Playbook: ansible-playbook playbook.yml -i inventory -K

Commands:

 xcode-select --install
 
 sudo pip3 install --upgrade pip
 
 sudo pip install ansible
 
 mkdir mac-ansible 
 
 cd mac-ansible 
 
 git clone https://github.com/natebeck72/Mac-Setup
 cd Mac-Setup
 ansible-galaxy install -r requirements.yml
 osascript -e 'tell application "Finder"' -e 'set _b to bounds of window of desktop' -e 'end tell'
 ansible-playbook playbook.yml -i inventory -K
