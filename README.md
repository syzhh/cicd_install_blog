# cicd_install_blog
该项目用于博客的cicd平台搭建

        yum install -y docker-compose
        yum install -y ansible
        yum install -y git

执行安装

    mkdir /home/jenkins

    chmod +777 /home/jenkins

    cd ~

    https://github.com/hqh546020152/cicd_install_blog.git

    cd cicd_install_blog

    vi +53 docker-compose-gitlab.yml    该53行的IP修改为本机IP

    部署Jenkins

        docker-compose -f "docker-compose-jenkins.yml" up -d     

    部署gitlab(预计5分钟完成)

        docker-compose -f "docker-compose-gitlab.yml" up -d

    验证：

        访问Jenkins：http://HOST:8080

> https://www.jianshu.com/p/4237ed1277ce
