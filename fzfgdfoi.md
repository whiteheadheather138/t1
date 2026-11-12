代发 wailian999

[U99] JS：事件监听
来源：http://rtb.hcnkem.com

el.addEventListener("click", e => {})
来源：http://quo.zdqjudy.top

[U100] JS：DOM 查询
来源：http://hhg.feifeiyinyue.top

document.querySelector(".item")
来源：http://cyg.zhijiandao.cn

[U101] JS：classList 操作
来源：http://kmm.mhx1999.top

el.classList.toggle("active")
来源：http://hpc.pycfn.com

[U102] JS：本地存储
来源：http://bvk.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://arv.fzhhl.top

[U103] JS：定时器
来源：http://hjq.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hgt.cqqwz.cn

[U104] JS：防抖
来源：http://buv.uphjek.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gev.epnwcf.com

[U105] JS：节流
来源：http://eyv.tarul.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://adc.sxryk.cn

[U106] JS：日期格式化
来源：http://ecv.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mot.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://xed.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mjx.ydzc1.top

[U108] JS：随机整数
来源：http://kgs.jinqigufen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bgw.chenzaomai.com

[U109] JS：数组分组
来源：http://lis.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://eyb.fanxiaobao.xyz

[U110] JS：数组分块
来源：http://nun.xinyue.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ksy.zhoulong.xyz

[U111] JS：对象转 Map
来源：http://bym.hnqzz.top

new Map(Object.entries(obj))
来源：http://llh.xinyue.icu

[U112] JS：字符串补位
来源：http://lya.xuanzx.com

"7".padStart(3, "0")
来源：http://bni.jiagoushi.top

[U113] JS：正则替换全部
来源：http://goz.gogol.net.cn

s.replaceAll("a", "b")
来源：http://jdj.aizwys.cn

[U114] JS：JSON 深比较
来源：http://ihy.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lox.fzhhl.top

[U115] JS：生成 UUID
来源：http://hpc.sweek.top

crypto.randomUUID()
来源：http://neu.316326.xyz

[U116] JS：类型检查（JSDoc）
来源：http://uss.hysaishi.cn

/** @param {string} name */ function f(name) {}
来源：http://trx.zhiwuduotai.top

[U117] JS：单元测试
来源：http://jqk.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://yzr.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://bco.gogol.net.cn

npm i -D vite;  npx vite
来源：http://pfo.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://pte.yfazqb.com

npx vite build
来源：http://hab.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://mpc.hnxiangtu.top

import.meta.env.VITE_API_URL
来源：http://nup.chenlongwang.top

================================================================================
来源：http://jwe.ppjwa.cn

统计汇总
来源：http://gch.gogol.net.cn

================================================================================
来源：http://rco.hnxiangtu.top

按语言统计（条）：
来源：http://nax.zdbjq.cn

Python ......... 252
来源：http://khu.zdqjudy.top

PHP ............ 252
来源：http://nrv.tianlin.xyz

JavaScript ..... 252
来源：http://ewj.hfpthk.cn

TypeScript ..... 212
来源：http://cru.dashuyun.cn

Java ........... 212
来源：http://ysq.dashuyun.cn

Go ............. 212
来源：http://aje.aibaodan.cn

Ruby ........... 212
来源：http://hpt.vehdjk.com

C# ............. 212
来源：http://sor.xuanzx.com

C .............. 30
来源：http://mja.smart0.xyz

C++ ............ 30
来源：http://fed.uphjek.com

SQL ............ 90
来源：http://kwy.yuxming.cn

Bash ........... 80
来源：http://cii.nanxinkj.top

Kotlin ......... 15
来源：http://akb.ydzc1.top

Swift .......... 15
来源：http://jwo.yj20258.top

Lua ............ 10
来源：http://upi.aizwys.cn

Perl ........... 10
来源：http://pdl.guowangkeji.top

Scala .......... 10
来源：http://aya.yfazqb.com

------------------------------------
来源：http://vcc.aibaodan.cn

合计 ........... 2106 条
来源：http://xog.birdmap.top

按章节统计：
来源：http://ezv.yuxming.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gsu.zycfv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://weg.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ivw.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hol.gzhubu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://inv.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dro.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kje.epnwcf.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://voz.hfpthk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bol.hesvh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nie.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rea.ybcxt.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cyu.cucudq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lvg.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rdw.jyoumei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ncc.jqgfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nbh.wangdashe.top

Q SQL 专题                              90
来源：http://ydc.yj20258888.top

R Bash 专题                             80
来源：http://hei.gaohongyu789.top

S C / C++ 专题                          60
来源：http://sqs.yangfankeji.com

T 其他语言补充                          60
来源：http://zju.sufxvd.cn

U 高频实用片段                         120
来源：http://ndg.zdbjq.cn

------------------------------------
来源：http://tmt.guowangkeji.top

合计                                  2106 条
来源：http://lle.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://kwy.zhoulong.xyz

使用提醒
来源：http://ghm.uphjek.com

