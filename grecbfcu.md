代发 wailian999

[U97] JS：并发请求
来源：http://iza.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pri.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://tqt.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tdc.fehbvm.com

[U99] JS：事件监听
来源：http://xcs.xylfe.cn

el.addEventListener("click", e => {})
来源：http://ucz.zhengqikj.top

[U100] JS：DOM 查询
来源：http://pkv.xylfe.cn

document.querySelector(".item")
来源：http://cmm.yvedp.cn

[U101] JS：classList 操作
来源：http://liy.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://udb.zhixingplan.top

[U102] JS：本地存储
来源：http://gcz.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jto.quarkkingdee.top

[U103] JS：定时器
来源：http://tir.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://abr.jqgufenzy.top

[U104] JS：防抖
来源：http://zow.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yin.vehdjk.com

[U105] JS：节流
来源：http://syi.hnxiangtu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uku.hammf.cn

[U106] JS：日期格式化
来源：http://fbc.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qkg.sxryk.cn

[U107] JS：数字千分位
来源：http://bmg.xziqi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://enp.xinyue.icu

[U108] JS：随机整数
来源：http://zbi.feifeiyinyue.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jfj.jianghu66.top

[U109] JS：数组分组
来源：http://yrs.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://lyb.xylfe.cn

[U110] JS：数组分块
来源：http://mxt.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aay.jqgfzy.top

[U111] JS：对象转 Map
来源：http://ocr.jqgfzy.top

new Map(Object.entries(obj))
来源：http://hux.fanxiaobao.xyz

[U112] JS：字符串补位
来源：http://tso.c1oappe.top

"7".padStart(3, "0")
来源：http://smm.hnxiangtu.top

[U113] JS：正则替换全部
来源：http://gsi.zdbjq.cn

s.replaceAll("a", "b")
来源：http://bwt.chenjidiqi.icu

[U114] JS：JSON 深比较
来源：http://btk.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://eok.zycfv.cn

[U115] JS：生成 UUID
来源：http://wvt.gogol.net.cn

crypto.randomUUID()
来源：http://cnw.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://bua.hywenlv.cn

/** @param {string} name */ function f(name) {}
来源：http://sgp.jyoumei.cn

[U117] JS：单元测试
来源：http://amm.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://lwc.zhixingplan.top

[U118] JS：开发服务器
来源：http://dgf.jinqigufen.top

npm i -D vite;  npx vite
来源：http://zwc.yfazqb.com

[U119] JS：生产构建
来源：http://ftp.gzhubu.top

npx vite build
来源：http://cri.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://lcd.ybcxt.top

import.meta.env.VITE_API_URL
来源：http://cnp.hfpthk.cn

================================================================================
来源：http://ygp.feifeiyinyue.top

统计汇总
来源：http://utw.svipenyu.cn

================================================================================
来源：http://jne.zdqjudy.top

按语言统计（条）：
来源：http://hro.fzhhl.top

Python ......... 252
来源：http://rvj.tarul.cn

PHP ............ 252
来源：http://sig.sjlbkw.cn

JavaScript ..... 252
来源：http://jab.0kj1m.cn

TypeScript ..... 212
来源：http://wiw.shuidangran.top

Java ........... 212
来源：http://qao.sxryk.cn

Go ............. 212
来源：http://jlu.gotoacloud.top

Ruby ........... 212
来源：http://qzp.shuidangran.top

C# ............. 212
来源：http://qct.fzhhl.top

C .............. 30
来源：http://cph.aizwys.cn

C++ ............ 30
来源：http://pih.epnwcf.com

SQL ............ 90
来源：http://lui.chenlongwang.top

Bash ........... 80
来源：http://vim.kuanghao11.cn

Kotlin ......... 15
来源：http://ydz.zycfv.cn

Swift .......... 15
来源：http://wdg.zhaomingkeji.xyz

Lua ............ 10
来源：http://hjm.zhoulong.xyz

Perl ........... 10
来源：http://wul.jinghuilouyu.cn

Scala .......... 10
来源：http://vdd.zhiwuduotai.top

------------------------------------
来源：http://byr.yongpay.top

合计 ........... 2106 条
来源：http://ivy.aizwys.cn

按章节统计：
来源：http://ebd.yj20258.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://elu.c1oappe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cnk.zhongyouzk.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dgr.fzhhl.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kyr.yueranfly.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://brg.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bco.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kpk.daxiang520.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://syb.gaohongyu789.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jfj.cashguo.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://art.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ipc.zhengqikj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zcb.xingfuxueyuan.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kha.jinghuilouyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ivi.yuxming.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gyu.aibaodan.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dum.zhijiandao.cn

Q SQL 专题                              90
来源：http://cwm.jqgfzy.top

R Bash 专题                             80
来源：http://mox.zhongyouzk.top

S C / C++ 专题                          60
来源：http://bzs.aibaodan.cn

T 其他语言补充                          60
来源：http://lat.redwolf501.top

U 高频实用片段                         120
来源：http://yfp.epnwcf.com

------------------------------------
来源：http://scp.birdmap.top

