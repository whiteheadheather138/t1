代发 wailian999

[U101] JS：classList 操作
来源：http://dki.ivvv.top

el.classList.toggle("active")
来源：http://oqk.gogol.net.cn

[U102] JS：本地存储
来源：http://sxh.ivvv.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hvs.zhijiandao.cn

[U103] JS：定时器
来源：http://rjs.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fgj.gogol.net.cn

[U104] JS：防抖
来源：http://yay.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://juw.chenjidiqi.icu

[U105] JS：节流
来源：http://vfh.dianchejie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://des.cdnleiting.top

[U106] JS：日期格式化
来源：http://dqb.cheryme.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://trj.sufxvd.cn

[U107] JS：数字千分位
来源：http://lie.fehbvm.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ipp.epnwcf.com

[U108] JS：随机整数
来源：http://xav.jiagoushi.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ios.fengsongda.top

[U109] JS：数组分组
来源：http://rls.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://gmi.cqqwz.cn

[U110] JS：数组分块
来源：http://xna.shangyingyoupin.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dne.yj202588.top

[U111] JS：对象转 Map
来源：http://icy.meibo888.top

new Map(Object.entries(obj))
来源：http://zgo.vqdsnc.cn

[U112] JS：字符串补位
来源：http://cvm.ywan-chungtsiang.top

"7".padStart(3, "0")
来源：http://yvy.yongpay.top

[U113] JS：正则替换全部
来源：http://vqc.yj20258.top

s.replaceAll("a", "b")
来源：http://utc.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://nwv.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://uvg.chenzaomai.com

[U115] JS：生成 UUID
来源：http://qje.jiagoushi.top

crypto.randomUUID()
来源：http://gbn.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://szu.aibaodan.cn

/** @param {string} name */ function f(name) {}
来源：http://oea.bbcook.cn

[U117] JS：单元测试
来源：http://jvt.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://vsa.ppjwa.cn

[U118] JS：开发服务器
来源：http://uxx.yj20258888.top

npm i -D vite;  npx vite
来源：http://wqm.havefunace.top

[U119] JS：生产构建
来源：http://jyk.zhoulong.xyz

npx vite build
来源：http://izy.shanyushiyangtech.top

[U120] JS：读取环境变量（Vite）
来源：http://bcz.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://qqe.xuetiantiany.cn

================================================================================
来源：http://wok.ctjpmb.com

统计汇总
来源：http://zww.zhixingplan.top

================================================================================
来源：http://nos.pycfn.com

按语言统计（条）：
来源：http://wsw.xinyue.icu

Python ......... 252
来源：http://xvv.hfpthk.cn

PHP ............ 252
来源：http://amc.jianghu66.top

JavaScript ..... 252
来源：http://dnb.pengpengdd.cyou

TypeScript ..... 212
来源：http://gts.vehdjk.com

Java ........... 212
来源：http://hdn.cdnleiting.top

Go ............. 212
来源：http://jcv.cdnleiting.top

Ruby ........... 212
来源：http://wjc.cucudq.cn

C# ............. 212
来源：http://tex.feifeiyinyue.top

C .............. 30
来源：http://yqr.52xcode.cn

C++ ............ 30
来源：http://wrg.xuetiantiany.cn

SQL ............ 90
来源：http://ufu.shuidangran.top

Bash ........... 80
来源：http://zih.nanxuanxn.top

Kotlin ......... 15
来源：http://shp.jlsjyb.cn

Swift .......... 15
来源：http://axn.hammf.cn

Lua ............ 10
来源：http://flb.hammf.cn

Perl ........... 10
来源：http://xix.andypj.xyz

Scala .......... 10
来源：http://fbj.yonumen.top

------------------------------------
来源：http://adg.haohaochexian.top

合计 ........... 2106 条
来源：http://pcu.zdbjq.cn

按章节统计：
来源：http://cpw.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xbn.bbcook.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qxi.hongshengwenyu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fbh.hesvh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tht.redwolf501.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ppn.tarul.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://egn.jianghu66.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://joz.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lob.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ygc.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kcl.snrcjt.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sxz.hesvh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://efg.ywan-chungtsiang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fid.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vlw.52xcode.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zkg.havefunace.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xuu.hcnkem.com

Q SQL 专题                              90
来源：http://zcl.ybcxt.top

R Bash 专题                             80
来源：http://xkr.chenzaomai.com

S C / C++ 专题                          60
来源：http://jwn.sxryk.cn

T 其他语言补充                          60
来源：http://bbo.yfazqb.com

U 高频实用片段                         120
来源：http://oqp.yvedp.cn

------------------------------------
来源：http://ump.fanxiaobao.xyz

合计                                  2106 条
来源：http://tdu.52xcode.cn

--------------------------------------------------------------------------------
来源：http://ubo.iojbl.cn

使用提醒
来源：http://uaq.smart0.xyz

--------------------------------------------------------------------------------
来源：http://bkn.gaohongyu789.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zbe.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://esw.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tax.ctjpmb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://uao.yanxiufei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bku.dianchejie.cn

—— 文件结束 ——
来源：http://cxe.yuxming.cn

