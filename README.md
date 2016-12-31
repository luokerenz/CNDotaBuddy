CNDotaBuddy
===========

感谢原作者的DotaBuddy(https://github.com/waylaidwanderer/DotaBuddy), 此为简单的汉化版本 
肉山和不朽盾的计时器没有测试过.

## 功能
* 一键自动化读取当前比赛中公开的玩家数据，包括各场比赛，输赢，KDA和GPM/XPM
* 肉山/不朽盾计时器
    * 按 **Insert** 来开始肉山/不朽盾计时器 (按 **Cmd或Ctrl+Alt+Insert** 来清除肉山/不朽盾计时器)
    * 按 **Alt+Insert** 来开始肉山计时器
    * 按 **Home** 来开始不朽盾计时器 (按 **Cmd或Ctrl+Alt+Home** 来清除不朽盾计时器)
    * 使用计时器需要的额外操作：
    
添加一个名为 `gamestate_integration_dotabuddy.cfg` 的文件在 `path\to\steamapps\common\dota 2 beta\game\dota\cfg\gamestate_integration` 目录下， 文件内容如下：

    "Dota 2 Integration Configuration"
	{
	    "uri"           "http://localhost:3222/"
	    "timeout"       "5.0"
	    "buffer"        "0.1"
	    "throttle"      "0.1"
	    "heartbeat"     "30.0"
	    "data"
	    {
	        "provider"      "1"
	        "map"           "1"
	        "player"        "1"
	        "hero"          "1"
	        "abilities"     "1"
	        "items"         "1"
	    }
	}

## License
* Released under the GPLv3 license. Built on top of electron-boilerplate (MIT).
