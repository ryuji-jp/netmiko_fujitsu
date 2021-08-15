# できること
* netmikoで富士通機器が利用できるようになる。

# 前提
* python3 がインストール済み
* コマンドプロンプトでgitコマンドが使える(コマンドプロンプトでgit --versionがたたける)

# 使い方
* ```\netmiko-develop```配下で以下を実行  
```py -m pip install -r requirements.txt```  
```py setup.py install```

# 実行ログ
```
C:\Work\python_contest\netmiko-develop>py -m pip install -r requirements.txt
Looking in indexes: https://pypi.python.org/simple/
Obtaining file:///C:/Work/python_contest/netmiko-develop (from -r requirements.txt (line 3))
Requirement already satisfied: setuptools>=38.4.0 in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from netmiko==4.0.0a4->-r requirements.txt (line 3)) (47.1.0)
Requirement already satisfied: paramiko>=2.6.0 in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from netmiko==4.0.0a4->-r requirements.txt (line 3)) (2.7.2)
Requirement already satisfied: scp>=0.13.2 in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from netmiko==4.0.0a4->-r requirements.txt (line 3)) (0.13.2)
Requirement already satisfied: tenacity in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from netmiko==4.0.0a4->-r requirements.txt (line 3)) (6.2.0)
Requirement already satisfied: textfsm>=1.1.2 in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from netmiko==4.0.0a4->-r requirements.txt (line 3)) (1.1.2)
Requirement already satisfied: ntc-templates>=2.0.0 in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from netmiko==4.0.0a4->-r requirements.txt (line 3)) (2.2.0)
Requirement already satisfied: pyserial in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from netmiko==4.0.0a4->-r requirements.txt (line 3)) (3.4)
Requirement already satisfied: bcrypt>=3.1.3 in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from paramiko>=2.6.0->netmiko==4.0.0a4->-r requirements.txt (line 3)) (3.2.0)
Requirement already satisfied: cryptography>=2.5 in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from paramiko>=2.6.0->netmiko==4.0.0a4->-r requirements.txt (line 3)) (3.1.1)
Requirement already satisfied: pynacl>=1.0.1 in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from paramiko>=2.6.0->netmiko==4.0.0a4->-r requirements.txt (line 3)) (1.4.0)
Requirement already satisfied: cffi>=1.1 in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from bcrypt>=3.1.3->paramiko>=2.6.0->netmiko==4.0.0a4->-r requirements.txt (line 3)) (1.14.3)
Requirement already satisfied: six>=1.4.1 in c:\users\ryuji\appdata\roaming\python\python37\site-packages (from bcrypt>=3.1.3->paramiko>=2.6.0->netmiko==4.0.0a4->-r requirements.txt (line 3)) (1.15.0)
Requirement already satisfied: pycparser in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from cffi>=1.1->bcrypt>=3.1.3->paramiko>=2.6.0->netmiko==4.0.0a4->-r requirements.txt (line 3)) (2.20)
Requirement already satisfied: future in c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages (from textfsm>=1.1.2->netmiko==4.0.0a4->-r requirements.txt (line 3)) (0.18.2)
Installing collected packages: netmiko
  Attempting uninstall: netmiko
    Found existing installation: netmiko 2.3.3
    Uninstalling netmiko-2.3.3:
      Successfully uninstalled netmiko-2.3.3
  Running setup.py develop for netmiko
Successfully installed netmiko

C:\Work\python_contest\netmiko-develop>
C:\Work\python_contest\netmiko-develop>
C:\Work\python_contest\netmiko-develop>
C:\Work\python_contest\netmiko-develop>
C:\Work\python_contest\netmiko-develop>ls
COMMON_ISSUES.md  README.md    docs                      mypy_status.txt       requirements-genie.txt  test.log
EXAMPLES.md       TESTING.md   examples                  netmiko               requirements-ttp.txt    tests
LICENSE           VENDOR.md    examples_old              netmiko.egg-info      requirements.txt        tests.sh
MANIFEST.in       _config.yml  images                    release_process.txt   setup.cfg
PLATFORMS.md      _release.sh  license-dependencies.txt  requirements-dev.txt  setup.py

C:\Work\python_contest\netmiko-develop>py setup.py install
running install
running bdist_egg
running egg_info
writing netmiko.egg-info\PKG-INFO
writing dependency_links to netmiko.egg-info\dependency_links.txt
writing entry points to netmiko.egg-info\entry_points.txt
writing requirements to netmiko.egg-info\requires.txt
writing top-level names to netmiko.egg-info\top_level.txt
reading manifest file 'netmiko.egg-info\SOURCES.txt'
reading manifest template 'MANIFEST.in'
warning: manifest_maker: MANIFEST.in, line 4: path 'tests/' cannot end with '/'

writing manifest file 'netmiko.egg-info\SOURCES.txt'
installing library code to build\bdist.win-amd64\egg
running install_lib
running build_py
creating build
creating build\lib
creating build\lib\netmiko
copying netmiko\base_connection.py -> build\lib\netmiko
copying netmiko\channel.py -> build\lib\netmiko
copying netmiko\cisco_base_connection.py -> build\lib\netmiko
copying netmiko\exceptions.py -> build\lib\netmiko
copying netmiko\netmiko_globals.py -> build\lib\netmiko
copying netmiko\no_config.py -> build\lib\netmiko
copying netmiko\no_enable.py -> build\lib\netmiko
copying netmiko\scp_functions.py -> build\lib\netmiko
copying netmiko\scp_handler.py -> build\lib\netmiko
copying netmiko\session_log.py -> build\lib\netmiko
copying netmiko\snmp_autodetect.py -> build\lib\netmiko
copying netmiko\ssh_auth.py -> build\lib\netmiko
copying netmiko\ssh_autodetect.py -> build\lib\netmiko
copying netmiko\ssh_dispatcher.py -> build\lib\netmiko
copying netmiko\utilities.py -> build\lib\netmiko
copying netmiko\__init__.py -> build\lib\netmiko
creating build\lib\netmiko\a10
copying netmiko\a10\a10_ssh.py -> build\lib\netmiko\a10
copying netmiko\a10\__init__.py -> build\lib\netmiko\a10
creating build\lib\netmiko\accedian
copying netmiko\accedian\accedian_ssh.py -> build\lib\netmiko\accedian
copying netmiko\accedian\__init__.py -> build\lib\netmiko\accedian
creating build\lib\netmiko\adtran
copying netmiko\adtran\adtran.py -> build\lib\netmiko\adtran
copying netmiko\adtran\__init__.py -> build\lib\netmiko\adtran
creating build\lib\netmiko\alcatel
copying netmiko\alcatel\alcatel_aos_ssh.py -> build\lib\netmiko\alcatel
copying netmiko\alcatel\__init__.py -> build\lib\netmiko\alcatel
creating build\lib\netmiko\allied_telesis
copying netmiko\allied_telesis\allied_telesis_awplus.py -> build\lib\netmiko\allied_telesis
copying netmiko\allied_telesis\__init__.py -> build\lib\netmiko\allied_telesis
creating build\lib\netmiko\apresia
copying netmiko\apresia\apresia_aeos.py -> build\lib\netmiko\apresia
copying netmiko\apresia\__init__.py -> build\lib\netmiko\apresia
creating build\lib\netmiko\arista
copying netmiko\arista\arista.py -> build\lib\netmiko\arista
copying netmiko\arista\__init__.py -> build\lib\netmiko\arista
creating build\lib\netmiko\aruba
copying netmiko\aruba\aruba_ssh.py -> build\lib\netmiko\aruba
copying netmiko\aruba\__init__.py -> build\lib\netmiko\aruba
creating build\lib\netmiko\broadcom
copying netmiko\broadcom\broadcom_icos_ssh.py -> build\lib\netmiko\broadcom
copying netmiko\broadcom\__init__.py -> build\lib\netmiko\broadcom
creating build\lib\netmiko\brocade
copying netmiko\brocade\brocade_fos_ssh.py -> build\lib\netmiko\brocade
copying netmiko\brocade\__init__.py -> build\lib\netmiko\brocade
creating build\lib\netmiko\calix
copying netmiko\calix\calix_b6.py -> build\lib\netmiko\calix
copying netmiko\calix\__init__.py -> build\lib\netmiko\calix
creating build\lib\netmiko\cdot
copying netmiko\cdot\cdot_cros_ssh.py -> build\lib\netmiko\cdot
copying netmiko\cdot\__init__.py -> build\lib\netmiko\cdot
creating build\lib\netmiko\centec
copying netmiko\centec\centec_os.py -> build\lib\netmiko\centec
copying netmiko\centec\__init__.py -> build\lib\netmiko\centec
creating build\lib\netmiko\checkpoint
copying netmiko\checkpoint\checkpoint_gaia_ssh.py -> build\lib\netmiko\checkpoint
copying netmiko\checkpoint\__init__.py -> build\lib\netmiko\checkpoint
creating build\lib\netmiko\ciena
copying netmiko\ciena\ciena_saos.py -> build\lib\netmiko\ciena
copying netmiko\ciena\__init__.py -> build\lib\netmiko\ciena
creating build\lib\netmiko\cisco
copying netmiko\cisco\cisco_asa_ssh.py -> build\lib\netmiko\cisco
copying netmiko\cisco\cisco_ftd_ssh.py -> build\lib\netmiko\cisco
copying netmiko\cisco\cisco_ios.py -> build\lib\netmiko\cisco
copying netmiko\cisco\cisco_nxos_ssh.py -> build\lib\netmiko\cisco
copying netmiko\cisco\cisco_s300.py -> build\lib\netmiko\cisco
copying netmiko\cisco\cisco_tp_tcce.py -> build\lib\netmiko\cisco
copying netmiko\cisco\cisco_viptela.py -> build\lib\netmiko\cisco
copying netmiko\cisco\cisco_wlc_ssh.py -> build\lib\netmiko\cisco
copying netmiko\cisco\cisco_xr.py -> build\lib\netmiko\cisco
copying netmiko\cisco\__init__.py -> build\lib\netmiko\cisco
creating build\lib\netmiko\citrix
copying netmiko\citrix\netscaler_ssh.py -> build\lib\netmiko\citrix
copying netmiko\citrix\__init__.py -> build\lib\netmiko\citrix
creating build\lib\netmiko\cli_tools
copying netmiko\cli_tools\netmiko_cfg.py -> build\lib\netmiko\cli_tools
copying netmiko\cli_tools\netmiko_grep.py -> build\lib\netmiko\cli_tools
copying netmiko\cli_tools\netmiko_show.py -> build\lib\netmiko\cli_tools
copying netmiko\cli_tools\__init__.py -> build\lib\netmiko\cli_tools
creating build\lib\netmiko\cloudgenix
copying netmiko\cloudgenix\cloudgenix_ion.py -> build\lib\netmiko\cloudgenix
copying netmiko\cloudgenix\__init__.py -> build\lib\netmiko\cloudgenix
creating build\lib\netmiko\coriant
copying netmiko\coriant\coriant_ssh.py -> build\lib\netmiko\coriant
copying netmiko\coriant\__init__.py -> build\lib\netmiko\coriant
creating build\lib\netmiko\dell
copying netmiko\dell\dell_dnos6.py -> build\lib\netmiko\dell
copying netmiko\dell\dell_force10_ssh.py -> build\lib\netmiko\dell
copying netmiko\dell\dell_isilon_ssh.py -> build\lib\netmiko\dell
copying netmiko\dell\dell_os10_ssh.py -> build\lib\netmiko\dell
copying netmiko\dell\dell_powerconnect.py -> build\lib\netmiko\dell
copying netmiko\dell\dell_sonic_ssh.py -> build\lib\netmiko\dell
copying netmiko\dell\__init__.py -> build\lib\netmiko\dell
creating build\lib\netmiko\dlink
copying netmiko\dlink\dlink_ds.py -> build\lib\netmiko\dlink
copying netmiko\dlink\__init__.py -> build\lib\netmiko\dlink
creating build\lib\netmiko\eltex
copying netmiko\eltex\eltex_esr_ssh.py -> build\lib\netmiko\eltex
copying netmiko\eltex\eltex_ssh.py -> build\lib\netmiko\eltex
copying netmiko\eltex\__init__.py -> build\lib\netmiko\eltex
creating build\lib\netmiko\endace
copying netmiko\endace\endace_ssh.py -> build\lib\netmiko\endace
copying netmiko\endace\__init__.py -> build\lib\netmiko\endace
creating build\lib\netmiko\enterasys
copying netmiko\enterasys\enterasys_ssh.py -> build\lib\netmiko\enterasys
copying netmiko\enterasys\__init__.py -> build\lib\netmiko\enterasys
creating build\lib\netmiko\ericsson
copying netmiko\ericsson\ericsson_ipos.py -> build\lib\netmiko\ericsson
copying netmiko\ericsson\__init__.py -> build\lib\netmiko\ericsson
creating build\lib\netmiko\extreme
copying netmiko\extreme\extreme_ers_ssh.py -> build\lib\netmiko\extreme
copying netmiko\extreme\extreme_exos.py -> build\lib\netmiko\extreme
copying netmiko\extreme\extreme_netiron.py -> build\lib\netmiko\extreme
copying netmiko\extreme\extreme_nos_ssh.py -> build\lib\netmiko\extreme
copying netmiko\extreme\extreme_slx_ssh.py -> build\lib\netmiko\extreme
copying netmiko\extreme\extreme_vsp_ssh.py -> build\lib\netmiko\extreme
copying netmiko\extreme\extreme_wing_ssh.py -> build\lib\netmiko\extreme
copying netmiko\extreme\__init__.py -> build\lib\netmiko\extreme
creating build\lib\netmiko\f5
copying netmiko\f5\f5_linux_ssh.py -> build\lib\netmiko\f5
copying netmiko\f5\f5_tmsh_ssh.py -> build\lib\netmiko\f5
copying netmiko\f5\__init__.py -> build\lib\netmiko\f5
creating build\lib\netmiko\flexvnf
copying netmiko\flexvnf\flexvnf_ssh.py -> build\lib\netmiko\flexvnf
copying netmiko\flexvnf\__init__.py -> build\lib\netmiko\flexvnf
creating build\lib\netmiko\fortinet
copying netmiko\fortinet\fortinet_ssh.py -> build\lib\netmiko\fortinet
copying netmiko\fortinet\__init__.py -> build\lib\netmiko\fortinet
creating build\lib\netmiko\fujitsu
copying netmiko\fujitsu\fujitsu_ssh.py -> build\lib\netmiko\fujitsu
copying netmiko\fujitsu\__init__.py -> build\lib\netmiko\fujitsu
creating build\lib\netmiko\hp
copying netmiko\hp\hp_comware.py -> build\lib\netmiko\hp
copying netmiko\hp\hp_procurve.py -> build\lib\netmiko\hp
copying netmiko\hp\__init__.py -> build\lib\netmiko\hp
creating build\lib\netmiko\huawei
copying netmiko\huawei\huawei.py -> build\lib\netmiko\huawei
copying netmiko\huawei\huawei_smartax.py -> build\lib\netmiko\huawei
copying netmiko\huawei\__init__.py -> build\lib\netmiko\huawei
creating build\lib\netmiko\ipinfusion
copying netmiko\ipinfusion\ipinfusion_ocnos.py -> build\lib\netmiko\ipinfusion
copying netmiko\ipinfusion\__init__.py -> build\lib\netmiko\ipinfusion
creating build\lib\netmiko\juniper
copying netmiko\juniper\juniper.py -> build\lib\netmiko\juniper
copying netmiko\juniper\juniper_screenos.py -> build\lib\netmiko\juniper
copying netmiko\juniper\__init__.py -> build\lib\netmiko\juniper
creating build\lib\netmiko\keymile
copying netmiko\keymile\keymile_nos_ssh.py -> build\lib\netmiko\keymile
copying netmiko\keymile\keymile_ssh.py -> build\lib\netmiko\keymile
copying netmiko\keymile\__init__.py -> build\lib\netmiko\keymile
creating build\lib\netmiko\linux
copying netmiko\linux\linux_ssh.py -> build\lib\netmiko\linux
copying netmiko\linux\__init__.py -> build\lib\netmiko\linux
creating build\lib\netmiko\mellanox
copying netmiko\mellanox\mellanox_mlnxos_ssh.py -> build\lib\netmiko\mellanox
copying netmiko\mellanox\__init__.py -> build\lib\netmiko\mellanox
creating build\lib\netmiko\mikrotik
copying netmiko\mikrotik\mikrotik_ssh.py -> build\lib\netmiko\mikrotik
copying netmiko\mikrotik\__init__.py -> build\lib\netmiko\mikrotik
creating build\lib\netmiko\mrv
copying netmiko\mrv\mrv_lx.py -> build\lib\netmiko\mrv
copying netmiko\mrv\mrv_ssh.py -> build\lib\netmiko\mrv
copying netmiko\mrv\__init__.py -> build\lib\netmiko\mrv
creating build\lib\netmiko\netapp
copying netmiko\netapp\netapp_cdot_ssh.py -> build\lib\netmiko\netapp
copying netmiko\netapp\__init__.py -> build\lib\netmiko\netapp
creating build\lib\netmiko\netgear
copying netmiko\netgear\netgear_prosafe_ssh.py -> build\lib\netmiko\netgear
copying netmiko\netgear\__init__.py -> build\lib\netmiko\netgear
creating build\lib\netmiko\nokia
copying netmiko\nokia\nokia_sros.py -> build\lib\netmiko\nokia
copying netmiko\nokia\__init__.py -> build\lib\netmiko\nokia
creating build\lib\netmiko\oneaccess
copying netmiko\oneaccess\oneaccess_oneos.py -> build\lib\netmiko\oneaccess
copying netmiko\oneaccess\__init__.py -> build\lib\netmiko\oneaccess
creating build\lib\netmiko\ovs
copying netmiko\ovs\ovs_linux_ssh.py -> build\lib\netmiko\ovs
copying netmiko\ovs\__init__.py -> build\lib\netmiko\ovs
creating build\lib\netmiko\paloalto
copying netmiko\paloalto\paloalto_panos.py -> build\lib\netmiko\paloalto
copying netmiko\paloalto\__init__.py -> build\lib\netmiko\paloalto
creating build\lib\netmiko\pluribus
copying netmiko\pluribus\pluribus_ssh.py -> build\lib\netmiko\pluribus
copying netmiko\pluribus\__init__.py -> build\lib\netmiko\pluribus
creating build\lib\netmiko\quanta
copying netmiko\quanta\quanta_mesh_ssh.py -> build\lib\netmiko\quanta
copying netmiko\quanta\__init__.py -> build\lib\netmiko\quanta
creating build\lib\netmiko\rad
copying netmiko\rad\rad_etx.py -> build\lib\netmiko\rad
copying netmiko\rad\__init__.py -> build\lib\netmiko\rad
creating build\lib\netmiko\raisecom
copying netmiko\raisecom\raisecom_roap.py -> build\lib\netmiko\raisecom
copying netmiko\raisecom\__init__.py -> build\lib\netmiko\raisecom
creating build\lib\netmiko\ruckus
copying netmiko\ruckus\ruckus_fastiron.py -> build\lib\netmiko\ruckus
copying netmiko\ruckus\__init__.py -> build\lib\netmiko\ruckus
creating build\lib\netmiko\ruijie
copying netmiko\ruijie\ruijie_os.py -> build\lib\netmiko\ruijie
copying netmiko\ruijie\__init__.py -> build\lib\netmiko\ruijie
creating build\lib\netmiko\sixwind
copying netmiko\sixwind\sixwind_os.py -> build\lib\netmiko\sixwind
copying netmiko\sixwind\__init__.py -> build\lib\netmiko\sixwind
creating build\lib\netmiko\sophos
copying netmiko\sophos\sophos_sfos_ssh.py -> build\lib\netmiko\sophos
copying netmiko\sophos\__init__.py -> build\lib\netmiko\sophos
creating build\lib\netmiko\supermicro
copying netmiko\supermicro\smci_smis.py -> build\lib\netmiko\supermicro
copying netmiko\supermicro\__init__.py -> build\lib\netmiko\supermicro
creating build\lib\netmiko\terminal_server
copying netmiko\terminal_server\terminal_server.py -> build\lib\netmiko\terminal_server
copying netmiko\terminal_server\__init__.py -> build\lib\netmiko\terminal_server
creating build\lib\netmiko\tplink
copying netmiko\tplink\tplink_jetstream.py -> build\lib\netmiko\tplink
copying netmiko\tplink\__init__.py -> build\lib\netmiko\tplink
creating build\lib\netmiko\ubiquiti
copying netmiko\ubiquiti\edgerouter_ssh.py -> build\lib\netmiko\ubiquiti
copying netmiko\ubiquiti\edge_ssh.py -> build\lib\netmiko\ubiquiti
copying netmiko\ubiquiti\unifiswitch_ssh.py -> build\lib\netmiko\ubiquiti
copying netmiko\ubiquiti\__init__.py -> build\lib\netmiko\ubiquiti
creating build\lib\netmiko\vyos
copying netmiko\vyos\vyos_ssh.py -> build\lib\netmiko\vyos
copying netmiko\vyos\__init__.py -> build\lib\netmiko\vyos
creating build\lib\netmiko\watchguard
copying netmiko\watchguard\fireware_ssh.py -> build\lib\netmiko\watchguard
copying netmiko\watchguard\__init__.py -> build\lib\netmiko\watchguard
creating build\lib\netmiko\yamaha
copying netmiko\yamaha\yamaha.py -> build\lib\netmiko\yamaha
copying netmiko\yamaha\__init__.py -> build\lib\netmiko\yamaha
creating build\lib\netmiko\zte
copying netmiko\zte\zte_zxros.py -> build\lib\netmiko\zte
copying netmiko\zte\__init__.py -> build\lib\netmiko\zte
creating build\bdist.win-amd64
creating build\bdist.win-amd64\egg
creating build\bdist.win-amd64\egg\netmiko
creating build\bdist.win-amd64\egg\netmiko\a10
copying build\lib\netmiko\a10\a10_ssh.py -> build\bdist.win-amd64\egg\netmiko\a10
copying build\lib\netmiko\a10\__init__.py -> build\bdist.win-amd64\egg\netmiko\a10
creating build\bdist.win-amd64\egg\netmiko\accedian
copying build\lib\netmiko\accedian\accedian_ssh.py -> build\bdist.win-amd64\egg\netmiko\accedian
copying build\lib\netmiko\accedian\__init__.py -> build\bdist.win-amd64\egg\netmiko\accedian
creating build\bdist.win-amd64\egg\netmiko\adtran
copying build\lib\netmiko\adtran\adtran.py -> build\bdist.win-amd64\egg\netmiko\adtran
copying build\lib\netmiko\adtran\__init__.py -> build\bdist.win-amd64\egg\netmiko\adtran
creating build\bdist.win-amd64\egg\netmiko\alcatel
copying build\lib\netmiko\alcatel\alcatel_aos_ssh.py -> build\bdist.win-amd64\egg\netmiko\alcatel
copying build\lib\netmiko\alcatel\__init__.py -> build\bdist.win-amd64\egg\netmiko\alcatel
creating build\bdist.win-amd64\egg\netmiko\allied_telesis
copying build\lib\netmiko\allied_telesis\allied_telesis_awplus.py -> build\bdist.win-amd64\egg\netmiko\allied_telesis
copying build\lib\netmiko\allied_telesis\__init__.py -> build\bdist.win-amd64\egg\netmiko\allied_telesis
creating build\bdist.win-amd64\egg\netmiko\apresia
copying build\lib\netmiko\apresia\apresia_aeos.py -> build\bdist.win-amd64\egg\netmiko\apresia
copying build\lib\netmiko\apresia\__init__.py -> build\bdist.win-amd64\egg\netmiko\apresia
creating build\bdist.win-amd64\egg\netmiko\arista
copying build\lib\netmiko\arista\arista.py -> build\bdist.win-amd64\egg\netmiko\arista
copying build\lib\netmiko\arista\__init__.py -> build\bdist.win-amd64\egg\netmiko\arista
creating build\bdist.win-amd64\egg\netmiko\aruba
copying build\lib\netmiko\aruba\aruba_ssh.py -> build\bdist.win-amd64\egg\netmiko\aruba
copying build\lib\netmiko\aruba\__init__.py -> build\bdist.win-amd64\egg\netmiko\aruba
copying build\lib\netmiko\base_connection.py -> build\bdist.win-amd64\egg\netmiko
creating build\bdist.win-amd64\egg\netmiko\broadcom
copying build\lib\netmiko\broadcom\broadcom_icos_ssh.py -> build\bdist.win-amd64\egg\netmiko\broadcom
copying build\lib\netmiko\broadcom\__init__.py -> build\bdist.win-amd64\egg\netmiko\broadcom
creating build\bdist.win-amd64\egg\netmiko\brocade
copying build\lib\netmiko\brocade\brocade_fos_ssh.py -> build\bdist.win-amd64\egg\netmiko\brocade
copying build\lib\netmiko\brocade\__init__.py -> build\bdist.win-amd64\egg\netmiko\brocade
creating build\bdist.win-amd64\egg\netmiko\calix
copying build\lib\netmiko\calix\calix_b6.py -> build\bdist.win-amd64\egg\netmiko\calix
copying build\lib\netmiko\calix\__init__.py -> build\bdist.win-amd64\egg\netmiko\calix
creating build\bdist.win-amd64\egg\netmiko\cdot
copying build\lib\netmiko\cdot\cdot_cros_ssh.py -> build\bdist.win-amd64\egg\netmiko\cdot
copying build\lib\netmiko\cdot\__init__.py -> build\bdist.win-amd64\egg\netmiko\cdot
creating build\bdist.win-amd64\egg\netmiko\centec
copying build\lib\netmiko\centec\centec_os.py -> build\bdist.win-amd64\egg\netmiko\centec
copying build\lib\netmiko\centec\__init__.py -> build\bdist.win-amd64\egg\netmiko\centec
copying build\lib\netmiko\channel.py -> build\bdist.win-amd64\egg\netmiko
creating build\bdist.win-amd64\egg\netmiko\checkpoint
copying build\lib\netmiko\checkpoint\checkpoint_gaia_ssh.py -> build\bdist.win-amd64\egg\netmiko\checkpoint
copying build\lib\netmiko\checkpoint\__init__.py -> build\bdist.win-amd64\egg\netmiko\checkpoint
creating build\bdist.win-amd64\egg\netmiko\ciena
copying build\lib\netmiko\ciena\ciena_saos.py -> build\bdist.win-amd64\egg\netmiko\ciena
copying build\lib\netmiko\ciena\__init__.py -> build\bdist.win-amd64\egg\netmiko\ciena
creating build\bdist.win-amd64\egg\netmiko\cisco
copying build\lib\netmiko\cisco\cisco_asa_ssh.py -> build\bdist.win-amd64\egg\netmiko\cisco
copying build\lib\netmiko\cisco\cisco_ftd_ssh.py -> build\bdist.win-amd64\egg\netmiko\cisco
copying build\lib\netmiko\cisco\cisco_ios.py -> build\bdist.win-amd64\egg\netmiko\cisco
copying build\lib\netmiko\cisco\cisco_nxos_ssh.py -> build\bdist.win-amd64\egg\netmiko\cisco
copying build\lib\netmiko\cisco\cisco_s300.py -> build\bdist.win-amd64\egg\netmiko\cisco
copying build\lib\netmiko\cisco\cisco_tp_tcce.py -> build\bdist.win-amd64\egg\netmiko\cisco
copying build\lib\netmiko\cisco\cisco_viptela.py -> build\bdist.win-amd64\egg\netmiko\cisco
copying build\lib\netmiko\cisco\cisco_wlc_ssh.py -> build\bdist.win-amd64\egg\netmiko\cisco
copying build\lib\netmiko\cisco\cisco_xr.py -> build\bdist.win-amd64\egg\netmiko\cisco
copying build\lib\netmiko\cisco\__init__.py -> build\bdist.win-amd64\egg\netmiko\cisco
copying build\lib\netmiko\cisco_base_connection.py -> build\bdist.win-amd64\egg\netmiko
creating build\bdist.win-amd64\egg\netmiko\citrix
copying build\lib\netmiko\citrix\netscaler_ssh.py -> build\bdist.win-amd64\egg\netmiko\citrix
copying build\lib\netmiko\citrix\__init__.py -> build\bdist.win-amd64\egg\netmiko\citrix
creating build\bdist.win-amd64\egg\netmiko\cli_tools
copying build\lib\netmiko\cli_tools\netmiko_cfg.py -> build\bdist.win-amd64\egg\netmiko\cli_tools
copying build\lib\netmiko\cli_tools\netmiko_grep.py -> build\bdist.win-amd64\egg\netmiko\cli_tools
copying build\lib\netmiko\cli_tools\netmiko_show.py -> build\bdist.win-amd64\egg\netmiko\cli_tools
copying build\lib\netmiko\cli_tools\__init__.py -> build\bdist.win-amd64\egg\netmiko\cli_tools
creating build\bdist.win-amd64\egg\netmiko\cloudgenix
copying build\lib\netmiko\cloudgenix\cloudgenix_ion.py -> build\bdist.win-amd64\egg\netmiko\cloudgenix
copying build\lib\netmiko\cloudgenix\__init__.py -> build\bdist.win-amd64\egg\netmiko\cloudgenix
creating build\bdist.win-amd64\egg\netmiko\coriant
copying build\lib\netmiko\coriant\coriant_ssh.py -> build\bdist.win-amd64\egg\netmiko\coriant
copying build\lib\netmiko\coriant\__init__.py -> build\bdist.win-amd64\egg\netmiko\coriant
creating build\bdist.win-amd64\egg\netmiko\dell
copying build\lib\netmiko\dell\dell_dnos6.py -> build\bdist.win-amd64\egg\netmiko\dell
copying build\lib\netmiko\dell\dell_force10_ssh.py -> build\bdist.win-amd64\egg\netmiko\dell
copying build\lib\netmiko\dell\dell_isilon_ssh.py -> build\bdist.win-amd64\egg\netmiko\dell
copying build\lib\netmiko\dell\dell_os10_ssh.py -> build\bdist.win-amd64\egg\netmiko\dell
copying build\lib\netmiko\dell\dell_powerconnect.py -> build\bdist.win-amd64\egg\netmiko\dell
copying build\lib\netmiko\dell\dell_sonic_ssh.py -> build\bdist.win-amd64\egg\netmiko\dell
copying build\lib\netmiko\dell\__init__.py -> build\bdist.win-amd64\egg\netmiko\dell
creating build\bdist.win-amd64\egg\netmiko\dlink
copying build\lib\netmiko\dlink\dlink_ds.py -> build\bdist.win-amd64\egg\netmiko\dlink
copying build\lib\netmiko\dlink\__init__.py -> build\bdist.win-amd64\egg\netmiko\dlink
creating build\bdist.win-amd64\egg\netmiko\eltex
copying build\lib\netmiko\eltex\eltex_esr_ssh.py -> build\bdist.win-amd64\egg\netmiko\eltex
copying build\lib\netmiko\eltex\eltex_ssh.py -> build\bdist.win-amd64\egg\netmiko\eltex
copying build\lib\netmiko\eltex\__init__.py -> build\bdist.win-amd64\egg\netmiko\eltex
creating build\bdist.win-amd64\egg\netmiko\endace
copying build\lib\netmiko\endace\endace_ssh.py -> build\bdist.win-amd64\egg\netmiko\endace
copying build\lib\netmiko\endace\__init__.py -> build\bdist.win-amd64\egg\netmiko\endace
creating build\bdist.win-amd64\egg\netmiko\enterasys
copying build\lib\netmiko\enterasys\enterasys_ssh.py -> build\bdist.win-amd64\egg\netmiko\enterasys
copying build\lib\netmiko\enterasys\__init__.py -> build\bdist.win-amd64\egg\netmiko\enterasys
creating build\bdist.win-amd64\egg\netmiko\ericsson
copying build\lib\netmiko\ericsson\ericsson_ipos.py -> build\bdist.win-amd64\egg\netmiko\ericsson
copying build\lib\netmiko\ericsson\__init__.py -> build\bdist.win-amd64\egg\netmiko\ericsson
copying build\lib\netmiko\exceptions.py -> build\bdist.win-amd64\egg\netmiko
creating build\bdist.win-amd64\egg\netmiko\extreme
copying build\lib\netmiko\extreme\extreme_ers_ssh.py -> build\bdist.win-amd64\egg\netmiko\extreme
copying build\lib\netmiko\extreme\extreme_exos.py -> build\bdist.win-amd64\egg\netmiko\extreme
copying build\lib\netmiko\extreme\extreme_netiron.py -> build\bdist.win-amd64\egg\netmiko\extreme
copying build\lib\netmiko\extreme\extreme_nos_ssh.py -> build\bdist.win-amd64\egg\netmiko\extreme
copying build\lib\netmiko\extreme\extreme_slx_ssh.py -> build\bdist.win-amd64\egg\netmiko\extreme
copying build\lib\netmiko\extreme\extreme_vsp_ssh.py -> build\bdist.win-amd64\egg\netmiko\extreme
copying build\lib\netmiko\extreme\extreme_wing_ssh.py -> build\bdist.win-amd64\egg\netmiko\extreme
copying build\lib\netmiko\extreme\__init__.py -> build\bdist.win-amd64\egg\netmiko\extreme
creating build\bdist.win-amd64\egg\netmiko\f5
copying build\lib\netmiko\f5\f5_linux_ssh.py -> build\bdist.win-amd64\egg\netmiko\f5
copying build\lib\netmiko\f5\f5_tmsh_ssh.py -> build\bdist.win-amd64\egg\netmiko\f5
copying build\lib\netmiko\f5\__init__.py -> build\bdist.win-amd64\egg\netmiko\f5
creating build\bdist.win-amd64\egg\netmiko\flexvnf
copying build\lib\netmiko\flexvnf\flexvnf_ssh.py -> build\bdist.win-amd64\egg\netmiko\flexvnf
copying build\lib\netmiko\flexvnf\__init__.py -> build\bdist.win-amd64\egg\netmiko\flexvnf
creating build\bdist.win-amd64\egg\netmiko\fortinet
copying build\lib\netmiko\fortinet\fortinet_ssh.py -> build\bdist.win-amd64\egg\netmiko\fortinet
copying build\lib\netmiko\fortinet\__init__.py -> build\bdist.win-amd64\egg\netmiko\fortinet
creating build\bdist.win-amd64\egg\netmiko\fujitsu
copying build\lib\netmiko\fujitsu\fujitsu_ssh.py -> build\bdist.win-amd64\egg\netmiko\fujitsu
copying build\lib\netmiko\fujitsu\__init__.py -> build\bdist.win-amd64\egg\netmiko\fujitsu
creating build\bdist.win-amd64\egg\netmiko\hp
copying build\lib\netmiko\hp\hp_comware.py -> build\bdist.win-amd64\egg\netmiko\hp
copying build\lib\netmiko\hp\hp_procurve.py -> build\bdist.win-amd64\egg\netmiko\hp
copying build\lib\netmiko\hp\__init__.py -> build\bdist.win-amd64\egg\netmiko\hp
creating build\bdist.win-amd64\egg\netmiko\huawei
copying build\lib\netmiko\huawei\huawei.py -> build\bdist.win-amd64\egg\netmiko\huawei
copying build\lib\netmiko\huawei\huawei_smartax.py -> build\bdist.win-amd64\egg\netmiko\huawei
copying build\lib\netmiko\huawei\__init__.py -> build\bdist.win-amd64\egg\netmiko\huawei
creating build\bdist.win-amd64\egg\netmiko\ipinfusion
copying build\lib\netmiko\ipinfusion\ipinfusion_ocnos.py -> build\bdist.win-amd64\egg\netmiko\ipinfusion
copying build\lib\netmiko\ipinfusion\__init__.py -> build\bdist.win-amd64\egg\netmiko\ipinfusion
creating build\bdist.win-amd64\egg\netmiko\juniper
copying build\lib\netmiko\juniper\juniper.py -> build\bdist.win-amd64\egg\netmiko\juniper
copying build\lib\netmiko\juniper\juniper_screenos.py -> build\bdist.win-amd64\egg\netmiko\juniper
copying build\lib\netmiko\juniper\__init__.py -> build\bdist.win-amd64\egg\netmiko\juniper
creating build\bdist.win-amd64\egg\netmiko\keymile
copying build\lib\netmiko\keymile\keymile_nos_ssh.py -> build\bdist.win-amd64\egg\netmiko\keymile
copying build\lib\netmiko\keymile\keymile_ssh.py -> build\bdist.win-amd64\egg\netmiko\keymile
copying build\lib\netmiko\keymile\__init__.py -> build\bdist.win-amd64\egg\netmiko\keymile
creating build\bdist.win-amd64\egg\netmiko\linux
copying build\lib\netmiko\linux\linux_ssh.py -> build\bdist.win-amd64\egg\netmiko\linux
copying build\lib\netmiko\linux\__init__.py -> build\bdist.win-amd64\egg\netmiko\linux
creating build\bdist.win-amd64\egg\netmiko\mellanox
copying build\lib\netmiko\mellanox\mellanox_mlnxos_ssh.py -> build\bdist.win-amd64\egg\netmiko\mellanox
copying build\lib\netmiko\mellanox\__init__.py -> build\bdist.win-amd64\egg\netmiko\mellanox
creating build\bdist.win-amd64\egg\netmiko\mikrotik
copying build\lib\netmiko\mikrotik\mikrotik_ssh.py -> build\bdist.win-amd64\egg\netmiko\mikrotik
copying build\lib\netmiko\mikrotik\__init__.py -> build\bdist.win-amd64\egg\netmiko\mikrotik
creating build\bdist.win-amd64\egg\netmiko\mrv
copying build\lib\netmiko\mrv\mrv_lx.py -> build\bdist.win-amd64\egg\netmiko\mrv
copying build\lib\netmiko\mrv\mrv_ssh.py -> build\bdist.win-amd64\egg\netmiko\mrv
copying build\lib\netmiko\mrv\__init__.py -> build\bdist.win-amd64\egg\netmiko\mrv
creating build\bdist.win-amd64\egg\netmiko\netapp
copying build\lib\netmiko\netapp\netapp_cdot_ssh.py -> build\bdist.win-amd64\egg\netmiko\netapp
copying build\lib\netmiko\netapp\__init__.py -> build\bdist.win-amd64\egg\netmiko\netapp
creating build\bdist.win-amd64\egg\netmiko\netgear
copying build\lib\netmiko\netgear\netgear_prosafe_ssh.py -> build\bdist.win-amd64\egg\netmiko\netgear
copying build\lib\netmiko\netgear\__init__.py -> build\bdist.win-amd64\egg\netmiko\netgear
copying build\lib\netmiko\netmiko_globals.py -> build\bdist.win-amd64\egg\netmiko
creating build\bdist.win-amd64\egg\netmiko\nokia
copying build\lib\netmiko\nokia\nokia_sros.py -> build\bdist.win-amd64\egg\netmiko\nokia
copying build\lib\netmiko\nokia\__init__.py -> build\bdist.win-amd64\egg\netmiko\nokia
copying build\lib\netmiko\no_config.py -> build\bdist.win-amd64\egg\netmiko
copying build\lib\netmiko\no_enable.py -> build\bdist.win-amd64\egg\netmiko
creating build\bdist.win-amd64\egg\netmiko\oneaccess
copying build\lib\netmiko\oneaccess\oneaccess_oneos.py -> build\bdist.win-amd64\egg\netmiko\oneaccess
copying build\lib\netmiko\oneaccess\__init__.py -> build\bdist.win-amd64\egg\netmiko\oneaccess
creating build\bdist.win-amd64\egg\netmiko\ovs
copying build\lib\netmiko\ovs\ovs_linux_ssh.py -> build\bdist.win-amd64\egg\netmiko\ovs
copying build\lib\netmiko\ovs\__init__.py -> build\bdist.win-amd64\egg\netmiko\ovs
creating build\bdist.win-amd64\egg\netmiko\paloalto
copying build\lib\netmiko\paloalto\paloalto_panos.py -> build\bdist.win-amd64\egg\netmiko\paloalto
copying build\lib\netmiko\paloalto\__init__.py -> build\bdist.win-amd64\egg\netmiko\paloalto
creating build\bdist.win-amd64\egg\netmiko\pluribus
copying build\lib\netmiko\pluribus\pluribus_ssh.py -> build\bdist.win-amd64\egg\netmiko\pluribus
copying build\lib\netmiko\pluribus\__init__.py -> build\bdist.win-amd64\egg\netmiko\pluribus
creating build\bdist.win-amd64\egg\netmiko\quanta
copying build\lib\netmiko\quanta\quanta_mesh_ssh.py -> build\bdist.win-amd64\egg\netmiko\quanta
copying build\lib\netmiko\quanta\__init__.py -> build\bdist.win-amd64\egg\netmiko\quanta
creating build\bdist.win-amd64\egg\netmiko\rad
copying build\lib\netmiko\rad\rad_etx.py -> build\bdist.win-amd64\egg\netmiko\rad
copying build\lib\netmiko\rad\__init__.py -> build\bdist.win-amd64\egg\netmiko\rad
creating build\bdist.win-amd64\egg\netmiko\raisecom
copying build\lib\netmiko\raisecom\raisecom_roap.py -> build\bdist.win-amd64\egg\netmiko\raisecom
copying build\lib\netmiko\raisecom\__init__.py -> build\bdist.win-amd64\egg\netmiko\raisecom
creating build\bdist.win-amd64\egg\netmiko\ruckus
copying build\lib\netmiko\ruckus\ruckus_fastiron.py -> build\bdist.win-amd64\egg\netmiko\ruckus
copying build\lib\netmiko\ruckus\__init__.py -> build\bdist.win-amd64\egg\netmiko\ruckus
creating build\bdist.win-amd64\egg\netmiko\ruijie
copying build\lib\netmiko\ruijie\ruijie_os.py -> build\bdist.win-amd64\egg\netmiko\ruijie
copying build\lib\netmiko\ruijie\__init__.py -> build\bdist.win-amd64\egg\netmiko\ruijie
copying build\lib\netmiko\scp_functions.py -> build\bdist.win-amd64\egg\netmiko
copying build\lib\netmiko\scp_handler.py -> build\bdist.win-amd64\egg\netmiko
copying build\lib\netmiko\session_log.py -> build\bdist.win-amd64\egg\netmiko
creating build\bdist.win-amd64\egg\netmiko\sixwind
copying build\lib\netmiko\sixwind\sixwind_os.py -> build\bdist.win-amd64\egg\netmiko\sixwind
copying build\lib\netmiko\sixwind\__init__.py -> build\bdist.win-amd64\egg\netmiko\sixwind
copying build\lib\netmiko\snmp_autodetect.py -> build\bdist.win-amd64\egg\netmiko
creating build\bdist.win-amd64\egg\netmiko\sophos
copying build\lib\netmiko\sophos\sophos_sfos_ssh.py -> build\bdist.win-amd64\egg\netmiko\sophos
copying build\lib\netmiko\sophos\__init__.py -> build\bdist.win-amd64\egg\netmiko\sophos
copying build\lib\netmiko\ssh_auth.py -> build\bdist.win-amd64\egg\netmiko
copying build\lib\netmiko\ssh_autodetect.py -> build\bdist.win-amd64\egg\netmiko
copying build\lib\netmiko\ssh_dispatcher.py -> build\bdist.win-amd64\egg\netmiko
creating build\bdist.win-amd64\egg\netmiko\supermicro
copying build\lib\netmiko\supermicro\smci_smis.py -> build\bdist.win-amd64\egg\netmiko\supermicro
copying build\lib\netmiko\supermicro\__init__.py -> build\bdist.win-amd64\egg\netmiko\supermicro
creating build\bdist.win-amd64\egg\netmiko\terminal_server
copying build\lib\netmiko\terminal_server\terminal_server.py -> build\bdist.win-amd64\egg\netmiko\terminal_server
copying build\lib\netmiko\terminal_server\__init__.py -> build\bdist.win-amd64\egg\netmiko\terminal_server
creating build\bdist.win-amd64\egg\netmiko\tplink
copying build\lib\netmiko\tplink\tplink_jetstream.py -> build\bdist.win-amd64\egg\netmiko\tplink
copying build\lib\netmiko\tplink\__init__.py -> build\bdist.win-amd64\egg\netmiko\tplink
creating build\bdist.win-amd64\egg\netmiko\ubiquiti
copying build\lib\netmiko\ubiquiti\edgerouter_ssh.py -> build\bdist.win-amd64\egg\netmiko\ubiquiti
copying build\lib\netmiko\ubiquiti\edge_ssh.py -> build\bdist.win-amd64\egg\netmiko\ubiquiti
copying build\lib\netmiko\ubiquiti\unifiswitch_ssh.py -> build\bdist.win-amd64\egg\netmiko\ubiquiti
copying build\lib\netmiko\ubiquiti\__init__.py -> build\bdist.win-amd64\egg\netmiko\ubiquiti
copying build\lib\netmiko\utilities.py -> build\bdist.win-amd64\egg\netmiko
creating build\bdist.win-amd64\egg\netmiko\vyos
copying build\lib\netmiko\vyos\vyos_ssh.py -> build\bdist.win-amd64\egg\netmiko\vyos
copying build\lib\netmiko\vyos\__init__.py -> build\bdist.win-amd64\egg\netmiko\vyos
creating build\bdist.win-amd64\egg\netmiko\watchguard
copying build\lib\netmiko\watchguard\fireware_ssh.py -> build\bdist.win-amd64\egg\netmiko\watchguard
copying build\lib\netmiko\watchguard\__init__.py -> build\bdist.win-amd64\egg\netmiko\watchguard
creating build\bdist.win-amd64\egg\netmiko\yamaha
copying build\lib\netmiko\yamaha\yamaha.py -> build\bdist.win-amd64\egg\netmiko\yamaha
copying build\lib\netmiko\yamaha\__init__.py -> build\bdist.win-amd64\egg\netmiko\yamaha
creating build\bdist.win-amd64\egg\netmiko\zte
copying build\lib\netmiko\zte\zte_zxros.py -> build\bdist.win-amd64\egg\netmiko\zte
copying build\lib\netmiko\zte\__init__.py -> build\bdist.win-amd64\egg\netmiko\zte
copying build\lib\netmiko\__init__.py -> build\bdist.win-amd64\egg\netmiko
byte-compiling build\bdist.win-amd64\egg\netmiko\a10\a10_ssh.py to a10_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\a10\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\accedian\accedian_ssh.py to accedian_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\accedian\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\adtran\adtran.py to adtran.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\adtran\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\alcatel\alcatel_aos_ssh.py to alcatel_aos_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\alcatel\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\allied_telesis\allied_telesis_awplus.py to allied_telesis_awplus.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\allied_telesis\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\apresia\apresia_aeos.py to apresia_aeos.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\apresia\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\arista\arista.py to arista.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\arista\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\aruba\aruba_ssh.py to aruba_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\aruba\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\base_connection.py to base_connection.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\broadcom\broadcom_icos_ssh.py to broadcom_icos_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\broadcom\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\brocade\brocade_fos_ssh.py to brocade_fos_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\brocade\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\calix\calix_b6.py to calix_b6.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\calix\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cdot\cdot_cros_ssh.py to cdot_cros_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cdot\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\centec\centec_os.py to centec_os.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\centec\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\channel.py to channel.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\checkpoint\checkpoint_gaia_ssh.py to checkpoint_gaia_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\checkpoint\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ciena\ciena_saos.py to ciena_saos.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ciena\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cisco\cisco_asa_ssh.py to cisco_asa_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cisco\cisco_ftd_ssh.py to cisco_ftd_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cisco\cisco_ios.py to cisco_ios.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cisco\cisco_nxos_ssh.py to cisco_nxos_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cisco\cisco_s300.py to cisco_s300.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cisco\cisco_tp_tcce.py to cisco_tp_tcce.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cisco\cisco_viptela.py to cisco_viptela.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cisco\cisco_wlc_ssh.py to cisco_wlc_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cisco\cisco_xr.py to cisco_xr.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cisco\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cisco_base_connection.py to cisco_base_connection.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\citrix\netscaler_ssh.py to netscaler_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\citrix\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cli_tools\netmiko_cfg.py to netmiko_cfg.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cli_tools\netmiko_grep.py to netmiko_grep.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cli_tools\netmiko_show.py to netmiko_show.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cli_tools\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cloudgenix\cloudgenix_ion.py to cloudgenix_ion.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\cloudgenix\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\coriant\coriant_ssh.py to coriant_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\coriant\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\dell\dell_dnos6.py to dell_dnos6.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\dell\dell_force10_ssh.py to dell_force10_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\dell\dell_isilon_ssh.py to dell_isilon_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\dell\dell_os10_ssh.py to dell_os10_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\dell\dell_powerconnect.py to dell_powerconnect.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\dell\dell_sonic_ssh.py to dell_sonic_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\dell\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\dlink\dlink_ds.py to dlink_ds.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\dlink\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\eltex\eltex_esr_ssh.py to eltex_esr_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\eltex\eltex_ssh.py to eltex_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\eltex\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\endace\endace_ssh.py to endace_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\endace\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\enterasys\enterasys_ssh.py to enterasys_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\enterasys\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ericsson\ericsson_ipos.py to ericsson_ipos.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ericsson\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\exceptions.py to exceptions.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\extreme\extreme_ers_ssh.py to extreme_ers_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\extreme\extreme_exos.py to extreme_exos.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\extreme\extreme_netiron.py to extreme_netiron.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\extreme\extreme_nos_ssh.py to extreme_nos_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\extreme\extreme_slx_ssh.py to extreme_slx_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\extreme\extreme_vsp_ssh.py to extreme_vsp_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\extreme\extreme_wing_ssh.py to extreme_wing_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\extreme\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\f5\f5_linux_ssh.py to f5_linux_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\f5\f5_tmsh_ssh.py to f5_tmsh_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\f5\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\flexvnf\flexvnf_ssh.py to flexvnf_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\flexvnf\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\fortinet\fortinet_ssh.py to fortinet_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\fortinet\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\fujitsu\fujitsu_ssh.py to fujitsu_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\fujitsu\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\hp\hp_comware.py to hp_comware.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\hp\hp_procurve.py to hp_procurve.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\hp\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\huawei\huawei.py to huawei.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\huawei\huawei_smartax.py to huawei_smartax.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\huawei\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ipinfusion\ipinfusion_ocnos.py to ipinfusion_ocnos.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ipinfusion\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\juniper\juniper.py to juniper.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\juniper\juniper_screenos.py to juniper_screenos.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\juniper\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\keymile\keymile_nos_ssh.py to keymile_nos_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\keymile\keymile_ssh.py to keymile_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\keymile\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\linux\linux_ssh.py to linux_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\linux\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\mellanox\mellanox_mlnxos_ssh.py to mellanox_mlnxos_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\mellanox\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\mikrotik\mikrotik_ssh.py to mikrotik_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\mikrotik\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\mrv\mrv_lx.py to mrv_lx.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\mrv\mrv_ssh.py to mrv_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\mrv\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\netapp\netapp_cdot_ssh.py to netapp_cdot_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\netapp\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\netgear\netgear_prosafe_ssh.py to netgear_prosafe_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\netgear\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\netmiko_globals.py to netmiko_globals.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\nokia\nokia_sros.py to nokia_sros.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\nokia\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\no_config.py to no_config.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\no_enable.py to no_enable.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\oneaccess\oneaccess_oneos.py to oneaccess_oneos.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\oneaccess\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ovs\ovs_linux_ssh.py to ovs_linux_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ovs\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\paloalto\paloalto_panos.py to paloalto_panos.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\paloalto\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\pluribus\pluribus_ssh.py to pluribus_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\pluribus\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\quanta\quanta_mesh_ssh.py to quanta_mesh_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\quanta\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\rad\rad_etx.py to rad_etx.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\rad\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\raisecom\raisecom_roap.py to raisecom_roap.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\raisecom\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ruckus\ruckus_fastiron.py to ruckus_fastiron.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ruckus\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ruijie\ruijie_os.py to ruijie_os.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ruijie\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\scp_functions.py to scp_functions.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\scp_handler.py to scp_handler.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\session_log.py to session_log.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\sixwind\sixwind_os.py to sixwind_os.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\sixwind\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\snmp_autodetect.py to snmp_autodetect.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\sophos\sophos_sfos_ssh.py to sophos_sfos_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\sophos\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ssh_auth.py to ssh_auth.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ssh_autodetect.py to ssh_autodetect.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ssh_dispatcher.py to ssh_dispatcher.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\supermicro\smci_smis.py to smci_smis.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\supermicro\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\terminal_server\terminal_server.py to terminal_server.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\terminal_server\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\tplink\tplink_jetstream.py to tplink_jetstream.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\tplink\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ubiquiti\edgerouter_ssh.py to edgerouter_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ubiquiti\edge_ssh.py to edge_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ubiquiti\unifiswitch_ssh.py to unifiswitch_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\ubiquiti\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\utilities.py to utilities.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\vyos\vyos_ssh.py to vyos_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\vyos\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\watchguard\fireware_ssh.py to fireware_ssh.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\watchguard\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\yamaha\yamaha.py to yamaha.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\yamaha\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\zte\zte_zxros.py to zte_zxros.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\zte\__init__.py to __init__.cpython-37.pyc
byte-compiling build\bdist.win-amd64\egg\netmiko\__init__.py to __init__.cpython-37.pyc
creating build\bdist.win-amd64\egg\EGG-INFO
copying netmiko.egg-info\PKG-INFO -> build\bdist.win-amd64\egg\EGG-INFO
copying netmiko.egg-info\SOURCES.txt -> build\bdist.win-amd64\egg\EGG-INFO
copying netmiko.egg-info\dependency_links.txt -> build\bdist.win-amd64\egg\EGG-INFO
copying netmiko.egg-info\entry_points.txt -> build\bdist.win-amd64\egg\EGG-INFO
copying netmiko.egg-info\requires.txt -> build\bdist.win-amd64\egg\EGG-INFO
copying netmiko.egg-info\top_level.txt -> build\bdist.win-amd64\egg\EGG-INFO
zip_safe flag not set; analyzing archive contents...
creating dist
creating 'dist\netmiko-4.0.0a4-py3.7.egg' and adding 'build\bdist.win-amd64\egg' to it
removing 'build\bdist.win-amd64\egg' (and everything under it)
Processing netmiko-4.0.0a4-py3.7.egg
Copying netmiko-4.0.0a4-py3.7.egg to c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Removing netmiko 4.0.0a4 from easy-install.pth file
Adding netmiko 4.0.0a4 to easy-install.pth file
Installing netmiko-cfg-script.py script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing netmiko-cfg.exe script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing netmiko-grep-script.py script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing netmiko-grep.exe script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing netmiko-show-script.py script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing netmiko-show.exe script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts

Installed c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages\netmiko-4.0.0a4-py3.7.egg
Processing dependencies for netmiko==4.0.0a4
Searching for pyserial==3.4
Best match: pyserial 3.4
Adding pyserial 3.4 to easy-install.pth file

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for ntc-templates==2.2.0
Best match: ntc-templates 2.2.0
Adding ntc-templates 2.2.0 to easy-install.pth file

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for textfsm==1.1.2
Best match: textfsm 1.1.2
Adding textfsm 1.1.2 to easy-install.pth file
Installing textfsm-script.py script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing textfsm.exe script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for tenacity==6.2.0
Best match: tenacity 6.2.0
Adding tenacity 6.2.0 to easy-install.pth file

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for scp==0.13.2
Best match: scp 0.13.2
Adding scp 0.13.2 to easy-install.pth file

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for paramiko==2.7.2
Best match: paramiko 2.7.2
Adding paramiko 2.7.2 to easy-install.pth file

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for setuptools==47.1.0
Best match: setuptools 47.1.0
Adding setuptools 47.1.0 to easy-install.pth file
Installing easy_install-script.py script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing easy_install.exe script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing easy_install-3.8-script.py script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing easy_install-3.8.exe script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for six==1.15.0
Best match: six 1.15.0
Adding six 1.15.0 to easy-install.pth file

Using c:\users\ryuji\appdata\roaming\python\python37\site-packages
Searching for future==0.18.2
Best match: future 0.18.2
Adding future 0.18.2 to easy-install.pth file
Installing futurize-script.py script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing futurize.exe script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing pasteurize-script.py script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts
Installing pasteurize.exe script to C:\Users\ryuji\AppData\Local\Programs\Python\Python37\Scripts

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for cryptography==3.1.1
Best match: cryptography 3.1.1
Adding cryptography 3.1.1 to easy-install.pth file

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for bcrypt==3.2.0
Best match: bcrypt 3.2.0
Adding bcrypt 3.2.0 to easy-install.pth file

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for PyNaCl==1.4.0
Best match: PyNaCl 1.4.0
Adding PyNaCl 1.4.0 to easy-install.pth file

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for cffi==1.14.3
Best match: cffi 1.14.3
Adding cffi 1.14.3 to easy-install.pth file

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Searching for pycparser==2.20
Best match: pycparser 2.20
Adding pycparser 2.20 to easy-install.pth file

Using c:\users\ryuji\appdata\local\programs\python\python37\lib\site-packages
Finished processing dependencies for netmiko==4.0.0a4

C:\Work\python_contest\netmiko-develop>
C:\Work\python_contest\netmiko-develop>
```
