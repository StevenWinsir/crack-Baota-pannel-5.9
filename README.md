# crack-Baota-pannel-5.9
crack Baota pannel 5.9
步骤：
1. wget -O https://raw.githubusercontent.com/StevenWinsir/crack-Baota-pannel-5.9/master/update.sh  https://raw.githubusercontent.com/StevenWinsir/crack-Baota-pannel-5.9/master/update_pro.sh && bash update.sh pro

2. 进入路径：“ /www/server/panel/class” 修改其中的 common.py 文件找到“data = panelAuth.panelAuth().get_order_status(None); ” 164行

修改成为：
data = {
  'status' : True,
  'msg' : {'endtime' : 32503651199 }
  };

3. 进入 “/www/server/panel/data” 新建一个文件 文件名为：“userInfo.json” 内容空 。

然后将下方代码写入userInfo.json：

/etc/init.d/bt restart

4. 重启宝塔 bt restart
