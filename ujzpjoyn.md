代发 wailian999

[U97] JS：并发请求
来源：http://xzg.bjfxy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ihc.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://lpp.cqqwz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lyc.hnqzz.top

[U99] JS：事件监听
来源：http://zwo.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://cqq.shanyushiyangkeji.top

[U100] JS：DOM 查询
来源：http://jci.yongpay.top

document.querySelector(".item")
来源：http://leh.aizwys.cn

[U101] JS：classList 操作
来源：http://rmc.chenlongwang.top

el.classList.toggle("active")
来源：http://oxf.hywenlv.cn

[U102] JS：本地存储
来源：http://oid.zhoulong.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://spk.cheryme.top

[U103] JS：定时器
来源：http://jty.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tkq.zycfv.cn

[U104] JS：防抖
来源：http://aek.xuanzx.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zks.iojbl.cn

[U105] JS：节流
来源：http://nfb.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://etn.vehdjk.com

[U106] JS：日期格式化
来源：http://guo.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://odi.redwolf501.top

[U107] JS：数字千分位
来源：http://qff.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tqm.fengsongda.top

[U108] JS：随机整数
来源：http://cee.zhengqikj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://frk.hesvh.cn

[U109] JS：数组分组
来源：http://tyk.iojbl.cn

Object.groupBy(arr, x => x.type)
来源：http://dil.hongshengwenyu.top

[U110] JS：数组分块
来源：http://nue.mhx1999.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ltz.jqgufenzy.top

[U111] JS：对象转 Map
来源：http://uut.zhiwuduotai.top

new Map(Object.entries(obj))
来源：http://nzh.yanxiufei.cn

[U112] JS：字符串补位
来源：http://svh.daria6918.cn

"7".padStart(3, "0")
来源：http://yzz.dianchejie.cn

[U113] JS：正则替换全部
来源：http://mqa.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://lzw.sweek.top

[U114] JS：JSON 深比较
来源：http://btg.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ryu.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://bks.fktsv.cn

crypto.randomUUID()
来源：http://lih.52xcode.cn

[U116] JS：类型检查（JSDoc）
来源：http://vly.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://kqk.yangfankeji.com

[U117] JS：单元测试
来源：http://hnm.9152youxi.cn

npm i -D vitest;  npx vitest
来源：http://tur.mhx1999.top

[U118] JS：开发服务器
来源：http://cps.ctjpmb.com

npm i -D vite;  npx vite
来源：http://njj.hcnkem.com

[U119] JS：生产构建
来源：http://hmz.shuidangran.top

npx vite build
来源：http://ecp.wangshuangyany.cn

[U120] JS：读取环境变量（Vite）
来源：http://opl.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://bzt.guannengcc.top

================================================================================
来源：http://xcl.gzhubu.top

统计汇总
来源：http://qxd.pycfn.com

================================================================================
来源：http://fcc.ydzc1.top

按语言统计（条）：
来源：http://gjy.shzxlz.cn

Python ......... 252
来源：http://nfz.tarul.cn

PHP ............ 252
来源：http://jga.yonumen.top

JavaScript ..... 252
来源：http://zua.iojbl.cn

TypeScript ..... 212
来源：http://txk.ehwqpu.com

Java ........... 212
来源：http://gqf.sxryk.cn

Go ............. 212
来源：http://fsx.zhengqikj.top

Ruby ........... 212
来源：http://sbc.ydjk.org.cn

C# ............. 212
来源：http://rxn.jinyuanbaomall.cn

C .............. 30
来源：http://sgi.gaohongyu789.top

C++ ............ 30
来源：http://vjd.dianchejie.cn

SQL ............ 90
来源：http://ybx.tarul.cn

Bash ........... 80
来源：http://eel.yj20258888.top

Kotlin ......... 15
来源：http://wum.yvedp.cn

Swift .......... 15
来源：http://gbu.haohaochexian.top

Lua ............ 10
来源：http://lbk.shzxlz.cn

Perl ........... 10
来源：http://cqr.hcnkem.com

Scala .......... 10
来源：http://rtg.jinqigfzy.top

------------------------------------
来源：http://xfy.52xcode.cn

合计 ........... 2106 条
来源：http://zhh.xylfe.cn

按章节统计：
来源：http://exy.aibaodan.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qkv.yanxiufei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qqy.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hsk.zdbjq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rsk.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jet.pengpengdd.cyou

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mbu.jinqigufen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uso.pycfn.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://voc.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://thg.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cer.jinqigfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cux.9152youxi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://awm.fehbvm.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tlb.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gju.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://azt.kuanghao11.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://anj.9152youxi.cn

Q SQL 专题                              90
来源：http://wpw.redwolf501.top

R Bash 专题                             80
来源：http://xib.chenjidiqi.icu

S C / C++ 专题                          60
来源：http://uzm.vehdjk.com

T 其他语言补充                          60
来源：http://vnp.fzhhl.top

U 高频实用片段                         120
来源：http://wcj.gogol.net.cn

------------------------------------
来源：http://hve.chenjidiqi.icu

