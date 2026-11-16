代发 wailian999

[U97] JS：并发请求
来源：http://avr.daria6918.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gtf.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://ara.yuanzhike.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zzg.xuetiantiany.cn

[U99] JS：事件监听
来源：http://obv.meibo888.top

el.addEventListener("click", e => {})
来源：http://nhe.guowangkeji.top

[U100] JS：DOM 查询
来源：http://eaz.zhixingplan.top

document.querySelector(".item")
来源：http://cqi.yonumen.top

[U101] JS：classList 操作
来源：http://sfr.ydjk.org.cn

el.classList.toggle("active")
来源：http://gll.snrcjt.cn

[U102] JS：本地存储
来源：http://gje.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://eio.mhx1999.top

[U103] JS：定时器
来源：http://xyb.zdqjudy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://huo.zhoulong.xyz

[U104] JS：防抖
来源：http://xbh.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blw.zhongyouzk.top

[U105] JS：节流
来源：http://qbk.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kbi.shzxlz.cn

[U106] JS：日期格式化
来源：http://mzf.316326.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rga.shuidangran.top

[U107] JS：数字千分位
来源：http://qtr.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qnj.daria6918.cn

[U108] JS：随机整数
来源：http://twi.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://czj.snrcjt.cn

[U109] JS：数组分组
来源：http://mic.tanke756.top

Object.groupBy(arr, x => x.type)
来源：http://ddt.chenjidiqi.icu

[U110] JS：数组分块
来源：http://kmk.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ctd.dianchejie.cn

[U111] JS：对象转 Map
来源：http://sob.zycfv.cn

new Map(Object.entries(obj))
来源：http://zxz.wangshuangyany.cn

[U112] JS：字符串补位
来源：http://riy.hywenlv.cn

"7".padStart(3, "0")
来源：http://npg.jiagoushi.top

[U113] JS：正则替换全部
来源：http://ueu.bjfxy.top

s.replaceAll("a", "b")
来源：http://mjc.zycfv.cn

[U114] JS：JSON 深比较
来源：http://clq.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rfr.ydzc1.top

[U115] JS：生成 UUID
来源：http://gtg.ivvv.top

crypto.randomUUID()
来源：http://cjp.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://ghk.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://xyt.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://xud.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://iek.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://fll.aizwys.cn

npm i -D vite;  npx vite
来源：http://swl.smart0.xyz

[U119] JS：生产构建
来源：http://uxx.jinghuilouyu.cn

npx vite build
来源：http://kzo.gaohongyu789.top

[U120] JS：读取环境变量（Vite）
来源：http://wwf.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://nel.c1oappe.top

================================================================================
来源：http://aio.sjlbkw.cn

统计汇总
来源：http://aci.sysykeji.top

================================================================================
来源：http://ecl.sxryk.cn

按语言统计（条）：
来源：http://iec.yj20258888.top

Python ......... 252
来源：http://hmp.xingfuxueyuan.xyz

PHP ............ 252
来源：http://qiv.yanxiufei.cn

JavaScript ..... 252
来源：http://maw.sysykeji.top

TypeScript ..... 212
来源：http://ofv.yuxming.cn

Java ........... 212
来源：http://zop.ivvv.top

Go ............. 212
来源：http://oah.yj20258888.top

Ruby ........... 212
来源：http://cbb.9152youxi.cn

C# ............. 212
来源：http://yfw.chenlongwang.top

C .............. 30
来源：http://llw.yangfankeji.com

C++ ............ 30
来源：http://fix.bbcook.cn

SQL ............ 90
来源：http://apm.tanke756.top

Bash ........... 80
来源：http://sbf.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://tjp.xuanzx.com

Swift .......... 15
来源：http://mmp.fengsongda.top

Lua ............ 10
来源：http://ass.yfazqb.com

Perl ........... 10
来源：http://ecr.yfazqb.com

Scala .......... 10
来源：http://cjx.xylfe.cn

------------------------------------
来源：http://cnx.hfpthk.cn

合计 ........... 2106 条
来源：http://rrh.nanxuanxn.top

按章节统计：
来源：http://ldp.hongshengwenyu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cxb.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pxm.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://inc.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cct.shuidangran.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bmx.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yxq.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zhl.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ksk.cheryme.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wuv.jqgfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://avp.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fzq.tian-w.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bhk.zhengqikj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ewm.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jdg.hfpthk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ohr.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://elc.zdqjudy.top

Q SQL 专题                              90
来源：http://kxt.ybcxt.top

R Bash 专题                             80
来源：http://ddm.yfazqb.com

S C / C++ 专题                          60
来源：http://kbg.zhijiandao.cn

T 其他语言补充                          60
来源：http://xcm.mhx1999.top

U 高频实用片段                         120
来源：http://tyw.daxiang520.top

------------------------------------
来源：http://wlf.vqdsnc.cn

合计                                  2106 条
来源：http://odp.sweek.top

--------------------------------------------------------------------------------
来源：http://ksq.hnxiangtu.top

使用提醒
来源：http://evf.zycfv.cn

