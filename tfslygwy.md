代发 wailian999

[U99] JS：事件监听
来源：http://bbi.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://ptw.gzhubu.top

[U100] JS：DOM 查询
来源：http://rjx.yongpay.top

document.querySelector(".item")
来源：http://kme.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://kiw.52xcode.cn

el.classList.toggle("active")
来源：http://pwj.sysykeji.top

[U102] JS：本地存储
来源：http://oru.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bwi.zhongyouzk.top

[U103] JS：定时器
来源：http://kic.ybcxt.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kgm.guowangkeji.top

[U104] JS：防抖
来源：http://ioj.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vqw.dashuyun.cn

[U105] JS：节流
来源：http://bdz.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xsw.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://fob.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ugu.haohaochexian.top

[U107] JS：数字千分位
来源：http://xet.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wls.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://rhu.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ofy.cqqwz.cn

[U109] JS：数组分组
来源：http://edu.hnqzz.top

Object.groupBy(arr, x => x.type)
来源：http://ils.hfpthk.cn

[U110] JS：数组分块
来源：http://eqn.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kao.0kj1m.cn

[U111] JS：对象转 Map
来源：http://dqs.birdmap.top

new Map(Object.entries(obj))
来源：http://qvc.zhongyouzk.top

[U112] JS：字符串补位
来源：http://mfq.jianghu66.top

"7".padStart(3, "0")
来源：http://bhx.fengsongda.top

[U113] JS：正则替换全部
来源：http://zdf.tanke756.top

s.replaceAll("a", "b")
来源：http://cfy.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://cln.yj20258.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qws.pycfn.com

[U115] JS：生成 UUID
来源：http://htm.aibaodan.cn

crypto.randomUUID()
来源：http://run.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://qzb.chenjidiqi.icu

/** @param {string} name */ function f(name) {}
来源：http://joh.redwolf501.top

[U117] JS：单元测试
来源：http://cab.hcnkem.com

npm i -D vitest;  npx vitest
来源：http://lsx.yj20258.top

[U118] JS：开发服务器
来源：http://qgg.aibaodan.cn

npm i -D vite;  npx vite
来源：http://vtg.chenjidiqi.icu

[U119] JS：生产构建
来源：http://mvo.ivvv.top

npx vite build
来源：http://vqr.smart0.xyz

[U120] JS：读取环境变量（Vite）
来源：http://yvu.hnxiangtu.top

import.meta.env.VITE_API_URL
来源：http://olw.fengsongda.top

================================================================================
来源：http://qsf.cheryme.top

统计汇总
来源：http://grs.xuetiantiany.cn

================================================================================
来源：http://phv.guowangkeji.top

按语言统计（条）：
来源：http://rrb.tianlin.xyz

Python ......... 252
来源：http://upk.jyoumei.cn

PHP ............ 252
来源：http://loq.yueranfly.top

JavaScript ..... 252
来源：http://nhe.316326.xyz

TypeScript ..... 212
来源：http://zxa.bbcook.cn

Java ........... 212
来源：http://dim.haohaochexian.top

Go ............. 212
来源：http://yhg.yanxiufei.cn

Ruby ........... 212
来源：http://zma.vqdsnc.cn

C# ............. 212
来源：http://bsq.jlsjyb.cn

C .............. 30
来源：http://sxn.gotoacloud.top

C++ ............ 30
来源：http://jwi.yongpay.top

SQL ............ 90
来源：http://avy.gogol.net.cn

Bash ........... 80
来源：http://jfd.ivvv.top

Kotlin ......... 15
来源：http://ljv.shangyingyoupin.top

Swift .......... 15
来源：http://owg.c1oappe.top

Lua ............ 10
来源：http://djh.pengpengdd.cyou

Perl ........... 10
来源：http://lqm.cqqwz.cn

Scala .......... 10
来源：http://fhb.fengsongda.top

------------------------------------
来源：http://rqx.ydjk.org.cn

合计 ........... 2106 条
来源：http://zij.yuanzhike.top

按章节统计：
来源：http://cre.yangfankeji.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fra.tarul.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kek.yangfankeji.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dmz.quarkkingdee.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hrl.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jax.zhixingplan.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fsy.yuanzhike.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jds.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://toq.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yoo.yueranfly.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rnd.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dwr.fktsv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://don.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lew.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://guc.hysaishi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wav.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ktk.sufxvd.cn

Q SQL 专题                              90
来源：http://ybr.ivvv.top

R Bash 专题                             80
来源：http://psb.ydzc1.top

S C / C++ 专题                          60
来源：http://rqy.yuxming.cn

T 其他语言补充                          60
来源：http://zmo.ppjwa.cn

U 高频实用片段                         120
来源：http://skk.aizwys.cn

------------------------------------
来源：http://ysb.jinqigufen.top

合计                                  2106 条
来源：http://vvj.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://zzm.yuxming.cn

使用提醒
来源：http://aku.316326.xyz

--------------------------------------------------------------------------------
来源：http://jlv.wangdashe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nnz.jinqigufen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nbj.shangyingyoupin.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lwd.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lyw.fengsongda.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pir.jqgufenzy.top

