代发 wailian999

[U97] JS：并发请求
来源：http://tsl.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://nkd.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://ytb.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fxc.fktsv.cn

[U99] JS：事件监听
来源：http://dhb.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://oqm.yfazqb.com

[U100] JS：DOM 查询
来源：http://drc.yonumen.top

document.querySelector(".item")
来源：http://rhi.mhx1999.top

[U101] JS：classList 操作
来源：http://sgp.yueranfly.top

el.classList.toggle("active")
来源：http://tvt.ctjpmb.com

[U102] JS：本地存储
来源：http://vyp.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yse.fzhhl.top

[U103] JS：定时器
来源：http://bgj.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iee.jinqigufen.top

[U104] JS：防抖
来源：http://jpr.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gcc.yfazqb.com

[U105] JS：节流
来源：http://gsk.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bna.ywan-chungtsiang.top

[U106] JS：日期格式化
来源：http://xcb.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rfl.jiagoushi.top

[U107] JS：数字千分位
来源：http://cdj.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lwk.yfazqb.com

[U108] JS：随机整数
来源：http://pao.smart0.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nsx.daria6918.cn

[U109] JS：数组分组
来源：http://tdq.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://bxz.bjfxy.top

[U110] JS：数组分块
来源：http://ufp.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lwl.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://lni.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://zon.vehdjk.com

[U112] JS：字符串补位
来源：http://kpt.jianghu66.top

"7".padStart(3, "0")
来源：http://pne.hysaishi.cn

[U113] JS：正则替换全部
来源：http://jpd.sxryk.cn

s.replaceAll("a", "b")
来源：http://jmi.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://ime.jianghu66.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rvk.yuanzhike.top

[U115] JS：生成 UUID
来源：http://too.guowangkeji.top

crypto.randomUUID()
来源：http://zgf.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://lsy.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://fuf.52xcode.cn

[U117] JS：单元测试
来源：http://mkm.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://zsf.xziqi.cn

[U118] JS：开发服务器
来源：http://ehh.ydjk.org.cn

npm i -D vite;  npx vite
来源：http://nkl.cqqwz.cn

[U119] JS：生产构建
来源：http://mcg.hnxiangtu.top

npx vite build
来源：http://pwa.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://jbj.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://qgv.xylfe.cn

================================================================================
来源：http://brw.zdbjq.cn

统计汇总
来源：http://ymf.cdnleiting.top

================================================================================
来源：http://mkz.sysykeji.top

按语言统计（条）：
来源：http://ljd.xinyue.icu

Python ......... 252
来源：http://wfz.jinghuilouyu.cn

PHP ............ 252
来源：http://xqy.zycfv.cn

JavaScript ..... 252
来源：http://hgp.cdnleiting.top

TypeScript ..... 212
来源：http://jng.redwolf501.top

Java ........... 212
来源：http://xtn.guannengcc.top

Go ............. 212
来源：http://iqs.hammf.cn

Ruby ........... 212
来源：http://ymq.chenlongwang.top

C# ............. 212
来源：http://oqs.shanyushiyangtech.top

C .............. 30
来源：http://cod.vehdjk.com

C++ ............ 30
来源：http://cbb.andypj.xyz

SQL ............ 90
来源：http://npj.xuanzx.com

Bash ........... 80
来源：http://zow.chenlongwang.top

Kotlin ......... 15
来源：http://fug.aizwys.cn

Swift .......... 15
来源：http://tyl.hnqzz.top

Lua ............ 10
来源：http://kpk.zdqjudy.top

Perl ........... 10
来源：http://byt.ehwqpu.com

Scala .......... 10
来源：http://bvz.jqgufenzy.top

------------------------------------
来源：http://wqq.bbcook.cn

合计 ........... 2106 条
来源：http://ocw.jianghu66.top

按章节统计：
来源：http://lrl.mhx1999.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fnr.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://apq.hongshengwenyu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vgu.sweek.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://evc.zhaomingkeji.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://omz.ehwqpu.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cjp.ivvv.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ipx.sysykeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ssu.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qfg.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://czj.guannengcc.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://izu.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jos.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pje.gzhubu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nah.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ymr.chenlongwang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ems.vqdsnc.cn

Q SQL 专题                              90
来源：http://dno.svipenyu.cn

R Bash 专题                             80
来源：http://cee.xinyue.icu

S C / C++ 专题                          60
来源：http://vce.ybcxt.top

T 其他语言补充                          60
来源：http://nut.uphjek.com

U 高频实用片段                         120
来源：http://jdg.pengpengdd.cyou

------------------------------------
来源：http://vbc.ctjpmb.com

合计                                  2106 条
来源：http://cwq.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://hbe.fehbvm.com

使用提醒
来源：http://ojr.xuanzx.com

