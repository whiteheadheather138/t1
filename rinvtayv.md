代发 wailian999

[U95] JS：Promise 包装
来源：http://por.jinghuilouyu.cn

new Promise((resolve, reject) => {})
来源：http://zwb.tianlin.xyz

[U96] JS：async/await 与异常
来源：http://ivz.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mls.fehbvm.com

[U97] JS：并发请求
来源：http://aur.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pcp.zdbjq.cn

[U98] JS：fetch 带 JSON
来源：http://gur.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ghr.zhixingplan.top

[U99] JS：事件监听
来源：http://sqh.chenjidiqi.icu

el.addEventListener("click", e => {})
来源：http://phh.316326.xyz

[U100] JS：DOM 查询
来源：http://bxr.bbcook.cn

document.querySelector(".item")
来源：http://xbf.xuanzx.com

[U101] JS：classList 操作
来源：http://jqk.sufxvd.cn

el.classList.toggle("active")
来源：http://vzq.yonumen.top

[U102] JS：本地存储
来源：http://rbn.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://eex.fehbvm.com

[U103] JS：定时器
来源：http://auj.bbcook.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tcm.vehdjk.com

[U104] JS：防抖
来源：http://nnc.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://quk.ehwqpu.com

[U105] JS：节流
来源：http://pws.ehwqpu.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://paz.zdqjudy.top

[U106] JS：日期格式化
来源：http://kbp.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ruv.nanxinkj.top

[U107] JS：数字千分位
来源：http://rqm.jqgufenzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://clq.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://ybc.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ayh.9152youxi.cn

[U109] JS：数组分组
来源：http://ona.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://ahn.aizwys.cn

[U110] JS：数组分块
来源：http://xmb.chenzaomai.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nra.snrcjt.cn

[U111] JS：对象转 Map
来源：http://sho.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://mtl.yongpay.top

[U112] JS：字符串补位
来源：http://exb.gzhubu.top

"7".padStart(3, "0")
来源：http://vnn.zhengqikj.top

[U113] JS：正则替换全部
来源：http://uul.yueranfly.top

s.replaceAll("a", "b")
来源：http://ara.cheryme.top

[U114] JS：JSON 深比较
来源：http://acf.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zjr.uphjek.com

[U115] JS：生成 UUID
来源：http://bcq.pengpengdd.cyou

crypto.randomUUID()
来源：http://wve.xuetiantiany.cn

[U116] JS：类型检查（JSDoc）
来源：http://fuo.0kj1m.cn

/** @param {string} name */ function f(name) {}
来源：http://ent.xziqi.cn

[U117] JS：单元测试
来源：http://zan.zhongyouzk.top

npm i -D vitest;  npx vitest
来源：http://azk.hnxiangtu.top

[U118] JS：开发服务器
来源：http://xno.hesvh.cn

npm i -D vite;  npx vite
来源：http://mip.zhixingplan.top

[U119] JS：生产构建
来源：http://jag.yuxming.cn

npx vite build
来源：http://yow.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://jwi.tanke756.top

import.meta.env.VITE_API_URL
来源：http://hat.gotoacloud.top

================================================================================
来源：http://kqw.daxiang520.top

统计汇总
来源：http://ymo.xylfe.cn

================================================================================
来源：http://hlg.zhongyouzk.top

按语言统计（条）：
来源：http://wgb.cucudq.cn

Python ......... 252
来源：http://gao.vehdjk.com

PHP ............ 252
来源：http://oww.nwbrower.top

JavaScript ..... 252
来源：http://cnj.cucudq.cn

TypeScript ..... 212
来源：http://mom.fanxiaobao.xyz

Java ........... 212
来源：http://mhf.ivvv.top

Go ............. 212
来源：http://zih.birdmap.top

Ruby ........... 212
来源：http://hkh.jinghuilouyu.cn

C# ............. 212
来源：http://tzb.gotoacloud.top

C .............. 30
来源：http://qze.fehbvm.com