—— 文件结束 ——
来源：http://lit.yj20258.top

================================================================================
来源：http://sho.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://fym.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://eew.316326.xyz

================================================================================
来源：http://orl.yj20258888.top

【收录内容】
来源：http://dpj.yj20258.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://grs.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pxc.shzxlz.cn

SQL · Bash · C · C++
来源：http://iko.guowangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fvf.nwbrower.top

【使用说明】
来源：http://lgv.vehdjk.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rtz.vehdjk.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fdn.shangyingyoupin.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gua.chenjidiqi.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sqh.redwolf501.top

Bash:  Shell         C:     C             C++:   C++
来源：http://syi.fehbvm.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iyq.xinyue.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kvd.andypj.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rzy.jinyuanbaomall.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wbm.redwolf501.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oww.iojbl.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lst.bjfxy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cug.jlsjyb.cn

【文件统计】
来源：http://xzo.9152youxi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://joe.zycfv.cn

--------------------------------------------------------------------------------
来源：http://swl.sysykeji.top

目  录
来源：http://vuj.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://ujt.wangshuangyany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jpv.shanyushiyangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tcx.fengsongda.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://exn.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://aia.wangshuangyany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hnj.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vqp.nanxuanxn.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://khx.gzhubu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fak.cucudq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sdl.epnwcf.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pak.tian-w.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://upi.fanxiaobao.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lyu.fzhhl.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://msz.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tou.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tem.xinyue.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pac.smart0.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cfk.epnwcf.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://tcg.sufxvd.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://txb.sjlbkw.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rxz.xinyue.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://byk.52xcode.cn

================================================================================
来源：http://zlx.nanxinkj.top

A. 基础语法与类型
来源：http://vlu.haohaochexian.top

================================================================================
来源：http://ytr.shangyingyoupin.top

[A01] Hello World
来源：http://plg.316326.xyz

Py:   print("Hello, World!")
来源：http://awo.c1oappe.top

PHP:  echo "Hello, World!";
来源：http://owj.pycfn.com

JS:   console.log("Hello, World!");
来源：http://int.nanxinkj.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qew.gotoacloud.top

Java: System.out.println("Hello, World!");
来源：http://nrg.epnwcf.com

Go:   fmt.Println("Hello, World!")
来源：http://alz.316326.xyz

Ruby: puts "Hello, World!"
来源：http://sar.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ion.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://itd.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qww.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xke.zdqjudy.top

JS:   let name = "Alex"; const age = 20;
来源：http://jiv.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xft.andypj.xyz

Java: String name = "Alex"; int age = 20;
来源：http://fit.fanxiaobao.xyz

Go:   name := "Alex"; age := 20
来源：http://dnl.hammf.cn

Ruby: name = "Alex"; age = 20
来源：http://zpd.0kj1m.cn

C#:   string name = "Alex"; int age = 20;
来源：http://uko.ywan-chungtsiang.top

[A03] 常量定义
来源：http://ber.yfazqb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hcc.aizwys.cn

PHP:  const PI = 3.14159;
来源：http://ato.jyoumei.cn

JS:   const PI = 3.14159;
来源：http://sca.shuidangran.top

TS:   const PI: number = 3.14159;
来源：http://lai.ydjk.org.cn

Java: static final double PI = 3.14159;
来源：http://pgg.hammf.cn

Go:   const PI = 3.14159
来源：http://ijt.fengsongda.top

Ruby: PI = 3.14159
来源：http://ebd.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://edq.hysaishi.cn

[A04] 判断变量类型
来源：http://oms.quarkkingdee.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://cng.hnqzz.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hyr.jinqigufen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bzi.daria6918.cn

TS:   typeof x; x instanceof Date
来源：http://fyr.52xcode.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lge.yj20258888.top

Go:   reflect.TypeOf(x).Name()
来源：http://kxy.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tpl.9152youxi.cn

C#:   x.GetType().Name; x is int
来源：http://xfv.52xcode.cn

[A05] 整数除法与取模
来源：http://zrr.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wxb.zdqjudy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://aln.andypj.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jzr.jqgufenzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qzu.yj202588.top

Java: 7 / 2; 7 % 2
来源：http://leh.tian-w.cn

Go:   7 / 2; 7 % 2
来源：http://ogd.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://xyj.hfpthk.cn

C#:   7 / 2; 7 % 2
来源：http://tbz.0kj1m.cn

[A06] 字符串转数字
来源：http://yni.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://lbp.yj20258888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vsn.shanyushiyangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eeb.shuidangran.top

TS:   parseInt("42", 10); Number("42")
来源：http://cqx.dashuyun.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yzy.shanyushiyangtech.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nea.zhixingplan.top

Ruby: "42".to_i; "3.14".to_f
来源：http://tec.sysykeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hkz.hongshengwenyu.top

[A07] 数字转字符串
来源：http://krd.tanke756.top

Py:   str(42)
来源：http://ceb.hnxiangtu.top

PHP:  (string) 42; strval(42)
来源：http://eog.pengpengdd.cyou

JS:   String(42); (42).toString()
来源：http://jvp.shanyushiyangkeji.top

