# 搭建第二个服务器 Web服务器 (nginx) 作业完成清单

**🎯 目标：** 搭建 nginx 服务器，允许远程访问

---

- [ ] **步骤 1：安装 nginx 服务**
  - 执行命令：`sudo apt install nginx -y`
  - *说明：一条命令即可完成安装。*
  ![alt text](image-3.1-1.png)

- [ ] **步骤 2：查询虚拟机 IP 地址**
  - 执行命令：`ifconfig`
  - 记录获取到的 IP 地址（图中示例为：`192.168.149.128`）
  ![alt text](image-3.2-1.png)

- [ ] **步骤 3：验证 nginx 默认页面**
  - 回到你的 Windows 电脑，打开浏览器。
  - 在地址栏输入刚刚查到的虚拟机 IP 地址（如：`http://192.168.149.128`）。
  - *预期结果：看到 "Welcome to nginx!" 的默认页面。*
  ![alt text](image-3.3-1.png)

- [ ] **步骤 4：切换到 root 用户并编辑网页内容**
  - [ ] 切换到 root 用户：`sudo su root`
  - [ ] 准备编辑工具：确保系统安装了 vim 编辑器，若没有可执行 `apt install vim`。也可以直接在虚拟机的图形界面下编辑。
  - [ ] 进入 Web 根目录：`/var/www/html`
  - [ ] 添加或修改 `index.html` 文件，内容如下：
    ```html
    <html><body>hello, njupt</body></html>
 ![alt text](image-3.4-1.png)

    ```

- [ ] **步骤 5：验证修改结果**
  - 回到 Windows 浏览器，刷新之前的 IP 地址页面。
  - *预期结果：页面内容由默认的 "Welcome to nginx!" 变更为 "hello, njupt"。*
 ![alt text](image-3.5-1.png)

