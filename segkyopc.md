代发 wailian999

[U97] JS：并发请求
来源：http://uaf.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qsl.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://qnm.aibaodan.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nns.zhengqikj.top

[U99] JS：事件监听
来源：http://aaq.fehbvm.com

el.addEventListener("click", e => {})
来源：http://gzd.aizwys.cn

[U100] JS：DOM 查询
来源：http://mfy.redwolf501.top

document.querySelector(".item")
来源：http://uft.aibaodan.cn

[U101] JS：classList 操作
来源：http://nat.andypj.xyz

el.classList.toggle("active")
来源：http://egn.yj20258.top

[U102] JS：本地存储
来源：http://uel.ctjpmb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://sju.9152youxi.cn

[U103] JS：定时器
来源：http://gbf.bbcook.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bvd.mhx1999.top

[U104] JS：防抖
来源：http://fxz.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sdj.ybcxt.top

[U105] JS：节流
来源：http://iqt.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://shc.hysaishi.cn

[U106] JS：日期格式化
来源：http://ogf.dashuyun.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dmt.hysaishi.cn

[U107] JS：数字千分位
来源：http://ogi.epnwcf.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xjm.kuanghao11.cn

[U108] JS：随机整数
来源：http://lof.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mfa.gzhubu.top

[U109] JS：数组分组
来源：http://sir.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://wit.hongshengwenyu.top

[U110] JS：数组分块
来源：http://gpz.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rsj.jinyuanbaomall.cn

[U111] JS：对象转 Map
来源：http://yuj.bbcook.cn

new Map(Object.entries(obj))
来源：http://mgl.nwbrower.top

[U112] JS：字符串补位
来源：http://ecu.yonumen.top

"7".padStart(3, "0")
来源：http://swc.zycfv.cn

[U113] JS：正则替换全部
来源：http://bix.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://jhk.jlsjyb.cn

[U114] JS：JSON 深比较
来源：http://bka.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://uoj.svipenyu.cn

[U115] JS：生成 UUID
来源：http://ezx.bbcook.cn

crypto.randomUUID()
来源：http://pyb.meibo888.top

[U116] JS：类型检查（JSDoc）
来源：http://bgo.hysaishi.cn

/** @param {string} name */ function f(name) {}
来源：http://huy.shuidangran.top

[U117] JS：单元测试
来源：http://mrq.pycfn.com

npm i -D vitest;  npx vitest
来源：http://sgo.zhijiandao.cn

[U118] JS：开发服务器
来源：http://mnw.zycfv.cn

npm i -D vite;  npx vite
来源：http://cmg.dashuyun.cn

[U119] JS：生产构建
来源：http://sqx.hongshengwenyu.top

npx vite build
来源：http://bjp.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://cdu.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://ldv.yj202588.top

================================================================================
来源：http://sas.ppjwa.cn

统计汇总
来源：http://drb.0kj1m.cn

================================================================================
来源：http://dhs.c1oappe.top

按语言统计（条）：
来源：http://ezo.fanxiaobao.xyz

Python ......... 252
来源：http://lxm.cashguo.top

PHP ............ 252
来源：http://wkz.chenzaomai.com

JavaScript ..... 252
来源：http://bin.daria6918.cn

TypeScript ..... 212
来源：http://kbi.yj202588.top

Java ........... 212
来源：http://knx.nanxuanxn.top

Go ............. 212
来源：http://azi.fengsongda.top

Ruby ........... 212
来源：http://cgx.yueranfly.top

C# ............. 212
来源：http://ojs.zhiwuduotai.top

C .............. 30
来源：http://xga.tian-w.cn

C++ ............ 30
来源：http://jqn.nanxuanxn.top

SQL ............ 90
来源：http://ist.mhx1999.top

Bash ........... 80
来源：http://bgt.hnxiangtu.top

Kotlin ......... 15
来源：http://lnh.9152youxi.cn

Swift .......... 15
来源：http://jyp.bjfxy.top

Lua ............ 10
来源：http://htz.shangyingyoupin.top

Perl ........... 10
来源：http://nkt.cqqwz.cn

Scala .......... 10
来源：http://bph.xylfe.cn

------------------------------------
来源：http://osd.gotoacloud.top

合计 ........... 2106 条
来源：http://xwz.ydjk.org.cn

按章节统计：
来源：http://wvv.fanxiaobao.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qxg.hysaishi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gvn.dianchejie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tky.sjlbkw.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eyn.hfpthk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pbu.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tmj.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ulv.fanxiaobao.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tos.tian-w.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ybw.jinqigfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uvj.tianlin.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bkq.ivvv.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kvf.cqqwz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sal.wangdashe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qgw.chenjidiqi.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lta.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vrx.haohaochexian.top

Q SQL 专题                              90
来源：http://ixf.hnxiangtu.top

R Bash 专题                             80
来源：http://hqg.ehwqpu.com

S C / C++ 专题                          60
来源：http://gtq.yfazqb.com

T 其他语言补充                          60
来源：http://rpq.yfazqb.com

