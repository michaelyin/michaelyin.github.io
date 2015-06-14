(from a forum)
我最近买了个 Amazon FireTV Stick。价钱不贵。 FireTV Stick有个好处。可以自己安装第三方的APP。方法如下：

从网上找到自己喜欢的视频APP。比如泰捷视频，VST全聚合，兔子视频，....等。这都是非常容易搜索到的。选几个下载。我本人下载了这三个，还有番茄视频等。 也可以在沙发网站（ http://www.shafa.com/49 ）下载电视必备。 里面都有了。注意不要下载沙发管家（很多人喜欢，我不喜欢）

下载安装一个软件 adb-setup-1.3. 网上搜索很容易找到。 
安装时，三个选项都是Y(es)。我在HP笔记本（Win81.)安装时没有成功。 后来在台上电脑上（Win8.1)安装了。

用adb把下载的APP装到FireTV Stick上。分几个步骤。

A）要知道FireTV的IP地址。 fireTV Stick接到TV上。打开电视后进入FireTV，找到Settings, System, about, Network. 这时就可以看到IP地址了。记下IP地址。

B） Goto Settings， System, Developer Options, 把里面的两个, ADB Debugging, APPs From Unknown 都Turn ON.

C) 开始安装： 在安装了ADB的电脑上运行CMD。 在cmd里面 adb connect IPADDRESS （这个IPADDRESS 
就是记下的FireTV Sticp的IP地址）。 连接成功后会看到 Connected to IPADDRESS:5555。

D) 一个个装APP: adb install Togic.apk (安装泰捷视频） ....

E) 通过adb安装的APP，在FireTV的Home里是看不到的。因此为了方便还要下载安装FiredTVLauncher-1.1.0.apk 。（注意： 是FiredTV, 不是FireTV）

希望大家喜欢。
