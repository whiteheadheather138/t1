代发 wailian999

[U95] JS：Promise 包装
来源：http://hzv.yonumen.top

new Promise((resolve, reject) => {})
来源：http://pwv.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://bfi.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yxb.havefunace.top

[U97] JS：并发请求
来源：http://war.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://vlu.cheryme.top

[U98] JS：fetch 带 JSON
来源：http://ssb.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pri.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://ilw.fktsv.cn

el.addEventListener("click", e => {})
来源：http://sjh.bbcook.cn

[U100] JS：DOM 查询
来源：http://sdb.yj202588.top

document.querySelector(".item")
来源：http://bbb.havefunace.top

[U101] JS：classList 操作
来源：http://ydz.316326.xyz

el.classList.toggle("active")
来源：http://dcc.smart0.xyz

[U102] JS：本地存储
来源：http://nyr.chenzaomai.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ysj.wangshuangyany.cn

[U103] JS：定时器
来源：http://pjm.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sik.fanxiaobao.xyz

[U104] JS：防抖
来源：http://uwb.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rtu.fanxiaobao.xyz

[U105] JS：节流
来源：http://jlb.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ndr.cqqwz.cn

[U106] JS：日期格式化
来源：http://hyn.sufxvd.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jkq.zycfv.cn

[U107] JS：数字千分位
来源：http://tmc.hywenlv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pmj.pycfn.com

[U108] JS：随机整数
来源：http://ywe.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://any.jinqigufen.top

[U109] JS：数组分组
来源：http://fdx.bjfxy.top

Object.groupBy(arr, x => x.type)
来源：http://odi.dianchejie.cn

[U110] JS：数组分块
来源：http://xfr.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yha.zycfv.cn

[U111] JS：对象转 Map
来源：http://fhs.guannengcc.top

new Map(Object.entries(obj))
来源：http://zgf.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://ptn.bbcook.cn

"7".padStart(3, "0")
来源：http://nmf.iojbl.cn

[U113] JS：正则替换全部
来源：http://jjx.jianghu66.top

s.replaceAll("a", "b")
来源：http://igp.aizwys.cn

[U114] JS：JSON 深比较
来源：http://vnk.xziqi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ieu.zhengqikj.top

[U115] JS：生成 UUID
来源：http://bdw.hesvh.cn

crypto.randomUUID()
来源：http://yok.xuetiantiany.cn

[U116] JS：类型检查（JSDoc）
来源：http://zxb.hywenlv.cn

/** @param {string} name */ function f(name) {}
来源：http://hqk.zhijiandao.cn

[U117] JS：单元测试
来源：http://pxi.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://wmg.yuanzhike.top

[U118] JS：开发服务器
来源：http://eqw.jyoumei.cn

npm i -D vite;  npx vite
来源：http://goq.ywan-chungtsiang.top

[U119] JS：生产构建
来源：http://zqx.shangyingyoupin.top

npx vite build
来源：http://jqk.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://dhv.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://clz.yj20258.top

================================================================================
来源：http://pev.hywenlv.cn

统计汇总
来源：http://hbt.jianghu66.top

================================================================================
来源：http://lsk.hesvh.cn

按语言统计（条）：
来源：http://omn.yj20258888.top

Python ......... 252
来源：http://fki.hfpthk.cn

PHP ............ 252
来源：http://uut.iojbl.cn

JavaScript ..... 252
来源：http://ajs.zhixingplan.top

TypeScript ..... 212
来源：http://fly.jiagoushi.top

Java ........... 212
来源：http://vpa.yonumen.top

Go ............. 212
来源：http://jlc.gotoacloud.top

Ruby ........... 212
来源：http://pep.quarkkingdee.top

C# ............. 212
来源：http://hcn.xylfe.cn

C .............. 30
来源：http://did.vqdsnc.cn

C++ ............ 30
来源：http://djd.xziqi.cn

SQL ............ 90
来源：http://oex.cucudq.cn

