## Schrödinger Public Binding Free Energy Benchmark

Data in this folder is sourced from [https://github.com/schrodinger/public_binding_free_energy_benchmark](https://github.com/schrodinger/public_binding_free_energy_benchmark).

The [license](LICENSE.md) file pertains to all files in this subdirectory.

The organization of files is slightly different, and the following minor structure modifications have been made where data quality issues were detected:

- JAK1 (Charge Annhil): The protein structure was identified to have an issue in that HIS 885 of the original protein structure was found to have 2 alternative geometries of approximately equal populations, the first instance of which was retained. This amino acid is approximately 11 Angstroms from the closest ligand, well outside the typical cut-out region of 5 Angstroms, and thus will not impact the result for QC Score for typical cut-out sizes.
  - [Original Structure](https://github.com/schrodinger/public_binding_free_energy_benchmark/blob/main/fep_benchmark_inputs/structure_inputs/charge_annhil/jak1_protein.pdb)
- JAK2 (Set 1 - Fragments): For this dataset we also identify a minor data issue with the protein. Alternative geometries were present for VAL 916, CYS 917, CYS  961, ILE  982, ARG  1117.  In each instance the dominant geometry was retained. All are far removed from the binding site, with the exception of ILE 982, the side chain of which in both variants was pointed away from the ligand binding site.
  - [Original Structure](https://github.com/schrodinger/public_binding_free_energy_benchmark/blob/main/fep_benchmark_inputs/structure_inputs/fragments/jak2_set1_protein.pdb) 