================================================================================
来源：http://tnr.zycfv.cn

程序语言常见例子速查手册（2024 版）
来源：http://prv.nanxuanxn.top

Common Programming Examples Cheat Book
来源：http://dyw.gaohongyu789.top

================================================================================
来源：http://rkk.fktsv.cn

【收录内容】
来源：http://pbb.andypj.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://yjl.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://myt.yuanzhike.top

SQL · Bash · C · C++
来源：http://whr.gogol.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jex.tian-w.cn

【使用说明】
来源：http://nrf.c1oappe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yoc.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mou.daxiang520.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gps.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lmo.yuanzhike.top

Bash:  Shell         C:     C             C++:   C++
来源：http://phq.vehdjk.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jej.gogol.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vfw.nwbrower.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kgt.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kxz.jinghuilouyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wnd.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bnd.shangyingyoupin.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://khx.zdqjudy.top

【文件统计】
来源：http://rvr.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xbz.ydzc1.top

--------------------------------------------------------------------------------
来源：http://laq.kuanghao11.cn

目  录
来源：http://kgn.wangdashe.top

--------------------------------------------------------------------------------
来源：http://ogl.chenjidiqi.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ttl.jinghuilouyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lyt.dashuyun.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zdq.yanxiufei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jin.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xwk.sufxvd.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ufv.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://goq.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://myq.aizwys.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ajn.c1oappe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wyn.yongpay.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fjd.hnqzz.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jwk.cdnleiting.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://inm.ctjpmb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pes.zdbjq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fxj.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ulm.yfazqb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nvg.redwolf501.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://hcv.tianlin.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uxv.daxiang520.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kdp.zhiwuduotai.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rmi.andypj.xyz

================================================================================
来源：http://lmd.gotoacloud.top

A. 基础语法与类型
来源：http://vfd.tianlin.xyz

================================================================================
来源：http://hdk.hesvh.cn

[A01] Hello World
来源：http://ngd.ehwqpu.com

Py:   print("Hello, World!")
来源：http://dlf.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://qdp.jinghuilouyu.cn

JS:   console.log("Hello, World!");
来源：http://elv.cqqwz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mef.yuanzhike.top

Java: System.out.println("Hello, World!");
来源：http://van.wangdashe.top

Go:   fmt.Println("Hello, World!")
来源：http://ajx.chenzaomai.com

Ruby: puts "Hello, World!"
来源：http://uqr.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://tos.ydzc1.top

[A02] 变量声明与赋值
来源：http://lvi.daxiang520.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wgq.cucudq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rin.yfazqb.com

JS:   let name = "Alex"; const age = 20;
来源：http://pkt.0kj1m.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fhb.zhoulong.xyz

Java: String name = "Alex"; int age = 20;
来源：http://amj.guannengcc.top

Go:   name := "Alex"; age := 20
来源：http://zon.daria6918.cn

Ruby: name = "Alex"; age = 20
来源：http://mbb.ywan-chungtsiang.top

C#:   string name = "Alex"; int age = 20;
来源：http://rmn.ppjwa.cn

[A03] 常量定义
来源：http://scj.pycfn.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hga.wangshuangyany.cn

PHP:  const PI = 3.14159;
来源：http://exg.aibaodan.cn

JS:   const PI = 3.14159;
来源：http://cfr.bjfxy.top

TS:   const PI: number = 3.14159;
来源：http://vgf.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://ffv.havefunace.top

Go:   const PI = 3.14159
来源：http://bpz.iojbl.cn

Ruby: PI = 3.14159
来源：http://png.guannengcc.top

C#:   const double PI = 3.14159;
来源：http://gnv.cheryme.top

[A04] 判断变量类型
来源：http://gqo.xziqi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://crc.zhongyouzk.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ozu.redwolf501.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cgl.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://oac.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dhh.xingfuxueyuan.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://qbd.zhongyouzk.top

Ruby: x.class; x.is_a?(Integer)
来源：http://url.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://ajw.yongpay.top

[A05] 整数除法与取模
来源：http://oic.ivvv.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cqm.zhaomingkeji.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://tib.shanyushiyangtech.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ala.gogol.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rwv.nwbrower.top

Java: 7 / 2; 7 % 2
来源：http://qsj.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://abw.sysykeji.top

Ruby: 7 / 2; 7 % 2
来源：http://pgb.shanyushiyangtech.top

C#:   7 / 2; 7 % 2
来源：http://ldi.sysykeji.top

[A06] 字符串转数字
来源：http://csr.yj20258.top

Py:   int("42"); float("3.14")
来源：http://mkd.birdmap.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jpd.ivvv.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qvd.yuanzhike.top

TS:   parseInt("42", 10); Number("42")
来源：http://pmd.yonumen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ozh.tarul.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://izs.ehwqpu.com

Ruby: "42".to_i; "3.14".to_f
来源：http://cey.guowangkeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wmf.316326.xyz

[A07] 数字转字符串
来源：http://gnk.shuidangran.top

Py:   str(42)
来源：http://fql.jiagoushi.top

PHP:  (string) 42; strval(42)
来源：http://eyu.c1oappe.top

