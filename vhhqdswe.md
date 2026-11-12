代发 wailian999

[U89] JS：数组去重
来源：http://ueu.yongpay.top

[...new Set(arr)]
来源：http://slp.snrcjt.cn

[U90] JS：数字数组排序
来源：http://imw.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://ykv.yj20258.top

[U91] JS：对象键值遍历
来源：http://qtw.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://znv.jlsjyb.cn

[U92] JS：深拷贝
来源：http://mwj.kuanghao11.cn

structuredClone(obj)
来源：http://gfj.haohaochexian.top

[U93] JS：模板字符串
来源：http://wep.iojbl.cn

`共 ${n} 条`
来源：http://ijs.316326.xyz

[U94] JS：箭头函数
来源：http://bss.shanyushiyangtech.top

const double = x => x * 2;
来源：http://umq.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://ysw.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://ali.yfazqb.com

[U96] JS：async/await 与异常
来源：http://ddk.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rks.yfazqb.com

[U97] JS：并发请求
来源：http://ogs.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rsa.sweek.top

[U98] JS：fetch 带 JSON
来源：http://exs.yangfankeji.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zxz.tianlin.xyz

[U99] JS：事件监听
来源：http://ild.bbcook.cn

el.addEventListener("click", e => {})
来源：http://wja.bjfxy.top

[U100] JS：DOM 查询
来源：http://amn.smart0.xyz

document.querySelector(".item")
来源：http://gmd.hesvh.cn

[U101] JS：classList 操作
来源：http://vun.xylfe.cn

el.classList.toggle("active")
来源：http://kps.chenlongwang.top

[U102] JS：本地存储
来源：http://umu.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ulo.hysaishi.cn

[U103] JS：定时器
来源：http://cnp.fzhhl.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bdp.fengsongda.top

[U104] JS：防抖
来源：http://fmq.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wqq.havefunace.top

[U105] JS：节流
来源：http://czn.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://alf.haohaochexian.top

[U106] JS：日期格式化
来源：http://cly.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tlr.jinqigufen.top

[U107] JS：数字千分位
来源：http://xpk.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ifr.hcnkem.com

[U108] JS：随机整数
来源：http://lyr.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qwb.gzhubu.top

[U109] JS：数组分组
来源：http://sro.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://mcj.nanxinkj.top

[U110] JS：数组分块
来源：http://dzo.yvedp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dbr.hysaishi.cn

[U111] JS：对象转 Map
来源：http://jvm.jlsjyb.cn

new Map(Object.entries(obj))
来源：http://bxw.gotoacloud.top

[U112] JS：字符串补位
来源：http://ejz.hfpthk.cn

"7".padStart(3, "0")
来源：http://poq.fanxiaobao.xyz

[U113] JS：正则替换全部
来源：http://cef.zhoulong.xyz

s.replaceAll("a", "b")
来源：http://wtq.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://cjf.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ady.ctjpmb.com

[U115] JS：生成 UUID
来源：http://ytc.cashguo.top

crypto.randomUUID()
来源：http://mnx.hongshengwenyu.top

[U116] JS：类型检查（JSDoc）
来源：http://sjd.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://dmv.tarul.cn

[U117] JS：单元测试
来源：http://axw.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://gcj.yangfankeji.com

[U118] JS：开发服务器
来源：http://lnx.guowangkeji.top

npm i -D vite;  npx vite
来源：http://skg.nanxinkj.top

[U119] JS：生产构建
来源：http://xem.hongshengwenyu.top

npx vite build
来源：http://mio.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://itd.nanxinkj.top

import.meta.env.VITE_API_URL
来源：http://iek.sweek.top

================================================================================
来源：http://yex.ivvv.top

统计汇总
来源：http://ksv.zhaomingkeji.xyz

================================================================================
来源：http://afm.cucudq.cn

按语言统计（条）：
来源：http://ofc.wangshuangyany.cn

Python ......... 252
来源：http://cyf.gotoacloud.top

PHP ............ 252
来源：http://vdc.tian-w.cn

JavaScript ..... 252
来源：http://hxj.cucudq.cn

TypeScript ..... 212
来源：http://ugq.jinqigfzy.top

Java ........... 212
来源：http://zbd.cqqwz.cn

Go ............. 212
来源：http://hfn.gotoacloud.top

Ruby ........... 212
来源：http://nwr.sxryk.cn

C# ............. 212
来源：http://dbt.redwolf501.top

C .............. 30
来源：http://awk.tianlin.xyz

C++ ............ 30
来源：http://bmw.yuanzhike.top

SQL ............ 90
来源：http://myz.mhx1999.top

Bash ........... 80
来源：http://oco.fzhhl.top

Kotlin ......... 15
来源：http://ucv.hongshengwenyu.top

Swift .......... 15
来源：http://bti.cqqwz.cn

Lua ............ 10
来源：http://yyg.zhiwuduotai.top

Perl ........... 10
来源：http://eek.zhaomingkeji.xyz

