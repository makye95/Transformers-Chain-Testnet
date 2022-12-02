## Transformers-Chain-Testnet

**1. Hardware requirements**：​

CPU: Recommend for Intel Pentium CPU series and above, core number 8 core and above.
Memory: Recommend for 16G And above
Disk: Recommend for 500G And above

**2. Software requirements**：​

Operation system：Run on CentOS 7、ubuntu-22.04-desktop-amd64 system.
Install Screen

>sudo apt-get update

>sudo apt-get install screen

**3. Create new directory for transformers, and enter the folder**

>mkdir transformers

>cd transformers

**4. Download the nodes software**

> wget -q fastcdn.uscloudmedia.com/transformers/test/tfs_v0.18.0_26a1149_devnet

**5. Give the file permission to run**: 
> chmod +x tfs_v0.18.0_26a1149_devnet

**6. Run the program to generate the configuration file** *config.json*:
> ./tfs_v0.18.0_26a1149_devnet -c

**7. Creating a session in Screen**:
> screen -S transformers

**8. Run the program c menu display mode, then automatically create your wallet, and generated a folder cert, which will store a private key for this wallet**:
>./tfs_v0.18.0_26a1149_devnet -m

After this, your node will start synchronizing.

**Control Screen**:

cntrl+A +D - disconnect from the current session, the node will continue to work in the background

screen -r transformers - join the session in which the node is running

cntrl+A +ESC - scrolling mode
