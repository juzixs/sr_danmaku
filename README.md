# sr_danmaku
Record SHOWROOM (showroom-live.com) live comments and save as niconico danmaku (弾幕 / bullets) subtitle ass file.

## Installation
Python 3 is required. It's better to be Python 3.8.0+

```
pip install -r requirements.txt
```

## Usage

1. Edit the file ***`rooms.ini`*** and add the rooms you want to monitor and record their comments.  
2. Run program:
```
python sr_danmaku.py
```

When program is running, you can enter the following command:
```
- Type "h" or "help" for help.
- Type "q" or "quit" to quit.
- Type "s" or "status" to view status.
- Type "c" or "comment" to turn on/off showing comments.
```

3. If the program is already recording rooms, but you need to emergently record a new room.
You can run another instance of the program with **`-u`** option.
Suppose the room url is `https://www.showroom-live.com/room_url_key`:
```
python sr_danmaku.py -u https://www.showroom-live.com/room_url_key
```
Or
```
python sr_danmaku.py -u room_url_key
```
Only comments from this room will be recorded.

4. When a live is finished, the recorded comments will be converted to danmaku subtitle, and it will be saved as an ***`.ass`*** file under the folder ***`comments`***.

## Links
- [Showroom Live Watcher](https://github.com/wlerin/showroom) : records Showroom live streams.

- [Showroom Comment and Gift Viewer](http://sr-viewer.sacra.co/) : view the comments and gifts, and be able to read the comments out loud.

- [Showroom Comment Viewer](http://sr-com.net/comment_viewer/pc/) : fancy comments and gifts viewer

- [Showroom Rokugatch](https://www.skypower.xyz/showroom_rokugatch.html) : Showroom recorder. Can be set up to work with Haishin Kakuninkun.

- [Haishin Kakuninkun](https://www.skypower.xyz/haishin_kakuninkun.html) : informs you when a room is on live. And calls Showroom Rokugatch to record the live.

- [Showroom Toolbox](https://chrome.google.com/webstore/detail/showroom-toolbox/jlelpggiclkhdadagnbdjblokcnnhanl) : chrome extension, provides useful tools for watching showroom.

- [Showroom Sukosuko Tool](https://chrome.google.com/webstore/detail/showroom-%E3%81%99%E3%81%93%E3%81%99%E3%81%93%E3%83%84%E3%83%BC%E3%83%AB/ohfkmalmidmhailhaiifeplheagoopap) : chrome extension, provides useful tools for watching showroom.

- [ShowRoomViewer](http://iroiro.konjiki.jp/) ([download page](http://iroiro.konjiki.jp/tool.html)) : provides overall information for rooms. 