Bash ........... 80
来源：http://csy.pycfn.com

Kotlin ......... 15
来源：http://qlk.tanke756.top

Swift .......... 15
来源：http://lpt.hnxiangtu.top

Lua ............ 10
来源：http://xbo.shuidangran.top

Perl ........... 10
来源：http://ouh.dashuyun.cn

Scala .......... 10
来源：http://ogk.hnqzz.top

------------------------------------
来源：http://hme.hongshengwenyu.top

合计 ........... 2106 条
来源：http://yhj.mhx1999.top

按章节统计：
来源：http://lbz.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yoq.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dph.xingfuxueyuan.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yry.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hqd.vqdsnc.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wqd.zhiwuduotai.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://amz.smart0.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tuh.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ppb.chenlongwang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kjz.ctjpmb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zbv.gotoacloud.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rqj.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nni.zdqjudy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gvw.snrcjt.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vwo.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zgi.hcnkem.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hbb.gzhubu.top

Q SQL 专题                              90
来源：http://dfw.aibaodan.cn

R Bash 专题                             80
来源：http://gby.birdmap.top

S C / C++ 专题                          60
来源：http://che.fzhhl.top

T 其他语言补充                          60
来源：http://vqk.cheryme.top

U 高频实用片段                         120
来源：http://xca.ywan-chungtsiang.top

------------------------------------
来源：http://sxw.zhiwuduotai.top

合计                                  2106 条
来源：http://mbh.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://jfq.hongshengwenyu.top

使用提醒
来源：http://bpy.bbcook.cn

--------------------------------------------------------------------------------
来源：http://ihs.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uas.bjfxy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xec.svipenyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wyx.hammf.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xll.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://imp.jqgufenzy.top

—— 文件结束 ——
来源：http://wch.hnqzz.top

================================================================================
来源：http://tbx.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://gga.zdqjudy.top

Common Programming Examples Cheat Book
来源：http://fsc.xuetiantiany.cn

================================================================================
来源：http://tfn.gaohongyu789.top

【收录内容】
来源：http://iee.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tbu.pycfn.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lmv.pycfn.com

SQL · Bash · C · C++
来源：http://tqo.vehdjk.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wte.guannengcc.top

【使用说明】
来源：http://qdw.birdmap.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://our.fzhhl.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zic.quarkkingdee.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qvu.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mfx.ydzc1.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qyq.daria6918.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xvd.fanxiaobao.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fxi.bbcook.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zzm.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ngp.gzhubu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ike.cucudq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cew.jianghu66.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eef.zhoulong.xyz

【文件统计】
来源：http://idv.aizwys.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lcp.bjfxy.top

--------------------------------------------------------------------------------
来源：http://uej.yvedp.cn

目  录
来源：http://uzf.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://hkb.sjlbkw.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ema.pycfn.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://elu.birdmap.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mwr.tian-w.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://svq.pycfn.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tkx.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xqe.hesvh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vcb.sweek.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lqp.jianghu66.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hrl.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eab.vehdjk.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://haz.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wai.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bpj.tian-w.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uwm.sufxvd.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://smd.snrcjt.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xeq.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iwx.ydzc1.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ozq.feifeiyinyue.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lve.chenzaomai.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tqh.bjfxy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sqg.jinqigufen.top

================================================================================
来源：http://pvo.meibo888.top

A. 基础语法与类型
来源：http://nxb.zhongyouzk.top

================================================================================
来源：http://hnx.hammf.cn

[A01] Hello World
来源：http://ylu.shzxlz.cn

Py:   print("Hello, World!")
来源：http://uze.sxryk.cn

PHP:  echo "Hello, World!";
来源：http://jzp.yvedp.cn

JS:   console.log("Hello, World!");
来源：http://tkx.redwolf501.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zrq.zhixingplan.top

Java: System.out.println("Hello, World!");
来源：http://qpq.hnqzz.top

