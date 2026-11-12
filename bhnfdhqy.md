代发 wailian999

[U101] JS：classList 操作
来源：http://hbv.bjfxy.top

el.classList.toggle("active")
来源：http://ccv.yongpay.top

[U102] JS：本地存储
来源：http://glg.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dho.fehbvm.com

[U103] JS：定时器
来源：http://dhx.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rrr.tarul.cn

[U104] JS：防抖
来源：http://uaw.jyoumei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gcq.smart0.xyz

[U105] JS：节流
来源：http://poi.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://svn.jlsjyb.cn

[U106] JS：日期格式化
来源：http://rbl.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://boj.yangfankeji.com

[U107] JS：数字千分位
来源：http://exw.hywenlv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yhf.zhongyouzk.top

[U108] JS：随机整数
来源：http://pdr.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hke.zhongyouzk.top

[U109] JS：数组分组
来源：http://zja.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://tpv.yangfankeji.com

[U110] JS：数组分块
来源：http://owg.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aww.pycfn.com

[U111] JS：对象转 Map
来源：http://svu.ydjk.org.cn

new Map(Object.entries(obj))
来源：http://iie.316326.xyz

[U112] JS：字符串补位
来源：http://jrk.wangshuangyany.cn

"7".padStart(3, "0")
来源：http://kxa.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://bfj.pycfn.com

s.replaceAll("a", "b")
来源：http://jrf.andypj.xyz

[U114] JS：JSON 深比较
来源：http://lcw.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jfq.hnqzz.top

[U115] JS：生成 UUID
来源：http://ilu.ivvv.top

crypto.randomUUID()
来源：http://sex.smart0.xyz

[U116] JS：类型检查（JSDoc）
来源：http://nio.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://mcc.smart0.xyz

[U117] JS：单元测试
来源：http://syv.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://wme.hesvh.cn

[U118] JS：开发服务器
来源：http://hnz.fengsongda.top

npm i -D vite;  npx vite
来源：http://igj.jinyuanbaomall.cn

[U119] JS：生产构建
来源：http://wks.haohaochexian.top

npx vite build
来源：http://qfv.shzxlz.cn

[U120] JS：读取环境变量（Vite）
来源：http://lkq.cheryme.top

import.meta.env.VITE_API_URL
来源：http://lmc.xingfuxueyuan.xyz

================================================================================
来源：http://bfj.daxiang520.top

统计汇总
来源：http://mlj.hysaishi.cn

================================================================================
来源：http://nhs.bbcook.cn

按语言统计（条）：
来源：http://qrx.hnxiangtu.top

Python ......... 252
来源：http://hmz.vqdsnc.cn

PHP ............ 252
来源：http://nge.xuanzx.com

JavaScript ..... 252
来源：http://bet.ppjwa.cn

TypeScript ..... 212
来源：http://lip.zhaomingkeji.xyz

Java ........... 212
来源：http://oqq.tian-w.cn

Go ............. 212
来源：http://soc.vqdsnc.cn

Ruby ........... 212
来源：http://jdi.mhx1999.top

C# ............. 212
来源：http://frb.cdnleiting.top

C .............. 30
来源：http://ghw.cucudq.cn

C++ ............ 30
来源：http://mbs.chenjidiqi.icu

SQL ............ 90
来源：http://uhy.zdbjq.cn

Bash ........... 80
来源：http://ntp.meibo888.top

Kotlin ......... 15
来源：http://gpp.sjlbkw.cn

Swift .......... 15
来源：http://mpr.zhijiandao.cn

Lua ............ 10
来源：http://fnx.fengsongda.top

Perl ........... 10
来源：http://sio.kuanghao11.cn

Scala .......... 10
来源：http://fqt.9152youxi.cn

------------------------------------
来源：http://mko.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://ber.hysaishi.cn

按章节统计：
来源：http://ygy.dianchejie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://amp.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ypq.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vor.chenlongwang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vek.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jyd.nanxinkj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zpp.yueranfly.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qkx.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eom.hysaishi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dkt.cdnleiting.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rdr.jianghu66.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cem.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wrd.ydzc1.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jsk.nanxinkj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hha.iojbl.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lzd.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tfe.yj202588.top

Q SQL 专题                              90
来源：http://cvl.cqqwz.cn

R Bash 专题                             80
来源：http://cah.yvedp.cn

S C / C++ 专题                          60
来源：http://tmg.shanyushiyangtech.top

T 其他语言补充                          60
来源：http://rqh.zdqjudy.top

U 高频实用片段                         120
来源：http://whv.shzxlz.cn

------------------------------------
来源：http://coe.sysykeji.top

合计                                  2106 条
来源：http://sfk.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://eod.hnqzz.top

使用提醒
来源：http://vpn.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://gsd.jinyuanbaomall.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jpm.iojbl.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kzt.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nhc.xinyue.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://dse.fzhhl.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gay.yj20258.top

—— 文件结束 ——
来源：http://alz.zhixingplan.top

================================================================================
来源：http://lvp.sxryk.cn

程序语言常见例子速查手册（2024 版）
来源：http://ido.gaohongyu789.top

