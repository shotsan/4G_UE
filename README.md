
Man in the Detection research paper uses a 4G network. This repo is fork from [srsRAN project](https://www.srsran.com).
Without any modifications to the source code, except to configure the frequency of operation, we use the project as is.

UE configuration file with modications is in the [repo](https://github.com/shotsan/4G_eNodeB_EPC/blob/3956297891cd4739f450ac30dc2ac81006304ccf/enb.conf)



## Instructions to run UE

1. Clone the repo

```
git clone https://github.com/shotsan/4G_UE/
```

2. Install UHD to use USRP, we used USRP X310 which interfaces to the host machine through ethernet interface.

https://files.ettus.com/manual/page_install.html

3. Build project

```
mkdir build
cd build
cmake 
make -j$(nproc)
```


4. Start UE 

```
srsueMIM <path to config file>

```

### SRS RAN PROJECT DETAILS

srsRAN
======

srsRAN is a 4G software radio suite developed by [SRS](http://www.srs.io).

See the [srsRAN project pages](https://www.srsran.com) for information, guides and project news.

The srsRAN suite includes:

  * srsENB - a full-stack SDR 4G/5G e(g)NodeB application
  * srsEPC - a light-weight 4G core network implementation with MME, HSS and S/P-GW

For application features, build instructions and user guides see the [srsRAN documentation](https://docs.srsran.com).

For license details, see LICENSE file.

Support
=======

Mailing list: https://lists.srsran.com/mailman/listinfo/srsran-users


