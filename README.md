# cibdb

---
[文档目录](SUMMARY.md)



cibdb是一个内部项目A拆分出来的数据模块，主要负责提供原项目所需的数据，并且按照一定的更新频度更新数据，旨在提高原系统获取数据的健壮性，使原系统与数据获取、更新等数据内部逻辑解耦，符合[最少知道原则](https://thelittlematch.gitbooks.io/design/content/er_3001_she_ji_mo_shi_de_liu_da_yuan_ze/53001_di_mi_te_fa_zeff08_zui_shao_zhi_dao_yuan_ze_.html)的设计模式。


###项目A v1.0

数据模块需要保证数据可用。
![](/assets/原项目1.0.png)

数据请求逻辑可能被长时间的数据更新阻塞住，造成数据请求实体长时间拿不到数据返回结果。

###项目A v2.0

数据模块不保证数据对于请求方可用，按照固定内部封闭的逻辑更新数据。
![](/assets/原项目2.0.png)

降低了数据请求方与数据模块的耦合，使得请求可以即时响应。