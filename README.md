# Send
CTGU自动报平安

### Step1
config.txt文件中按示例添加用户信息  
如用户不需要接收邮件，将该用户的邮箱地址设为“null”即可
  
仓库首页 Settings -> Secrets -> New secret, 添加信息  
需要设置两个secret
name即FROMEMAIL和POP3KEY
value即对应的邮箱地址和授权码

### Step2  
代码拷到本地
进入项目主目录，使用“pip install -r requirements.txt”安装所需依赖文件

send.py -f <发送方邮箱地址> -k <邮箱授权码>  
[注]：不可使用git bash，应该使用cmd
