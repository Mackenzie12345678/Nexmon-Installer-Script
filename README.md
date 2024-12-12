This bash script installs Nexmon
This is what the file does

Install some dependencies: sudo apt-get install git gawk qpdf adb flex bison
For x86_64 systems, install i386 libs:
sudo dpkg --add-architecture i386
sudo apt-get update
sudo apt-get install libc6:i386 libncurses5:i386 libstdc++6:i386
Clone our repository: git clone https://github.com/seemoo-lab/nexmon.git
Chmod 777 nexmon directory
In the root directory of the repository: cd nexmon
Setup the build environment: source setup_env.sh
Compile some build tools and extract the ucode and flashpatches from the original firmware files: make

Instructions:
Place "nexmoninstaller" file in home (/home/)
Run in terminal sudo ./nexmoninstaller (sudo is mandatory)