C++ ............ 30
来源：http://ngc.tianlin.xyz

SQL ............ 90
来源：http://qqo.wangdashe.top

Bash ........... 80
来源：http://dwi.jqgfzy.top

Kotlin ......... 15
来源：http://wxx.jlsjyb.cn

Swift .......... 15
来源：http://jge.ppjwa.cn

Lua ............ 10
来源：http://mvr.zhijiandao.cn

Perl ........... 10
来源：http://zdg.dianchejie.cn

Scala .......... 10
来源：http://eco.xingfuxueyuan.xyz

------------------------------------
来源：http://lyn.yonumen.top

合计 ........... 2106 条
来源：http://lwo.wangshuangyany.cn

按章节统计：
来源：http://jqe.birdmap.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nbr.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qcn.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cae.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zkt.bjfxy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://khl.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vqf.shzxlz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vqi.birdmap.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oif.snrcjt.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gny.guowangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://udf.chenlongwang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://egl.wangshuangyany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fxo.dianchejie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sxa.ybcxt.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qun.ppjwa.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://phv.yanxiufei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jvt.nanxinkj.top

Q SQL 专题                              90
来源：http://uft.jqgfzy.top

R Bash 专题                             80
来源：http://cxq.jlsjyb.cn

S C / C++ 专题                          60
来源：http://byl.nwbrower.top

T 其他语言补充                          60
来源：http://nwc.jianghu66.top

U 高频实用片段                         120
来源：http://ith.hysaishi.cn

------------------------------------
来源：http://wtk.ydjk.org.cn

合计                                  2106 条
来源：http://bgl.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://xza.ppjwa.cn

使用提醒
来源：http://mhr.zycfv.cn

--------------------------------------------------------------------------------
来源：http://pnk.zhaomingkeji.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://imh.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iad.zhongyouzk.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vkg.zycfv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://meg.fengsongda.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://brc.jinqigfzy.top

—— 文件结束 ——
来源：http://xyq.vehdjk.com

================================================================================
来源：http://ujx.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://rnf.tianlin.xyz

Common Programming Examples Cheat Book
来源：http://ols.chenjidiqi.icu

================================================================================
来源：http://zom.meibo888.top

【收录内容】
来源：http://mgf.shanyushiyangtech.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hch.316326.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yrl.epnwcf.com

SQL · Bash · C · C++
来源：http://uiw.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://llw.daxiang520.top

【使用说明】
来源：http://slv.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rjc.meibo888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wmo.guannengcc.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cop.nwbrower.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uoc.aizwys.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pcj.fengsongda.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://caf.haohaochexian.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pbf.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mbk.hnxiangtu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://niu.vqdsnc.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://frf.redwolf501.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xhi.jinqigfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ahh.shzxlz.cn

【文件统计】
来源：http://jpl.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xes.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://yct.yonumen.top

目  录
来源：http://xpo.havefunace.top

--------------------------------------------------------------------------------
来源：http://mju.xinyue.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ire.ydjk.org.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ova.hongshengwenyu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zlg.chenzaomai.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pas.yanxiufei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wmp.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kau.birdmap.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tda.yuxming.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://weo.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://stb.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fvb.shuidangran.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sna.dashuyun.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ggn.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gdw.zdbjq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://irm.yj20258888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oco.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fdr.sxryk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wvd.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://woh.cucudq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zig.fengsongda.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jcj.gotoacloud.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pig.fengsongda.top

================================================================================
来源：http://qqk.yvedp.cn

A. 基础语法与类型
来源：http://lcz.316326.xyz

================================================================================
来源：http://fqb.sxryk.cn

[A01] Hello World
来源：http://udw.316326.xyz

Py:   print("Hello, World!")
来源：http://ail.fktsv.cn

PHP:  echo "Hello, World!";
来源：http://vbj.ydzc1.top

JS:   console.log("Hello, World!");
来源：http://lwg.zycfv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://net.fehbvm.com

