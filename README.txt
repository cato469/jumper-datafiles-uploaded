this folder contains data files:

justBiarticularsPOS3.txt
justHipPOS3.txt
baselinePOS3.txt.txt
optPOS3.txt

the file importC loads the datafiles (header and time-series data) into Matlab. The meaning of each column is transparent from the loading function. 

init = initial conditions of the model (24 states)
istim = initial stimulation of the muscles
tstim = stim onset times for the muscles
m = segment masses
j = segment inertias
l = segment lengths
d = distance between proximal joint and segment mass center
fmax = maximum isometric muscle force
rlceopt = optimum muscle length
rlsenul = tendon slack length

dt=1/1000;
out.t = time
out.state = ode states
out.phi = angles (external reference frame, angles all from positive X axis)
out.phiseg = inter-segment angles
ddt_phiseg
out.ddt_phi
out.base = position of the foot
out.lcerel = contractile element length
 out.gamma = calcium concentration
out.x = center of mass horizontal position
out.y = center of mass vertical position
out.cmx = position of segments
out.cmy = position of segments
out.tor = net joint torques
out.fse = force in the series-elastic element
out.fpe = force in the parallel-elastic element
out.loi = muscle-tendon complex length
out.ese = tendon excursion
out.q = muscle active state
out.stim = muscle stimulation