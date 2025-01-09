# ML_SOC_Estimation_ACS_Energy_Letters

Raw data for the paper "Enhanced SOC Estimation for LFP Batteries: A Synergistic Approach Using Coulomb Counting Reset, Machine Learning, and Relaxation".

If you make use of this dataset, please cite: Che, Y., Xu, L., Teodorescu, R., Hu, X., Onori, S., Enhanced SOC Estimation for LFP Batteries: A Synergistic Approach Using Coulomb Counting Reset, Machine Learning, and Relaxation. ACS Energy Letters (2025). DOI: 10.1021/acsenergylett.4c03223.

Raw data contains 7 folders: Capacity test, GITT test, Pseudo OCV test, training-validation test under 25℃, training-validation test under 45℃, training-validation test under 10℃, and training-validation test under 35℃. The detailed experiments are described below.

**1. Capacity test**
Battery capacity was determined by fully charging the cell from 0% SOC to 100% SOC using C/5 current (i.e., Qch) and fully discharging it from 100% SOC to 0% SOC using C/5 current (i.e., Qdis). This test was performed at 10℃, 25℃ and 45℃ for cells 1 to 6, and was performed at 25 ℃ and 35 ℃ for cells 7 and 8. Then the capacity was obtained by averaging the charge and discharge capacity: Q=(Qch+Qdis)/2.

**2. GITT OCV test**
The batteries were firstly fully charged or discharged using 1C CC-CV, and then the mini-cycle of discharging or charging 2.5% SOC followed by 2-hour rest was repeated to obtain the GITT OCV curve. This experiment was conducted under 10℃, 25℃, 35 ℃, and 45℃.

**3. Pseudo OCV test**
Pseudo OCV is tested to compare with the GITT OCV. The batteries were firstly fully charged or discharged using 1C CC-CV, and then discharged or charged with C/30, C/20, and C/10 until the lower (2.0 V) or upper (3.6 V) voltage limit. Pseudo OCV test was conducted under 10℃, 25℃, and 45℃.

**(4-7) Training-validation test**
Four kinds of loading profiles including CC charge, CC discharge, WLTP discharge, and HPPC+WLTP discharge were conducted. This test generated in total of 434 cases, and the detailed case calculation can refer to Note S2 in the Supplementary Information of the paper.

**4. Training-validation test data under 25℃**. The data contains CC charge, CC discharge, WLTP, and HPPC+WLTP tests. Three average current rates including 1 C, C/2, and C/10 were applied.

**5. Training-validation test data under 45℃**. The data contains CC charge, CC discharge, WLTP, and HPPC+WLTP tests. Three average current rates including 1 C, C/2, and C/10 were applied.

**6. Training-validation test data under 10℃**. The data contains CC charge, CC discharge, WLTP, and HPPC+WLTP tests. Three average current rates including 1 C, C/2, and C/10 were applied.

**7. Training-validation test data under 35℃** . This is the unseen test containing WLTP and shifted WLTP using cell 7 and cell 8. Two average current rates including 1 C and C/2 were applied.

Notation for each test profile:

**-- CC charge**
The cells were first fully discharged using 1C CC-CV. Then, three current rates of 1C, C/2, and C/10 were applied to charge the cells to different SOCs followed by 1-hour rest. This experiment was conducted under 10℃, 25℃, and 45℃.

**-- CC discharge**
The cells were first fully charged using 1C CC-CV. Then, three current rates of 1C, C/2, and C/10 were applied to discharge the cells to different SOCs followed by 1-hour rest. This experiment was conducted under 10℃, 25℃, and 45℃.

**-- WLTP**
The cells were first fully charged using 1C CC-CV. Then, WLTP profiles with three average current rates of 1C, C/2, and C/10 were applied to discharge the cells to different SOCs followed by 1-hour rest. This experiment was conducted under 10℃, 25℃, and 45℃.
In addition, the shifted WLTP (see Figure S4 in the Supplementary Information of the paper) was used to discharge Cell 7 and Cell 8 using two average current rates (1C and C/2) under 25℃, and 35℃ to form the unseen validation conditions. 

**-- HPPC+WLTP**
In this test procedure, the battery was first fully charged. Then, the WLTP protocol was used to discharge the battery to 90% SOC, and rest for 1 hour. After that, an HPPC test (1 charge and 1 discharge pulse) was conducted. The HPPC+WLTP test was repeated (SOC decreases by 10% for each repeat) until SOC reached 10%. Three average current rates of 1C, C/2, and C/10 were applied and the experiment was conducted under 10℃, 25℃, and 45℃.


