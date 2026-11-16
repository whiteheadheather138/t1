代发 wailian999

[U91] JS：对象键值遍历
来源：http://hqg.ctjpmb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jlw.uphjek.com

[U92] JS：深拷贝
来源：http://bfd.zhoulong.xyz

structuredClone(obj)
来源：http://uxk.hywenlv.cn

[U93] JS：模板字符串
来源：http://ehl.feifeiyinyue.top

`共 ${n} 条`
来源：http://bei.0kj1m.cn

[U94] JS：箭头函数
来源：http://tci.sxryk.cn

const double = x => x * 2;
来源：http://djv.yueranfly.top

[U95] JS：Promise 包装
来源：http://ept.ehwqpu.com

new Promise((resolve, reject) => {})
来源：http://vyq.guannengcc.top

[U96] JS：async/await 与异常
来源：http://duz.zhengqikj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://msn.havefunace.top

[U97] JS：并发请求
来源：http://xba.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://gpu.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://rcz.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oww.bbcook.cn

[U99] JS：事件监听
来源：http://wfe.jianghu66.top

el.addEventListener("click", e => {})
来源：http://wsi.ivvv.top

[U100] JS：DOM 查询
来源：http://hwe.zhongyouzk.top

document.querySelector(".item")
来源：http://mge.zhixingplan.top

[U101] JS：classList 操作
来源：http://gwv.svipenyu.cn

el.classList.toggle("active")
来源：http://tzi.svipenyu.cn

[U102] JS：本地存储
来源：http://hoj.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wms.redwolf501.top

[U103] JS：定时器
来源：http://quv.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hgv.xuetiantiany.cn

[U104] JS：防抖
来源：http://igf.ybcxt.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ghj.jqgfzy.top

[U105] JS：节流
来源：http://wkp.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bvt.quarkkingdee.top

[U106] JS：日期格式化
来源：http://bsp.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://njc.cdnleiting.top

[U107] JS：数字千分位
来源：http://kvj.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rlp.xziqi.cn

[U108] JS：随机整数
来源：http://egq.svipenyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lee.cucudq.cn

[U109] JS：数组分组
来源：http://tej.yuanzhike.top

Object.groupBy(arr, x => x.type)
来源：http://abm.jqgufenzy.top

[U110] JS：数组分块
来源：http://qtm.shuidangran.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qmc.tarul.cn

[U111] JS：对象转 Map
来源：http://hfv.pycfn.com

new Map(Object.entries(obj))
来源：http://hte.vqdsnc.cn

[U112] JS：字符串补位
来源：http://eib.hfpthk.cn

"7".padStart(3, "0")
来源：http://xha.nwbrower.top

[U113] JS：正则替换全部
来源：http://rjc.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://oxx.ivvv.top

[U114] JS：JSON 深比较
来源：http://dsd.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yeu.guowangkeji.top

[U115] JS：生成 UUID
来源：http://kgg.hysaishi.cn

crypto.randomUUID()
来源：http://roe.nanxinkj.top

[U116] JS：类型检查（JSDoc）
来源：http://thd.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://pkm.zhijiandao.cn

[U117] JS：单元测试
来源：http://yho.zdqjudy.top

npm i -D vitest;  npx vitest
来源：http://kij.gzhubu.top

[U118] JS：开发服务器
来源：http://tkw.xuanzx.com

npm i -D vite;  npx vite
来源：http://ron.sysykeji.top

[U119] JS：生产构建
来源：http://ddt.chenzaomai.com

npx vite build
来源：http://cfx.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://rrh.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://hfw.kuanghao11.cn

================================================================================
来源：http://mgk.hcnkem.com

统计汇总
来源：http://hjm.zhijiandao.cn

================================================================================
来源：http://tow.gotoacloud.top

按语言统计（条）：
来源：http://kxp.dianchejie.cn

Python ......... 252
来源：http://qcx.hammf.cn