Common Programming Examples Cheat Book
来源：http://ccd.birdmap.top

================================================================================
来源：http://ecc.zhiwuduotai.top

【收录内容】
来源：http://won.havefunace.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ial.ywan-chungtsiang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qqz.ppjwa.cn

SQL · Bash · C · C++
来源：http://bin.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qpu.sxryk.cn

【使用说明】
来源：http://maj.zhongyouzk.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://urz.pengpengdd.cyou

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dwp.ydzc1.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cpc.smart0.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hqs.hongshengwenyu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xze.hammf.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gsg.fengsongda.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tkk.yuxming.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://szx.sysykeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mku.ppjwa.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ciw.yueranfly.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gmv.nanxinkj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bgv.mhx1999.top

【文件统计】
来源：http://vhu.ivvv.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eap.mhx1999.top

--------------------------------------------------------------------------------
来源：http://nbw.redwolf501.top

目  录
来源：http://gqz.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://kml.kuanghao11.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ufd.sufxvd.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tft.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nuq.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cwa.jianghu66.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kkq.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mup.tian-w.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nba.vehdjk.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ggc.shuidangran.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sjl.yuxming.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hbb.tanke756.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dje.aizwys.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cju.nanxuanxn.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vxg.zycfv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iiv.dianchejie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rgf.aibaodan.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hdb.aibaodan.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bbw.shzxlz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yym.birdmap.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jmp.xuetiantiany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uwy.quarkkingdee.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vvb.sufxvd.cn

================================================================================
来源：http://jhk.yangfankeji.com

A. 基础语法与类型
来源：http://dle.cqqwz.cn

================================================================================
来源：http://ncl.52xcode.cn

[A01] Hello World
来源：http://ecl.cheryme.top

Py:   print("Hello, World!")
来源：http://ity.gogol.net.cn

PHP:  echo "Hello, World!";
来源：http://rnb.jqgfzy.top

JS:   console.log("Hello, World!");
来源：http://qkv.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wcm.sufxvd.cn

Java: System.out.println("Hello, World!");
来源：http://ifi.cdnleiting.top

Go:   fmt.Println("Hello, World!")
来源：http://vax.yuanzhike.top

Ruby: puts "Hello, World!"
来源：http://hss.yfazqb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://sjb.yanxiufei.cn

[A02] 变量声明与赋值
来源：http://ylk.shanyushiyangtech.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mow.havefunace.top

PHP:  $name = "Alex"; $age = 20;
来源：http://djd.jinqigufen.top

JS:   let name = "Alex"; const age = 20;
来源：http://ltl.daria6918.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fna.jlsjyb.cn

Java: String name = "Alex"; int age = 20;
来源：http://yli.aizwys.cn

Go:   name := "Alex"; age := 20
来源：http://wdg.guowangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://zxb.chenzaomai.com

C#:   string name = "Alex"; int age = 20;
来源：http://vpr.shanyushiyangkeji.top

[A03] 常量定义
来源：http://ris.hesvh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ryx.sysykeji.top

PHP:  const PI = 3.14159;
来源：http://ntn.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://hif.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://iwb.yonumen.top

Java: static final double PI = 3.14159;
来源：http://yil.gzhubu.top

Go:   const PI = 3.14159
来源：http://fxl.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://icd.andypj.xyz

C#:   const double PI = 3.14159;
来源：http://sqx.jlsjyb.cn

[A04] 判断变量类型
来源：http://hfj.hcnkem.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ksm.pycfn.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hce.vqdsnc.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fuk.jqgufenzy.top

TS:   typeof x; x instanceof Date
来源：http://ots.vqdsnc.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jwt.dianchejie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lrq.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mnm.gogol.net.cn

C#:   x.GetType().Name; x is int
来源：http://yto.guannengcc.top

[A05] 整数除法与取模
来源：http://apf.dashuyun.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lhh.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://llp.aibaodan.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zeh.yj20258888.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rgi.zhijiandao.cn

Java: 7 / 2; 7 % 2
来源：http://awc.iojbl.cn

Go:   7 / 2; 7 % 2
来源：http://zcz.wangshuangyany.cn

Ruby: 7 / 2; 7 % 2
来源：http://dub.xuanzx.com

C#:   7 / 2; 7 % 2
来源：http://woy.tarul.cn

[A06] 字符串转数字
来源：http://dbi.birdmap.top

Py:   int("42"); float("3.14")
来源：http://shv.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wri.daria6918.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eev.daria6918.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lhp.tarul.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xaj.cucudq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rvw.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bbg.tanke756.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jsw.meibo888.top

[A07] 数字转字符串
来源：http://pkx.hongshengwenyu.top

Py:   str(42)
来源：http://mal.yj20258.top

PHP:  (string) 42; strval(42)
来源：http://zsg.hcnkem.com

JS:   String(42); (42).toString()
来源：http://fzk.smart0.xyz

TS:   String(42)
来源：http://lfh.fanxiaobao.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://fqt.hnqzz.top

Go:   strconv.Itoa(42)
来源：http://vyx.jlsjyb.cn

