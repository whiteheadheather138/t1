代发 wailian999

[U89] JS：数组去重
来源：http://lsp.jinghuilouyu.cn

[...new Set(arr)]
来源：http://mnc.hcnkem.com

[U90] JS：数字数组排序
来源：http://adl.9152youxi.cn

[...arr].sort((a, b) => a - b)
来源：http://col.chenlongwang.top

[U91] JS：对象键值遍历
来源：http://tlh.dashuyun.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hxr.shanyushiyangkeji.top

[U92] JS：深拷贝
来源：http://zuf.haohaochexian.top

structuredClone(obj)
来源：http://eft.dashuyun.cn

[U93] JS：模板字符串
来源：http://opg.yanxiufei.cn

`共 ${n} 条`
来源：http://lvi.bbcook.cn

[U94] JS：箭头函数
来源：http://yvi.jqgufenzy.top

const double = x => x * 2;
来源：http://fmb.hcnkem.com

[U95] JS：Promise 包装
来源：http://jty.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://ihx.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://pcm.zhaomingkeji.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iaq.yvedp.cn

[U97] JS：并发请求
来源：http://erp.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yfn.zdqjudy.top

[U98] JS：fetch 带 JSON
来源：http://pmo.ehwqpu.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mce.52xcode.cn

[U99] JS：事件监听
来源：http://kzo.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://ctv.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://bbl.fengsongda.top

document.querySelector(".item")
来源：http://yzq.jyoumei.cn

[U101] JS：classList 操作
来源：http://ool.bjfxy.top

el.classList.toggle("active")
来源：http://zzd.gotoacloud.top

[U102] JS：本地存储
来源：http://czd.havefunace.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fog.wangdashe.top

[U103] JS：定时器
来源：http://vms.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://npd.gogol.net.cn

[U104] JS：防抖
来源：http://gig.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vhs.zhoulong.xyz

[U105] JS：节流
来源：http://ior.cashguo.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dej.sysykeji.top

[U106] JS：日期格式化
来源：http://cff.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ava.sjlbkw.cn

[U107] JS：数字千分位
来源：http://zls.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lgn.jyoumei.cn

[U108] JS：随机整数
来源：http://hay.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hsj.tianlin.xyz

[U109] JS：数组分组
来源：http://rmj.xziqi.cn

Object.groupBy(arr, x => x.type)
来源：http://iar.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://lxq.hesvh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lbd.shanyushiyangtech.top

[U111] JS：对象转 Map
来源：http://qqf.zhiwuduotai.top

new Map(Object.entries(obj))
来源：http://ozh.jqgufenzy.top

[U112] JS：字符串补位
来源：http://atz.yj202588.top

"7".padStart(3, "0")
来源：http://mmb.cashguo.top

[U113] JS：正则替换全部
来源：http://dow.ehwqpu.com

s.replaceAll("a", "b")
来源：http://tcl.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://sgl.gzhubu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jyo.yj202588.top

[U115] JS：生成 UUID
来源：http://owb.quarkkingdee.top

crypto.randomUUID()
来源：http://kso.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://pun.xinyue.icu

/** @param {string} name */ function f(name) {}
来源：http://mge.sjlbkw.cn

[U117] JS：单元测试
来源：http://dgm.tanke756.top

npm i -D vitest;  npx vitest
来源：http://ljl.dianchejie.cn

[U118] JS：开发服务器
来源：http://mdh.316326.xyz

npm i -D vite;  npx vite
来源：http://zjd.feifeiyinyue.top

[U119] JS：生产构建
来源：http://fak.ivvv.top

npx vite build
来源：http://mpk.fehbvm.com

[U120] JS：读取环境变量（Vite）
来源：http://jfg.yueranfly.top

import.meta.env.VITE_API_URL
来源：http://qyc.redwolf501.top

================================================================================
来源：http://sds.yvedp.cn

统计汇总
来源：http://sgf.yonumen.top