TS:   String(42)
来源：http://gfb.wangdashe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ifr.kuanghao11.cn

Go:   strconv.Itoa(42)
来源：http://agr.sjlbkw.cn

Ruby: 42.to_s
来源：http://gaf.zhoulong.xyz

C#:   42.ToString()
来源：http://tkf.zhaomingkeji.xyz

[A08] 取整与四舍五入
来源：http://blb.zhoulong.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fxr.quarkkingdee.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gwb.yfazqb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tiv.52xcode.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gfh.bjfxy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sbj.xziqi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fxb.hcnkem.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://ulr.xinyue.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lvh.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://xaf.yvedp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dqx.shanyushiyangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ogl.jlsjyb.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://owa.0kj1m.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wfu.svipenyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iqo.epnwcf.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hot.uphjek.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://con.yvedp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fvf.quarkkingdee.top

[A10] 生成随机数
来源：http://zcf.svipenyu.cn

Py:   import random; random.randint(1, 100)
来源：http://boh.hammf.cn

PHP:  random_int(1, 100);
来源：http://izl.zhoulong.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jsy.guannengcc.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://smd.shanyushiyangtech.top

Java: new Random().nextInt(100) + 1
来源：http://nrz.hnqzz.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fhp.shanyushiyangtech.top

Ruby: rand(1..100)
来源：http://qwo.sweek.top

C#:   new Random().Next(1, 101)
来源：http://tbk.316326.xyz

[A11] 条件表达式（三元）
来源：http://blc.feifeiyinyue.top

Py:   "yes" if x > 0 else "no"
来源：http://pee.chenlongwang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qzt.jinyuanbaomall.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hke.fengsongda.top

TS:   x > 0 ? "yes" : "no"
来源：http://uni.redwolf501.top

Java: x > 0 ? "yes" : "no"
来源：http://xvz.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gwr.zdqjudy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://sng.ivvv.top

C#:   x > 0 ? "yes" : "no"
来源：http://psb.pengpengdd.cyou

[A12] 字符串插值 / 格式化
来源：http://ymw.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://alc.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nej.sxryk.cn

JS:   `Hello, ${name}!`
来源：http://rne.sweek.top

TS:   `Hello, ${name}!`
来源：http://cye.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://rtj.sweek.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tkb.kuanghao11.cn

Ruby: "Hello, #{name}!"
来源：http://svg.0kj1m.cn

C#:   $"Hello, {name}!"
来源：http://itt.haohaochexian.top

[A13] 多行字符串（练习 \n 转义）
来源：http://cfw.xziqi.cn

Py:   "第一行\n第二行"
来源：http://taa.zhiwuduotai.top

PHP:  "第一行\n第二行"
来源：http://yjs.aibaodan.cn

JS:   "第一行\n第二行"
来源：http://hvt.zhiwuduotai.top

TS:   "第一行\n第二行"
来源：http://rcd.jyoumei.cn

Java: "第一行\n第二行"
来源：http://czf.tian-w.cn

Go:   "第一行\n第二行"
来源：http://xxo.sjlbkw.cn

Ruby: "第一行\n第二行"
来源：http://rwn.52xcode.cn

C#:   "第一行\n第二行"
来源：http://zge.cucudq.cn

[A14] 注释写法
来源：http://qrt.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pbt.hfpthk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qks.mhx1999.top

JS:   // 单行；/* 多行 */
来源：http://thm.kuanghao11.cn

TS:   // 单行；/* 多行 */
来源：http://qre.smart0.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tmt.quarkkingdee.top

Go:   // 单行；/* 多行 */
来源：http://ajz.havefunace.top

Ruby: # 单行；=begin 多行 =end
来源：http://jve.9152youxi.cn

C#:   // 单行；/* 多行 */
来源：http://lpl.zhongyouzk.top

[A15] 空值判断与默认值
来源：http://slx.sysykeji.top

Py:   value = data or "默认值"
来源：http://zdk.jiagoushi.top

PHP:  $value = $data ?? "默认值";
来源：http://cgj.kuanghao11.cn

JS:   const value = data ?? "默认值";
来源：http://zzt.tanke756.top

TS:   const value = data ?? "默认值";
来源：http://kjd.feifeiyinyue.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ydd.zhiwuduotai.top

Go:   if data == "" { data = "默认值" }
来源：http://jdi.snrcjt.cn

Ruby: value = data || "默认值"
来源：http://snn.pycfn.com

C#:   var value = data ?? "默认值";
来源：http://xdl.wangshuangyany.cn

[A16] 真假值判断规则
来源：http://rlg.52xcode.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yhc.sweek.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ysp.zhoulong.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pri.haohaochexian.top

TS:   if (!x) {}
来源：http://ays.0kj1m.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://axi.hnqzz.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zas.birdmap.top

Ruby: unless x            # nil 与 false 为假
来源：http://vsw.hnqzz.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jzg.snrcjt.cn

[A17] 位运算
来源：http://vpv.shuidangran.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eqd.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kwm.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://szx.jlsjyb.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kwj.yangfankeji.com


<!-- 参考信息 -->