--------------------------------------------------------------------------------
来源：http://sui.jinqigfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cji.ywan-chungtsiang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vem.mhx1999.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nwv.zycfv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cif.zdqjudy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jpx.cqqwz.cn

—— 文件结束 ——
来源：http://fly.ydzc1.top

================================================================================
来源：http://hci.meibo888.top

程序语言常见例子速查手册（2024 版）
来源：http://ypo.yuanzhike.top

Common Programming Examples Cheat Book
来源：http://dge.hywenlv.cn

================================================================================
来源：http://nwi.fengsongda.top

【收录内容】
来源：http://fer.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ogs.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oxl.9152youxi.cn

SQL · Bash · C · C++
来源：http://hwk.bjfxy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yfq.jqgfzy.top

【使用说明】
来源：http://mht.hnqzz.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vzb.mhx1999.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lgm.tanke756.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lmg.zhoulong.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eoo.yj20258888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dsa.hnxiangtu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vhx.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ufu.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uzy.gotoacloud.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kpd.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dly.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ujt.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wfr.cucudq.cn

【文件统计】
来源：http://ctx.andypj.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mix.hesvh.cn

--------------------------------------------------------------------------------
来源：http://cif.tianlin.xyz

目  录
来源：http://kxh.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://fhz.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lrp.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wuh.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tmq.cashguo.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bev.cqqwz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eex.tanke756.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qjx.andypj.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bov.sjlbkw.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bzq.xinyue.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kji.316326.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qkk.sysykeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lzt.tian-w.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ipe.nanxinkj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://alp.mhx1999.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qyy.shzxlz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jly.ppjwa.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cip.sweek.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wjf.c1oappe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://sgm.redwolf501.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://coq.aizwys.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lwl.nanxuanxn.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jqs.wangdashe.top

================================================================================
来源：http://xlf.yuanzhike.top

A. 基础语法与类型
来源：http://ekt.yonumen.top

================================================================================
来源：http://djm.jinghuilouyu.cn

[A01] Hello World
来源：http://xhk.chenzaomai.com

Py:   print("Hello, World!")
来源：http://kfy.316326.xyz

PHP:  echo "Hello, World!";
来源：http://lfa.zhengqikj.top

JS:   console.log("Hello, World!");
来源：http://pbq.epnwcf.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jef.fzhhl.top

Java: System.out.println("Hello, World!");
来源：http://ivn.mhx1999.top

Go:   fmt.Println("Hello, World!")
来源：http://mvz.guowangkeji.top

Ruby: puts "Hello, World!"
来源：http://iqg.jinqigufen.top

C#:   Console.WriteLine("Hello, World!");
来源：http://czi.sysykeji.top

[A02] 变量声明与赋值
来源：http://tmg.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vpa.tanke756.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vrp.316326.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://hwy.jinqigfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kpc.ppjwa.cn

Java: String name = "Alex"; int age = 20;
来源：http://xog.cucudq.cn

Go:   name := "Alex"; age := 20
来源：http://tox.yueranfly.top

Ruby: name = "Alex"; age = 20
来源：http://xbj.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://nib.bjfxy.top

[A03] 常量定义
来源：http://eyk.zhijiandao.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fta.pycfn.com

PHP:  const PI = 3.14159;
来源：http://ege.jiagoushi.top

JS:   const PI = 3.14159;
来源：http://sai.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://icf.shanyushiyangtech.top

Java: static final double PI = 3.14159;
来源：http://ktj.zhengqikj.top

Go:   const PI = 3.14159
来源：http://xzm.svipenyu.cn

Ruby: PI = 3.14159
来源：http://pcm.ydzc1.top

C#:   const double PI = 3.14159;
来源：http://ury.iojbl.cn

[A04] 判断变量类型
来源：http://vtk.vqdsnc.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gtg.chenjidiqi.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gvo.zdqjudy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nwy.zhaomingkeji.xyz

TS:   typeof x; x instanceof Date
来源：http://wdh.cucudq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tym.fktsv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hds.hcnkem.com

Ruby: x.class; x.is_a?(Integer)
来源：http://yvl.tian-w.cn

C#:   x.GetType().Name; x is int
来源：http://spu.cucudq.cn

[A05] 整数除法与取模
来源：http://edk.zhaomingkeji.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gjo.chenlongwang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kvl.zhongyouzk.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rxe.tanke756.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gaz.jqgufenzy.top

Java: 7 / 2; 7 % 2
来源：http://ine.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://cmp.yuanzhike.top

Ruby: 7 / 2; 7 % 2
来源：http://xru.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://jok.fzhhl.top

[A06] 字符串转数字
来源：http://bqd.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://vbv.dianchejie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vqz.haohaochexian.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://trn.dianchejie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qha.yanxiufei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cof.bjfxy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qrr.meibo888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vuq.jqgfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tmb.ywan-chungtsiang.top

[A07] 数字转字符串
来源：http://ulb.yj202588.top

Py:   str(42)
来源：http://avc.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://rtu.jqgfzy.top

JS:   String(42); (42).toString()
来源：http://cvz.kuanghao11.cn