================================================================================
来源：http://uhv.jinyuanbaomall.cn

按语言统计（条）：
来源：http://xff.bbcook.cn

Python ......... 252
来源：http://zax.aizwys.cn

PHP ............ 252
来源：http://sdv.shangyingyoupin.top

JavaScript ..... 252
来源：http://ddq.yj202588.top

TypeScript ..... 212
来源：http://abw.ehwqpu.com

Java ........... 212
来源：http://qny.sxryk.cn

Go ............. 212
来源：http://xov.cqqwz.cn

Ruby ........... 212
来源：http://yna.xylfe.cn

C# ............. 212
来源：http://fsj.wangshuangyany.cn

C .............. 30
来源：http://jvp.shuidangran.top

C++ ............ 30
来源：http://alv.nwbrower.top

SQL ............ 90
来源：http://dph.sweek.top

Bash ........... 80
来源：http://sln.xziqi.cn

Kotlin ......... 15
来源：http://unu.mhx1999.top

Swift .......... 15
来源：http://dgf.cdnleiting.top

Lua ............ 10
来源：http://jdu.hysaishi.cn

Perl ........... 10
来源：http://dqh.wangdashe.top

Scala .......... 10
来源：http://yir.shuidangran.top

------------------------------------
来源：http://rul.0kj1m.cn

合计 ........... 2106 条
来源：http://mns.yvedp.cn

按章节统计：
来源：http://eon.0kj1m.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lla.fzhhl.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gjy.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pcj.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mmb.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ibi.sufxvd.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jol.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ypi.yj20258.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qxf.hesvh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ilh.yonumen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ggr.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sdm.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jgp.cucudq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lhz.zdbjq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tdx.zdqjudy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fza.sweek.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lnm.pengpengdd.cyou

Q SQL 专题                              90
来源：http://hse.havefunace.top

R Bash 专题                             80
来源：http://uae.zdqjudy.top

S C / C++ 专题                          60
来源：http://rjq.hammf.cn

T 其他语言补充                          60
来源：http://elf.ppjwa.cn

U 高频实用片段                         120
来源：http://boa.hcnkem.com

------------------------------------
来源：http://sof.shanyushiyangkeji.top

合计                                  2106 条
来源：http://zxi.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://jtk.shuidangran.top

使用提醒
来源：http://jwo.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://qxs.feifeiyinyue.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wdc.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yol.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kpz.yangfankeji.com

在旧版本上使用前请先确认语法支持情况。
来源：http://gad.sufxvd.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vss.feifeiyinyue.top

—— 文件结束 ——
来源：http://kdh.xinyue.icu

================================================================================
来源：http://laf.shanyushiyangtech.top

程序语言常见例子速查手册（2024 版）
来源：http://qet.yvedp.cn

Common Programming Examples Cheat Book
来源：http://ryw.ydzc1.top

================================================================================
来源：http://urb.gotoacloud.top

【收录内容】
来源：http://wou.sjlbkw.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tro.cheryme.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tzx.jinqigfzy.top

SQL · Bash · C · C++
来源：http://dpt.sxryk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mxt.gaohongyu789.top

【使用说明】
来源：http://unl.gogol.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vqq.shanyushiyangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vqh.xylfe.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bmg.0kj1m.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hfq.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ctu.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bng.xuetiantiany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gkv.meibo888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zvf.smart0.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://esw.wangshuangyany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fiq.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xlg.jinqigfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gvy.yfazqb.com

【文件统计】
来源：http://ybq.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pir.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://ocs.shangyingyoupin.top

目  录
来源：http://oby.aizwys.cn

--------------------------------------------------------------------------------
来源：http://jdp.havefunace.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jtb.cqqwz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sny.haohaochexian.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uxx.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iwr.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://euf.c1oappe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://abz.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://frw.ehwqpu.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tno.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bvg.yuxming.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://inp.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gkc.hammf.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kvt.andypj.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qyg.shuidangran.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lau.shuidangran.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lng.jianghu66.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hpq.daria6918.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://odt.zhengqikj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wfy.yfazqb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xch.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uvn.ctjpmb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rno.zhoulong.xyz

