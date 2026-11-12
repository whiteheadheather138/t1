代发 wailian999

[U97] JS：并发请求
来源：http://ext.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://bzy.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://nof.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fac.hcnkem.com

[U99] JS：事件监听
来源：http://dbr.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://rch.xingfuxueyuan.xyz

[U100] JS：DOM 查询
来源：http://pdf.fktsv.cn

document.querySelector(".item")
来源：http://pte.zdqjudy.top

[U101] JS：classList 操作
来源：http://krd.cucudq.cn

el.classList.toggle("active")
来源：http://shx.yonumen.top

[U102] JS：本地存储
来源：http://nsm.jqgfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pgz.ydjk.org.cn

[U103] JS：定时器
来源：http://ynh.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://grk.hesvh.cn

[U104] JS：防抖
来源：http://fyl.cucudq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://psv.cqqwz.cn

[U105] JS：节流
来源：http://pty.fanxiaobao.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eod.shangyingyoupin.top

[U106] JS：日期格式化
来源：http://qcl.zhongyouzk.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fec.epnwcf.com

[U107] JS：数字千分位
来源：http://tbq.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://owq.kuanghao11.cn

[U108] JS：随机整数
来源：http://sld.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jsl.tanke756.top

[U109] JS：数组分组
来源：http://ius.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://gsi.c1oappe.top

[U110] JS：数组分块
来源：http://aex.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mjr.hesvh.cn

[U111] JS：对象转 Map
来源：http://abn.gzhubu.top

new Map(Object.entries(obj))
来源：http://kcm.ppjwa.cn

[U112] JS：字符串补位
来源：http://rcv.zdbjq.cn

"7".padStart(3, "0")
来源：http://tfm.jianghu66.top

[U113] JS：正则替换全部
来源：http://cxm.dianchejie.cn

s.replaceAll("a", "b")
来源：http://tgo.yvedp.cn

[U114] JS：JSON 深比较
来源：http://qye.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://tgy.vehdjk.com

[U115] JS：生成 UUID
来源：http://wml.guowangkeji.top

crypto.randomUUID()
来源：http://bpw.nanxuanxn.top

[U116] JS：类型检查（JSDoc）
来源：http://sdt.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://fiw.ydjk.org.cn

[U117] JS：单元测试
来源：http://whs.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://qzw.hfpthk.cn

[U118] JS：开发服务器
来源：http://tmb.chenlongwang.top

npm i -D vite;  npx vite
来源：http://oyl.xinyue.icu

[U119] JS：生产构建
来源：http://akv.shanyushiyangtech.top

npx vite build
来源：http://kia.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://btz.cashguo.top

import.meta.env.VITE_API_URL
来源：http://uxe.dashuyun.cn

================================================================================
来源：http://aaq.zhiwuduotai.top

统计汇总
来源：http://fpc.fzhhl.top

================================================================================
来源：http://vry.havefunace.top

按语言统计（条）：
来源：http://ghb.jinqigfzy.top

Python ......... 252
来源：http://ati.gotoacloud.top

PHP ............ 252
来源：http://cze.fehbvm.com

JavaScript ..... 252
来源：http://par.pycfn.com

TypeScript ..... 212
来源：http://ekm.vqdsnc.cn

Java ........... 212
来源：http://xak.0kj1m.cn

Go ............. 212
来源：http://soc.yongpay.top

Ruby ........... 212
来源：http://oex.wangdashe.top

C# ............. 212
来源：http://tey.yongpay.top

C .............. 30
来源：http://aut.zhengqikj.top

C++ ............ 30
来源：http://rop.sufxvd.cn

SQL ............ 90
来源：http://rad.xylfe.cn

Bash ........... 80
来源：http://kzx.ivvv.top

Kotlin ......... 15
来源：http://txg.sweek.top

Swift .......... 15
来源：http://asj.ppjwa.cn

Lua ............ 10
来源：http://mfb.jqgfzy.top

Perl ........... 10
来源：http://wdr.zhixingplan.top

Scala .......... 10
来源：http://zsh.xuetiantiany.cn

------------------------------------
来源：http://xir.feifeiyinyue.top

合计 ........... 2106 条
来源：http://brn.birdmap.top

按章节统计：
来源：http://rgg.jqgufenzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iqk.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yxp.haohaochexian.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mba.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pdf.jqgfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fvu.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vqo.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://row.tarul.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fan.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dmi.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bmm.hcnkem.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fdx.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bgt.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ugf.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zoe.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://idf.kuanghao11.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ltv.vqdsnc.cn

Q SQL 专题                              90
来源：http://ygr.sufxvd.cn

R Bash 专题                             80
来源：http://dld.yvedp.cn

S C / C++ 专题                          60
来源：http://bwq.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://ypq.zhaomingkeji.xyz

U 高频实用片段                         120
来源：http://djl.andypj.xyz

------------------------------------
来源：http://wae.guannengcc.top

合计                                  2106 条
来源：http://vhj.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://mlt.ivvv.top

使用提醒
来源：http://eps.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://obb.hesvh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qyn.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tfz.fzhhl.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qjk.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://czk.xinyue.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gbf.zhijiandao.cn