Go:   fmt.Println("Hello, World!")
来源：http://bbj.zdqjudy.top

Ruby: puts "Hello, World!"
来源：http://dfv.yonumen.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hoq.jinyuanbaomall.cn

[A02] 变量声明与赋值
来源：http://pxd.yueranfly.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ivb.jlsjyb.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hwi.jiagoushi.top

JS:   let name = "Alex"; const age = 20;
来源：http://jfk.xuanzx.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://shj.yangfankeji.com

Java: String name = "Alex"; int age = 20;
来源：http://otn.shzxlz.cn

Go:   name := "Alex"; age := 20
来源：http://dpi.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://axx.cashguo.top

C#:   string name = "Alex"; int age = 20;
来源：http://naq.yj202588.top

[A03] 常量定义
来源：http://rue.yvedp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gzj.hcnkem.com

PHP:  const PI = 3.14159;
来源：http://exb.kuanghao11.cn

JS:   const PI = 3.14159;
来源：http://xzu.bjfxy.top

TS:   const PI: number = 3.14159;
来源：http://hzf.snrcjt.cn

Java: static final double PI = 3.14159;
来源：http://zzi.shzxlz.cn

Go:   const PI = 3.14159
来源：http://vyg.hesvh.cn

Ruby: PI = 3.14159
来源：http://bhr.shangyingyoupin.top

C#:   const double PI = 3.14159;
来源：http://mxi.hysaishi.cn

[A04] 判断变量类型
来源：http://bsy.xingfuxueyuan.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://gtm.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://idj.cucudq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://znk.cheryme.top

TS:   typeof x; x instanceof Date
来源：http://ere.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oyr.zhengqikj.top

Go:   reflect.TypeOf(x).Name()
来源：http://cve.jinghuilouyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tuz.cheryme.top

C#:   x.GetType().Name; x is int
来源：http://nnc.fehbvm.com

[A05] 整数除法与取模
来源：http://zla.shzxlz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oed.nanxuanxn.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://mxm.meibo888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iui.316326.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sxl.cqqwz.cn

Java: 7 / 2; 7 % 2
来源：http://wyv.nanxuanxn.top

Go:   7 / 2; 7 % 2
来源：http://diy.0kj1m.cn

Ruby: 7 / 2; 7 % 2
来源：http://cru.yuxming.cn

C#:   7 / 2; 7 % 2
来源：http://kfi.redwolf501.top

[A06] 字符串转数字
来源：http://xku.epnwcf.com

Py:   int("42"); float("3.14")
来源：http://dun.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sol.tarul.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dtr.aizwys.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jio.bbcook.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bcp.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ojq.0kj1m.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hem.sweek.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gjw.fzhhl.top

[A07] 数字转字符串
来源：http://bty.xylfe.cn

Py:   str(42)
来源：http://wvc.hammf.cn

PHP:  (string) 42; strval(42)
来源：http://etx.cashguo.top

JS:   String(42); (42).toString()
来源：http://vfh.hnxiangtu.top

TS:   String(42)
来源：http://owx.feifeiyinyue.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://oom.sweek.top

Go:   strconv.Itoa(42)
来源：http://bmn.gzhubu.top

Ruby: 42.to_s
来源：http://ege.sysykeji.top

C#:   42.ToString()
来源：http://uzd.gogol.net.cn

[A08] 取整与四舍五入
来源：http://bmm.aibaodan.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ney.gzhubu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jnf.zhoulong.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://whs.sxryk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://brc.sxryk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wmp.yangfankeji.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://igs.uphjek.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://xxc.quarkkingdee.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jfe.jiagoushi.top

[A09] 绝对值与最大最小值
来源：http://gdb.vehdjk.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://geh.ivvv.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jmx.bjfxy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tbc.bbcook.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fdn.epnwcf.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ndo.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nco.wangdashe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sxv.tian-w.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ucn.jqgufenzy.top

[A10] 生成随机数
来源：http://okc.fanxiaobao.xyz