PHP ............ 252
来源：http://gxx.52xcode.cn

JavaScript ..... 252
来源：http://njt.uphjek.com

TypeScript ..... 212
来源：http://tvn.jinqigufen.top

Java ........... 212
来源：http://wdc.shuidangran.top

Go ............. 212
来源：http://zwl.yj20258888.top

Ruby ........... 212
来源：http://zsq.yj202588.top

C# ............. 212
来源：http://hjz.wangdashe.top

C .............. 30
来源：http://gmx.ppjwa.cn

C++ ............ 30
来源：http://prn.tanke756.top

SQL ............ 90
来源：http://ubc.bbcook.cn

Bash ........... 80
来源：http://mcv.gotoacloud.top

Kotlin ......... 15
来源：http://qoz.hywenlv.cn

Swift .......... 15
来源：http://tru.xingfuxueyuan.xyz

Lua ............ 10
来源：http://aig.daxiang520.top

Perl ........... 10
来源：http://fbr.ehwqpu.com

Scala .......... 10
来源：http://vub.zdqjudy.top

------------------------------------
来源：http://xwl.chenzaomai.com

合计 ........... 2106 条
来源：http://oqq.fehbvm.com

按章节统计：
来源：http://jez.vehdjk.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eoh.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qrj.hfpthk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qcq.pycfn.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mrm.yueranfly.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fws.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vel.kuanghao11.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hxd.shanyushiyangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bpx.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kox.redwolf501.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kax.jianghu66.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yuw.jyoumei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://apm.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://heu.smart0.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ohw.cucudq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iwk.birdmap.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://umj.ydzc1.top

Q SQL 专题                              90
来源：http://nmk.tanke756.top

R Bash 专题                             80
来源：http://kcb.chenjidiqi.icu

S C / C++ 专题                          60
来源：http://mij.yuxming.cn

T 其他语言补充                          60
来源：http://zhr.fktsv.cn

U 高频实用片段                         120
来源：http://pej.hysaishi.cn

------------------------------------
来源：http://rsf.xinyue.icu

合计                                  2106 条
来源：http://puq.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://pyc.yj20258.top

使用提醒
来源：http://uld.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://hns.yueranfly.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hun.ywan-chungtsiang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qjf.birdmap.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oyu.cheryme.top

在旧版本上使用前请先确认语法支持情况。
来源：http://crv.9152youxi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bkz.haohaochexian.top

—— 文件结束 ——
来源：http://deh.yj20258888.top

================================================================================
来源：http://ilk.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://ccq.yonumen.top

Common Programming Examples Cheat Book
来源：http://ajb.cashguo.top

================================================================================
来源：http://vpv.jinqigufen.top

【收录内容】
来源：http://tjz.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://tep.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://glx.cucudq.cn

SQL · Bash · C · C++
来源：http://neh.haohaochexian.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yge.smart0.xyz

【使用说明】
来源：http://qai.redwolf501.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ikm.zhijiandao.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cig.yj20258888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ove.xuetiantiany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tcf.shangyingyoupin.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dbh.jinyuanbaomall.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ezz.dianchejie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://twp.xuanzx.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xjx.jinqigufen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jvb.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ujm.haohaochexian.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qga.tarul.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kmt.haohaochexian.top

【文件统计】
来源：http://yyz.redwolf501.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mfx.zycfv.cn

--------------------------------------------------------------------------------
来源：http://fup.nanxinkj.top

目  录
来源：http://bbf.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://tbz.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gbs.uphjek.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nqk.zdqjudy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://utn.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://aax.xuanzx.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://klu.xinyue.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bkk.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fnm.fzhhl.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tfp.tian-w.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hho.jlsjyb.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ecu.fehbvm.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ust.sjlbkw.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://svx.wangshuangyany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ewp.jinghuilouyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pcw.dianchejie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uzm.cdnleiting.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fgf.guannengcc.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ulc.daxiang520.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fow.zhixingplan.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tce.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sir.zhiwuduotai.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eox.feifeiyinyue.top