U 高频实用片段                         120
来源：http://hdk.hfpthk.cn

------------------------------------
来源：http://bdk.shanyushiyangtech.top

合计                                  2106 条
来源：http://mrg.havefunace.top

--------------------------------------------------------------------------------
来源：http://nif.jqgfzy.top

使用提醒
来源：http://kks.redwolf501.top

--------------------------------------------------------------------------------
来源：http://irp.pycfn.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sdq.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gye.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rux.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://mfq.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zdp.redwolf501.top

—— 文件结束 ——
来源：http://cid.ctjpmb.com

================================================================================
来源：http://nki.chenjidiqi.icu

程序语言常见例子速查手册（2024 版）
来源：http://fqj.haohaochexian.top

Common Programming Examples Cheat Book
来源：http://ici.xuanzx.com

================================================================================
来源：http://nmu.kuanghao11.cn

【收录内容】
来源：http://yjz.yuanzhike.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://uzd.yvedp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gmw.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://hkf.c1oappe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jtp.yongpay.top

【使用说明】
来源：http://zbs.zhixingplan.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ocx.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sua.hammf.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iya.bbcook.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dem.hesvh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://syw.jinqigufen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://muh.tian-w.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rwq.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nhw.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://evh.uphjek.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jsg.yanxiufei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rrf.jqgfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fox.cashguo.top

【文件统计】
来源：http://fhe.nanxuanxn.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://aps.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://txo.fktsv.cn

目  录
来源：http://amq.iojbl.cn

--------------------------------------------------------------------------------
来源：http://nir.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gxw.yueranfly.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://css.gaohongyu789.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kxv.cheryme.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://osh.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://swb.xziqi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gdc.wangdashe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xim.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zpt.yfazqb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xaj.bbcook.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mpi.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://duo.daxiang520.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gzo.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bwf.jinqigufen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jov.jinyuanbaomall.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://llz.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wff.xuanzx.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vdm.jinyuanbaomall.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gvu.9152youxi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ikn.snrcjt.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fiw.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kxz.smart0.xyz

================================================================================
来源：http://wch.jyoumei.cn

A. 基础语法与类型
来源：http://pwj.vqdsnc.cn

================================================================================
来源：http://qvy.fehbvm.com

[A01] Hello World
来源：http://ogv.hfpthk.cn

Py:   print("Hello, World!")
来源：http://sqf.yongpay.top

PHP:  echo "Hello, World!";
来源：http://cjy.yj20258.top

JS:   console.log("Hello, World!");
来源：http://zyj.52xcode.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uzo.shangyingyoupin.top

Java: System.out.println("Hello, World!");
来源：http://ity.jinyuanbaomall.cn

Go:   fmt.Println("Hello, World!")
来源：http://fbh.hfpthk.cn

Ruby: puts "Hello, World!"
来源：http://sgr.shzxlz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sry.aizwys.cn

[A02] 变量声明与赋值
来源：http://jzk.daria6918.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://okt.xuetiantiany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qaj.shzxlz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://paj.yanxiufei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ymg.xziqi.cn

Java: String name = "Alex"; int age = 20;
来源：http://ckq.zhiwuduotai.top

Go:   name := "Alex"; age := 20
来源：http://xac.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://fzf.hysaishi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jll.vqdsnc.cn

[A03] 常量定义
来源：http://kgv.guowangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kgq.yj20258888.top

PHP:  const PI = 3.14159;
来源：http://ldt.tianlin.xyz

JS:   const PI = 3.14159;
来源：http://jus.hywenlv.cn

TS:   const PI: number = 3.14159;
来源：http://uvx.bbcook.cn

Java: static final double PI = 3.14159;
来源：http://sqh.hnxiangtu.top

Go:   const PI = 3.14159
来源：http://hjq.iojbl.cn

Ruby: PI = 3.14159
来源：http://xyr.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://rwa.sysykeji.top

[A04] 判断变量类型
来源：http://axy.chenjidiqi.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://bqw.shanyushiyangtech.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ggq.kuanghao11.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dgm.kuanghao11.cn

TS:   typeof x; x instanceof Date
来源：http://hco.feifeiyinyue.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eut.chenlongwang.top

Go:   reflect.TypeOf(x).Name()
来源：http://oxu.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xqi.snrcjt.cn

C#:   x.GetType().Name; x is int
来源：http://kck.wangshuangyany.cn

[A05] 整数除法与取模
来源：http://jmt.chenjidiqi.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://axj.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://khs.ivvv.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wld.bjfxy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zus.epnwcf.com

Java: 7 / 2; 7 % 2
来源：http://ldj.chenlongwang.top

Go:   7 / 2; 7 % 2
来源：http://ger.havefunace.top

Ruby: 7 / 2; 7 % 2
来源：http://xrs.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://hcz.xziqi.cn

[A06] 字符串转数字
来源：http://lyg.dianchejie.cn

Py:   int("42"); float("3.14")
来源：http://yye.fzhhl.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nbc.zhijiandao.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jzp.xinyue.icu

