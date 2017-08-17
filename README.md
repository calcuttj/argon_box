# argon_box
Primitive Python-based Geant4 simulation of particle interactions in liquid argon

Dependencies:
 ROOT
 Geant4
 g4py (which requires boost and XercesC)

Example Usage:

  Mono-energetic particles:
  $ python argon_box.py --nevents=100 --source='e-' --energy=2.0 --output='electron_2GeV_sim.root'

  HepEVT data:
  $ python argon_box.py --nevents=100 --source='input.hepevt' --output='hepevt_sim.root'

Other useful options:
  --seed=<N>: Change random seed
  --disable_edepsim: Disable primitive simulation of energy depositions
