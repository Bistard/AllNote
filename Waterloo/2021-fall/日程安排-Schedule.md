

| **Subject**                                                  | **Description**                                              | **Deadline**                                                 |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [**MATH 237**](https://learn.uwaterloo.ca/d2l/le/content/701924/viewContent/3881420/View) |                                                              |                                                              |
|                                                              |                                                              |                                                              |
| [**MATH 239**](https://learn.uwaterloo.ca/d2l/le/content/708429/Home) |                                                              |                                                              |
|                                                              | ✔A09                                                         |                                                              |
| [**CS 245**](https://learn.uwaterloo.ca/d2l/le/content/709696/Home) |                                                              |                                                              |
| [**CS 246E**](https://student.cs.uwaterloo.ca/~cs246e/F21/assignments.shtml) | git clone ssh://s795li@linux.student.cs.uwaterloo<br />.ca/u/cs246e/pubrepo/1219/.git | ssh -Y s795li@linux.student.cs.uwaterloo.ca<br />            |
|                                                              | lecture ✔nov2, ✔nov4, ✔nov9, ✔nov11, nov16, nov18, nov23, nov25 |                                                              |
|                                                              | AGE engine (Controller, Model, View, Motion, Gravity, Collision, Quadtree, game1, game2) | Friday, December 14, 5pm                                     |
| [**SPOCOM 100**](https://learn.uwaterloo.ca/d2l/le/content/726790/Home) |                                                              |                                                              |
|                                                              | ✍3 comments for each week (>= 100 words) (comment should no longer than 3 weeks) |                                                              |
| **PD1**                                                      |                                                              |                                                              |
|                                                              | apply for coop work-permit                                   |                                                              |
| **DWZQ-coop**                                                |                                                              |                                                              |
| #1                                                           | ✔compilation                                                 |                                                              |
|                                                              | ✔develop on xxx.xxx.xxx.167                                  |                                                              |
|                                                              | ✔connect A5, MySQL                                           |                                                              |
|                                                              | ✔[write configuration]                                       |                                                              |
|                                                              | ✔ login A5 first                                             | reference: *dataproxy.cpp & xxxassistant.cpp                 |
|                                                              | ✔ async: get rsp - test                                      |                                                              |
|                                                              | ✔ LEARN: XML API                                             |                                                              |
|                                                              | ✔ read a5_fielddef.xml                                       |                                                              |
|                                                              | ✔ async: get rsp from A5                                     |                                                              |
|                                                              | ✔ (read a5_fielddef.xml to get coressponding field key (id value -> string field key) - e.g '605' -> 'FID_KHH' |                                                              |
|                                                              | ✔new API: create TABLE                                       |                                                              |
|                                                              | ✔合成MySQL语句 + 插入 (update map) - (MySQL.insert())        |                                                              |
|                                                              | ✔read mapConfig.xml to auto send request to A5               |                                                              |
|                                                              | ✔fix cannot get login arguments                              | mysql IP: root@10.142.13.9                                   |
| #2                                                           |                                                              |                                                              |
|                                                              | ✔协议protobuf (google protocol buffer)                       |                                                              |
|                                                              | ✔修167上dwzq-map-test的bug先 (out_of_range) (密码错误)       |                                                              |
|                                                              | ✔本地: 装protobuf , 测试服: 需要compile过后的protobuf文件    |                                                              |
|                                                              | ✔protoc -I=./ --cpp_out=./ ./funcMessage.proto               |                                                              |
|                                                              | ✔本地: 测试收发序列化/反序列化protobuf                       |                                                              |
|                                                              | ✔在同一个线程或者开一个线程来监听                            |                                                              |
|                                                              | ✔(原生API) 去监听多个listeners                               |                                                              |
|                                                              | ✔远程: 成功编译 (带protobuf)                                 |                                                              |
|                                                              | ✔远程: 从另一台远程发送数据进行测试                          |                                                              |
|                                                              | ✔利用protobuf反序列化                                        |                                                              |
|                                                              | ✔测试是否成功                                                |                                                              |
|                                                              | ✔发送对应的mysql语句                                         |                                                              |
|                                                              | ✔获得mysql的response                                         |                                                              |
|                                                              | ✔设计protobuf协议: 用来传输接受其他protobuf协议的协议        |                                                              |
|                                                              | ✔cd /root/src/midtrade/MidTrade0902/depends/a5mock           |                                                              |
|                                                              | ✔解决缺少库: xml, log, a5, dwmysql, protobuf                 |                                                              |
|                                                              | ✔复制了: common/log, common/dwmysql                          |                                                              |
|                                                              | 记链接库的笔记                                               |                                                              |
|                                                              | ✔写成一个库 (.so), 需要开放类似于A5的API (参考/root/src/midtrade/MidTrade0902/common/a5) |                                                              |
|                                                              | ✔测试.so能否正常work                                         |                                                              |
|                                                              | ✔线程安全queue                                               |                                                              |
|                                                              | ✔然后开一个额外线程, 专用消耗该队列 (同步), 同时利用async发送rsp给client |                                                              |
|                                                              | ✔发送rsp给listeners                                          |                                                              |
|                                                              | ✔exception safe                                              |                                                              |
|                                                              | ✔重修以下a5mySQLTable (单纯的作为一个服务, 只会一次性update一次mysql) |                                                              |
|                                                              | 最终检测                                                     | ssh root@10.142.13.7<br />mysql -u root -p<br />SHOW DATABASES;<br />USE a5mock;<br />SHOW TABLES;<br />SELECT * FROM ``; |
| **MarkdownNote**                                             |                                                              |                                                              |
|                                                              | architecture explanation.md                                  |                                                              |
|                                                              | UML for DI                                                   |                                                              |
|                                                              | UML && 时序图 - FileService                                  |                                                              |
|                                                              | 观察stream如何按chunk读文件                                  |                                                              |
|                                                              | decode DataBuffer                                            |                                                              |
|                                                              | 替换/实装service                                             |                                                              |
|                                                              | 测试按chunk读取 vs. 一次性读取                               |                                                              |
|                                                              | performanceService?                                          |                                                              |
|                                                              | writeFile功能                                                |                                                              |
|                                                              | 优化uri.ts                                                   |                                                              |
|                                                              | 完善fileService和diskFileSystemProvider                      |                                                              |
|                                                              | 研究protobuf技术 (效率 + 体积 + 是否足够轻便?)               |                                                              |
|                                                              | 如果protobuf整个数据集太臃肿了, 要不要试一下json+部分protobuf数据集? |                                                              |
|                                                              | 每个notebook都用一个单独的protobuf去记录, 这样子当只修改了一个notebook的时候不需要全部重新生成新的protobuf |                                                              |
|                                                              | 重构file tree                                                |                                                              |



| 产品名称               | 订阅价格   | 间隔 | 订阅起始日期  | 下次收费      |
| ---------------------- | ---------- | ---- | ------------- | ------------- |
| Microsoft 365 personal | CAD $79.00 | 1年  |               | 2022年5月14日 |
| bilibili年度会员       | 108$       | 1年  | 2021年9月30日 | 2022年9月30日 |



## vscode fileService Step By Step

* [ ] fileService

  * [ ] doReadFile()

  * [ ] _doReadFile()

  * [ ] _doReadFileStream()

    * [ ] readFileUnbuffered()

    * [x] readFileStreamed(provider)

      * [x] call: provider.readFileStream() - diskFileSystemProvider

        * [x] newWriteableStream()

        * [x] readFileIntoStream()

          * [x] ⭐doReadFileIntoStream()

            * [x] const handle = await provider.open();

            * [x] let buffer = VSBuffer.alloc();

            * [x] do {

              ​	bytesRead = await provider.read(handle, posInFile, buffer.buffer, posInBuffer, buffer.byteLength - posInBu);

              provider.write(buffer);
            
              buffer = VSBuffer.alloc();
            
            * [x] } while (bytesread > 0);

    * [ ] readFileBuffered()

    * [ ] ...

  * [ ] streamToBuffer()

    * [ ] streams.consumeStream()



* class `Compoennt` base class 和 一堆超级简单无脑的迷你继承`Component`s, 比如velocity, position, render, texture, 
    * 记得写一个helper function用来为每个不同的component type生成一个unique id， see `chrisli/component.h`

* class `Object` (对应ECS中的`Entity`)
    * wrapper of `Component`s
    * 必顶有个vector存`Component`
    * 额外的一些details：
        * 需要些APIs去add/remove `Compoennt` (最好不用写在`Entity`里面， 写在`ObjectManger`)
* class `ObjectManager` (对应的就是我的`Registry`)
    * fields:
        * vector of `Object`
    * APIs:
        * Object &createObject(); 唯一正确途径去创建一个`Object`
        * 
        * ComponentType &addComponent\<ComponentType, Arg...\>(Object &, Args... args); [note: 必定是个template function]
        * removeComponent<>() [对应的是我的Regisry::remove()]
        * bool hasComponent<>(Object &);
        * ComponentType &getComponent<>(Object &);
        * void destroyObject(Object &);
        * void clearAllObjects();
        *  
        * vector\<Object *\> query\<ComponentType\>();
            * 注释：用来搜索所有Object which obtains the provided ComponentType.
            * 实现：for loop every `Object`, for each `component` in `Object`, check if the component is the same as the `ComponentType`, if so , add a pointer to that Obejct into a vector, if not , pass it. Return the vector at last.