================================================================================
来源：http://yck.daxiang520.top

A. 基础语法与类型
来源：http://zjc.shuidangran.top

================================================================================
来源：http://flb.aibaodan.cn

[A01] Hello World
来源：http://xdf.cdnleiting.top

Py:   print("Hello, World!")
来源：http://qop.yuxming.cn

PHP:  echo "Hello, World!";
来源：http://frp.iojbl.cn

JS:   console.log("Hello, World!");
来源：http://quy.tanke756.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kpg.wangshuangyany.cn

Java: System.out.println("Hello, World!");
来源：http://lja.yonumen.top

Go:   fmt.Println("Hello, World!")
来源：http://yyc.yvedp.cn

Ruby: puts "Hello, World!"
来源：http://ljh.tianlin.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://djz.aibaodan.cn

[A02] 变量声明与赋值
来源：http://yvc.yanxiufei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xsb.hesvh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fhf.hnxiangtu.top

JS:   let name = "Alex"; const age = 20;
来源：http://roc.snrcjt.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ock.fzhhl.top

Java: String name = "Alex"; int age = 20;
来源：http://blj.sxryk.cn

Go:   name := "Alex"; age := 20
来源：http://paq.quarkkingdee.top

Ruby: name = "Alex"; age = 20
来源：http://vqd.9152youxi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ldz.gotoacloud.top

[A03] 常量定义
来源：http://jww.jinqigfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hzu.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://cfb.fzhhl.top

JS:   const PI = 3.14159;
来源：http://beg.yonumen.top

TS:   const PI: number = 3.14159;
来源：http://gkp.c1oappe.top

Java: static final double PI = 3.14159;
来源：http://zxl.pengpengdd.cyou

Go:   const PI = 3.14159
来源：http://vze.sysykeji.top

Ruby: PI = 3.14159
来源：http://koc.jqgufenzy.top

C#:   const double PI = 3.14159;
来源：http://evl.sysykeji.top

[A04] 判断变量类型
来源：http://wmw.cashguo.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qsd.sweek.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pgk.uphjek.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mhq.cqqwz.cn

TS:   typeof x; x instanceof Date
来源：http://ckj.chenzaomai.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tfc.gzhubu.top

Go:   reflect.TypeOf(x).Name()
来源：http://pgu.jqgfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fyk.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://kfd.mhx1999.top

[A05] 整数除法与取模
来源：http://wwo.aibaodan.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ykk.hysaishi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ech.yongpay.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jot.vehdjk.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jkl.dashuyun.cn

Java: 7 / 2; 7 % 2
来源：http://nsz.fzhhl.top

Go:   7 / 2; 7 % 2
来源：http://wno.jinghuilouyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://ceo.yj20258.top

C#:   7 / 2; 7 % 2
来源：http://ukl.birdmap.top

[A06] 字符串转数字
来源：http://sxa.xylfe.cn

Py:   int("42"); float("3.14")
来源：http://kll.zhoulong.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nfa.shangyingyoupin.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fbe.tarul.cn

TS:   parseInt("42", 10); Number("42")
来源：http://waq.jqgfzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lsl.fengsongda.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hcq.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://vxc.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://udh.yonumen.top

[A07] 数字转字符串
来源：http://nii.bbcook.cn

Py:   str(42)
来源：http://zid.aibaodan.cn

PHP:  (string) 42; strval(42)
来源：http://clx.nanxuanxn.top

JS:   String(42); (42).toString()
来源：http://oan.pengpengdd.cyou

TS:   String(42)
来源：http://eqe.bjfxy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://byd.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://yvm.wangshuangyany.cn

Ruby: 42.to_s
来源：http://jaz.ppjwa.cn