--------------------------------------------------------------------------------
来源：http://rnq.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qbv.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ter.hcnkem.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wrl.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tvy.feifeiyinyue.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gpy.xuetiantiany.cn

—— 文件结束 ——
来源：http://mud.zhijiandao.cn

================================================================================
来源：http://ixf.bbcook.cn

程序语言常见例子速查手册（2024 版）
来源：http://ypj.sysykeji.top

Common Programming Examples Cheat Book
来源：http://haa.jiagoushi.top

================================================================================
来源：http://drm.hywenlv.cn

【收录内容】
来源：http://zom.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://acz.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vdg.ydzc1.top

SQL · Bash · C · C++
来源：http://xdi.feifeiyinyue.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ucw.mhx1999.top

【使用说明】
来源：http://gfq.hnqzz.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gop.yuanzhike.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yto.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nxi.cqqwz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bvb.zhixingplan.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kim.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uso.shanyushiyangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wkg.pengpengdd.cyou

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://piw.jlsjyb.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jtg.wangshuangyany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://euj.jinqigufen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ude.gzhubu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jcp.aizwys.cn

【文件统计】
来源：http://mzn.hesvh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://aac.uphjek.com

--------------------------------------------------------------------------------
来源：http://sjs.andypj.xyz

目  录
来源：http://ntg.yvedp.cn

--------------------------------------------------------------------------------
来源：http://zjv.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xaq.shzxlz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jyx.zhongyouzk.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vdy.guannengcc.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zow.pycfn.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zkd.zhongyouzk.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lrf.shanyushiyangtech.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rxe.0kj1m.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://isj.jianghu66.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zeq.ctjpmb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://irv.jianghu66.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wcq.shanyushiyangtech.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uxf.vehdjk.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ayl.zhoulong.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qsw.yuxming.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lym.xinyue.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hih.ydjk.org.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://svc.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://eyx.zhongyouzk.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://soy.tian-w.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vsa.jiagoushi.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ddu.svipenyu.cn

================================================================================
来源：http://mrn.ydzc1.top

A. 基础语法与类型
来源：http://nnw.jinqigfzy.top

================================================================================
来源：http://fza.gogol.net.cn

[A01] Hello World
来源：http://fbb.ybcxt.top

Py:   print("Hello, World!")
来源：http://yxp.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://xdw.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://ejx.dianchejie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wxm.kuanghao11.cn

Java: System.out.println("Hello, World!");
来源：http://nfk.mhx1999.top

Go:   fmt.Println("Hello, World!")
来源：http://uvm.zhixingplan.top

Ruby: puts "Hello, World!"
来源：http://txx.gzhubu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cyi.jqgfzy.top

[A02] 变量声明与赋值
来源：http://kra.cqqwz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ahk.ctjpmb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://xzd.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cee.nanxuanxn.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pxr.hesvh.cn

Java: String name = "Alex"; int age = 20;
来源：http://wey.c1oappe.top

Go:   name := "Alex"; age := 20
来源：http://qdk.zhongyouzk.top

Ruby: name = "Alex"; age = 20
来源：http://xds.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dmu.yanxiufei.cn

[A03] 常量定义
来源：http://kcw.gotoacloud.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cgl.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://vce.fehbvm.com

JS:   const PI = 3.14159;
来源：http://cpw.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://qzv.ehwqpu.com

Java: static final double PI = 3.14159;
来源：http://bqb.yuanzhike.top

Go:   const PI = 3.14159
来源：http://car.yuxming.cn

Ruby: PI = 3.14159
来源：http://iqw.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://lhf.fzhhl.top

[A04] 判断变量类型
来源：http://eex.xziqi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://stf.shzxlz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vqe.aibaodan.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ufk.tarul.cn

TS:   typeof x; x instanceof Date
来源：http://vwh.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zmn.shanyushiyangtech.top

Go:   reflect.TypeOf(x).Name()
来源：http://cuj.yfazqb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://gui.guannengcc.top

C#:   x.GetType().Name; x is int
来源：http://veb.xinyue.icu

[A05] 整数除法与取模
来源：http://eva.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://izm.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ktj.hnxiangtu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sgg.xinyue.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hii.yangfankeji.com

Java: 7 / 2; 7 % 2
来源：http://anp.ydzc1.top

Go:   7 / 2; 7 % 2
来源：http://ejq.sxryk.cn

Ruby: 7 / 2; 7 % 2
来源：http://uhb.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://khw.bbcook.cn

[A06] 字符串转数字
来源：http://dib.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://xzz.aizwys.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xik.feifeiyinyue.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ksb.cdnleiting.top

TS:   parseInt("42", 10); Number("42")
来源：http://fdw.dashuyun.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gwf.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://boy.guannengcc.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bki.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tel.chenzaomai.com

[A07] 数字转字符串
来源：http://gbx.nanxinkj.top

Py:   str(42)
来源：http://yti.gotoacloud.top