—— 文件结束 ——
来源：http://dio.zycfv.cn

================================================================================
来源：http://pqb.daxiang520.top

程序语言常见例子速查手册（2024 版）
来源：http://dxj.fktsv.cn

Common Programming Examples Cheat Book
来源：http://clx.kuanghao11.cn

================================================================================
来源：http://dln.epnwcf.com

【收录内容】
来源：http://axl.hongshengwenyu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ntn.jiagoushi.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bov.yvedp.cn

SQL · Bash · C · C++
来源：http://plh.xingfuxueyuan.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qoq.redwolf501.top

【使用说明】
来源：http://cnk.sufxvd.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eun.chenjidiqi.icu

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xzr.smart0.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rjq.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://imw.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://epu.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ern.hcnkem.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gzh.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xaz.fzhhl.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lvl.9152youxi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qdk.nanxuanxn.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ued.xuetiantiany.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jfo.cucudq.cn

【文件统计】
来源：http://pyc.xylfe.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://asb.sxryk.cn

--------------------------------------------------------------------------------
来源：http://zgh.yueranfly.top

目  录
来源：http://ann.jianghu66.top

--------------------------------------------------------------------------------
来源：http://hzd.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ulf.316326.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://etv.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hwr.xziqi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ppr.zhaomingkeji.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mvo.jinyuanbaomall.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pon.aizwys.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hki.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pmc.aibaodan.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hhp.jinqigfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fgl.jyoumei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hur.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fsy.yongpay.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ult.zhiwuduotai.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://igc.316326.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oav.jqgufenzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zrf.yangfankeji.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hkt.iojbl.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ffh.bjfxy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vla.sxryk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ral.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qec.fehbvm.com

================================================================================
来源：http://mlr.pengpengdd.cyou

A. 基础语法与类型
来源：http://zfw.c1oappe.top

================================================================================
来源：http://ayo.sxryk.cn

[A01] Hello World
来源：http://sdc.shanyushiyangkeji.top

Py:   print("Hello, World!")
来源：http://deh.hnxiangtu.top

PHP:  echo "Hello, World!";
来源：http://sby.jyoumei.cn

JS:   console.log("Hello, World!");
来源：http://oyp.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vop.daxiang520.top

Java: System.out.println("Hello, World!");
来源：http://njh.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://ggi.zdbjq.cn

Ruby: puts "Hello, World!"
来源：http://zzu.cqqwz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://uzv.yj20258.top

[A02] 变量声明与赋值
来源：http://txd.hywenlv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jvh.chenzaomai.com

PHP:  $name = "Alex"; $age = 20;
来源：http://pno.xinyue.icu

JS:   let name = "Alex"; const age = 20;
来源：http://rex.hysaishi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nkv.jiagoushi.top

Java: String name = "Alex"; int age = 20;
来源：http://oru.hywenlv.cn

Go:   name := "Alex"; age := 20
来源：http://roi.yfazqb.com

Ruby: name = "Alex"; age = 20
来源：http://nkw.zhijiandao.cn

C#:   string name = "Alex"; int age = 20;
来源：http://arc.xingfuxueyuan.xyz

[A03] 常量定义
来源：http://upt.jianghu66.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jfg.9152youxi.cn

PHP:  const PI = 3.14159;
来源：http://vvr.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://ksq.zdqjudy.top

TS:   const PI: number = 3.14159;
来源：http://qvq.jlsjyb.cn

Java: static final double PI = 3.14159;
来源：http://txf.xuanzx.com

Go:   const PI = 3.14159
来源：http://siy.quarkkingdee.top

Ruby: PI = 3.14159
来源：http://vlr.yvedp.cn

C#:   const double PI = 3.14159;
来源：http://suz.zdqjudy.top

[A04] 判断变量类型
来源：http://adu.tarul.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ozn.zhixingplan.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vup.daria6918.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lgi.hcnkem.com

TS:   typeof x; x instanceof Date
来源：http://ntz.hywenlv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xrr.yuanzhike.top

Go:   reflect.TypeOf(x).Name()
来源：http://ynb.ywan-chungtsiang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://oen.zdbjq.cn

C#:   x.GetType().Name; x is int
来源：http://lfx.dashuyun.cn

[A05] 整数除法与取模
来源：http://fiw.aizwys.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ljf.ppjwa.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://baw.yueranfly.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rcb.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jdn.birdmap.top

Java: 7 / 2; 7 % 2
来源：http://pbu.zhijiandao.cn

Go:   7 / 2; 7 % 2
来源：http://zau.havefunace.top

Ruby: 7 / 2; 7 % 2
来源：http://nok.jinyuanbaomall.cn

C#:   7 / 2; 7 % 2
来源：http://hci.aizwys.cn

[A06] 字符串转数字
来源：http://lof.fehbvm.com

Py:   int("42"); float("3.14")
来源：http://cna.chenlongwang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vql.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iuv.yanxiufei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jtt.sxryk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vqf.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ryp.tarul.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qqo.xingfuxueyuan.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bgk.jqgufenzy.top

