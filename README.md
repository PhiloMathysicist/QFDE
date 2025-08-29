# Quantum Algorithm as a PDE Solver for Computational Fluid Dynamics (CFD) 
WOMANIUM &amp; WISER 2025 Quantum Projects

# Work In Progress [Phase 2]

Going forward, this branch is going to represent the phase 2/face of this repository [For the initial pushes, you may temporarily check the "main" branch.]! Since, upon inquiring further, there was no concrete desire/determination from the peers to carry on with the mission (this having been already established amid the project), until further notice, MKM may opt to pursue the remaining tasks/visions alone and shall do so irregularly. The initial phase of the project was the end-product of access to only 25 days (and only partially) out of the 40 days, initially determined for the projects due to the factors not in control!

Notable potential points of modification, upgrades, and future scope (curated by MKM):

1. Despite the initially (and consistently) observed superior performance of QTT, compared to the classical FDM solver (e.g., an 8%-advantage in memory in one case),  upon further inspection, it has been concluded that this only applies to a fairly restricted set of the combintaion of free parameters rather randomly (in fact the notebook in the benchmark directory already points out a case against the QTT's advantage, which had skipped our attention due to the lack of time). This did not change upon tweaking many parameters and manipulating the rounding operations (to reduce the TT ranks) accross a range of values. As a consequence, one significant point of investigation now would be either further evaluation of the current QTT framework, or building every single operation from the ground up, or indeed utilizing other existing frameworks for that purpose!


2. We wish to build a faithful scheme for the translation of the resultant MPS to a quantum circuit, as there have been some reports, specifying some degrees of advantage for doing that (a translation, which applies to any non-linear PDE directly. As an example there seem to be some ideas in the literature, concerning the transition of MPSs to MPOs and retrieving the Unitary gates out of the latter, through QR decomposition (as well as applying SVD following that to reduce bond dimensions) for instance)! The Cole-Hopf transformation can also be a candidate for a transition to a wavefunction format so that a transition to quantum circuits be potentially more convenient. This latter case needs to be investigated (, nevertheless, it is only applicable to a distinctively special case (Burgers eq.) and hence not generalizable to more complicated settings!).


3. The current QTN implementation is fairly easy to be extended to higher-dimensional VBEs (you just need to adjust the allocation of the two/three components with a desirable number of entries (depending on the level of your choosing precision for each component) within a flattened initial array, having them sit beside one another!). We wish to finalize this very extension eventually, and then investigate its effectiveness, as at the end of the day, the QTT framework is not quite appropriate for D>1 spatial dimensions per se (you may trace the initial roots of the method in quantum spin chains). Upon extracting inferior performance, another interesting strategy will be immediately pursued (more to follow later)...


4. Since the HSE framework is maximally capable of capturing the Schrodinger's flow, we wish to generate and measure the final circuit of a hybrid QTN-HSE method, capable of actually representing the 1DVBE (more shall follow). The higher-dimensional cases seem too distant in terms of the reach of this analysis though, since the VBE accounts for compressible fluids in D>=2 spatial dimensions. Having no constant density profile or the inexistence of the div(u)=0 condition, prompts one to face the involved non-linearities directly, which is extremely complicated to say the least!

5. The explicit form of the exact solution, appropriate for both the IC & BCs will be investigated. The integral, containing the absolute values in one of the stages must be dealt with initially by breaking in two, and there may be a way to retrieve the exact functionality of all the parameters in a final form subsequently. In addition, the more well-known case over the infinite-domain doesn't apply here, as we are dealing with finite bounded intervals. The complication is largely due to that (the existence of BCs on top of the ICs)!

6. A collection of noiseless simulation, noisy simulation and QPU run of the stage 4 (along with perhaps a noiseless variant for that of 2) could be feasible. This shall be on the agenda later (barring the QPU run currently for factors out of control!).




**Please review the participation guidelines [here](https://www.thewiser.org/quantum-projects) for the projects.**

## Project Information:

### Team Size:
  - team size = 3
  - While individual participation is also welcome, we highly recommend team participation :)

### Eligibility:
  - To take part in the WISER Quantum Projects, you must be successfully enrolled in the Womanium & WISER 2025 Quantum Program.
  - We welcome participants from all nationalities, genders, and age groups. The program is designed to be inclusive and global, encouraging collaboration across:
      - University students (undergraduate, masters, PhD, PostDocs)
      - Early career professionals
      - Researchers and scientists
      - Industry practitioners exploring quantum
      - Lifelong learners & career changers
  - If you're curious, committed, and ready to work on real-world quantum challenges, you're welcome here.

### Project Description:
  - Click [here](https://www.thewiser.org/quantum-pde-solvers-for-cfd) to view the project description.
  - YouTube recording of the project description - [link](https://youtu.be/Yi6eh-Bp768)

## Project Submission:
All information in this section will be considered for project submission and judging.

Ensure your repository is public and submitted by **August 10, 2025, 23:59pm US ET**.

Ensure your repository does not contain any personal or team tokens/access information to access backends. Ensure your repository does not contain any third-party intellectual property (logos, company names, copied literature, or code). Any resources used must be open source or appropriately referenced.

### Team Information:

Team Member 1:
 - Full Name: Mohammadreza Khodajou Masouleh
 - Womanium & WISER Program Enrollment ID: gst-iAloBEqFJMO9Y0w


Team Member 2:
 - Full Name: Truong Le Gia Khanh
 - Womanium & WISER Program Enrollment ID: gst-OP0O6T7e5bf7u0x


Team Member 3:
 - Full Name: Abhishek Racharla
 - Womanium & WISER Program Enrollment ID: gst-6n0BRXAtkLWM3im


### Project Solution:
_Include a comprehensive summary of all important information about your project solution here._



All necessary code files and any additional information required to judge your project solution should be included in the repository. 

### Project Presentation Deck:
_Upload/ Link a 3min. presentation deck here._


[https://docs.google.com/presentation/d/1s4WZhg0Xdc48tiEDxg4iBenwstyCZl7d/edit?usp=sharing&ouid=111343293882647029409&rtpof=true&sd=true](https://docs.google.com/presentation/d/1s4WZhg0Xdc48tiEDxg4iBenwstyCZl7d/edit?usp=sharing&ouid=111343293882647029409&rtpof=true&sd=true)


See project presentation guidelines [here](https://www.thewiser.org/quantum-projects)


[https://docs.google.com/presentation/d/1s4WZhg0Xdc48tiEDxg4iBenwstyCZl7d/edit?usp=sharing&ouid=111343293882647029409&rtpof=true&sd=true](https://docs.google.com/presentation/d/1s4WZhg0Xdc48tiEDxg4iBenwstyCZl7d/edit?usp=sharing&ouid=111343293882647029409&rtpof=true&sd=true)


See project presentation guidelines [here](https://www.thewiser.org/quantum-projects)