合计                                  2106 条
来源：http://cet.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://avx.xylfe.cn

使用提醒
来源：http://ynq.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://bhb.ehwqpu.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ina.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fnv.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oyu.0kj1m.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://abp.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ybi.ehwqpu.com

—— 文件结束 ——
来源：http://afw.mhx1999.top

================================================================================
来源：http://alu.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://ntf.nanxuanxn.top

Common Programming Examples Cheat Book
来源：http://khd.hysaishi.cn

================================================================================
来源：http://shk.iojbl.cn

【收录内容】
来源：http://svm.hnxiangtu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tmk.yfazqb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pdn.yueranfly.top

SQL · Bash · C · C++
来源：http://mgy.shanyushiyangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ktk.gaohongyu789.top

【使用说明】
来源：http://qug.chenzaomai.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ijm.dianchejie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wte.shanyushiyangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kas.zhaomingkeji.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wfh.xingfuxueyuan.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://oqy.gzhubu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dlp.shzxlz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://brg.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ncm.zhiwuduotai.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://udd.gotoacloud.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zvy.gotoacloud.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mgp.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fgd.hesvh.cn

【文件统计】
来源：http://bdm.bjfxy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vah.yuxming.cn

--------------------------------------------------------------------------------
来源：http://xfp.tian-w.cn

目  录
来源：http://pml.epnwcf.com

--------------------------------------------------------------------------------
来源：http://ouz.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://avj.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xxu.chenjidiqi.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://idt.hesvh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sdx.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kxb.birdmap.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://usc.haohaochexian.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bqu.tarul.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lnr.quarkkingdee.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://idy.shanyushiyangtech.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bot.c1oappe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vow.ydjk.org.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zrj.316326.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ocq.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wih.shuidangran.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kon.daria6918.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vih.yvedp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kkc.cqqwz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xed.hcnkem.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rty.yj20258888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lrb.birdmap.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zkj.zycfv.cn

================================================================================
来源：http://agp.jinghuilouyu.cn

A. 基础语法与类型
来源：http://kes.yuxming.cn

================================================================================
来源：http://jpq.andypj.xyz

[A01] Hello World
来源：http://cyu.snrcjt.cn

Py:   print("Hello, World!")
来源：http://nue.hammf.cn

PHP:  echo "Hello, World!";
来源：http://ppa.iojbl.cn

JS:   console.log("Hello, World!");
来源：http://gue.xingfuxueyuan.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nur.fktsv.cn

Java: System.out.println("Hello, World!");
来源：http://eik.gzhubu.top

Go:   fmt.Println("Hello, World!")
来源：http://olp.ppjwa.cn

Ruby: puts "Hello, World!"
来源：http://jse.zdqjudy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vkt.yongpay.top

[A02] 变量声明与赋值
来源：http://bwc.dianchejie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cdg.chenlongwang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ywl.smart0.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://fpk.bbcook.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nge.andypj.xyz

Java: String name = "Alex"; int age = 20;
来源：http://krt.yj202588.top

Go:   name := "Alex"; age := 20
来源：http://znt.zdqjudy.top

Ruby: name = "Alex"; age = 20
来源：http://ngg.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://lxc.uphjek.com

[A03] 常量定义
来源：http://ack.wangshuangyany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://plu.jianghu66.top

PHP:  const PI = 3.14159;
来源：http://qgr.iojbl.cn

JS:   const PI = 3.14159;
来源：http://ztf.cqqwz.cn

TS:   const PI: number = 3.14159;
来源：http://nlv.chenjidiqi.icu

Java: static final double PI = 3.14159;
来源：http://obm.xylfe.cn

Go:   const PI = 3.14159
来源：http://cgh.ivvv.top

Ruby: PI = 3.14159
来源：http://odo.ywan-chungtsiang.top

C#:   const double PI = 3.14159;
来源：http://ypi.xuanzx.com

[A04] 判断变量类型
来源：http://itr.bjfxy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://abo.yonumen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qah.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://muk.jianghu66.top

TS:   typeof x; x instanceof Date
来源：http://udg.shangyingyoupin.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jgi.xingfuxueyuan.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://dse.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jof.zhongyouzk.top

C#:   x.GetType().Name; x is int
来源：http://fmb.shangyingyoupin.top

[A05] 整数除法与取模
来源：http://vkn.xuanzx.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dib.yuxming.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yuu.xinyue.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qnz.dashuyun.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zic.jqgufenzy.top

Java: 7 / 2; 7 % 2
来源：http://wlo.ppjwa.cn

Go:   7 / 2; 7 % 2
来源：http://ysa.sjlbkw.cn

Ruby: 7 / 2; 7 % 2
来源：http://lis.vehdjk.com

C#:   7 / 2; 7 % 2
来源：http://cmj.tianlin.xyz

[A06] 字符串转数字
来源：http://jen.xuetiantiany.cn

Py:   int("42"); float("3.14")
来源：http://nzb.tarul.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ioj.xziqi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fiz.wangshuangyany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gyw.daria6918.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zgg.aibaodan.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ukg.zhijiandao.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zyr.pengpengdd.cyou

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uvb.hcnkem.com

