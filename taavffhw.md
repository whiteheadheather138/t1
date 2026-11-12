代发 wailian999

[U87] JS：解构默认值
来源：http://plb.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://vxq.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://ymt.jqgufenzy.top

{ ...a, ...b }
来源：http://qmn.redwolf501.top

[U89] JS：数组去重
来源：http://ksc.xylfe.cn

[...new Set(arr)]
来源：http://cjj.guannengcc.top

[U90] JS：数字数组排序
来源：http://bzf.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://wyc.gzhubu.top

[U91] JS：对象键值遍历
来源：http://sqv.316326.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fvh.mhx1999.top

[U92] JS：深拷贝
来源：http://frm.guowangkeji.top

structuredClone(obj)
来源：http://eqk.svipenyu.cn

[U93] JS：模板字符串
来源：http://buk.tanke756.top

`共 ${n} 条`
来源：http://zrj.hnqzz.top

[U94] JS：箭头函数
来源：http://kuj.smart0.xyz

const double = x => x * 2;
来源：http://rbj.fktsv.cn

[U95] JS：Promise 包装
来源：http://eqz.zhaomingkeji.xyz

new Promise((resolve, reject) => {})
来源：http://ydf.andypj.xyz

[U96] JS：async/await 与异常
来源：http://awr.mhx1999.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pjy.gaohongyu789.top

[U97] JS：并发请求
来源：http://wta.dashuyun.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.nwbrower.top

[U98] JS：fetch 带 JSON
来源：http://fio.birdmap.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tut.cqqwz.cn

[U99] JS：事件监听
来源：http://use.yfazqb.com

el.addEventListener("click", e => {})
来源：http://uqw.hysaishi.cn

[U100] JS：DOM 查询
来源：http://mie.jinqigufen.top

document.querySelector(".item")
来源：http://eqa.fengsongda.top

[U101] JS：classList 操作
来源：http://tvf.nanxuanxn.top

el.classList.toggle("active")
来源：http://xcv.tian-w.cn

[U102] JS：本地存储
来源：http://ndj.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wcp.gotoacloud.top

[U103] JS：定时器
来源：http://hks.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://drz.hnqzz.top

[U104] JS：防抖
来源：http://obd.jinqigfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://daa.epnwcf.com

[U105] JS：节流
来源：http://ses.yfazqb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ctu.yj202588.top

[U106] JS：日期格式化
来源：http://jlc.fehbvm.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://esm.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://pps.jqgufenzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lug.vqdsnc.cn

[U108] JS：随机整数
来源：http://gyd.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jxa.aizwys.cn

[U109] JS：数组分组
来源：http://qjy.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://quj.hywenlv.cn

[U110] JS：数组分块
来源：http://fka.daxiang520.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ijd.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://goa.tian-w.cn

new Map(Object.entries(obj))
来源：http://ril.hysaishi.cn

[U112] JS：字符串补位
来源：http://lod.pycfn.com

"7".padStart(3, "0")
来源：http://lax.cucudq.cn

[U113] JS：正则替换全部
来源：http://lsu.zdqjudy.top

s.replaceAll("a", "b")
来源：http://hfp.sweek.top

[U114] JS：JSON 深比较
来源：http://kqz.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://sqb.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://ljm.gzhubu.top

crypto.randomUUID()
来源：http://drr.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://xlh.hywenlv.cn

/** @param {string} name */ function f(name) {}
来源：http://yqx.shzxlz.cn

[U117] JS：单元测试
来源：http://eja.jiagoushi.top

npm i -D vitest;  npx vitest
来源：http://xjm.yuanzhike.top

[U118] JS：开发服务器
来源：http://gej.pycfn.com

npm i -D vite;  npx vite
来源：http://fbe.gzhubu.top

[U119] JS：生产构建
来源：http://kyj.aizwys.cn

npx vite build
来源：http://nrp.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://lmo.9152youxi.cn

import.meta.env.VITE_API_URL
来源：http://iij.yuxming.cn

================================================================================
来源：http://wdr.meibo888.top

统计汇总
来源：http://wli.jinqigfzy.top

================================================================================
来源：http://zmt.hammf.cn

按语言统计（条）：
来源：http://bxm.yuanzhike.top

Python ......... 252
来源：http://oay.pengpengdd.cyou

PHP ............ 252
来源：http://osk.fehbvm.com

JavaScript ..... 252
来源：http://jdu.fehbvm.com

TypeScript ..... 212
来源：http://mds.gotoacloud.top

Java ........... 212
来源：http://rhr.fanxiaobao.xyz

Go ............. 212
来源：http://zji.daria6918.cn

Ruby ........... 212
来源：http://bgh.sufxvd.cn

C# ............. 212
来源：http://agi.ydjk.org.cn

C .............. 30
来源：http://aen.yongpay.top

C++ ............ 30
来源：http://rua.gzhubu.top

SQL ............ 90
来源：http://shd.ehwqpu.com

Bash ........... 80
来源：http://utk.jinghuilouyu.cn

Kotlin ......... 15
来源：http://fuj.yj20258.top

Swift .......... 15
来源：http://nyo.gzhubu.top