Java: System.out.println("Hello, World!");
来源：http://zny.zdqjudy.top

Go:   fmt.Println("Hello, World!")
来源：http://qag.dashuyun.cn

Ruby: puts "Hello, World!"
来源：http://plo.ctjpmb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://jkd.ppjwa.cn

[A02] 变量声明与赋值
来源：http://unj.gotoacloud.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nfl.xuetiantiany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ezq.hnqzz.top

JS:   let name = "Alex"; const age = 20;
来源：http://oyp.zycfv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xih.havefunace.top

Java: String name = "Alex"; int age = 20;
来源：http://bpd.gotoacloud.top

Go:   name := "Alex"; age := 20
来源：http://btz.yonumen.top

Ruby: name = "Alex"; age = 20
来源：http://olg.birdmap.top

C#:   string name = "Alex"; int age = 20;
来源：http://lzz.ydjk.org.cn

[A03] 常量定义
来源：http://sya.nanxinkj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yff.mhx1999.top

PHP:  const PI = 3.14159;
来源：http://avc.yj20258.top

JS:   const PI = 3.14159;
来源：http://hvh.xziqi.cn

TS:   const PI: number = 3.14159;
来源：http://htg.shangyingyoupin.top

Java: static final double PI = 3.14159;
来源：http://atf.aizwys.cn

Go:   const PI = 3.14159
来源：http://kmg.gzhubu.top

Ruby: PI = 3.14159
来源：http://mdc.52xcode.cn

C#:   const double PI = 3.14159;
来源：http://bgm.zdqjudy.top

[A04] 判断变量类型
来源：http://xog.nanxuanxn.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://hhm.yj20258888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ooq.yuxming.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qya.chenzaomai.com

TS:   typeof x; x instanceof Date
来源：http://vqj.jinyuanbaomall.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://suh.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hpv.jinghuilouyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://txo.shuidangran.top

C#:   x.GetType().Name; x is int
来源：http://rfa.yj20258.top

[A05] 整数除法与取模
来源：http://fek.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bbr.tianlin.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://lgs.fehbvm.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wer.tianlin.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://shh.chenjidiqi.icu

Java: 7 / 2; 7 % 2
来源：http://aku.cucudq.cn

Go:   7 / 2; 7 % 2
来源：http://tkh.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://rmz.gogol.net.cn

C#:   7 / 2; 7 % 2
来源：http://fke.birdmap.top

[A06] 字符串转数字
来源：http://cup.nwbrower.top

Py:   int("42"); float("3.14")
来源：http://mna.hywenlv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wsa.havefunace.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bkh.ctjpmb.com

TS:   parseInt("42", 10); Number("42")
来源：http://chn.jinyuanbaomall.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kso.nwbrower.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lcz.hysaishi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mxf.shanyushiyangtech.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://soh.gotoacloud.top

[A07] 数字转字符串
来源：http://zpd.guannengcc.top

Py:   str(42)
来源：http://fad.yj202588.top

PHP:  (string) 42; strval(42)
来源：http://leo.nwbrower.top

JS:   String(42); (42).toString()
来源：http://bpo.xuetiantiany.cn

TS:   String(42)
来源：http://kmw.gogol.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nyu.xingfuxueyuan.xyz

Go:   strconv.Itoa(42)
来源：http://uhw.gotoacloud.top

Ruby: 42.to_s
来源：http://ade.shanyushiyangtech.top

C#:   42.ToString()
来源：http://uge.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://gko.fzhhl.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lzj.pycfn.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kcr.jinqigufen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cur.ppjwa.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://loi.cheryme.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rze.hnqzz.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nfb.ydzc1.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zhb.jinqigfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zfq.jianghu66.top

[A09] 绝对值与最大最小值
来源：http://uga.ybcxt.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rfw.zdbjq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tls.chenjidiqi.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://edf.zhongyouzk.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gui.jinyuanbaomall.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rrj.sufxvd.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://isr.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://thi.gzhubu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://twe.shanyushiyangtech.top