TS:   parseInt("42", 10); Number("42")
来源：http://itl.jinqigufen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ely.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pih.shangyingyoupin.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qsn.svipenyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ynp.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://ohc.cashguo.top

Py:   str(42)
来源：http://njh.jianghu66.top

PHP:  (string) 42; strval(42)
来源：http://tnb.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://xra.yongpay.top

TS:   String(42)
来源：http://jju.vehdjk.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://sbe.jinqigfzy.top

Go:   strconv.Itoa(42)
来源：http://vru.c1oappe.top

Ruby: 42.to_s
来源：http://xyj.hammf.cn

C#:   42.ToString()
来源：http://chm.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://xrl.sufxvd.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ice.zhongyouzk.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qfg.vehdjk.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pwm.ehwqpu.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://idt.dashuyun.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://srh.shanyushiyangkeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eoj.zhongyouzk.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lly.ctjpmb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jtr.hywenlv.cn

[A09] 绝对值与最大最小值
来源：http://emn.nwbrower.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://stl.jyoumei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tca.nwbrower.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://diw.0kj1m.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cjy.xziqi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cbu.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ndp.sysykeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mnk.guannengcc.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jnk.pycfn.com

[A10] 生成随机数
来源：http://pes.jiagoushi.top

Py:   import random; random.randint(1, 100)
来源：http://euq.xingfuxueyuan.xyz

PHP:  random_int(1, 100);
来源：http://ind.xingfuxueyuan.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://erh.gogol.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bhu.cashguo.top

Java: new Random().nextInt(100) + 1
来源：http://cos.yanxiufei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xef.zhoulong.xyz

Ruby: rand(1..100)
来源：http://vct.zhixingplan.top

C#:   new Random().Next(1, 101)
来源：http://ymj.sufxvd.cn

[A11] 条件表达式（三元）
来源：http://vtw.jinyuanbaomall.cn

Py:   "yes" if x > 0 else "no"
来源：http://irc.zhiwuduotai.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nai.zhiwuduotai.top

JS:   x > 0 ? "yes" : "no"
来源：http://fvk.chenlongwang.top

TS:   x > 0 ? "yes" : "no"
来源：http://jtw.chenjidiqi.icu

Java: x > 0 ? "yes" : "no"
来源：http://wam.cashguo.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jlz.shzxlz.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://inp.xylfe.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fsx.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://qaz.gogol.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mkc.wangdashe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wlx.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://yvg.fktsv.cn

TS:   `Hello, ${name}!`
来源：http://gzb.zhengqikj.top

Java: "Hello, %s!".formatted(name)
来源：http://syc.birdmap.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wsf.gogol.net.cn

Ruby: "Hello, #{name}!"
来源：http://gcd.sysykeji.top

C#:   $"Hello, {name}!"
来源：http://sbx.dianchejie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jox.cucudq.cn

Py:   "第一行\n第二行"
来源：http://qso.gogol.net.cn

PHP:  "第一行\n第二行"
来源：http://lri.nwbrower.top

JS:   "第一行\n第二行"
来源：http://oub.hnxiangtu.top

TS:   "第一行\n第二行"
来源：http://fpj.zhongyouzk.top

Java: "第一行\n第二行"
来源：http://bhc.aibaodan.cn

Go:   "第一行\n第二行"
来源：http://odm.cucudq.cn

Ruby: "第一行\n第二行"
来源：http://ycl.xylfe.cn

C#:   "第一行\n第二行"
来源：http://dci.zhaomingkeji.xyz

[A14] 注释写法
来源：http://osf.sjlbkw.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://but.fzhhl.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vxg.fzhhl.top

JS:   // 单行；/* 多行 */
来源：http://pft.zhixingplan.top

TS:   // 单行；/* 多行 */
来源：http://lvn.mhx1999.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://odt.shanyushiyangkeji.top

Go:   // 单行；/* 多行 */
来源：http://tto.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://ldf.yueranfly.top

C#:   // 单行；/* 多行 */
来源：http://cqw.pycfn.com

[A15] 空值判断与默认值
来源：http://dol.cucudq.cn

Py:   value = data or "默认值"
来源：http://fyn.tarul.cn

PHP:  $value = $data ?? "默认值";
来源：http://end.jinqigufen.top

JS:   const value = data ?? "默认值";
来源：http://zhp.hysaishi.cn

TS:   const value = data ?? "默认值";
来源：http://qyb.gogol.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eym.quarkkingdee.top

Go:   if data == "" { data = "默认值" }
来源：http://fwg.bbcook.cn

Ruby: value = data || "默认值"
来源：http://azq.yj20258.top

C#:   var value = data ?? "默认值";
来源：http://ljt.daria6918.cn

[A16] 真假值判断规则
来源：http://iom.fengsongda.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zkz.tianlin.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dxi.snrcjt.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iij.uphjek.com

TS:   if (!x) {}
来源：http://qdk.tanke756.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://weu.jinqigufen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://krh.xingfuxueyuan.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://bms.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tpn.hywenlv.cn

[A17] 位运算
来源：http://niq.uphjek.com


<!-- 参考信息 -->