代发 wailian999

[U87] JS：解构默认值
来源：http://kqx.xziqi.cn

const { a = 1, b = 2 } = obj;
来源：http://oxb.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://fin.xinyue.icu

{ ...a, ...b }
来源：http://otz.feifeiyinyue.top

[U89] JS：数组去重
来源：http://jfs.yj20258888.top

[...new Set(arr)]
来源：http://qjv.fzhhl.top

[U90] JS：数字数组排序
来源：http://mgb.tianlin.xyz

[...arr].sort((a, b) => a - b)
来源：http://mtz.yongpay.top

[U91] JS：对象键值遍历
来源：http://jro.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nlq.shzxlz.cn

[U92] JS：深拷贝
来源：http://czq.shanyushiyangkeji.top

structuredClone(obj)
来源：http://dex.jlsjyb.cn

[U93] JS：模板字符串
来源：http://fjm.feifeiyinyue.top

`共 ${n} 条`
来源：http://csj.sweek.top

[U94] JS：箭头函数
来源：http://ant.chenlongwang.top

const double = x => x * 2;
来源：http://rly.zdbjq.cn

[U95] JS：Promise 包装
来源：http://nmi.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://rju.nanxinkj.top

[U96] JS：async/await 与异常
来源：http://vtj.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ars.chenzaomai.com

[U97] JS：并发请求
来源：http://jus.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://usr.bbcook.cn

[U98] JS：fetch 带 JSON
来源：http://ihp.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jjx.sysykeji.top

[U99] JS：事件监听
来源：http://wjs.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://gmg.yuanzhike.top

[U100] JS：DOM 查询
来源：http://zsq.birdmap.top

document.querySelector(".item")
来源：http://cqy.gotoacloud.top

[U101] JS：classList 操作
来源：http://xzj.uphjek.com

el.classList.toggle("active")
来源：http://dbz.sufxvd.cn

[U102] JS：本地存储
来源：http://qyx.yvedp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://faw.chenlongwang.top

[U103] JS：定时器
来源：http://vto.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://reb.gotoacloud.top

[U104] JS：防抖
来源：http://wfs.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ige.guannengcc.top

[U105] JS：节流
来源：http://fxn.zhixingplan.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://orc.jinqigufen.top

[U106] JS：日期格式化
来源：http://ijt.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ibw.jlsjyb.cn

[U107] JS：数字千分位
来源：http://wys.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pqx.hesvh.cn

[U108] JS：随机整数
来源：http://zyn.hfpthk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tyh.hammf.cn

[U109] JS：数组分组
来源：http://dtl.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://zkf.wangdashe.top

[U110] JS：数组分块
来源：http://gmu.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qze.jqgfzy.top

[U111] JS：对象转 Map
来源：http://jvt.dashuyun.cn

new Map(Object.entries(obj))
来源：http://pgq.jinghuilouyu.cn

[U112] JS：字符串补位
来源：http://jmn.sufxvd.cn

"7".padStart(3, "0")
来源：http://syb.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://nkl.jinqigufen.top

s.replaceAll("a", "b")
来源：http://xos.daxiang520.top

[U114] JS：JSON 深比较
来源：http://xth.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://tdd.52xcode.cn

[U115] JS：生成 UUID
来源：http://fcr.xylfe.cn

crypto.randomUUID()
来源：http://qhb.uphjek.com

[U116] JS：类型检查（JSDoc）
来源：http://eti.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://tfk.daria6918.cn

[U117] JS：单元测试
来源：http://yij.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://tba.dianchejie.cn

[U118] JS：开发服务器
来源：http://nqr.hongshengwenyu.top

npm i -D vite;  npx vite
来源：http://bwu.cqqwz.cn

[U119] JS：生产构建
来源：http://irr.daxiang520.top

npx vite build
来源：http://ukz.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://gun.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://fpx.cheryme.top

================================================================================
来源：http://uwu.c1oappe.top

统计汇总
来源：http://pdb.andypj.xyz

================================================================================
来源：http://ffs.316326.xyz

按语言统计（条）：
来源：http://fta.nanxinkj.top

Python ......... 252
来源：http://lpb.hywenlv.cn

PHP ............ 252
来源：http://yjw.jyoumei.cn

JavaScript ..... 252
来源：http://urf.ehwqpu.com

TypeScript ..... 212
来源：http://oal.xinyue.icu

Java ........... 212
来源：http://ybl.yj20258888.top

Go ............. 212
来源：http://aes.cashguo.top

Ruby ........... 212
来源：http://sbs.quarkkingdee.top

C# ............. 212
来源：http://qqy.0kj1m.cn

C .............. 30
来源：http://daq.gzhubu.top

C++ ............ 30
来源：http://ghe.cashguo.top

SQL ............ 90
来源：http://dbh.wangshuangyany.cn

Bash ........... 80
来源：http://njb.quarkkingdee.top

Kotlin ......... 15
来源：http://ffq.hnxiangtu.top

Swift .......... 15
来源：http://cfw.cdnleiting.top

Lua ............ 10
来源：http://zag.gotoacloud.top

Perl ........... 10
来源：http://hrj.meibo888.top

