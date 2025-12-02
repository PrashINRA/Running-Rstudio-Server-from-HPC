# Run RStudio Server on Your HPC (Simple Guide)

This guide explains how to run RStudio Server directly on your HPC using a container.

---

## Step 1: Log in to your HPC

Open a terminal and log in to your HPC account:
```bash
ssh your_username@hpc.address.nl
```

## Step 2: Download the RStudio startup script
```bash
wget https://raw.githubusercontent.com/PrashINRA/Running-Rstudio-Server-from-HPC/main/prstudio.sh
```

## Step 3: Make it executable
```bash
chmod +x prstudio.sh
```

## Step 4: Run the shell script
```bash
./prstudio.sh
```

Let it run for a few minutes as it builds a container for R and RStudio.

## Step 5: Open your browser

Navigate to:
```
http://localhost:8787
```

> **Note:** The port may vary (e.g., 8788, 8789) depending on availability.

This will open RStudio in your browser, connected to your HPC server with full compute power.

