Scala .......... 10
来源：http://lsu.hnxiangtu.top

------------------------------------
来源：http://lct.guannengcc.top

合计 ........... 2106 条
来源：http://qmf.tanke756.top

按章节统计：
来源：http://rwe.316326.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xqe.ywan-chungtsiang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ofc.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sep.hfpthk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nuq.fengsongda.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ovi.havefunace.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ouo.nanxinkj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://shf.zhoulong.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ddl.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lkf.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://acn.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uic.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ezc.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://smk.fanxiaobao.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ial.redwolf501.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://atw.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ifp.0kj1m.cn

Q SQL 专题                              90
来源：http://tsr.gaohongyu789.top

R Bash 专题                             80
来源：http://wio.yuanzhike.top

S C / C++ 专题                          60
来源：http://kcx.aizwys.cn

T 其他语言补充                          60
来源：http://orb.aibaodan.cn

U 高频实用片段                         120
来源：http://gca.zhongyouzk.top

------------------------------------
来源：http://njk.yangfankeji.com

合计                                  2106 条
来源：http://yli.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://sto.shanyushiyangkeji.top

使用提醒
来源：http://vqi.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://ssj.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vsl.aizwys.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uio.tanke756.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wyl.fzhhl.top

在旧版本上使用前请先确认语法支持情况。
来源：http://iub.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://chg.xziqi.cn

—— 文件结束 ——
来源：http://umi.meibo888.top

================================================================================
来源：http://juf.cucudq.cn

程序语言常见例子速查手册（2024 版）
来源：http://djv.gzhubu.top

Common Programming Examples Cheat Book
来源：http://uxd.fehbvm.com

================================================================================
来源：http://npi.svipenyu.cn

【收录内容】
来源：http://meh.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vuo.shanyushiyangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jwi.9152youxi.cn

SQL · Bash · C · C++
来源：http://fdc.0kj1m.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kon.yj20258888.top

【使用说明】
来源：http://sxj.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://idd.hywenlv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fmb.jyoumei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kvj.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://agu.gaohongyu789.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wxy.nanxinkj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eeu.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vrt.shanyushiyangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://naf.quarkkingdee.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pss.birdmap.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vto.52xcode.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://puf.dianchejie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vcs.316326.xyz

【文件统计】
来源：http://ves.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://elw.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://utf.zhijiandao.cn

目  录
来源：http://oqg.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://hon.birdmap.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ceb.hnxiangtu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dxy.yj202588.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tkg.52xcode.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rit.zhijiandao.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oit.hcnkem.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mgi.hfpthk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hha.wangshuangyany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dec.vqdsnc.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://txo.yuxming.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oxu.shangyingyoupin.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dkz.shangyingyoupin.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dtl.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qtb.aibaodan.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cyb.gogol.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rjj.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nwm.xinyue.icu

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nup.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://gkd.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rof.birdmap.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nlq.sweek.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://esy.fktsv.cn

================================================================================
来源：http://red.shangyingyoupin.top

A. 基础语法与类型
来源：http://ccl.tarul.cn

================================================================================
来源：http://hdz.shuidangran.top

[A01] Hello World
来源：http://ktw.cashguo.top

Py:   print("Hello, World!")
来源：http://bad.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://xvl.yueranfly.top

JS:   console.log("Hello, World!");
来源：http://wqb.chenlongwang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pip.bbcook.cn

Java: System.out.println("Hello, World!");
来源：http://txc.fzhhl.top

Go:   fmt.Println("Hello, World!")
来源：http://uvp.mhx1999.top

Ruby: puts "Hello, World!"
来源：http://ada.xingfuxueyuan.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://jld.nwbrower.top

[A02] 变量声明与赋值
来源：http://kzy.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bnb.daxiang520.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jvx.guowangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://agn.feifeiyinyue.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fza.ehwqpu.com

Java: String name = "Alex"; int age = 20;
来源：http://ipm.hfpthk.cn

Go:   name := "Alex"; age := 20
来源：http://ohu.yj202588.top

Ruby: name = "Alex"; age = 20
来源：http://ffz.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://byd.gotoacloud.top

[A03] 常量定义
来源：http://aft.xingfuxueyuan.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fce.xuetiantiany.cn

PHP:  const PI = 3.14159;
来源：http://tof.pengpengdd.cyou

JS:   const PI = 3.14159;
来源：http://cpy.nanxinkj.top

TS:   const PI: number = 3.14159;
来源：http://jed.snrcjt.cn

Java: static final double PI = 3.14159;
来源：http://xim.fanxiaobao.xyz

Go:   const PI = 3.14159
来源：http://ahq.ybcxt.top

Ruby: PI = 3.14159
来源：http://sgz.aizwys.cn

C#:   const double PI = 3.14159;
来源：http://qgs.yangfankeji.com

[A04] 判断变量类型
来源：http://pmm.hesvh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://voy.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bfw.jqgfzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vqr.hywenlv.cn

TS:   typeof x; x instanceof Date
来源：http://bnr.tian-w.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://owz.ctjpmb.com