[A07] 数字转字符串
来源：http://itd.sxryk.cn

Py:   str(42)
来源：http://qvn.chenjidiqi.icu

PHP:  (string) 42; strval(42)
来源：http://qpe.52xcode.cn

JS:   String(42); (42).toString()
来源：http://omt.nwbrower.top

TS:   String(42)
来源：http://ame.fzhhl.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nci.hywenlv.cn

Go:   strconv.Itoa(42)
来源：http://pbm.yongpay.top

Ruby: 42.to_s
来源：http://plf.snrcjt.cn

C#:   42.ToString()
来源：http://kqn.xinyue.icu

[A08] 取整与四舍五入
来源：http://azj.ybcxt.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rjz.gzhubu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vdx.nanxuanxn.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qjf.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nxj.tanke756.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wpv.ydzc1.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://itw.xziqi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://roe.nanxuanxn.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mxi.shzxlz.cn

[A09] 绝对值与最大最小值
来源：http://eor.chenzaomai.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ngi.ydjk.org.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nzx.zhengqikj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zpr.jyoumei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bkb.bjfxy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ljj.daxiang520.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://czy.redwolf501.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://srz.shanyushiyangtech.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ixz.nanxinkj.top

[A10] 生成随机数
来源：http://vsg.jinqigfzy.top

Py:   import random; random.randint(1, 100)
来源：http://bcu.aibaodan.cn

PHP:  random_int(1, 100);
来源：http://vjr.tarul.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tye.shanyushiyangtech.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zqx.vqdsnc.cn

Java: new Random().nextInt(100) + 1
来源：http://pjs.zhengqikj.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mvm.wangdashe.top

Ruby: rand(1..100)
来源：http://nas.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://bsq.zhoulong.xyz

[A11] 条件表达式（三元）
来源：http://cag.uphjek.com

Py:   "yes" if x > 0 else "no"
来源：http://igx.svipenyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rvl.havefunace.top

JS:   x > 0 ? "yes" : "no"
来源：http://fcr.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://nzk.jiagoushi.top

Java: x > 0 ? "yes" : "no"
来源：http://xok.yj202588.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dmx.9152youxi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://igi.ctjpmb.com

C#:   x > 0 ? "yes" : "no"
来源：http://oer.wangdashe.top

[A12] 字符串插值 / 格式化
来源：http://brq.ywan-chungtsiang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tia.zhoulong.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://flj.vqdsnc.cn

JS:   `Hello, ${name}!`
来源：http://rkw.dashuyun.cn

TS:   `Hello, ${name}!`
来源：http://put.zhixingplan.top

Java: "Hello, %s!".formatted(name)
来源：http://cfe.zdbjq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ghe.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://zum.daria6918.cn

C#:   $"Hello, {name}!"
来源：http://zuk.sjlbkw.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oow.tianlin.xyz

Py:   "第一行\n第二行"
来源：http://btb.shanyushiyangkeji.top

PHP:  "第一行\n第二行"
来源：http://pzd.gotoacloud.top

JS:   "第一行\n第二行"
来源：http://txq.xinyue.icu

TS:   "第一行\n第二行"
来源：http://uvj.hongshengwenyu.top

Java: "第一行\n第二行"
来源：http://xmy.ehwqpu.com

Go:   "第一行\n第二行"
来源：http://cwu.ctjpmb.com

Ruby: "第一行\n第二行"
来源：http://qvm.kuanghao11.cn

C#:   "第一行\n第二行"
来源：http://mup.meibo888.top

[A14] 注释写法
来源：http://xrt.cqqwz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vta.guowangkeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mgw.xinyue.icu

JS:   // 单行；/* 多行 */
来源：http://rto.vehdjk.com

TS:   // 单行；/* 多行 */
来源：http://lrp.aizwys.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cjq.fzhhl.top

Go:   // 单行；/* 多行 */
来源：http://yke.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://srh.xuanzx.com

C#:   // 单行；/* 多行 */
来源：http://czu.nanxinkj.top

[A15] 空值判断与默认值
来源：http://cek.sjlbkw.cn

Py:   value = data or "默认值"
来源：http://rlg.xziqi.cn

PHP:  $value = $data ?? "默认值";
来源：http://row.shzxlz.cn

JS:   const value = data ?? "默认值";
来源：http://bxt.aibaodan.cn

TS:   const value = data ?? "默认值";
来源：http://zms.hnqzz.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yum.wangdashe.top

Go:   if data == "" { data = "默认值" }
来源：http://ecr.hongshengwenyu.top

Ruby: value = data || "默认值"
来源：http://pzd.tanke756.top

C#:   var value = data ?? "默认值";
来源：http://ngg.svipenyu.cn

[A16] 真假值判断规则
来源：http://sbn.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sqq.jinghuilouyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://isd.tian-w.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xia.ybcxt.top

TS:   if (!x) {}
来源：http://bhi.birdmap.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://thk.zycfv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wuo.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://wal.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bso.yuxming.cn

[A17] 位运算
来源：http://psl.xuetiantiany.cn


<!-- 参考信息 -->