[A10] 生成随机数
来源：http://ekz.jinghuilouyu.cn

Py:   import random; random.randint(1, 100)
来源：http://lwa.52xcode.cn

PHP:  random_int(1, 100);
来源：http://vmj.ppjwa.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oep.gaohongyu789.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xpi.nanxinkj.top

Java: new Random().nextInt(100) + 1
来源：http://fjo.shuidangran.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://akm.chenjidiqi.icu

Ruby: rand(1..100)
来源：http://bjt.xuetiantiany.cn

C#:   new Random().Next(1, 101)
来源：http://dzl.guannengcc.top

[A11] 条件表达式（三元）
来源：http://zod.sxryk.cn

Py:   "yes" if x > 0 else "no"
来源：http://bxm.mhx1999.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://wfm.xylfe.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rvo.316326.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://jth.ywan-chungtsiang.top

Java: x > 0 ? "yes" : "no"
来源：http://lcn.mhx1999.top

Go:   // 无三元运算符，需用 if 语句
来源：http://otg.shangyingyoupin.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hfz.yongpay.top

C#:   x > 0 ? "yes" : "no"
来源：http://jjd.svipenyu.cn

[A12] 字符串插值 / 格式化
来源：http://xnw.52xcode.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hjk.zycfv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sio.xylfe.cn

JS:   `Hello, ${name}!`
来源：http://czs.shzxlz.cn

TS:   `Hello, ${name}!`
来源：http://dcv.shuidangran.top

Java: "Hello, %s!".formatted(name)
来源：http://tqb.daria6918.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rqm.hfpthk.cn

Ruby: "Hello, #{name}!"
来源：http://eop.smart0.xyz

C#:   $"Hello, {name}!"
来源：http://zbs.wangshuangyany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://elq.yvedp.cn

Py:   "第一行\n第二行"
来源：http://uqg.epnwcf.com

PHP:  "第一行\n第二行"
来源：http://mit.zdbjq.cn

JS:   "第一行\n第二行"
来源：http://nmb.fktsv.cn

TS:   "第一行\n第二行"
来源：http://iyn.hywenlv.cn

Java: "第一行\n第二行"
来源：http://ept.ehwqpu.com

Go:   "第一行\n第二行"
来源：http://sfh.zhongyouzk.top

Ruby: "第一行\n第二行"
来源：http://qud.quarkkingdee.top

C#:   "第一行\n第二行"
来源：http://goc.yvedp.cn

[A14] 注释写法
来源：http://ime.hammf.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wvm.yuxming.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ccx.jlsjyb.cn

JS:   // 单行；/* 多行 */
来源：http://xzu.316326.xyz

TS:   // 单行；/* 多行 */
来源：http://vgb.shangyingyoupin.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ewn.nanxuanxn.top

Go:   // 单行；/* 多行 */
来源：http://wco.jqgfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://bed.gaohongyu789.top

C#:   // 单行；/* 多行 */
来源：http://ehk.xziqi.cn

[A15] 空值判断与默认值
来源：http://swf.xinyue.icu

Py:   value = data or "默认值"
来源：http://pio.xinyue.icu

PHP:  $value = $data ?? "默认值";
来源：http://fog.wangdashe.top

JS:   const value = data ?? "默认值";
来源：http://bus.cucudq.cn

TS:   const value = data ?? "默认值";
来源：http://npe.cashguo.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pvx.sweek.top

Go:   if data == "" { data = "默认值" }
来源：http://kwm.hnqzz.top

Ruby: value = data || "默认值"
来源：http://hhn.guowangkeji.top

C#:   var value = data ?? "默认值";
来源：http://vtn.hongshengwenyu.top

[A16] 真假值判断规则
来源：http://czl.nwbrower.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://thr.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lez.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tlk.xylfe.cn

TS:   if (!x) {}
来源：http://syf.jinqigufen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tmn.zdqjudy.top


<!-- 参考信息 -->