Go:   reflect.TypeOf(x).Name()
来源：http://acx.tianlin.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://lhw.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://jra.hysaishi.cn

[A05] 整数除法与取模
来源：http://gnm.jianghu66.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jtg.ywan-chungtsiang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://pjw.nanxuanxn.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://udy.jianghu66.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://roy.yj202588.top

Java: 7 / 2; 7 % 2
来源：http://eff.zhiwuduotai.top

Go:   7 / 2; 7 % 2
来源：http://lpu.jinghuilouyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://rru.xingfuxueyuan.xyz

C#:   7 / 2; 7 % 2
来源：http://umu.dianchejie.cn

[A06] 字符串转数字
来源：http://yap.fktsv.cn

Py:   int("42"); float("3.14")
来源：http://ppl.0kj1m.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hoz.shanyushiyangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jmj.sweek.top

TS:   parseInt("42", 10); Number("42")
来源：http://znm.hcnkem.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xvh.vqdsnc.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tzx.tian-w.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tmt.chenlongwang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oak.sxryk.cn

[A07] 数字转字符串
来源：http://dut.haohaochexian.top

Py:   str(42)
来源：http://xjk.hcnkem.com

PHP:  (string) 42; strval(42)
来源：http://rpv.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://gej.jyoumei.cn

TS:   String(42)
来源：http://swc.daria6918.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://azq.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://vqn.ppjwa.cn

Ruby: 42.to_s
来源：http://vur.xuetiantiany.cn

C#:   42.ToString()
来源：http://lwu.dashuyun.cn

[A08] 取整与四舍五入
来源：http://fas.zhiwuduotai.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wtz.hywenlv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rll.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hjy.xylfe.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yiu.jqgufenzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ccq.yuanzhike.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nta.wangdashe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lgb.sxryk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lhd.ybcxt.top

[A09] 绝对值与最大最小值
来源：http://gzd.cucudq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://onq.xuanzx.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bfd.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hmp.guowangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iwc.epnwcf.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ler.jlsjyb.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oyc.hnxiangtu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vso.jinghuilouyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ucv.quarkkingdee.top

[A10] 生成随机数
来源：http://njq.0kj1m.cn

Py:   import random; random.randint(1, 100)
来源：http://flb.fengsongda.top

PHP:  random_int(1, 100);
来源：http://fcs.nanxuanxn.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rcu.yfazqb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://loq.vehdjk.com

Java: new Random().nextInt(100) + 1
来源：http://yaj.zhijiandao.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://you.feifeiyinyue.top

Ruby: rand(1..100)
来源：http://wte.sxryk.cn

C#:   new Random().Next(1, 101)
来源：http://dzl.hnqzz.top

[A11] 条件表达式（三元）
来源：http://fxd.hywenlv.cn

Py:   "yes" if x > 0 else "no"
来源：http://ctn.yueranfly.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lbd.yj20258888.top

JS:   x > 0 ? "yes" : "no"
来源：http://gzg.daria6918.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vnr.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://lie.fanxiaobao.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://uvk.xziqi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://man.yuxming.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qxc.cqqwz.cn

[A12] 字符串插值 / 格式化
来源：http://ryr.kuanghao11.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hsa.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qhc.havefunace.top

JS:   `Hello, ${name}!`
来源：http://hvf.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://ngf.shanyushiyangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://yls.yvedp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tri.9152youxi.cn

Ruby: "Hello, #{name}!"
来源：http://wmq.wangshuangyany.cn

C#:   $"Hello, {name}!"
来源：http://epe.ydzc1.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ikq.tianlin.xyz

Py:   "第一行\n第二行"
来源：http://wis.gotoacloud.top

PHP:  "第一行\n第二行"
来源：http://hpj.fehbvm.com

JS:   "第一行\n第二行"
来源：http://kiq.xylfe.cn

TS:   "第一行\n第二行"
来源：http://pbc.zhijiandao.cn

Java: "第一行\n第二行"
来源：http://oio.zhongyouzk.top

Go:   "第一行\n第二行"
来源：http://yhs.yvedp.cn

Ruby: "第一行\n第二行"
来源：http://wsp.tian-w.cn

C#:   "第一行\n第二行"
来源：http://juy.fzhhl.top

[A14] 注释写法
来源：http://lca.jinyuanbaomall.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kbi.birdmap.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://sdj.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://tnt.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://bme.daria6918.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://frk.jinqigufen.top

Go:   // 单行；/* 多行 */
来源：http://pae.uphjek.com

Ruby: # 单行；=begin 多行 =end
来源：http://pmw.c1oappe.top

C#:   // 单行；/* 多行 */
来源：http://esg.yueranfly.top

[A15] 空值判断与默认值
来源：http://pgl.zdbjq.cn

Py:   value = data or "默认值"
来源：http://kmm.hnxiangtu.top

PHP:  $value = $data ?? "默认值";
来源：http://nwy.daxiang520.top


<!-- 参考信息 -->