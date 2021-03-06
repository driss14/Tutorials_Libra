| [HOME](README.md) |   [Videos](VIDEOS.md)       |
| -------- | ------------------------------------ |

# Tutorials_Libra
Tutorials showcasing various capabilities of Libra

## TOC

1. Rigid body
 * 1.1. [Construct & describe properties of rigid bodies](1_rigid_body/1_setup)

2. Integrators
 * 2.1. [Runge-Kutta 4-th order](2_integrators/1_runge_kutta_4th_order)

3. Linear algebra
 * 3.1. [operations with VECTOR, MATRIX, and CMATRIX data types](3_linear_algebra/1_vector_matrix_cmatrix_basics)

4. Optimization
 * 4.1. [Gradient descent optimizer](4_optimization/1_gradient_descent)
 * 4.2. [line search using DIIS](4_optimization/2_diis)

5. Electronic structure calculations in Libra
 * 5.1. [Extended Huckel Theory, EHT](5_electronic_structure/1_eht)
    * 5.1.1. [Compact version](5_electronic_structure/1_eht/1_compact)
    * 5.1.2. [Detailed version](5_electronic_structure/1_eht/2_detailed)

 * 5.2. [Incomplete Neglect of Differential Overlap, INDO](5_electronic_structure/2_indo)
    * 5.2.1. [Compact version](5_electronic_structure/2_indo/1_compact)

6. Dynamics with Libra
 * 6.1. [Quantum-classical, trajectory methods](6_dynamics/1_trajectory_based)
   * 6.1.1. [Model, adiabatic MD](6_dynamics/1_trajectory_based/1_model_adiabatic)
        * 6.1.1.1. [NVE ensemble](6_dynamics/1_trajectory_based/1_model_adiabatic/1_nve)
        * 6.1.1.2. [NVT ensemble](6_dynamics/1_trajectory_based/1_model_adiabatic/2_nvt)
             * 6.1.1.2.1 [1 electronic state](6_dynamics/1_trajectory_based/1_model_adiabatic/2_nvt/1_1_state)
    * 6.1.2. [Model, common approach to adiabatic, Ehrenfest, and TSH](6_dynamics/1_trajectory_based/2_model_adiabatic)
    * 6.1.3. [Model, Ehrenfest recipes](6_dynamics/1_trajectory_based/3_model_ehrenfest_recipes)
    * 6.1.5. [Atomistic, adiabatic dynamics, ground/excited](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states)
    * 6.1.6. [Model, NBRA and non-NBRA](6_dynamics/1_trajectory_based/6_model_nbra)
    * 6.1.7. [Model, TSH with thermostat, quantum-vs-classical partitioning of DOFs, and constrining](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath)

 * 6.2. [Quantum-classical, neglect-of-back-reaction trajectory workflows](6_dynamics/2_nbra_workflows)
    * 6.2.1. [step 1 with DFTB+](6_dynamics/2_nbra_workflows/1_step1_dftb)
    * 6.2.2. [step 1 with QE](6_dynamics/2_nbra_workflows/2_step1_qe)
    * 6.2.3. [step 2 with QE](6_dynamics/2_nbra_workflows/3_step2_qe)
    * 6.2.4. [step 3](6_dynamics/2_nbra_workflows/4_step3)
      * 6.2.4.1 [build_SD_basis](6_dynamics/2_nbra_workflows/4_step3/1_build_SD_basis)
    * 6.2.5. [step 4](6_dynamics/2_nbra_workflows/5_step4)
      * 6.2.5.1 [Initialze_data](6_dynamics/2_nbra_workflows/5_step4/1_initialize_data)
    * 6.2.6. [step 4](6_dynamics/2_nbra_workflows/5_step4)
      * 6.2.6.1 [Dynamics](6_dynamics/2_nbra_workflows/5_step4/2_dynamics)

 * 6.3. [Hierarchical equations of motion, HEOM](6_dynamics/3_heom)
    * 6.3.1. [Computing population dynamics and lineshapes](6_dynamics/3_heom/1_dynamics_and_lineshapes)

 * 6.4. [DVR, on-the-grid wavepackets](6_dynamics/4_wavepackets)
    * 6.4.1. [Gaussian wavepackets](6_dynamics/4_wavepackets/1_gaussian)
      * 6.4.1.1. [Computing matrix elements](6_dynamics/4_wavepackets/1_gaussian/1_matrix_elements)

 * 6.5. [Fermi Golden Rule rates, FGR](6_dynamics/5_fgr)