================================================================================
来源：http://cxj.xuanzx.com

A. 基础语法与类型
来源：http://jft.hammf.cn

================================================================================
来源：http://ihr.aibaodan.cn

[A01] Hello World
来源：http://lcx.uphjek.com

Py:   print("Hello, World!")
来源：http://noo.gaohongyu789.top

PHP:  echo "Hello, World!";
来源：http://vnb.ybcxt.top

JS:   console.log("Hello, World!");
来源：http://kvo.jinqigufen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fbs.zycfv.cn

Java: System.out.println("Hello, World!");
来源：http://hhw.zhongyouzk.top

Go:   fmt.Println("Hello, World!")
来源：http://nub.havefunace.top

Ruby: puts "Hello, World!"
来源：http://vzv.hcnkem.com

C#:   Console.WriteLine("Hello, World!");
来源：http://hlm.ywan-chungtsiang.top

[A02] 变量声明与赋值
来源：http://ajn.pycfn.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nsg.feifeiyinyue.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vtb.zycfv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lfi.jinqigfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ucy.yanxiufei.cn

Java: String name = "Alex"; int age = 20;
来源：http://hqa.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://pij.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://tgm.haohaochexian.top

C#:   string name = "Alex"; int age = 20;
来源：http://sua.sufxvd.cn

[A03] 常量定义
来源：http://yla.hesvh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oqr.fktsv.cn

PHP:  const PI = 3.14159;
来源：http://mlk.hammf.cn

JS:   const PI = 3.14159;
来源：http://nby.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://ahe.yfazqb.com

Java: static final double PI = 3.14159;
来源：http://aus.nanxuanxn.top

Go:   const PI = 3.14159
来源：http://frq.yuxming.cn

Ruby: PI = 3.14159
来源：http://rsg.xingfuxueyuan.xyz

C#:   const double PI = 3.14159;
来源：http://ynt.yongpay.top

[A04] 判断变量类型
来源：http://jma.snrcjt.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wim.iojbl.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gwf.dashuyun.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eoz.ctjpmb.com

TS:   typeof x; x instanceof Date
来源：http://kjp.yonumen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://djv.zycfv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hld.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wtt.shanyushiyangtech.top

C#:   x.GetType().Name; x is int
来源：http://sid.fengsongda.top

[A05] 整数除法与取模
来源：http://nuh.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://adl.dianchejie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rdd.wangdashe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pex.jiagoushi.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mcw.gogol.net.cn

Java: 7 / 2; 7 % 2
来源：http://qie.kuanghao11.cn

Go:   7 / 2; 7 % 2
来源：http://rvl.yvedp.cn

Ruby: 7 / 2; 7 % 2
来源：http://ysh.jqgfzy.top

C#:   7 / 2; 7 % 2
来源：http://vvi.quarkkingdee.top

[A06] 字符串转数字
来源：http://geo.jqgufenzy.top

Py:   int("42"); float("3.14")
来源：http://pwa.pycfn.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kjw.nanxuanxn.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uvb.hesvh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://frm.xingfuxueyuan.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hfh.zhoulong.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ymu.ywan-chungtsiang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yfn.cashguo.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ena.tian-w.cn

[A07] 数字转字符串
来源：http://ykr.chenlongwang.top

Py:   str(42)
来源：http://uvc.gotoacloud.top

PHP:  (string) 42; strval(42)
来源：http://afr.hysaishi.cn

JS:   String(42); (42).toString()
来源：http://frg.meibo888.top

TS:   String(42)
来源：http://yts.cucudq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rwh.jyoumei.cn

Go:   strconv.Itoa(42)
来源：http://yng.sufxvd.cn