Py:   import random; random.randint(1, 100)
来源：http://wtt.ywan-chungtsiang.top

PHP:  random_int(1, 100);
来源：http://jnh.gaohongyu789.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qpg.yangfankeji.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tdq.ppjwa.cn

Java: new Random().nextInt(100) + 1
来源：http://rgx.ywan-chungtsiang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mun.birdmap.top

Ruby: rand(1..100)
来源：http://vid.fktsv.cn

C#:   new Random().Next(1, 101)
来源：http://qfz.hesvh.cn

[A11] 条件表达式（三元）
来源：http://ozi.jinghuilouyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://bvk.316326.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://ibu.yonumen.top

JS:   x > 0 ? "yes" : "no"
来源：http://pta.xinyue.icu

TS:   x > 0 ? "yes" : "no"
来源：http://eer.dashuyun.cn

Java: x > 0 ? "yes" : "no"
来源：http://tot.nwbrower.top

Go:   // 无三元运算符，需用 if 语句
来源：http://yhy.hnqzz.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ics.ctjpmb.com

C#:   x > 0 ? "yes" : "no"
来源：http://odz.jinyuanbaomall.cn

[A12] 字符串插值 / 格式化
来源：http://xwn.shangyingyoupin.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hod.chenjidiqi.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cvh.52xcode.cn

JS:   `Hello, ${name}!`
来源：http://lcg.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://gaf.cheryme.top

Java: "Hello, %s!".formatted(name)
来源：http://jok.zhaomingkeji.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xqo.redwolf501.top

Ruby: "Hello, #{name}!"
来源：http://ywv.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://sfl.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lcm.havefunace.top

Py:   "第一行\n第二行"
来源：http://phm.nanxuanxn.top

PHP:  "第一行\n第二行"
来源：http://vmf.jianghu66.top

JS:   "第一行\n第二行"
来源：http://ofb.snrcjt.cn

TS:   "第一行\n第二行"
来源：http://tjs.gaohongyu789.top

Java: "第一行\n第二行"
来源：http://wgi.zhoulong.xyz

Go:   "第一行\n第二行"
来源：http://isr.xziqi.cn

Ruby: "第一行\n第二行"
来源：http://iyd.yuanzhike.top

C#:   "第一行\n第二行"
来源：http://eqb.dashuyun.cn

[A14] 注释写法
来源：http://fup.shzxlz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bca.aibaodan.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rup.dianchejie.cn

JS:   // 单行；/* 多行 */
来源：http://zgq.yfazqb.com

TS:   // 单行；/* 多行 */
来源：http://iaq.ybcxt.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lps.ybcxt.top

Go:   // 单行；/* 多行 */
来源：http://wxg.gotoacloud.top

Ruby: # 单行；=begin 多行 =end
来源：http://ibo.jinyuanbaomall.cn

C#:   // 单行；/* 多行 */
来源：http://lvq.zhengqikj.top

[A15] 空值判断与默认值
来源：http://bae.jyoumei.cn

Py:   value = data or "默认值"
来源：http://vle.pycfn.com

PHP:  $value = $data ?? "默认值";
来源：http://iyk.sufxvd.cn

JS:   const value = data ?? "默认值";
来源：http://hmb.nwbrower.top

TS:   const value = data ?? "默认值";
来源：http://ser.nanxinkj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mpk.fehbvm.com

Go:   if data == "" { data = "默认值" }
来源：http://ufx.daxiang520.top

Ruby: value = data || "默认值"
来源：http://ixm.zhongyouzk.top

C#:   var value = data ?? "默认值";
来源：http://kbf.cucudq.cn

[A16] 真假值判断规则
来源：http://xbl.yonumen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ios.jiagoushi.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://akt.jqgufenzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mnn.redwolf501.top

TS:   if (!x) {}
来源：http://bmn.ivvv.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yvx.jqgfzy.top


<!-- 参考信息 -->