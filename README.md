# AnisotropicBirefringence_patches
Results found in Bortolami et al. (2022).

Here we publish the data Cosmic Birefringence (CB) angle maps and spectra.

The CB maps can be found in the folder CB_maps. The names of the files follow the structure `CB_map_<RELEASE>_<COMPSEP>.fits`, where:
* `<RELEASE>` = PR3, NPIPE
* `<COMPSEP>` = commander, nilc, sevem, smica

The CB maps can be read with the healpy routine `healpy.fitsfunc.read_map`. The loaded array will have the CB angle values and standard deviation in the first and second column, respectively.

The CB spectra in terms of bandpowers can be found in the folder CB_spectra. The names of the files follow the structure `a<X>_<RELEASE>_spectra_data_<COMPSEP>.fits`, where:
* `<X>` = a, T, E, B
* `<RELEASE>` = PR3, NPIPE
* `<COMPSEP>` = commander, nilc, sevem, smica

The CB spectra can be read with the healpy routine `healpy.fitsfunc.read_cl`. The loaded array will have the multipoles, spectra value and error in the first, second and thirs column, respectively.
