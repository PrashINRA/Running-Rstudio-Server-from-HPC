#Download the prstudio.sh and run the bellow on terminal
chmod +x ./prstudio.sh
./prstudio.sh

##This will create an instruction 
#Open a new terminal and paste the instructions which would be like
ssh -N -L 8787:localhost:8787 psingh@your_compute_node

#Now point your browser to Point your web browser at http://localhost:8787

#An Rstudio Server is ready to bounce.


