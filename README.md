# IceCubeRucioSync
IceCube rucio sync scripts


To use the script you need:

1. A valid proxy with an IceCube VOMS extension
1. And the rucio client configuration pointing at $RUCIO_HOME/etc/rucio.cfg

The script have several modes of operation see --help for details

For a common use case registering the files of dataset `/IceCube/2016/filtered/level2pass2/0104/Run00127357_13` in container `testRucioEdgar1`

 X509_USER_PROXY=/opt/rucio/etc/web/x509up python IceCubeSyncSite.py --container testRucioEdgar1 --dataset /IceCube/2016/filtered/level2pass2/0104/Run00127357_13