7. Special functions
 * 7.1. [Sorting, matrix statistics](7_special_functions/1_sorting_matrix_statistics)
 * 7.2. [Fitting distributions to a superposition of Gaussians](7_special_functions/2_gaussian_kernel_algorithm)

8. Model Hamiltonians
 * 8.1. [Define model Hamiltonians and plot PES](8_model_hamiltonians/1_pes_plotting)
 * 8.2. [Define atomistic Hamiltonians and plot PES](8_model_hamiltonians/2_interfaces_with_qchem_codes)

_______________________________

## Use cases

1. Create a chemical system
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
  
2. EHT calculations with Libra
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)

3. INDO calculations with Libra
  * [5.2.1.](5_electronic_structure/2_indo/1_compact/tutorial.ipynb)

4. Compute .cube files from orbitals computed with Libra
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
  * [5.2.1.](5_electronic_structure/2_indo/1_compact/tutorial.ipynb)

5. Visualize the MOs from .cube files
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
  * [5.2.1.](5_electronic_structure/2_eht/1_compact/tutorial.ipynb)

6. Compute pDOS from built-in electronic structure calculations in Libra
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)

7. Plot pDOS computed with Libra
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)

8. Visualize MD trajectory with py3Dmol:
  * [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)
  * [6.2.1.](6_dynamics/2_nbra_workflows/1_step1_dftb/tutorial.ipynb)
  * [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)

9. Construct the vibronic Hamiltonian from the QE MD calculations
  * [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)

