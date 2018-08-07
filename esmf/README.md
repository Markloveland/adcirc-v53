Instructions to build esmf
# 1. Copy tar file into a directory on lonestar
# 2. Extract with tar -xvf filename
# 3. Create directory "install" on same level as esmf directory
# 4. export following variables(must be done inside of esmf directory):
export ESMF_ABI=64
export ESMF_BOPT=g
export ESMF_COMM=mpich2
export ESMF_COMPILER=intel
export ESMF_DIR=${PWD}
export ESMF_INSTALL_PREFIX=${PWD}/../install
export ESMF_NETCDF=split
export ESMF_NETCDF_INCLUDE=$TACC_NETCDF_INC
export ESMF_NETCDF_LIBPATH=$TACC_NETCDF_LIB
export ESMF_OS=Linux
# 5. type make all while inside of esmf directory