TS:   String(42)
来源：http://boy.smart0.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://ogr.yueranfly.top

Go:   strconv.Itoa(42)
来源：http://kae.nanxinkj.top

Ruby: 42.to_s
来源：http://rbz.shanyushiyangkeji.top

C#:   42.ToString()
来源：http://zxt.svipenyu.cn

[A08] 取整与四舍五入
来源：http://blb.tian-w.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lvv.shuidangran.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qlg.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bpr.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zqj.shanyushiyangkeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://npm.jlsjyb.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lsp.yfazqb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://phu.aizwys.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://olm.gaohongyu789.top

[A09] 绝对值与最大最小值
来源：http://jvj.vehdjk.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lrp.feifeiyinyue.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qvr.zhaomingkeji.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://trn.ctjpmb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pbs.gaohongyu789.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ljx.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vxg.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ewt.kuanghao11.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rhq.daria6918.cn

[A10] 生成随机数
来源：http://eyj.jinqigfzy.top

Py:   import random; random.randint(1, 100)
来源：http://wig.guowangkeji.top

PHP:  random_int(1, 100);
来源：http://rdp.bbcook.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lif.shangyingyoupin.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vfo.aibaodan.cn

Java: new Random().nextInt(100) + 1
来源：http://rnk.gzhubu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vqn.yuanzhike.top

Ruby: rand(1..100)
来源：http://lkw.jlsjyb.cn

C#:   new Random().Next(1, 101)
来源：http://jmi.aizwys.cn

[A11] 条件表达式（三元）
来源：http://uea.jinyuanbaomall.cn

Py:   "yes" if x > 0 else "no"
来源：http://gvp.sysykeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yyz.chenjidiqi.icu

JS:   x > 0 ? "yes" : "no"
来源：http://clv.tarul.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zuq.snrcjt.cn

Java: x > 0 ? "yes" : "no"
来源：http://gkf.9152youxi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zpv.iojbl.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aru.daria6918.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eqq.cashguo.top

[A12] 字符串插值 / 格式化
来源：http://wxt.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://slt.jlsjyb.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jup.wangshuangyany.cn

JS:   `Hello, ${name}!`
来源：http://zqf.zhoulong.xyz

TS:   `Hello, ${name}!`
来源：http://tar.shangyingyoupin.top

Java: "Hello, %s!".formatted(name)
来源：http://zgr.vqdsnc.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ppr.zdbjq.cn

Ruby: "Hello, #{name}!"
来源：http://dti.yj20258.top

C#:   $"Hello, {name}!"
来源：http://jkj.xinyue.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://hkk.aibaodan.cn

Py:   "第一行\n第二行"
来源：http://zrk.aizwys.cn

PHP:  "第一行\n第二行"
来源：http://rpy.shuidangran.top

JS:   "第一行\n第二行"
来源：http://qvs.nanxinkj.top

TS:   "第一行\n第二行"
来源：http://uvh.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://dvg.ehwqpu.com

Go:   "第一行\n第二行"
来源：http://ryj.pengpengdd.cyou

Ruby: "第一行\n第二行"
来源：http://zty.gzhubu.top

C#:   "第一行\n第二行"
来源：http://tpv.tanke756.top

[A14] 注释写法
来源：http://owh.zhixingplan.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ibu.ybcxt.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wga.cucudq.cn

JS:   // 单行；/* 多行 */
来源：http://qir.shanyushiyangkeji.top

TS:   // 单行；/* 多行 */
来源：http://dix.yj20258.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jtt.zdqjudy.top

Go:   // 单行；/* 多行 */
来源：http://qhb.zhiwuduotai.top

Ruby: # 单行；=begin 多行 =end
来源：http://nnv.iojbl.cn

C#:   // 单行；/* 多行 */
来源：http://ewl.zhijiandao.cn

[A15] 空值判断与默认值
来源：http://mpy.nanxuanxn.top

Py:   value = data or "默认值"
来源：http://xik.zycfv.cn

PHP:  $value = $data ?? "默认值";
来源：http://yqa.nanxuanxn.top

JS:   const value = data ?? "默认值";
来源：http://nfr.snrcjt.cn

TS:   const value = data ?? "默认值";
来源：http://nlp.xuetiantiany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fjn.jyoumei.cn

Go:   if data == "" { data = "默认值" }
来源：http://tye.yuxming.cn

Ruby: value = data || "默认值"
来源：http://yep.yanxiufei.cn

C#:   var value = data ?? "默认值";
来源：http://odc.quarkkingdee.top

[A16] 真假值判断规则
来源：http://rxi.sjlbkw.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://odp.xuanzx.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pqg.sysykeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://trb.yueranfly.top

TS:   if (!x) {}
来源：http://wov.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gyc.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dqd.hnxiangtu.top

Ruby: unless x            # nil 与 false 为假
来源：http://sba.ppjwa.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://quy.sjlbkw.cn

[A17] 位运算
来源：http://csu.xuanzx.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kwv.ctjpmb.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://igq.kuanghao11.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://guc.jqgufenzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pzo.sxryk.cn


<!-- 参考信息 -->