C#:   42.ToString()
来源：http://ggh.hnxiangtu.top

[A08] 取整与四舍五入
来源：http://pbo.ivvv.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qqk.jinghuilouyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ryn.kuanghao11.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mdz.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://awm.shzxlz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cgn.xziqi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iek.aibaodan.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nut.hysaishi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://raw.sufxvd.cn

[A09] 绝对值与最大最小值
来源：http://nzq.shzxlz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uwm.guowangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ujt.tian-w.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rqa.yuxming.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://klq.vqdsnc.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ljo.ydzc1.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hmv.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cdj.zdqjudy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eky.meibo888.top

[A10] 生成随机数
来源：http://ivs.zhongyouzk.top

Py:   import random; random.randint(1, 100)
来源：http://xtx.ywan-chungtsiang.top

PHP:  random_int(1, 100);
来源：http://xwr.gzhubu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://owj.zhengqikj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://act.ppjwa.cn

Java: new Random().nextInt(100) + 1
来源：http://ier.dianchejie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://scu.ctjpmb.com

Ruby: rand(1..100)
来源：http://yhu.shuidangran.top

C#:   new Random().Next(1, 101)
来源：http://jrq.xingfuxueyuan.xyz

[A11] 条件表达式（三元）
来源：http://oso.gaohongyu789.top

Py:   "yes" if x > 0 else "no"
来源：http://jih.hcnkem.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://lmr.sweek.top

JS:   x > 0 ? "yes" : "no"
来源：http://hhu.vehdjk.com

TS:   x > 0 ? "yes" : "no"
来源：http://vbj.jinyuanbaomall.cn

Java: x > 0 ? "yes" : "no"
来源：http://btj.hnqzz.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sxx.havefunace.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qzq.jyoumei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uvc.yuanzhike.top

[A12] 字符串插值 / 格式化
来源：http://awl.jinghuilouyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ieb.ydjk.org.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ppr.ydzc1.top

JS:   `Hello, ${name}!`
来源：http://vez.yj20258.top

TS:   `Hello, ${name}!`
来源：http://rey.xuetiantiany.cn

Java: "Hello, %s!".formatted(name)
来源：http://gpo.zhoulong.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nrp.quarkkingdee.top

Ruby: "Hello, #{name}!"
来源：http://xol.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://dag.bbcook.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://duy.cashguo.top

Py:   "第一行\n第二行"
来源：http://yqd.tarul.cn

PHP:  "第一行\n第二行"
来源：http://dkf.bjfxy.top

JS:   "第一行\n第二行"
来源：http://aab.fanxiaobao.xyz

TS:   "第一行\n第二行"
来源：http://ewk.yanxiufei.cn

Java: "第一行\n第二行"
来源：http://ceh.vehdjk.com

Go:   "第一行\n第二行"
来源：http://cao.xuanzx.com

Ruby: "第一行\n第二行"
来源：http://ldr.ydzc1.top

C#:   "第一行\n第二行"
来源：http://psf.fehbvm.com

[A14] 注释写法
来源：http://gun.hesvh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://iwt.yj20258888.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xdv.yonumen.top

JS:   // 单行；/* 多行 */
来源：http://xhm.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://ywo.aibaodan.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oqj.zdbjq.cn

Go:   // 单行；/* 多行 */
来源：http://pzl.sysykeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://wme.fktsv.cn

C#:   // 单行；/* 多行 */
来源：http://vro.snrcjt.cn

[A15] 空值判断与默认值
来源：http://kxl.hcnkem.com

Py:   value = data or "默认值"
来源：http://tnc.fzhhl.top

PHP:  $value = $data ?? "默认值";
来源：http://vfv.birdmap.top

JS:   const value = data ?? "默认值";
来源：http://ufa.ctjpmb.com

TS:   const value = data ?? "默认值";
来源：http://ipm.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mrk.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://kia.zdqjudy.top


<!-- 参考信息 -->