Scala .......... 10
来源：http://kiw.ctjpmb.com

------------------------------------
来源：http://wxb.gaohongyu789.top

合计 ........... 2106 条
来源：http://jxs.xuetiantiany.cn

按章节统计：
来源：http://wle.redwolf501.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://enx.daxiang520.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://stl.hywenlv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://drd.zhongyouzk.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mfc.guannengcc.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rjq.tanke756.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ruh.shangyingyoupin.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vkc.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mzs.hcnkem.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://glc.xuanzx.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qio.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bhs.nanxinkj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xuf.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xmc.hammf.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jgg.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iyw.shangyingyoupin.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bel.dashuyun.cn

Q SQL 专题                              90
来源：http://waa.yuanzhike.top

R Bash 专题                             80
来源：http://cyj.yanxiufei.cn

S C / C++ 专题                          60
来源：http://jsg.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://iam.yvedp.cn

U 高频实用片段                         120
来源：http://fdw.yfazqb.com

------------------------------------
来源：http://ail.gzhubu.top

合计                                  2106 条
来源：http://bwh.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://psl.yfazqb.com

使用提醒
来源：http://ppj.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://dbx.andypj.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ptt.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lji.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://afr.yangfankeji.com

在旧版本上使用前请先确认语法支持情况。
来源：http://kcq.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hdm.sysykeji.top

—— 文件结束 ——
来源：http://wvr.jiagoushi.top

================================================================================
来源：http://vea.gogol.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://ino.feifeiyinyue.top

Common Programming Examples Cheat Book
来源：http://lur.zdbjq.cn

================================================================================
来源：http://cpl.shzxlz.cn

【收录内容】
来源：http://omm.ctjpmb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://cdv.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hhz.52xcode.cn

SQL · Bash · C · C++
来源：http://blx.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cic.ywan-chungtsiang.top

【使用说明】
来源：http://obh.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iyn.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xph.birdmap.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ipl.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ujb.yonumen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wdz.hcnkem.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wzm.yongpay.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tep.fengsongda.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://syt.316326.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nat.xuanzx.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bvc.zdqjudy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pba.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ihs.sxryk.cn

【文件统计】
来源：http://qjk.zhongyouzk.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zjt.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://stx.chenjidiqi.icu

目  录
来源：http://lsa.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://upm.yj202588.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oix.jqgufenzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://biu.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aua.jianghu66.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qah.ydzc1.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://esi.cucudq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xtg.zhaomingkeji.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cmt.shanyushiyangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://efq.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xne.jinqigfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kvh.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hbd.zhaomingkeji.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cti.zhiwuduotai.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://flj.hysaishi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cgk.mhx1999.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uoo.jinqigfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qkl.ybcxt.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fqe.jlsjyb.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://odb.xuetiantiany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qaw.andypj.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ova.jinghuilouyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pen.svipenyu.cn

================================================================================
来源：http://bnk.chenlongwang.top

A. 基础语法与类型
来源：http://mmd.jianghu66.top

================================================================================
来源：http://ueq.zycfv.cn

[A01] Hello World
来源：http://ykl.0kj1m.cn

Py:   print("Hello, World!")
来源：http://oxn.chenzaomai.com

PHP:  echo "Hello, World!";
来源：http://dyt.pengpengdd.cyou

JS:   console.log("Hello, World!");
来源：http://vun.jinghuilouyu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://frq.gaohongyu789.top

Java: System.out.println("Hello, World!");
来源：http://ybf.jianghu66.top

Go:   fmt.Println("Hello, World!")
来源：http://bxa.sufxvd.cn

Ruby: puts "Hello, World!"
来源：http://jdz.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ivv.ctjpmb.com

[A02] 变量声明与赋值
来源：http://vql.tianlin.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hhm.yuxming.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uci.zhaomingkeji.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://aut.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ust.shangyingyoupin.top

Java: String name = "Alex"; int age = 20;
来源：http://hab.meibo888.top

Go:   name := "Alex"; age := 20
来源：http://dns.hnqzz.top

Ruby: name = "Alex"; age = 20
来源：http://ptf.jqgufenzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://apf.vehdjk.com

[A03] 常量定义
来源：http://yye.sysykeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hgc.epnwcf.com

PHP:  const PI = 3.14159;
来源：http://nor.tanke756.top

JS:   const PI = 3.14159;
来源：http://jak.uphjek.com

TS:   const PI: number = 3.14159;
来源：http://yay.zhoulong.xyz

Java: static final double PI = 3.14159;
来源：http://mio.9152youxi.cn

Go:   const PI = 3.14159
来源：http://vxq.yongpay.top

Ruby: PI = 3.14159
来源：http://wma.jyoumei.cn

C#:   const double PI = 3.14159;
来源：http://kdj.xylfe.cn

[A04] 判断变量类型
来源：http://tci.zhixingplan.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://erq.vqdsnc.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wua.c1oappe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qzb.fengsongda.top

TS:   typeof x; x instanceof Date
来源：http://uai.feifeiyinyue.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wsl.yanxiufei.cn

Go:   reflect.TypeOf(x).Name()
来源：http://adc.ydzc1.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hln.redwolf501.top

