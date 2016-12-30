# cibdb

---
[文档目录](SUMMARY.md)



cibdb是一个内部项目A拆分出来的模块，主要负责提供原项目所需的数据，并且按照一定的更新频度更新数据，旨在提高原系统获取数据的健壮性，使原系统与数据获取、更新等数据内部逻辑解耦，符合[最少知道原则](https://thelittlematch.gitbooks.io/design/content/er_3001_she_ji_mo_shi_de_liu_da_yuan_ze/53001_di_mi_te_fa_zeff08_zui_shao_zhi_dao_yuan_ze_.html)的设计模式。


###原项目A

![](/assets/原项目1.0.png)