# Force-Field-Bonded-Terms-under-Structural-Inconsistency
data for "Force Field Bonded Terms under Structural Inconsistency"

"list.residues" list of residues in the data set

"nma/"              optimization of CHARMM force field parameters for bond and angle terms; and normal mode analysis;

"stability_test/"   the stability test on the optimized force field parameters.
                    'random_fc_bond/'  : optimization of bond term parameters starting with random force constants
                    'random_fc_angle/' : optimization of angle term parameters starting with random force constants
                                      'run.sh' : script to perform optimization
                                      'print_stat.run' : script to print statistics on optimized parameters
                                      'random_[1..5]' : 5 optimization runs 
                                      'molecule/' 'start.pdb' : initial geometry
                                                  'top.inp'   : topology file
                                                  'opt1.out' and 'opt1.pdb' : g16 optimization output and geometry
                                                  'restrdihe.inp' : restraints for soft dihedrals
                                                  'emp.card/pdb' : CHARMM geometry
                                                  'minimize.out' : CHARMM output for minimizaion without PES scan constraints
                                                  'term.list' : list of terms to optimize
                                                  'pes.out' : CHARMM output for PES scans
                                                  'intra.inp' : script for the optimization program (developer.exe)
                                                  'intra.out' : optimization output

"program/"          'developer.exe' : the program for optimization of force field parameters; 
                    'charmm/' : charmm scripts for minimization; 
