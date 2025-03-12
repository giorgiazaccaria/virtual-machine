# virtual-machine-cellGMM
This repository is related to the paper _Cellwise outlier detection in heterogeneous populations_ by Giorgia Zaccaria, Luis A. García-Escudero, Francesca Greselin, and Agustín Mayo-Íscar. It contains the codes for reproducing some of the analyses presented in the paper via a Github Codespace.

Specifically, the relevant codes for reproducing the analyses are the following:
-  "Code for Reproducibility Simulation Technometrics_Scen1_5out_0mis.R" $\rightarrow$ This is a sub-example of the simulation study for Scenario 1 with $5\%$ of cellwise contamination. At the end of the script, there is a code for reproducing the part of Table 1 in the Main Article corresponding to Scenario 1 with $5\%$ outlying values.

> [!IMPORTANT]
> The number of samples is currently set to $10$ in the R script, although the simulations in the paper were run on $100$ samples. Increasing the number of samples increases the computational time required for exectuing the code. It is worth noting that the simulations were run on virtual machines with $12$ cores, whereas the one created below has only $4$ cores. The user can change the number of samples up to $100$.

- "Code for Reproducibility Simulation Figure Technometrics_Fast.R" $\rightarrow$ This script generates Figures 1 and 2 of the Main Article for all three scenarios. The code starts by loading the file "Data for Figure Reproducibility.RData", which contains the results for the three scenarios presented in the simulation study of the Main Article.

-  "Code for Reproducibility Simulation and Figure Technometrics_EntireScen1" (available in two formats: .Rmd and .html) $\rightarrow$ This script provides the complete simulation study for Scenario 1 with cellwise contamination levels of $0\%$, $5\%$, and $10\%$. It is used to reproduce Figures 1 and 2 of the Main Article for Scenario 1 and runs in approximately 1 hour.

We have prepared a **Github Codespace** that can be used to automatically set-up an Rstudio Server and explore the codes in an interactive way. Instructions to access the Github Codespace are reported below.

> [!WARNING]
> Please note that you need a Github account to access the Github Codespace.

1. **Click on** <a href="https://codespaces.new/giorgiazaccaria/virtual-machine-cellGMM" target="_blank">https://codespaces.new/giorgiazaccaria/virtual-machine-cellGMM</a> to set-up your own version of the Codespace; **set** the Machine type option equal to **4-core**, and **click on** the green button named `Create codespace` (see the pictures below).
   
![image](https://github.com/user-attachments/assets/6b2c4137-4ede-4950-ae28-14e7c89a6d83)

2. Wait for the Codespace to be created. This operation can take some minutes. Wait until the number 2 appears next to `Ports`. You should see something like the following screen.
   
![image](https://github.com/user-attachments/assets/f97af82d-1ac5-4307-bb67-0b54c795cb7e)
   
4. Click on the `Ports` tab (which is highlighted in the previous image). Drag the mouse over the Forwarded Addresses field in the 8787 port and click on the globe icon, as displayed in the following image.
   
![image](https://github.com/user-attachments/assets/7dd1b898-e1e3-4a62-9db5-acdfc25f4610)

5. The previous action will open a new tab in your browser with the Rstudio Server interface, as follows.

![image](https://github.com/user-attachments/assets/1a6afe6b-73d9-4b13-8186-a6f131ae2419)
   
7. Login into the Rstudio server using the following credentials:
Username: `rstudio`
Password: `rstudio`
These operations will create an Rstudio session in your browser. When the Rstudio session is ready, click on the file "virtual-machine-cellGMM" (bottom-right panel in R Studio). Now you can explore the codes interactively!

> [!NOTE]
> GitHub Codespaces is paid for either by an organization, an enterprise, or a personal account. The Free and Pro plans for personal accounts include free use of GitHub Codespaces up to a fixed amount of usage every month.
 We refer to the <a href="https://docs.github.com/en/billing/managing-billing-for-your-products/managing-billing-for-github-codespaces/about-billing-for-github-codespaces">official docs</a> for more details.