10. Read the vibronic Hamiltonian data files to obtain its properties
  * [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)
  * [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/1_build_SD_basis/tutorial.ipynb)
  * [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
  * [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)

11. Compute the time-averaged nonadiabatic couplings of the vibronic Hamiltonian
  * [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)
  * [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/1_build_SD_basis/tutorial.ipynb)

12. Manually construct a Slater Determinant basis
  * [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/1_build_SD_basis/tutorial.ipynb)

13. Auto-generate a Slater Determinant basis
  * [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/1_build_SD_basis/tutorial.ipynb)

14. Compute the energies and nonadiabatic couplings in the SD basis
  * [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/1_build_SD_basis/tutorial.ipynb)

15. Calculate population and coherence dynamics of a quantum system embedded in a bath
  * [6.3.1.](6_dynamics/1_dynamics_and_lineshapes/3_heom/tutorial.ipynb)
   
16. Calculate absorbance spectral lineshapes of a quantum system embedded in a bath
  * [6.3.1.](6_dynamics/3_heom/1_dynamics_and_lineshapes/tutorial.ipynb)

17. Construct and plot the Heller's wavepackets
  * [6.4.1.1.](6_dynamics/4_wavepackets/1_gaussian/1_matrix_elements/tutorial.ipynb)

18. Compute the matrix elements of various operators with Heller's wavepackets
  * [6.4.1.1.](6_dynamics/4_wavepackets/1_gaussian/1_matrix_elements/tutorial.ipynb)

19. Define diabatic abstract model Hamiltonian 
  * [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb)
  * [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)

20. Define adiabatic abstract model Hamiltonian
  * [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb)

21. Define adiabatic file-based model Hamiltonian
  * [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb)
  * [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)

22. Plot 1D PES 
  * [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb)
  * [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)
  * [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
  * [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)

23. Plot diabatic-to-adiabatic transformaitons vs. coordinate in 1D
  * [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb)

24. Plot 1D PES vs. time
  * [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb)
  * [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
  * [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)

25. Define Libra/Psi4 intraface Hamiltonian 
  * [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)

26. Define Libra/DFTB+ intraface Hamiltonian
  * [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)
  * [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)

27. Plot the PES of LiH at the EOM-CCSD/sto-3G level computed via interface of Libra with Psi4
  * [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)

28. Plot the 1D PES of HFCO at the TD-DFTB level compute with interface of Libra with DFTB+
  * [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)

29. Generate XYZ trajectory from a list of matrices
  * [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)

30. Perform a ground state adiabatic MD with Libra
  * [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)
  * [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)

31. Perform an excited state adiabatic MD with Libra
  * [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)
  * [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)

32. Compute MD with DFTB+ via Libra
  * [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)

33. Generate XYZ trajectory from HDF5 files
 * [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)

34. Compute trajectory-averaged dephasing times
  * [6.2.5.1](6_dynamics/2_nbra_workflows/5_step4/1_initialize_data)

35. Compute trajectory-averaged energy gaps
  * [6.2.5.1](6_dynamics/2_nbra_workflows/5_step4/1_initialize_data)

36. Plot trajectory-averaged dephasing times
  * [6.2.5.1](6_dynamics/2_nbra_workflows/5_step4/1_initialize_data)

37. Fit the probability density of randomly distributed point with Gaussian density kernel functions
 * [7.2.](7_special_functions/2_gaussian_kernel_algorithm/tutorial.ipynb)

38. Read the HDF5 files to setup Hamiltonians
  * [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)

39. Read the HDF5 files to plot results of dynamical calculations
  * [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
  * [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)

40. Compute nonadiabatic dynamics for atomistic systems with NBRA using Kohn-Sham states
  * [6.2.5.1.](6_dynamics/2_nbra_workflows/5_step4/2_dynamics/tutorial.ipynb)

41. Plot the PES profiles with multidimensional model Hamiltonians
  * [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)

42. MD and NAMD in the NVT ensemble
  * [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)

43. Partitioning quantum and classical DOFs
  * [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)

44. Coupling classical DOFs to thermostat
  * [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)

45. Constraining DOFs in dynamics
  * [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)


_______________________________


## Functions

- `liblibra::libdyn::libgwp`
  - `gwp_coupling` [6.4.1.1.](6_dynamics/4_wavepackets/1_gaussian/1_matrix_elements/tutorial.ipynb)
  - `gwp_dipole` [6.4.1.1.](6_dynamics/4_wavepackets/1_gaussian/1_matrix_elements/tutorial.ipynb)
  - `gwp_kinetic` [6.4.1.1.](6_dynamics/4_wavepackets/1_gaussian/1_matrix_elements/tutorial.ipynb)
  - `gwp_overlap` [6.4.1.1.](6_dynamics/4_wavepackets/1_gaussian/1_matrix_elements/tutorial.ipynb)
  - `gwp_value` [6.4.1.1.](6_dynamics/4_wavepackets/1_gaussian/1_matrix_elements/tutorial.ipynb)


- `liblibra::libqm_tools`
  - `charge_density` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
  - `compute_dos` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)

- `libra_py`
  - `dynamics`
    - `heom`
      - `compute` 
        - `run_dynamics` [6.3.1.](6_dynamics/3_heom/1_dynamics_and_lineshapes/tutorial.ipynb)
    - `tsh`
      - `compute`
        - `generic_recipe` [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb) | 
            [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)
        - `init_electronic_dyn_var` [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb) 
        - `init_nuclear_dyn_var` [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb) |
            [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb) |
            [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)
        - `run_dynamics` [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)
      - `plot`
        - `add_basis_transform` [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
        - `add_coordinates_vs_t` [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
        - `add_energies` [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
        - `add_momentum_vs_t` [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
        - `add_phase_space` [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
        - `add_populations` [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
        - `add_time_overlap_projectors` [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
        - `add_trajectory_resolved_ham_property` [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
        - `hdf2xyz` [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)
        - `plot_dyn` [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)
        - `plot_dynamics` [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb) |
            [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)
      - `recipes`
        - `adiabatic_md_interfaces_params` [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)

  - `models`
    - `Holstein`
      - `Holstein2` [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb)
    - `Tully`
      - `chain_potential` [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)

  - `workflows`
    - `nbra`
      - `decoherence_times`
        - `energy_gaps_ave` [6.2.3.](/6_dynamics/2_nbra_workflows/5_step4/1_initialize_data/tutorial.ipynb)
        - `decoherence_times_ave` [6.2.3.](/6_dynamics/2_nbra_workflows/5_step4/1_initialize_data/tutorial.ipynb)
      - `step2`
        - `run` [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)
      - `step3`
        - `build_SD_basis` [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/1_build_SD_basis/tutorial.ipynb)
        - `run` [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/1_build_SD_basis/tutorial.ipynb)
      - `step4`
        - `get_Hvib2` [6.2.3.](/6_dynamics/2_nbra_workflows/5_step4/1_initialize_data/tutorial.ipynb)
        - `run` [6.2.5.](/6_dynamics/2_nbra_workflows/5_step4/1_initialize_data/tutorial.ipynb)

  - `data_conv`
    - `make_list` [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)
    - `matrix2list` [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)

  - `data_outs`
    - `print_matrix` [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)

  - `data_read`
    - `get_data_sets` [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)

  - `data_stat`
    - `cmat_stat2` [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)

  - `data_visualize`
    - `colors` [7.2.](7_special_functions/2_gaussian_kernel_algorithm/tutorial.ipynb)
    - `plot_map` [6.4.1.1.](6_dynamics/4_wavepackets/1_gaussian/1_matrix_elements/tutorial.ipynb)
    - `plot_map_nparray` [6.2.5.1](6_dynamics/2_nbra_workflows/5_step4/1_initialize_data)
    - `plot_MATRIX2nparray` [6.2.5.1](6_dynamics/2_nbra_workflows/5_step4/1_initialize_data)

  - `DFTB_methods`
    - `read_dftb_output` [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)
    - `run_dftb_adi` [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb) | 
       [6.1.5.](6_dynamics/1_trajectory_based/5_atomistic_adiabatic_excited_states/tutorial.ipynb)
    - `make_dftb_input` [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)

  - `dynamics_plotting`
    - `plot_pes_properties` [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb) | [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)
    - `plot_surfaces` [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb) | 
            [6.1.6.](6_dynamics/1_trajectory_based/6_model_nbra/tutorial.ipynb) |
            [6.1.7.](6_dynamics/1_trajectory_based/7_model_nonadiabatic_system_bath/tutorial.ipynb)

  - `ft`
    - `ft2`[6.3.1.](6_dynamics/3_heom/1_dynamics_and_lineshapes/tutorial.ipynb)

  - `gaussian_kernel_algorithm`
    - `compute_apriory_prob_densities_1D` [7.2.](7_special_functions/2_gaussian_kernel_algorithm/tutorial.ipynb)
    - `compute_widths_1D` [7.2.](7_special_functions/2_gaussian_kernel_algorithm/tutorial.ipynb)
    - `gaussian_density_estimator_1D` [7.2.](7_special_functions/2_gaussian_kernel_algorithm/tutorial.ipynb)
    - `gaussian_kernel_algorithm_iteration_1D` [7.2.](7_special_functions/2_gaussian_kernel_algorithm/tutorial.ipynb)

  - `hpc_utils`
    - `distribute` [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)

  - `LoadMolecule`
    - `Load_Molecule` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
   
  - `LoadPT`
    - `Load_PT` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    
  - `pdos`
    - `libra_pdos` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)

  - `psi4_methods`
    - `run_psi4_adi` [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)

  - `QE_methods`
    - `out2inp` [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)
        
  - `scan`
    - `coords2xyz` [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)
    - `make_path_xyz2` [8.2.](8_model_hamiltonians/2_interfaces_with_qchem_codes/tutorial.ipynb)


_______________________________


## Classes and class members

- `liblibra::libcontrol_parameters::Control_Parameters` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)


- `liblibra::libchemobjects`
  - `libchemsys::System`
    - `Number_of_atoms` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_xyz` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
        
    
  - `libuniverse::Universe` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)


- `liblibra::libhamiltonian::libhamiltonian_atomistic::libhamiltonian_qm`
  - `listHamiltonian_QM`
    - `compute_scf` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_electronic_structure` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `basis_ao` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `atom_to_ao_map` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)


  - `Electronic_Structure`
    - `Nelec` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `Norb` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_bands_alp` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_bands_bet` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_occ_alp` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_occ_bet` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)


- `liblibra::librandom`
  - `Random`
    - `normal` [7.2.](7_special_functions/2_gaussian_kernel_algorithm/tutorial.ipynb)

- `libra_py`
  - `data_savers`
    - `hdf5_saver`
      - `set_compression_level` [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb)
      - `add_dataset` [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb)
      - `save_matrix` [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb)
      - `hdf5_saver` [8.1.](8_model_hamiltonians/1_pes_plotting/tutorial.ipynb)

