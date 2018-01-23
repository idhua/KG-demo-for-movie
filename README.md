# Data文件夹
包含ER图模型文件和创建数据库、表，插入所有数据的sql文件。用户可以直接使用sql文件导入数据到mysql中。

# kg\_demo_movie文件夹
crawler中的movie_crawler用于从The Movie DB下载数据，用户需要自己去网站注册账号，申请API KEY。在脚本中填入自己的API KEY，填写mysql相关参数即可运行。用户需要额外下载的包:requests和pymysql。tradition2simple用于将繁体字转为简体字（声明一下，我找不到该文件的出处了，我是从网上找到的解决方案，如果有用户知道该作者，麻烦告知，我会备注）。

# ontology.owl
通过protege构建的本体，用户可以直接用protege打开，查看或修改。

# kg\_demo\_movie_mapping.ttl
根据d2rq mapping language编辑的映射文件，将数据库中的数据映射到我们构建的本体上。

# kg\_demo_movie.nt
利用d2rq，根据mapping文件，由Mysql数据库转换得到的RDF数据。

# fuseki_conf.ttl
fuseki server配置文件，指定推理引擎，本体文件路径，规则文件路径，TDB路径等

# rules.ttl
规则文件，用于基于规则的推理。