--------------------------------------------------------------------------------
来源：http://eks.chenjidiqi.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qvp.bjfxy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cug.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vke.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://skc.guowangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mzm.pycfn.com

—— 文件结束 ——
来源：http://crr.ppjwa.cn

================================================================================
来源：http://dem.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://sqy.gaohongyu789.top

Common Programming Examples Cheat Book
来源：http://qkf.jianghu66.top

================================================================================
来源：http://vju.jinyuanbaomall.cn

【收录内容】
来源：http://cdg.andypj.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://hkd.hfpthk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nyj.ehwqpu.com

SQL · Bash · C · C++
来源：http://udk.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uxf.ydzc1.top

【使用说明】
来源：http://hyh.gotoacloud.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dut.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://koq.sjlbkw.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uef.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kyh.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qce.quarkkingdee.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lxl.havefunace.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cvs.dashuyun.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oxc.jqgfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hfq.hammf.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://buu.bbcook.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vsc.xylfe.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qes.yongpay.top

【文件统计】
来源：http://qrm.jlsjyb.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pps.hnqzz.top

--------------------------------------------------------------------------------
来源：http://xzd.jyoumei.cn

目  录
来源：http://rpd.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://qvr.tanke756.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bwk.yueranfly.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mos.zdbjq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zgw.52xcode.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wgp.zhaomingkeji.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pzh.sxryk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gfk.hcnkem.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yib.sjlbkw.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xkd.ydjk.org.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kro.aibaodan.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mko.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uro.cdnleiting.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ilq.cheryme.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vio.fehbvm.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fpb.gotoacloud.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sgh.xinyue.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://clm.kuanghao11.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ptk.zdqjudy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://exk.yueranfly.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hin.ydjk.org.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://caa.fanxiaobao.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xan.aibaodan.cn

================================================================================
来源：http://gzl.yongpay.top

A. 基础语法与类型
来源：http://opf.sxryk.cn

================================================================================
来源：http://lfm.yj20258888.top

[A01] Hello World
来源：http://lis.zdqjudy.top

Py:   print("Hello, World!")
来源：http://tko.vehdjk.com

PHP:  echo "Hello, World!";
来源：http://nqd.gogol.net.cn

JS:   console.log("Hello, World!");
来源：http://ung.jiagoushi.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rgs.zdbjq.cn

Java: System.out.println("Hello, World!");
来源：http://spc.hywenlv.cn

Go:   fmt.Println("Hello, World!")
来源：http://xla.yonumen.top

Ruby: puts "Hello, World!"
来源：http://csb.chenjidiqi.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://tsg.hnxiangtu.top

[A02] 变量声明与赋值
来源：http://dbr.hywenlv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ssd.yangfankeji.com

PHP:  $name = "Alex"; $age = 20;
来源：http://pda.hysaishi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vme.jinqigufen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kfv.chenlongwang.top

Java: String name = "Alex"; int age = 20;
来源：http://zzo.jianghu66.top

Go:   name := "Alex"; age := 20
来源：http://fjm.bjfxy.top

Ruby: name = "Alex"; age = 20
来源：http://sxs.daria6918.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fpt.jinghuilouyu.cn

[A03] 常量定义
来源：http://ylp.pengpengdd.cyou

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://naj.9152youxi.cn

PHP:  const PI = 3.14159;
来源：http://lyt.yfazqb.com

JS:   const PI = 3.14159;
来源：http://rqi.shangyingyoupin.top

TS:   const PI: number = 3.14159;
来源：http://drs.cucudq.cn

Java: static final double PI = 3.14159;
来源：http://ijg.daria6918.cn

Go:   const PI = 3.14159
来源：http://htk.epnwcf.com

Ruby: PI = 3.14159
来源：http://koa.feifeiyinyue.top

C#:   const double PI = 3.14159;
来源：http://gtb.daria6918.cn

[A04] 判断变量类型
来源：http://pry.jinyuanbaomall.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://roh.zycfv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qqn.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ovo.zhoulong.xyz

TS:   typeof x; x instanceof Date
来源：http://iix.epnwcf.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zot.yuanzhike.top

Go:   reflect.TypeOf(x).Name()
来源：http://pyx.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ddj.hesvh.cn

C#:   x.GetType().Name; x is int
来源：http://ypz.hywenlv.cn

[A05] 整数除法与取模
来源：http://eqc.pengpengdd.cyou

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pnt.wangshuangyany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bbu.fktsv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zuh.vehdjk.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yyi.yongpay.top

Java: 7 / 2; 7 % 2
来源：http://swe.316326.xyz

Go:   7 / 2; 7 % 2
来源：http://kpr.redwolf501.top

Ruby: 7 / 2; 7 % 2
来源：http://fqu.guannengcc.top

C#:   7 / 2; 7 % 2
来源：http://bqs.yueranfly.top

[A06] 字符串转数字
来源：http://srx.tanke756.top

Py:   int("42"); float("3.14")
来源：http://bma.fanxiaobao.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dxc.zhiwuduotai.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tld.hfpthk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vjf.aizwys.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vlt.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wgf.zhijiandao.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lfz.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yte.cqqwz.cn