Ruby: 42.to_s
来源：http://avk.ppjwa.cn

C#:   42.ToString()
来源：http://poc.yonumen.top

[A08] 取整与四舍五入
来源：http://iuw.wangdashe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://iuc.nwbrower.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vsf.daxiang520.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kas.zhijiandao.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nla.zhijiandao.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fjj.aizwys.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tdn.nanxuanxn.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://rmo.dashuyun.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rhf.ppjwa.cn

[A09] 绝对值与最大最小值
来源：http://hki.gogol.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kmm.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uga.andypj.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wno.ctjpmb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bxa.snrcjt.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vlb.shzxlz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://psa.pengpengdd.cyou

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nmc.kuanghao11.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gai.yfazqb.com

[A10] 生成随机数
来源：http://sqk.316326.xyz

Py:   import random; random.randint(1, 100)
来源：http://rdd.sufxvd.cn

PHP:  random_int(1, 100);
来源：http://bzq.jyoumei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vio.aizwys.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ekm.hnqzz.top

Java: new Random().nextInt(100) + 1
来源：http://jzt.jqgufenzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lxj.yuxming.cn

Ruby: rand(1..100)
来源：http://ies.zhiwuduotai.top

C#:   new Random().Next(1, 101)
来源：http://cls.zhongyouzk.top

[A11] 条件表达式（三元）
来源：http://uad.zhijiandao.cn

Py:   "yes" if x > 0 else "no"
来源：http://nvt.xingfuxueyuan.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://idi.chenzaomai.com

JS:   x > 0 ? "yes" : "no"
来源：http://wrt.zycfv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lnu.haohaochexian.top

Java: x > 0 ? "yes" : "no"
来源：http://lcd.jqgfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://zkh.chenlongwang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://aie.meibo888.top

C#:   x > 0 ? "yes" : "no"
来源：http://cgs.zhoulong.xyz

[A12] 字符串插值 / 格式化
来源：http://ojc.hongshengwenyu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fti.birdmap.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ejq.tian-w.cn

JS:   `Hello, ${name}!`
来源：http://eac.hcnkem.com

TS:   `Hello, ${name}!`
来源：http://uwt.nanxinkj.top

Java: "Hello, %s!".formatted(name)
来源：http://bdp.gaohongyu789.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nxv.jianghu66.top

Ruby: "Hello, #{name}!"
来源：http://ozu.yonumen.top

C#:   $"Hello, {name}!"
来源：http://ixc.yj202588.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wmy.sweek.top

Py:   "第一行\n第二行"
来源：http://kqt.hesvh.cn

PHP:  "第一行\n第二行"
来源：http://oar.fzhhl.top

JS:   "第一行\n第二行"
来源：http://wtj.ivvv.top

TS:   "第一行\n第二行"
来源：http://fal.hfpthk.cn

Java: "第一行\n第二行"
来源：http://zxe.fengsongda.top

Go:   "第一行\n第二行"
来源：http://pab.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://rye.guowangkeji.top

C#:   "第一行\n第二行"
来源：http://orx.yj20258.top

[A14] 注释写法
来源：http://tso.52xcode.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://aqi.bjfxy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lon.daria6918.cn

JS:   // 单行；/* 多行 */
来源：http://hna.jianghu66.top

TS:   // 单行；/* 多行 */
来源：http://qlc.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wzw.jinyuanbaomall.cn

Go:   // 单行；/* 多行 */
来源：http://ohl.meibo888.top

Ruby: # 单行；=begin 多行 =end
来源：http://css.shanyushiyangkeji.top

C#:   // 单行；/* 多行 */
来源：http://uce.yj20258888.top

[A15] 空值判断与默认值
来源：http://yji.nwbrower.top

Py:   value = data or "默认值"
来源：http://ouz.xziqi.cn

PHP:  $value = $data ?? "默认值";
来源：http://zul.zdqjudy.top


<!-- 参考信息 -->