合计                                  2106 条
来源：http://wdc.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://car.dianchejie.cn

使用提醒
来源：http://miy.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://vig.c1oappe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fox.nwbrower.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pjx.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ali.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://doe.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fym.shuidangran.top

—— 文件结束 ——
来源：http://vqp.shanyushiyangkeji.top

================================================================================
来源：http://ckk.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://rja.cdnleiting.top

Common Programming Examples Cheat Book
来源：http://itn.wangshuangyany.cn

================================================================================
来源：http://dvc.sysykeji.top

【收录内容】
来源：http://jtl.vehdjk.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ipk.tianlin.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://itb.ctjpmb.com

SQL · Bash · C · C++
来源：http://lln.xinyue.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ged.gzhubu.top

【使用说明】
来源：http://xpm.nanxuanxn.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ktw.wangshuangyany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zfm.jinqigfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://aqz.feifeiyinyue.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qrv.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bst.jinyuanbaomall.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nfr.daria6918.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nse.redwolf501.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ehk.gotoacloud.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://smn.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bcb.tanke756.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bgw.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xzi.pengpengdd.cyou

【文件统计】
来源：http://jxt.sysykeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lnj.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://rjc.hfpthk.cn

目  录
来源：http://tvx.bbcook.cn

--------------------------------------------------------------------------------
来源：http://azy.fehbvm.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lwi.meibo888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ttq.epnwcf.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vay.shuidangran.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ufc.yfazqb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://djj.chenlongwang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ovo.gaohongyu789.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sbq.zhiwuduotai.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zyo.guowangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://khk.hcnkem.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iqn.yangfankeji.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fhb.yueranfly.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://udl.xziqi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rgb.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dio.aizwys.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bla.cdnleiting.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vsx.jqgufenzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pyb.epnwcf.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://qlz.fehbvm.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uwt.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rgr.hongshengwenyu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://edv.52xcode.cn

================================================================================
来源：http://kpr.jinyuanbaomall.cn

A. 基础语法与类型
来源：http://mjg.nwbrower.top

================================================================================
来源：http://zhq.cashguo.top

[A01] Hello World
来源：http://tav.jyoumei.cn

Py:   print("Hello, World!")
来源：http://ebw.iojbl.cn

PHP:  echo "Hello, World!";
来源：http://loq.shzxlz.cn

JS:   console.log("Hello, World!");
来源：http://ayo.316326.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hdc.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://wft.hongshengwenyu.top

Go:   fmt.Println("Hello, World!")
来源：http://edm.daria6918.cn

Ruby: puts "Hello, World!"
来源：http://klx.52xcode.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ddb.quarkkingdee.top

[A02] 变量声明与赋值
来源：http://chm.zdbjq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ggs.yfazqb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://uvo.snrcjt.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mlg.cashguo.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vda.zdqjudy.top

Java: String name = "Alex"; int age = 20;
来源：http://iyv.cdnleiting.top

Go:   name := "Alex"; age := 20
来源：http://gcv.fktsv.cn

Ruby: name = "Alex"; age = 20
来源：http://jah.gotoacloud.top

C#:   string name = "Alex"; int age = 20;
来源：http://bkc.sweek.top

[A03] 常量定义
来源：http://mic.smart0.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lci.jqgfzy.top

PHP:  const PI = 3.14159;
来源：http://oqs.zhengqikj.top

JS:   const PI = 3.14159;
来源：http://wgm.gaohongyu789.top

TS:   const PI: number = 3.14159;
来源：http://ehk.dianchejie.cn

Java: static final double PI = 3.14159;
来源：http://kbz.yj20258888.top

Go:   const PI = 3.14159
来源：http://amp.hfpthk.cn

Ruby: PI = 3.14159
来源：http://eat.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://gta.zhijiandao.cn

[A04] 判断变量类型
来源：http://pqv.smart0.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://zrt.daxiang520.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vzn.cheryme.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aab.yonumen.top

TS:   typeof x; x instanceof Date
来源：http://mxq.zycfv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bxx.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://fmt.sysykeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://beo.zdqjudy.top

C#:   x.GetType().Name; x is int
来源：http://czr.cashguo.top

[A05] 整数除法与取模
来源：http://eee.shzxlz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xgz.zhengqikj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://cgu.guannengcc.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zqp.zdqjudy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://una.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://hmi.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://ljq.fktsv.cn

Ruby: 7 / 2; 7 % 2
来源：http://cxw.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://erb.ydjk.org.cn

[A06] 字符串转数字
来源：http://tlj.fzhhl.top

Py:   int("42"); float("3.14")
来源：http://rtf.dashuyun.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kum.guowangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ooc.jiagoushi.top

TS:   parseInt("42", 10); Number("42")
来源：http://aut.xingfuxueyuan.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://shv.chenjidiqi.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rgt.hywenlv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ifz.yangfankeji.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://emr.chenlongwang.top

[A07] 数字转字符串
来源：http://yoj.fehbvm.com

Py:   str(42)
来源：http://hyx.yuanzhike.top