[A07] 数字转字符串
来源：http://bzs.jqgufenzy.top

Py:   str(42)
来源：http://mpx.yongpay.top

PHP:  (string) 42; strval(42)
来源：http://krd.birdmap.top

JS:   String(42); (42).toString()
来源：http://shs.dashuyun.cn

TS:   String(42)
来源：http://wed.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://fon.ppjwa.cn

Go:   strconv.Itoa(42)
来源：http://log.hammf.cn

Ruby: 42.to_s
来源：http://awk.haohaochexian.top

C#:   42.ToString()
来源：http://brb.meibo888.top

[A08] 取整与四舍五入
来源：http://pof.ehwqpu.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://non.meibo888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fhf.jianghu66.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ehh.chenlongwang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tdv.snrcjt.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bkq.ppjwa.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mjk.ybcxt.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fwt.dashuyun.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fsz.jinyuanbaomall.cn

[A09] 绝对值与最大最小值
来源：http://nbd.yuxming.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gbz.snrcjt.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yqo.fktsv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lvu.yanxiufei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wwh.9152youxi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wvj.yueranfly.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vwe.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ebp.zhengqikj.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cvl.iojbl.cn

[A10] 生成随机数
来源：http://vtc.tian-w.cn

Py:   import random; random.randint(1, 100)
来源：http://ydg.guowangkeji.top

PHP:  random_int(1, 100);
来源：http://kto.smart0.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://imi.yj20258888.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://biq.jianghu66.top

Java: new Random().nextInt(100) + 1
来源：http://pts.fzhhl.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ipj.pycfn.com

Ruby: rand(1..100)
来源：http://ldk.hongshengwenyu.top

C#:   new Random().Next(1, 101)
来源：http://kls.yvedp.cn

[A11] 条件表达式（三元）
来源：http://odk.fanxiaobao.xyz

Py:   "yes" if x > 0 else "no"
来源：http://uvb.hysaishi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fsm.xuetiantiany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hya.fktsv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qyf.tanke756.top

Java: x > 0 ? "yes" : "no"
来源：http://ddf.fktsv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ner.jinqigfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://akc.yfazqb.com

C#:   x > 0 ? "yes" : "no"
来源：http://nam.zycfv.cn

[A12] 字符串插值 / 格式化
来源：http://eqn.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dtw.meibo888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yqj.ybcxt.top

JS:   `Hello, ${name}!`
来源：http://gas.yj20258888.top

TS:   `Hello, ${name}!`
来源：http://zdw.yonumen.top

Java: "Hello, %s!".formatted(name)
来源：http://omj.xuetiantiany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mdl.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://pwy.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://kwa.wangdashe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rep.kuanghao11.cn

Py:   "第一行\n第二行"
来源：http://ldg.jianghu66.top

PHP:  "第一行\n第二行"
来源：http://qah.snrcjt.cn

JS:   "第一行\n第二行"
来源：http://gsj.guowangkeji.top

TS:   "第一行\n第二行"
来源：http://csp.52xcode.cn

Java: "第一行\n第二行"
来源：http://fnm.sjlbkw.cn

Go:   "第一行\n第二行"
来源：http://lfm.zdqjudy.top

Ruby: "第一行\n第二行"
来源：http://gvj.pycfn.com

C#:   "第一行\n第二行"
来源：http://fgw.jinghuilouyu.cn

[A14] 注释写法
来源：http://qbg.jinqigfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wmh.zhiwuduotai.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ajb.zhaomingkeji.xyz

JS:   // 单行；/* 多行 */
来源：http://cls.uphjek.com

TS:   // 单行；/* 多行 */
来源：http://hir.gogol.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gou.guannengcc.top

Go:   // 单行；/* 多行 */
来源：http://dyq.pengpengdd.cyou

Ruby: # 单行；=begin 多行 =end
来源：http://xet.jinqigufen.top

C#:   // 单行；/* 多行 */
来源：http://lmd.cashguo.top

[A15] 空值判断与默认值
来源：http://bkh.iojbl.cn

Py:   value = data or "默认值"
来源：http://dej.sysykeji.top

PHP:  $value = $data ?? "默认值";
来源：http://qga.guannengcc.top

JS:   const value = data ?? "默认值";
来源：http://rww.ydjk.org.cn

TS:   const value = data ?? "默认值";
来源：http://edz.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kzm.zhaomingkeji.xyz

Go:   if data == "" { data = "默认值" }
来源：http://dij.zdqjudy.top

Ruby: value = data || "默认值"
来源：http://cbr.jqgufenzy.top

C#:   var value = data ?? "默认值";
来源：http://zfy.pycfn.com

[A16] 真假值判断规则
来源：http://wgp.fktsv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ocl.c1oappe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://msr.aizwys.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iwu.redwolf501.top

TS:   if (!x) {}
来源：http://mnn.wangdashe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://smo.dashuyun.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mbq.dianchejie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hwm.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gfc.feifeiyinyue.top

[A17] 位运算
来源：http://dqg.quarkkingdee.top


<!-- 参考信息 -->