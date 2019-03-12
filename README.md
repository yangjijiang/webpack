# webpack
webpack前端工程打包（webpack4+vue2.x+less3.x）
步骤：cd 进入目录 src\main\webapp\

    1：初始化：
        npm install
    
    2：生产环境打包：
        npm run prod
    
    3：运行开发环境：
        npm run dev-server
       
    启动参数说明：
        webpack   
            --config webpack.prod.config.js   # 指定webpack运行加载的配置文件
            --watch            # 当打包中的文件内容有变动时自动触发打包
            --progress         # 空制台显示打包过程
            --display-reason   # 显示为什么要打包这个模块的原因 
        
        webpack-dev-server    # 使用dev server服务器启动（默认端口8080）
            --open            # dev server服务启动后自动打开浏览器窗口（默认打开页面index.html）
            --hot             # 热部署（当资源发生改变 - 重新加载改变的部分）
            --inline          # 刷新浏览器（当资源发生改变）

注意：在安装别的开发包时要注意版本的兼任性，与webpack(当前版本为^4.22.0)不兼任时npm run xxx时会报错，尽量在命令行中使用 npm install 包名 --save-dev 安装最新包，避免复制粘贴版本号后全局npm install。