JS:   String(42); (42).toString()
来源：http://cto.hammf.cn

TS:   String(42)
来源：http://ngl.gogol.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://opu.vehdjk.com

Go:   strconv.Itoa(42)
来源：http://yfd.jqgfzy.top

Ruby: 42.to_s
来源：http://zvj.cashguo.top

C#:   42.ToString()
来源：http://uvb.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://zfk.tanke756.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://trf.nanxinkj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wbw.xuetiantiany.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ggl.ppjwa.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gnb.yvedp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rfg.jiagoushi.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vis.gotoacloud.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cwr.yfazqb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bck.jinqigfzy.top

[A09] 绝对值与最大最小值
来源：http://vdl.daxiang520.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pnn.zhiwuduotai.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gvi.quarkkingdee.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wfn.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yza.hammf.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lsg.xylfe.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jje.gzhubu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ksr.hfpthk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zyx.xingfuxueyuan.xyz

[A10] 生成随机数
来源：http://nnc.jyoumei.cn

Py:   import random; random.randint(1, 100)
来源：http://uvg.cqqwz.cn

PHP:  random_int(1, 100);
来源：http://jyh.jinqigfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pwg.hesvh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fcn.shangyingyoupin.top

Java: new Random().nextInt(100) + 1
来源：http://lys.yvedp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xxf.dashuyun.cn

Ruby: rand(1..100)
来源：http://wpe.meibo888.top

C#:   new Random().Next(1, 101)
来源：http://knz.yueranfly.top

[A11] 条件表达式（三元）
来源：http://ftv.fehbvm.com

Py:   "yes" if x > 0 else "no"
来源：http://djz.zhongyouzk.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yze.daxiang520.top

JS:   x > 0 ? "yes" : "no"
来源：http://gng.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://jmq.jyoumei.cn

Java: x > 0 ? "yes" : "no"
来源：http://luk.jianghu66.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nym.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wqi.chenlongwang.top

C#:   x > 0 ? "yes" : "no"
来源：http://tmq.yuanzhike.top

[A12] 字符串插值 / 格式化
来源：http://bzn.jqgfzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pld.yanxiufei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ryj.yuanzhike.top

JS:   `Hello, ${name}!`
来源：http://tao.snrcjt.cn

TS:   `Hello, ${name}!`
来源：http://ksp.xylfe.cn

Java: "Hello, %s!".formatted(name)
来源：http://ldb.jiagoushi.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sff.yfazqb.com

Ruby: "Hello, #{name}!"
来源：http://ehi.gzhubu.top

C#:   $"Hello, {name}!"
来源：http://oba.ehwqpu.com

[A13] 多行字符串（练习 \n 转义）
来源：http://cpw.feifeiyinyue.top

Py:   "第一行\n第二行"
来源：http://hdw.chenjidiqi.icu

PHP:  "第一行\n第二行"
来源：http://bpr.smart0.xyz

JS:   "第一行\n第二行"
来源：http://skj.guannengcc.top

TS:   "第一行\n第二行"
来源：http://orr.aizwys.cn

Java: "第一行\n第二行"
来源：http://atc.cucudq.cn

Go:   "第一行\n第二行"
来源：http://dbi.mhx1999.top

Ruby: "第一行\n第二行"
来源：http://ifi.zhijiandao.cn

C#:   "第一行\n第二行"
来源：http://vww.52xcode.cn

[A14] 注释写法
来源：http://ble.zhixingplan.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://cso.jiagoushi.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://cdu.haohaochexian.top

JS:   // 单行；/* 多行 */
来源：http://amc.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://tkg.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mkk.cqqwz.cn

Go:   // 单行；/* 多行 */
来源：http://jmx.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://uys.birdmap.top

C#:   // 单行；/* 多行 */
来源：http://iea.hesvh.cn

[A15] 空值判断与默认值
来源：http://igy.xuanzx.com

Py:   value = data or "默认值"
来源：http://hsf.xylfe.cn

PHP:  $value = $data ?? "默认值";
来源：http://bsr.hongshengwenyu.top

JS:   const value = data ?? "默认值";
来源：http://nds.birdmap.top

TS:   const value = data ?? "默认值";
来源：http://uba.sysykeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pif.jiagoushi.top

Go:   if data == "" { data = "默认值" }
来源：http://alc.sjlbkw.cn

Ruby: value = data || "默认值"
来源：http://naf.guowangkeji.top

C#:   var value = data ?? "默认值";
来源：http://qmq.jinqigfzy.top

[A16] 真假值判断规则
来源：http://qlb.yuanzhike.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ldf.aizwys.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://knx.tianlin.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wgn.daxiang520.top

TS:   if (!x) {}
来源：http://mrs.aibaodan.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gpr.jianghu66.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://img.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://xmw.yj20258888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ffj.shuidangran.top

[A17] 位运算
来源：http://mvb.havefunace.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lum.yj20258888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rhj.ywan-chungtsiang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://roi.shanyushiyangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ruh.fzhhl.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://csv.aibaodan.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://afw.bjfxy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lga.pycfn.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nxt.ydzc1.top


<!-- 参考信息 -->