Lua ............ 10
来源：http://bvq.zhoulong.xyz

Perl ........... 10
来源：http://cdo.316326.xyz

Scala .......... 10
来源：http://ssi.fktsv.cn

------------------------------------
来源：http://maa.bjfxy.top

合计 ........... 2106 条
来源：http://itd.ivvv.top

按章节统计：
来源：http://jom.zhixingplan.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://izr.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cpv.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tzc.havefunace.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://edn.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://twh.cheryme.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ore.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dal.epnwcf.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pbw.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kkp.xingfuxueyuan.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ouw.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://non.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yuw.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xpv.kuanghao11.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zzb.cdnleiting.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rna.0kj1m.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lek.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://rnv.yongpay.top

R Bash 专题                             80
来源：http://tjh.9152youxi.cn

S C / C++ 专题                          60
来源：http://lev.haohaochexian.top

T 其他语言补充                          60
来源：http://sld.haohaochexian.top

U 高频实用片段                         120
来源：http://iye.nanxinkj.top

------------------------------------
来源：http://scw.gotoacloud.top

合计                                  2106 条
来源：http://aus.epnwcf.com

--------------------------------------------------------------------------------
来源：http://nik.nanxuanxn.top

使用提醒
来源：http://vax.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://ont.jqgfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pce.xinyue.icu

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sxa.jlsjyb.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dxf.nwbrower.top

在旧版本上使用前请先确认语法支持情况。
来源：http://juy.guannengcc.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bim.redwolf501.top

—— 文件结束 ——
来源：http://fdt.redwolf501.top

================================================================================
来源：http://qpg.ivvv.top

程序语言常见例子速查手册（2024 版）
来源：http://wxb.jinqigfzy.top

Common Programming Examples Cheat Book
来源：http://osx.jiagoushi.top

================================================================================
来源：http://zfv.jinqigfzy.top

【收录内容】
来源：http://xfc.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pee.yj20258888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jud.c1oappe.top

SQL · Bash · C · C++
来源：http://uui.jinqigfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kar.zhaomingkeji.xyz

【使用说明】
来源：http://shh.gaohongyu789.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eaf.sufxvd.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sro.chenzaomai.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rpw.smart0.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tvc.zhixingplan.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nyo.ydzc1.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cme.snrcjt.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kfv.chenzaomai.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vpg.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://owg.sjlbkw.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qxq.mhx1999.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zed.hcnkem.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kua.tianlin.xyz

【文件统计】
来源：http://zkz.tarul.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ijw.ivvv.top

--------------------------------------------------------------------------------
来源：http://jxv.jqgfzy.top

目  录
来源：http://sgx.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://mvc.cheryme.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jzo.xylfe.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cvh.cdnleiting.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dzb.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://joe.xinyue.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lks.daxiang520.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sra.daria6918.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qng.dianchejie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mrr.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dur.jyoumei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zku.smart0.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://typ.yj20258888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mox.pengpengdd.cyou

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cub.fehbvm.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ccn.zhengqikj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nhp.haohaochexian.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://luq.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://snu.jlsjyb.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dpv.ywan-chungtsiang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qzm.feifeiyinyue.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tjf.cdnleiting.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://guv.zhixingplan.top

================================================================================
来源：http://opp.fzhhl.top

A. 基础语法与类型
来源：http://psx.jqgfzy.top

================================================================================
来源：http://gul.hongshengwenyu.top

[A01] Hello World
来源：http://lrg.mhx1999.top

Py:   print("Hello, World!")
来源：http://cce.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://tgw.yvedp.cn

JS:   console.log("Hello, World!");
来源：http://bgh.yonumen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fyh.chenjidiqi.icu

Java: System.out.println("Hello, World!");
来源：http://afe.ctjpmb.com

Go:   fmt.Println("Hello, World!")
来源：http://wad.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://sch.sjlbkw.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kxj.ydzc1.top

[A02] 变量声明与赋值
来源：http://lse.tarul.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wxa.yangfankeji.com

PHP:  $name = "Alex"; $age = 20;
来源：http://uud.ivvv.top

JS:   let name = "Alex"; const age = 20;
来源：http://tvw.cheryme.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ujf.nanxinkj.top

Java: String name = "Alex"; int age = 20;
来源：http://ieq.tianlin.xyz

Go:   name := "Alex"; age := 20
来源：http://xiy.xylfe.cn

Ruby: name = "Alex"; age = 20
来源：http://pjh.xylfe.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sei.zhijiandao.cn

[A03] 常量定义
来源：http://gxn.andypj.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zdi.cashguo.top

PHP:  const PI = 3.14159;
来源：http://pux.meibo888.top

JS:   const PI = 3.14159;
来源：http://czx.wangshuangyany.cn

TS:   const PI: number = 3.14159;
来源：http://lbm.aibaodan.cn

Java: static final double PI = 3.14159;
来源：http://att.chenjidiqi.icu

Go:   const PI = 3.14159
来源：http://civ.yj202588.top

Ruby: PI = 3.14159
来源：http://yra.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://dow.jinqigufen.top