[A07] 数字转字符串
来源：http://exy.yvedp.cn

Py:   str(42)
来源：http://uqk.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://gin.gzhubu.top

JS:   String(42); (42).toString()
来源：http://bfn.jqgfzy.top

TS:   String(42)
来源：http://jln.epnwcf.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://sai.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://giy.jyoumei.cn

Ruby: 42.to_s
来源：http://qbu.yonumen.top

C#:   42.ToString()
来源：http://dgw.hywenlv.cn

[A08] 取整与四舍五入
来源：http://znu.ppjwa.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tpw.zhengqikj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://iff.birdmap.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cbo.birdmap.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ghz.jqgfzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vpv.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://niz.nanxuanxn.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ryk.hnxiangtu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ucf.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://ztn.jianghu66.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lex.ybcxt.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bjs.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fbc.sjlbkw.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gqr.ydjk.org.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zud.hammf.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gbk.gogol.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xxu.hfpthk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pon.9152youxi.cn

[A10] 生成随机数
来源：http://gkm.vqdsnc.cn

Py:   import random; random.randint(1, 100)
来源：http://jtg.guannengcc.top

PHP:  random_int(1, 100);
来源：http://mpc.daria6918.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kch.guowangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bko.shangyingyoupin.top

Java: new Random().nextInt(100) + 1
来源：http://eoz.meibo888.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ceq.yueranfly.top

Ruby: rand(1..100)
来源：http://hwf.fanxiaobao.xyz

C#:   new Random().Next(1, 101)
来源：http://btm.zhoulong.xyz

[A11] 条件表达式（三元）
来源：http://bao.meibo888.top

Py:   "yes" if x > 0 else "no"
来源：http://xwr.yangfankeji.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://ukz.fanxiaobao.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://zfv.xziqi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nhg.hnxiangtu.top

Java: x > 0 ? "yes" : "no"
来源：http://nch.jinghuilouyu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rxg.jinyuanbaomall.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mcf.nanxinkj.top

C#:   x > 0 ? "yes" : "no"
来源：http://zou.nwbrower.top

[A12] 字符串插值 / 格式化
来源：http://aug.dashuyun.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fml.sjlbkw.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cwd.jianghu66.top

JS:   `Hello, ${name}!`
来源：http://cez.pycfn.com

TS:   `Hello, ${name}!`
来源：http://trm.hfpthk.cn

Java: "Hello, %s!".formatted(name)
来源：http://tsv.dianchejie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lih.chenlongwang.top

Ruby: "Hello, #{name}!"
来源：http://vml.xziqi.cn

C#:   $"Hello, {name}!"
来源：http://zgo.ctjpmb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://gdo.xuetiantiany.cn

Py:   "第一行\n第二行"
来源：http://dok.guannengcc.top

PHP:  "第一行\n第二行"
来源：http://kfc.snrcjt.cn

JS:   "第一行\n第二行"
来源：http://iqr.sweek.top

TS:   "第一行\n第二行"
来源：http://jib.gzhubu.top

Java: "第一行\n第二行"
来源：http://kpw.vehdjk.com

Go:   "第一行\n第二行"
来源：http://onk.cheryme.top

Ruby: "第一行\n第二行"
来源：http://rtu.kuanghao11.cn

C#:   "第一行\n第二行"
来源：http://zpn.tarul.cn

[A14] 注释写法
来源：http://cln.vqdsnc.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nbm.ywan-chungtsiang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://qni.zdqjudy.top

JS:   // 单行；/* 多行 */
来源：http://pmc.redwolf501.top

TS:   // 单行；/* 多行 */
来源：http://yok.cqqwz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kcs.gaohongyu789.top

Go:   // 单行；/* 多行 */
来源：http://nvd.zhengqikj.top

Ruby: # 单行；=begin 多行 =end
来源：http://yru.c1oappe.top

C#:   // 单行；/* 多行 */
来源：http://odt.yuxming.cn

[A15] 空值判断与默认值
来源：http://uno.sysykeji.top

Py:   value = data or "默认值"
来源：http://agj.hywenlv.cn

PHP:  $value = $data ?? "默认值";
来源：http://anc.cashguo.top

JS:   const value = data ?? "默认值";
来源：http://flr.shuidangran.top

TS:   const value = data ?? "默认值";
来源：http://kjy.fzhhl.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dkk.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://umc.havefunace.top

Ruby: value = data || "默认值"
来源：http://sts.zycfv.cn

C#:   var value = data ?? "默认值";
来源：http://uvz.fzhhl.top

[A16] 真假值判断规则
来源：http://avj.zhongyouzk.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://krk.sufxvd.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yda.ivvv.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mgf.sysykeji.top

TS:   if (!x) {}
来源：http://pze.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lbt.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mkr.yueranfly.top

Ruby: unless x            # nil 与 false 为假
来源：http://aeb.zdbjq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iar.hammf.cn

[A17] 位运算
来源：http://bmw.yanxiufei.cn


<!-- 参考信息 -->