# A. Installing Linux (in Windows computer)

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

Initialize the conda using the following code:

```
conda init --all
```

Close the terminal after the initialization concludes.

# Step 7

Open the terminal and update the conda using the following code:

```
conda update conda
```

System might ask you Yes/No.

Go with **Yes** by typing y and enter. 


# Step 8

Create a conda environment using the following code:

```
conda env create \
  --name qiime2-amplicon-2025.4 \
  --file https://raw.githubusercontent.com/qiime2/distributions/refs/heads/dev/2025.4/amplicon/released/qiime2-amplicon-ubuntu-latest-conda.yml
```

This should take a while. 

# Step 9

Once the **Step 8** concludes **QIIME2** is installed.

So just to confirm, run the followin code:

```
conda deactivate
conda activate qiime2-amplicon-2025.4
qiime info
```

If you see no error (red lines in your Terminal) **Congratulations you have QIIME2.**









