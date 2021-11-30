# ReverseProxy
ReverseProxy in golang

## Use:

	./ReverseProxy_[OS]_[ARCH] -h
	
	Usage of ReverseProxy_[OS]_[ARCH]:
	  -l string
	        listen on ip:port (default "0.0.0.0:8888")
	  -r string
	        reverse proxy addr (default "http://idea.lanyus.com:80")


	./ReverseProxy_windows_amd64.exe -l "0.0.0.0:8081" -r "https://www.baidu.com"

	Listening on 0.0.0.0:8081, forwarding to https://www.baidu.com





# 下载镜像
docker pull qierkang/golang-reverseproxy
# 以后台方式启动镜像，端口映射为11011(端口请自行修改) 
docker run --name jrebel -d -p 11011:8888 qierkang/golang-reverseproxy
搭建成功后激活地址为： http://你的服务器ip:11011/{ GUID }
