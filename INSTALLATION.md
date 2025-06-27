# A. Installing Linux in Windows

For windows, we need to install Linux in your windows computer. And then install QIIME2 in that Linux.
We will install Linux with *Windows Subsystem for Linux*


# Step 1

On the **Windows menu** (left bottom corner), Right click on **Command Prompt**

You should see **More** option where you shpuld click on **Run as administrator**

System might ask you Yes/No or even your Password (PC password).

Go with **Yes** or provide the password. 

# Step 2

Install wsl using the following command in your **Command Prompt**

```
wsl --install
```

This command may take up to 10 minutes.

Again, system might ask you Yes/No or even your Password (PC password).

Go with **Yes** or provide the password. 

# Step 3

After the code in the **Step 2** concludes. 

Close the **Command Prompt** and **Restart** the computer.

# Step 4 

After the restart, the prompt will ask to create a new linux user.

So, you have to provide a new **username** as well as **password**

The **password** should be entered twice to confirm.

This will be your **username** and **password** for linux (ubuntu). 

# Step 5 

Close everything and **Restart** the computer.


# B. Installing QIIME2

# Step 1 

**Open Ubuntu**

Click on the **Windows** logo. You should see an icon for **Ubuntu** ![image](https://github.com/user-attachments/assets/fa4303e0-0cd5-4eaf-a627-e35a8b53ec05)

This will open Ubuntu terminal.

# Step 2 

Create a miniconda directory and download the script (.sh) file in that directrory. To do so use the following two codes in your Ubuntu terminal.

```
mkdir -p ~/miniconda3
```

```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
```

# Step 3 

Run the downloaded script using the following code:

```
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
```

# Step 4

Remove the script file after the run using the following code:

```
rm ~/miniconda3/miniconda.sh
```

# Step 5

Refresh the terminal using the following code:

```
source ~/miniconda3/bin/activate
```

# Step 6







