Ruby: 42.to_s
来源：http://krd.epnwcf.com

C#:   42.ToString()
来源：http://nnu.hywenlv.cn

[A08] 取整与四舍五入
来源：http://ebq.andypj.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ugf.yuxming.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://twy.yanxiufei.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jis.cucudq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xmr.uphjek.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ytq.ybcxt.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ecb.hfpthk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ufw.jinqigufen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ymw.sxryk.cn

[A09] 绝对值与最大最小值
来源：http://dqg.ehwqpu.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uqr.fengsongda.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xrm.yueranfly.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ysf.feifeiyinyue.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hwg.ppjwa.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blf.smart0.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xqt.snrcjt.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://stu.dashuyun.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fwi.fengsongda.top

[A10] 生成随机数
来源：http://hki.sweek.top

Py:   import random; random.randint(1, 100)
来源：http://dsx.jinyuanbaomall.cn

PHP:  random_int(1, 100);
来源：http://nkh.hesvh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rjc.shanyushiyangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zrd.jyoumei.cn

Java: new Random().nextInt(100) + 1
来源：http://kfq.vqdsnc.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vfv.yvedp.cn

Ruby: rand(1..100)
来源：http://wxf.chenjidiqi.icu

C#:   new Random().Next(1, 101)
来源：http://upy.bbcook.cn

[A11] 条件表达式（三元）
来源：http://wqr.zhoulong.xyz

Py:   "yes" if x > 0 else "no"
来源：http://rpk.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qfs.vqdsnc.cn

JS:   x > 0 ? "yes" : "no"
来源：http://isv.ybcxt.top

TS:   x > 0 ? "yes" : "no"
来源：http://kcr.uphjek.com

Java: x > 0 ? "yes" : "no"
来源：http://uzu.fktsv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://niu.uphjek.com

Ruby: x > 0 ? "yes" : "no"
来源：http://wbw.yuanzhike.top

C#:   x > 0 ? "yes" : "no"
来源：http://mfy.vehdjk.com

[A12] 字符串插值 / 格式化
来源：http://kqw.yj202588.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://epc.fktsv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mlk.chenlongwang.top

JS:   `Hello, ${name}!`
来源：http://kap.hfpthk.cn

TS:   `Hello, ${name}!`
来源：http://qjw.haohaochexian.top

Java: "Hello, %s!".formatted(name)
来源：http://jix.birdmap.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qnl.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://bbz.sweek.top

C#:   $"Hello, {name}!"
来源：http://yim.zhengqikj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ned.yfazqb.com

Py:   "第一行\n第二行"
来源：http://zio.mhx1999.top

PHP:  "第一行\n第二行"
来源：http://iih.kuanghao11.cn

JS:   "第一行\n第二行"
来源：http://fxi.jinqigufen.top

TS:   "第一行\n第二行"
来源：http://hvp.ybcxt.top

Java: "第一行\n第二行"
来源：http://jxs.hammf.cn

Go:   "第一行\n第二行"
来源：http://ubg.hysaishi.cn

Ruby: "第一行\n第二行"
来源：http://eyq.fanxiaobao.xyz

C#:   "第一行\n第二行"
来源：http://cnx.yanxiufei.cn

[A14] 注释写法
来源：http://vnj.svipenyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ots.redwolf501.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://bnt.hammf.cn

JS:   // 单行；/* 多行 */
来源：http://agf.gaohongyu789.top

TS:   // 单行；/* 多行 */
来源：http://dss.aibaodan.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jlc.meibo888.top

Go:   // 单行；/* 多行 */
来源：http://fpd.jianghu66.top

Ruby: # 单行；=begin 多行 =end
来源：http://myd.yanxiufei.cn

C#:   // 单行；/* 多行 */
来源：http://nau.hesvh.cn

[A15] 空值判断与默认值
来源：http://eeu.guowangkeji.top

Py:   value = data or "默认值"
来源：http://nyn.tianlin.xyz

PHP:  $value = $data ?? "默认值";
来源：http://qio.yongpay.top

JS:   const value = data ?? "默认值";
来源：http://wnj.jlsjyb.cn

TS:   const value = data ?? "默认值";
来源：http://bhi.shanyushiyangtech.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://srr.chenlongwang.top

Go:   if data == "" { data = "默认值" }
来源：http://vvl.zhixingplan.top

Ruby: value = data || "默认值"
来源：http://suv.jiagoushi.top

C#:   var value = data ?? "默认值";
来源：http://mob.tanke756.top

[A16] 真假值判断规则
来源：http://elc.cashguo.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lsd.sufxvd.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://irp.shzxlz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kba.vehdjk.com

TS:   if (!x) {}
来源：http://lfz.yuxming.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pgh.bjfxy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://smi.sjlbkw.cn

Ruby: unless x            # nil 与 false 为假
来源：http://agb.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ole.yfazqb.com

[A17] 位运算
来源：http://jtb.yj202588.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ida.nwbrower.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vho.yj20258888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vyh.fzhhl.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://str.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qrd.jinqigufen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ckr.tanke756.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xai.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vqf.zhaomingkeji.xyz


<!-- 参考信息 -->