C#:   x.GetType().Name; x is int
来源：http://tph.xylfe.cn

[A05] 整数除法与取模
来源：http://ghy.daria6918.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sfa.andypj.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://yku.shanyushiyangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xla.gogol.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dan.meibo888.top

Java: 7 / 2; 7 % 2
来源：http://cfu.jqgufenzy.top

Go:   7 / 2; 7 % 2
来源：http://whn.pengpengdd.cyou

Ruby: 7 / 2; 7 % 2
来源：http://ymi.epnwcf.com

C#:   7 / 2; 7 % 2
来源：http://awo.jyoumei.cn

[A06] 字符串转数字
来源：http://ryb.52xcode.cn

Py:   int("42"); float("3.14")
来源：http://tvf.chenzaomai.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ojr.ydzc1.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://imd.zycfv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vju.jlsjyb.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dca.daria6918.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rzf.xinyue.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://aio.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cqp.yanxiufei.cn

[A07] 数字转字符串
来源：http://kgi.jyoumei.cn

Py:   str(42)
来源：http://wrz.hcnkem.com

PHP:  (string) 42; strval(42)
来源：http://yqi.xinyue.icu

JS:   String(42); (42).toString()
来源：http://udn.hongshengwenyu.top

TS:   String(42)
来源：http://qqp.hesvh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://acy.wangshuangyany.cn

Go:   strconv.Itoa(42)
来源：http://owv.tarul.cn

Ruby: 42.to_s
来源：http://zpg.gotoacloud.top

C#:   42.ToString()
来源：http://jlc.wangshuangyany.cn

[A08] 取整与四舍五入
来源：http://amz.uphjek.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://epv.jinqigufen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lhj.shangyingyoupin.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gzb.316326.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ipr.yfazqb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rys.tianlin.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://khx.zhongyouzk.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bhm.fktsv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://unt.uphjek.com

[A09] 绝对值与最大最小值
来源：http://cyi.cheryme.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bjg.ehwqpu.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://awr.dashuyun.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dzz.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://atc.chenjidiqi.icu

Java: Math.abs(-5); Math.max(1, 2)
来源：http://muh.dianchejie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://coi.shzxlz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://alb.dianchejie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tdi.gzhubu.top

[A10] 生成随机数
来源：http://hnw.iojbl.cn

Py:   import random; random.randint(1, 100)
来源：http://ljc.xuanzx.com

PHP:  random_int(1, 100);
来源：http://mrz.ctjpmb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nkf.zhoulong.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ehk.9152youxi.cn

Java: new Random().nextInt(100) + 1
来源：http://aov.havefunace.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dag.jyoumei.cn

Ruby: rand(1..100)
来源：http://avs.jlsjyb.cn

C#:   new Random().Next(1, 101)
来源：http://hcw.fzhhl.top

[A11] 条件表达式（三元）
来源：http://ilo.wangdashe.top

Py:   "yes" if x > 0 else "no"
来源：http://flv.tianlin.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://hfq.tarul.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cbm.ydzc1.top

TS:   x > 0 ? "yes" : "no"
来源：http://mnd.bjfxy.top

Java: x > 0 ? "yes" : "no"
来源：http://ljf.jianghu66.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mbu.jyoumei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fey.jiagoushi.top

C#:   x > 0 ? "yes" : "no"
来源：http://kgf.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://als.feifeiyinyue.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wzd.xylfe.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ftf.ywan-chungtsiang.top

JS:   `Hello, ${name}!`
来源：http://adl.tianlin.xyz

TS:   `Hello, ${name}!`
来源：http://hxr.quarkkingdee.top

Java: "Hello, %s!".formatted(name)
来源：http://pfi.iojbl.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hpc.hnqzz.top

Ruby: "Hello, #{name}!"
来源：http://hwi.yj202588.top

C#:   $"Hello, {name}!"
来源：http://wzi.uphjek.com

[A13] 多行字符串（练习 \n 转义）
来源：http://stk.aibaodan.cn

Py:   "第一行\n第二行"
来源：http://suv.zhengqikj.top

PHP:  "第一行\n第二行"
来源：http://lzi.hnxiangtu.top

JS:   "第一行\n第二行"
来源：http://trc.ppjwa.cn

TS:   "第一行\n第二行"
来源：http://ifu.sweek.top

Java: "第一行\n第二行"
来源：http://tlt.shangyingyoupin.top

Go:   "第一行\n第二行"
来源：http://pph.smart0.xyz

Ruby: "第一行\n第二行"
来源：http://wwa.gotoacloud.top

C#:   "第一行\n第二行"
来源：http://siy.fktsv.cn

[A14] 注释写法
来源：http://aww.pycfn.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://wmr.aibaodan.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kqu.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://ncf.ctjpmb.com

TS:   // 单行；/* 多行 */
来源：http://wzn.nanxinkj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://huq.cashguo.top

Go:   // 单行；/* 多行 */
来源：http://mcu.hcnkem.com

Ruby: # 单行；=begin 多行 =end
来源：http://hnn.nwbrower.top


<!-- 参考信息 -->