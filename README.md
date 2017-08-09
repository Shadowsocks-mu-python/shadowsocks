# shadowsocks

这是shadowsocks的python2.x版本
多用启
用户数据保存在mysql数据库中

此代码需要安装依赖：
yum install gcc python-devel openssl-devel
cd       //将get-pip.py保存在用户家目录
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python get-pip.py
pip install cymysql M2Crypto

运行方式：
nohup python /shadowsocks/server.py -c /shadowsocks/config.json &
其中路径以实际为准

数据库连接参数配置在Config.py文件：
#Config
MYSQL_HOST = ‘000.000.000.000’     //mysql服务器的IP
MYSQL_PORT = 3306                  //mysql服务器端口
MYSQL_USER = ‘root’                //mysql用户名
MYSQL_PASS = ‘mysqlpasswd’         //mysql密码
MYSQL_DB = ‘shadowsocks’           //数据库名称
