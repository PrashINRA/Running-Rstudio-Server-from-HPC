# Run RStudio Server on Your HPC (Simple Guide)

This guide explains how to run RStudio Server directly on your HPC using a container.  
No bioinformatics or DevOps background required.

---

## **Step 1: Log in to your HPC**

Open a terminal on your HPC and login to your account

```bash
ssh your_username@hpc.address.nl

## **Step 2: Download the RStudio startup script**

wget https://raw.githubusercontent.com/PrashINRA/Running-Rstudio-Server-from-HPC/main/prstudio.sh


## **Step 3: Make it executable**

chmod +x prstudio.sh

## **Step 4: Run the shell script**

./prstudio.sh

#Let it run for few min as it is building a container for R and Rstudio
#Follow the instructions printed on the screen.
#The script will tell you to open a new terminal on your hpc and run a command similar to:

ssh -N -L 8787:localhost:8787 your_username@node123

## **Step 5: Open the browser and**

http://localhost:8787

#he port may also be 8788, 8789, etc., depending on availability.

You should now see RStudio Server running on your HPC node with full compute power.

Done!

You can now use RStudio in your browser, backed by your HPC’s high-performance compute resources.

**An Rstudio Server is ready to bounce**





















