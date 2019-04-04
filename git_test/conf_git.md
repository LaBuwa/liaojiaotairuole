生成密鑰
	ssh-keygen -t rsa -C "youremail@example.com"
	-t	密鑰類型，没有指定则默认生成用于SSH-2的RSA密钥
	-C	指定注释注釋字段，可標識密鑰，指出密钥的用途或其他有用的信息。所以在这里输入自己的邮箱或者其他都行。


设置用户名和密码
	git config --global user.name "Liter"
	git config --global user.email "Email@.com"

查看 git 配置
	git config user.name
	git config user.email

	git config --global --list
	git config --system --list
	
	查看当前仓库配置信息
	git config --local --list