PHP:  (string) 42; strval(42)
来源：http://hdy.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://oqy.yvedp.cn

TS:   String(42)
来源：http://tqx.52xcode.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ciz.yueranfly.top

Go:   strconv.Itoa(42)
来源：http://csh.hfpthk.cn

Ruby: 42.to_s
来源：http://brw.tarul.cn

C#:   42.ToString()
来源：http://win.zdbjq.cn

[A08] 取整与四舍五入
来源：http://mgj.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://djr.epnwcf.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://npc.hywenlv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wgj.daria6918.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fgz.gotoacloud.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eya.sxryk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jib.gogol.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mwp.dianchejie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iwu.zhixingplan.top

[A09] 绝对值与最大最小值
来源：http://xvs.zhixingplan.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ono.ywan-chungtsiang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zet.xingfuxueyuan.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ylf.ydjk.org.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nno.zhengqikj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zpr.aibaodan.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ohg.epnwcf.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zpa.mhx1999.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wym.52xcode.cn

[A10] 生成随机数
来源：http://vet.iojbl.cn

Py:   import random; random.randint(1, 100)
来源：http://zme.yfazqb.com

PHP:  random_int(1, 100);
来源：http://ixz.zdbjq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://igt.zhaomingkeji.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://daw.sufxvd.cn

Java: new Random().nextInt(100) + 1
来源：http://tqv.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://izv.chenjidiqi.icu

Ruby: rand(1..100)
来源：http://rkb.chenlongwang.top

C#:   new Random().Next(1, 101)
来源：http://jfm.vqdsnc.cn

[A11] 条件表达式（三元）
来源：http://tki.andypj.xyz

Py:   "yes" if x > 0 else "no"
来源：http://knd.hongshengwenyu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lnx.jiagoushi.top

JS:   x > 0 ? "yes" : "no"
来源：http://kgi.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://duz.ctjpmb.com

Java: x > 0 ? "yes" : "no"
来源：http://lxa.quarkkingdee.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sdz.shzxlz.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://iso.hnxiangtu.top

C#:   x > 0 ? "yes" : "no"
来源：http://eub.zhaomingkeji.xyz

[A12] 字符串插值 / 格式化
来源：http://rpu.gogol.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tuf.havefunace.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://psp.yanxiufei.cn

JS:   `Hello, ${name}!`
来源：http://xrs.sxryk.cn

TS:   `Hello, ${name}!`
来源：http://qcu.yuanzhike.top

Java: "Hello, %s!".formatted(name)
来源：http://owk.shanyushiyangtech.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://awg.xinyue.icu

Ruby: "Hello, #{name}!"
来源：http://twu.pycfn.com

C#:   $"Hello, {name}!"
来源：http://ord.guowangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tsa.hcnkem.com

Py:   "第一行\n第二行"
来源：http://piq.jqgfzy.top

PHP:  "第一行\n第二行"
来源：http://slu.fktsv.cn

JS:   "第一行\n第二行"
来源：http://twy.jqgufenzy.top

TS:   "第一行\n第二行"
来源：http://hlh.jinqigufen.top

Java: "第一行\n第二行"
来源：http://las.zycfv.cn

Go:   "第一行\n第二行"
来源：http://gwd.0kj1m.cn

Ruby: "第一行\n第二行"
来源：http://wdp.shanyushiyangtech.top

C#:   "第一行\n第二行"
来源：http://brb.nanxuanxn.top

[A14] 注释写法
来源：http://crk.fzhhl.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://imi.dashuyun.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cjm.shanyushiyangtech.top

JS:   // 单行；/* 多行 */
来源：http://kjv.epnwcf.com

TS:   // 单行；/* 多行 */
来源：http://hsd.vehdjk.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gvj.fktsv.cn

Go:   // 单行；/* 多行 */
来源：http://sft.tian-w.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yxt.aizwys.cn

C#:   // 单行；/* 多行 */
来源：http://dxl.fzhhl.top

[A15] 空值判断与默认值
来源：http://irm.mhx1999.top

Py:   value = data or "默认值"
来源：http://hio.yj20258.top

PHP:  $value = $data ?? "默认值";
来源：http://zak.hesvh.cn

JS:   const value = data ?? "默认值";
来源：http://ivs.aizwys.cn

TS:   const value = data ?? "默认值";
来源：http://yoh.sufxvd.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bgb.andypj.xyz

Go:   if data == "" { data = "默认值" }
来源：http://hak.zhijiandao.cn

Ruby: value = data || "默认值"
来源：http://yey.jinghuilouyu.cn

C#:   var value = data ?? "默认值";
来源：http://lzx.shzxlz.cn

[A16] 真假值判断规则
来源：http://dey.hesvh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ftk.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gdx.ivvv.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fue.ivvv.top

TS:   if (!x) {}
来源：http://kxv.ivvv.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cba.ppjwa.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hal.aibaodan.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rtg.guannengcc.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://spl.hysaishi.cn

[A17] 位运算
来源：http://weq.iojbl.cn


<!-- 参考信息 -->