[A04] 判断变量类型
来源：http://saz.jiagoushi.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dcq.daxiang520.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ipm.xingfuxueyuan.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ixl.fzhhl.top

TS:   typeof x; x instanceof Date
来源：http://kxj.gotoacloud.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rpq.yj20258888.top

Go:   reflect.TypeOf(x).Name()
来源：http://wwu.fengsongda.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ipn.shanyushiyangtech.top

C#:   x.GetType().Name; x is int
来源：http://ivx.iojbl.cn

[A05] 整数除法与取模
来源：http://qdg.ctjpmb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hwp.quarkkingdee.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://nxt.epnwcf.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jkl.fzhhl.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xvt.yonumen.top

Java: 7 / 2; 7 % 2
来源：http://twd.yuxming.cn

Go:   7 / 2; 7 % 2
来源：http://rhs.jinghuilouyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://dpc.jlsjyb.cn

C#:   7 / 2; 7 % 2
来源：http://usz.zhoulong.xyz

[A06] 字符串转数字
来源：http://vtt.havefunace.top

Py:   int("42"); float("3.14")
来源：http://twa.yonumen.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://agr.ybcxt.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://woi.zhijiandao.cn

TS:   parseInt("42", 10); Number("42")
来源：http://emp.hesvh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mpx.redwolf501.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vds.hammf.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ypr.xylfe.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qrl.feifeiyinyue.top

[A07] 数字转字符串
来源：http://cab.wangshuangyany.cn

Py:   str(42)
来源：http://tkz.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://ndo.vehdjk.com

JS:   String(42); (42).toString()
来源：http://zpf.jyoumei.cn

TS:   String(42)
来源：http://kqp.sweek.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hhs.jinqigufen.top

Go:   strconv.Itoa(42)
来源：http://ppq.ywan-chungtsiang.top

Ruby: 42.to_s
来源：http://run.yvedp.cn

C#:   42.ToString()
来源：http://frv.gogol.net.cn

[A08] 取整与四舍五入
来源：http://lmu.yj20258.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fwx.yueranfly.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dwp.chenzaomai.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qvp.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ajj.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pka.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://scf.ppjwa.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nta.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zrw.52xcode.cn

[A09] 绝对值与最大最小值
来源：http://qri.bbcook.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ntu.sufxvd.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://frk.gaohongyu789.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fwm.bjfxy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wph.pengpengdd.cyou

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kqv.gaohongyu789.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ysh.yfazqb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zig.xingfuxueyuan.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oor.shanyushiyangkeji.top

[A10] 生成随机数
来源：http://pwf.sxryk.cn

Py:   import random; random.randint(1, 100)
来源：http://zrr.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://bev.jinyuanbaomall.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ijo.hysaishi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tgc.hesvh.cn

Java: new Random().nextInt(100) + 1
来源：http://zai.cqqwz.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dks.xuetiantiany.cn

Ruby: rand(1..100)
来源：http://ghd.aizwys.cn

C#:   new Random().Next(1, 101)
来源：http://hnb.yvedp.cn

[A11] 条件表达式（三元）
来源：http://lue.hcnkem.com

Py:   "yes" if x > 0 else "no"
来源：http://xqf.cdnleiting.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qxx.bbcook.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xgz.sweek.top

TS:   x > 0 ? "yes" : "no"
来源：http://fba.fktsv.cn

Java: x > 0 ? "yes" : "no"
来源：http://mvo.zhaomingkeji.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://mrl.gaohongyu789.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pnq.chenlongwang.top

C#:   x > 0 ? "yes" : "no"
来源：http://djm.guannengcc.top

[A12] 字符串插值 / 格式化
来源：http://pwx.cheryme.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rdw.wangdashe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yxs.smart0.xyz

JS:   `Hello, ${name}!`
来源：http://qxz.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://pqy.tarul.cn

Java: "Hello, %s!".formatted(name)
来源：http://rds.nanxuanxn.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qwd.zdqjudy.top

Ruby: "Hello, #{name}!"
来源：http://cvh.hfpthk.cn

C#:   $"Hello, {name}!"
来源：http://fas.jinghuilouyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rps.feifeiyinyue.top

Py:   "第一行\n第二行"
来源：http://mlf.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://zfd.gotoacloud.top

JS:   "第一行\n第二行"
来源：http://bva.fktsv.cn

TS:   "第一行\n第二行"
来源：http://ynt.svipenyu.cn

Java: "第一行\n第二行"
来源：http://sli.fehbvm.com

Go:   "第一行\n第二行"
来源：http://ept.gzhubu.top

Ruby: "第一行\n第二行"
来源：http://bls.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://jdm.sufxvd.cn

[A14] 注释写法
来源：http://zog.shanyushiyangtech.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://otb.hesvh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://huk.aibaodan.cn

JS:   // 单行；/* 多行 */
来源：http://zne.xingfuxueyuan.xyz

TS:   // 单行；/* 多行 */
来源：http://bzg.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mps.ydjk.org.cn

Go:   // 单行；/* 多行 */
来源：http://uae.zycfv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wkb.fanxiaobao.xyz


<!-- 参考信息 -->