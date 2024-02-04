对于⽆⽤的内建程式，保留在电脑内既占空间⼜毫⽆⽤途，例如酷我⾳乐、市集、Xbox 这些很少⼈⽤的到，但由于是“内建”，所以不能直接解除安装。

其实内建软件也有卸载的⽅法，就是透过「Windows PowerShell」来卸载，⾸先利⽤搜寻器找出 Windows PowerShell ，之后按右键并选按“以系统管理员⾝份执⾏”。 最后便会打开 Windows PowerShell 的视窗，然后在视窗中输入指令并按下 Enter ，便会立刻移除指令代表的应⽤软件，以 Xbox 为例，就要输入：

Get-AppxPackage *xboxapp* | Remove-AppxPackage
当按下「Enter」后，应⽤软件便会⾃动卸载。

**指令列表：**

> 3D Builder：Get-AppxPackage *3dbuilder* | Remove-AppxPackage
> 闹钟与时钟：Get-AppxPackage *windowsalarms* | Remove-AppxPackage
> ⾏事历：Get-AppxPackage *windowscalculator* | Remove-AppxPackage
> ⾏事历与邮件：Get-AppxPackage *windowscommunicationsapps* | Remove-AppxPackage
> 相机：Get-AppxPackage *windowscamera* | Remove-AppxPackage
> 取得 Office：Get-AppxPackage *officehub* | Remove-AppxPackage
> 取得 Skype：Get-AppxPackage *skypeapp* | Remove-AppxPackage
> 取得开始：Get-AppxPackage *getstarted* | Remove-AppxPackage
> Groove ⾳乐：Get-AppxPackage *zunemusic* | Remove-AppxPackage
> 地图：Get-AppxPackage *windowsmaps* | Remove-AppxPackage
> Microsoft Solitaire Collection：Get-AppxPackage *solitairecollection* | Remove-AppxPackage
> 财经：Get-AppxPackage *bingfinance* | Remove-AppxPackage
> Movies & TV：Get-AppxPackage *zunevideo* | Remove-AppxPackage
> 新闻：Get-AppxPackage *bingnews* | Remove-AppxPackage
> OneNote：Get-AppxPackage *onenote* | Remove-AppxPackage
> 联络⼈：Get-AppxPackage *people* | Remove-AppxPackage
> ⼿机⼩帮⼿：Get-AppxPackage *windowsphone* | Remove-AppxPackage
> 相片：Get-AppxPackage *photos* | Remove-AppxPackage
> 市集：Get-AppxPackage *windowsstore* | Remove-AppxPackage
> 运动：Get-AppxPackage *bingsports* | Remove-AppxPackage
> 语⾳录⾳机：Get-AppxPackage *soundrecorder* | Remove-AppxPackage
> 天⽓：Get-AppxPackage *bingweather* | Remove-AppxPackage