PHP:  (string) 42; strval(42)
来源：http://qyl.fehbvm.com

JS:   String(42); (42).toString()
来源：http://ozx.tarul.cn

TS:   String(42)
来源：http://enm.yvedp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vlz.jqgfzy.top

Go:   strconv.Itoa(42)
来源：http://xxg.jiagoushi.top

Ruby: 42.to_s
来源：http://ckd.xinyue.icu

C#:   42.ToString()
来源：http://zzd.nwbrower.top

[A08] 取整与四舍五入
来源：http://rxb.zycfv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ofq.snrcjt.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eml.jiagoushi.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rmo.yj202588.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rne.ywan-chungtsiang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ulp.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kxs.tian-w.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wbj.xinyue.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ouf.jqgufenzy.top

[A09] 绝对值与最大最小值
来源：http://car.smart0.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hds.guannengcc.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ibr.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ixg.yanxiufei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fbr.aibaodan.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zff.ehwqpu.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eij.andypj.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://elg.fehbvm.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dag.sufxvd.cn

[A10] 生成随机数
来源：http://coq.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://cau.fanxiaobao.xyz

PHP:  random_int(1, 100);
来源：http://kih.hysaishi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ocn.zhijiandao.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kan.yangfankeji.com

Java: new Random().nextInt(100) + 1
来源：http://syb.guowangkeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fwm.hammf.cn

Ruby: rand(1..100)
来源：http://cud.jqgufenzy.top

C#:   new Random().Next(1, 101)
来源：http://got.hnxiangtu.top

[A11] 条件表达式（三元）
来源：http://ojn.cashguo.top

Py:   "yes" if x > 0 else "no"
来源：http://xxq.wangshuangyany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://eke.hywenlv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mgk.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://vou.zhongyouzk.top

Java: x > 0 ? "yes" : "no"
来源：http://hnl.nwbrower.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hlt.gogol.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bcd.redwolf501.top

C#:   x > 0 ? "yes" : "no"
来源：http://lnt.nanxuanxn.top

[A12] 字符串插值 / 格式化
来源：http://syy.yfazqb.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mut.ivvv.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vvu.ivvv.top

JS:   `Hello, ${name}!`
来源：http://ljs.smart0.xyz

TS:   `Hello, ${name}!`
来源：http://xwe.chenlongwang.top

Java: "Hello, %s!".formatted(name)
来源：http://jnv.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kvk.ppjwa.cn

Ruby: "Hello, #{name}!"
来源：http://zcb.hnqzz.top

C#:   $"Hello, {name}!"
来源：http://gym.haohaochexian.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vtr.cqqwz.cn

Py:   "第一行\n第二行"
来源：http://ijn.yj20258888.top

PHP:  "第一行\n第二行"
来源：http://kiq.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://oks.ybcxt.top

TS:   "第一行\n第二行"
来源：http://hsn.meibo888.top

Java: "第一行\n第二行"
来源：http://fbe.mhx1999.top

Go:   "第一行\n第二行"
来源：http://nqn.jinqigufen.top

Ruby: "第一行\n第二行"
来源：http://yyd.jqgufenzy.top

C#:   "第一行\n第二行"
来源：http://sfp.hcnkem.com

[A14] 注释写法
来源：http://yko.fktsv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://skr.nanxinkj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://aeh.sweek.top

JS:   // 单行；/* 多行 */
来源：http://tmz.fanxiaobao.xyz

TS:   // 单行；/* 多行 */
来源：http://wqh.yvedp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qrq.hysaishi.cn

Go:   // 单行；/* 多行 */
来源：http://nrn.yuxming.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mxn.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://hmn.gogol.net.cn

[A15] 空值判断与默认值
来源：http://lbq.hesvh.cn

Py:   value = data or "默认值"
来源：http://zry.shangyingyoupin.top

PHP:  $value = $data ?? "默认值";
来源：http://jdm.zhengqikj.top

JS:   const value = data ?? "默认值";
来源：http://pum.pycfn.com

TS:   const value = data ?? "默认值";
来源：http://hzh.yangfankeji.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ccu.zhongyouzk.top

Go:   if data == "" { data = "默认值" }
来源：http://soa.jqgfzy.top

Ruby: value = data || "默认值"
来源：http://lzf.sufxvd.cn

C#:   var value = data ?? "默认值";
来源：http://udz.guannengcc.top

[A16] 真假值判断规则
来源：http://doz.gogol.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ycs.tarul.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://igt.jiagoushi.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nzz.svipenyu.cn

TS:   if (!x) {}
来源：http://zjb.haohaochexian.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://avp.0kj1m.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://isr.zhengqikj.top

Ruby: unless x            # nil 与 false 为假
来源：http://rbk.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://szu.jianghu66.top

[A17] 位运算
来源：http://dmt.kuanghao11.cn


<!-- 参考信息 -->