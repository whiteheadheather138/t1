代发 wailian999

[U85] JS：可选链
来源：http://nby.cucudq.cn

a?.b?.c
来源：http://yjh.cheryme.top

[U86] JS：空值合并
来源：http://pin.havefunace.top

a ?? b
来源：http://svo.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://qlm.zhoulong.xyz

const { a = 1, b = 2 } = obj;
来源：http://pbs.zdbjq.cn

[U88] JS：对象展开合并
来源：http://efp.smart0.xyz

{ ...a, ...b }
来源：http://yjm.bbcook.cn

[U89] JS：数组去重
来源：http://cnu.cqqwz.cn

[...new Set(arr)]
来源：http://mvq.gotoacloud.top

[U90] JS：数字数组排序
来源：http://qcs.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://gww.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://orp.cheryme.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nwr.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://hgc.hnqzz.top

structuredClone(obj)
来源：http://oqa.gzhubu.top

[U93] JS：模板字符串
来源：http://mif.jlsjyb.cn

`共 ${n} 条`
来源：http://ibe.gzhubu.top

[U94] JS：箭头函数
来源：http://dva.cashguo.top

const double = x => x * 2;
来源：http://hzo.zhixingplan.top

[U95] JS：Promise 包装
来源：http://tic.jyoumei.cn

new Promise((resolve, reject) => {})
来源：http://xdz.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://pow.daria6918.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ofs.c1oappe.top

[U97] JS：并发请求
来源：http://iln.52xcode.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yqq.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://hmi.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hry.chenjidiqi.icu

[U99] JS：事件监听
来源：http://nwc.zhaomingkeji.xyz

el.addEventListener("click", e => {})
来源：http://amf.cheryme.top

[U100] JS：DOM 查询
来源：http://ayq.yuanzhike.top

document.querySelector(".item")
来源：http://gkv.uphjek.com

[U101] JS：classList 操作
来源：http://tyg.feifeiyinyue.top

el.classList.toggle("active")
来源：http://olo.haohaochexian.top

[U102] JS：本地存储
来源：http://ntf.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://rmf.wangdashe.top

[U103] JS：定时器
来源：http://ncb.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rzd.shanyushiyangtech.top

[U104] JS：防抖
来源：http://rjq.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://edr.cucudq.cn

[U105] JS：节流
来源：http://oui.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pxr.redwolf501.top

[U106] JS：日期格式化
来源：http://lbw.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iko.bjfxy.top

[U107] JS：数字千分位
来源：http://xgb.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dbp.bbcook.cn

[U108] JS：随机整数
来源：http://rpm.hnqzz.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wxm.xziqi.cn

[U109] JS：数组分组
来源：http://zij.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://zzh.vehdjk.com

[U110] JS：数组分块
来源：http://wcg.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://neu.xziqi.cn

[U111] JS：对象转 Map
来源：http://mnu.hywenlv.cn

new Map(Object.entries(obj))
来源：http://ecm.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://wtk.tanke756.top

"7".padStart(3, "0")
来源：http://lkw.xylfe.cn

[U113] JS：正则替换全部
来源：http://coq.uphjek.com

s.replaceAll("a", "b")
来源：http://awy.fktsv.cn

[U114] JS：JSON 深比较
来源：http://iow.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://awo.yuanzhike.top

[U115] JS：生成 UUID
来源：http://syw.gaohongyu789.top

crypto.randomUUID()
来源：http://gza.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://ptn.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://cct.ydzc1.top

[U117] JS：单元测试
来源：http://fbl.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://hqb.wangdashe.top

[U118] JS：开发服务器
来源：http://mxd.tian-w.cn

npm i -D vite;  npx vite
来源：http://cwi.meibo888.top

[U119] JS：生产构建
来源：http://oxq.zdbjq.cn

npx vite build
来源：http://bep.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://ajq.ydzc1.top

import.meta.env.VITE_API_URL
来源：http://pxp.ivvv.top

================================================================================
来源：http://iwx.zycfv.cn

统计汇总
来源：http://ocg.cucudq.cn

================================================================================
来源：http://swb.bjfxy.top

按语言统计（条）：
来源：http://kaq.52xcode.cn

Python ......... 252
来源：http://vuo.tianlin.xyz

PHP ............ 252
来源：http://xry.cheryme.top

JavaScript ..... 252
来源：http://npd.52xcode.cn

TypeScript ..... 212
来源：http://itg.sufxvd.cn

Java ........... 212
来源：http://onz.haohaochexian.top

Go ............. 212
来源：http://rie.chenjidiqi.icu

Ruby ........... 212
来源：http://ora.nwbrower.top

C# ............. 212
来源：http://xdr.wangshuangyany.cn

C .............. 30
来源：http://kkh.zhixingplan.top

C++ ............ 30
来源：http://qwi.snrcjt.cn

SQL ............ 90
来源：http://zvy.tanke756.top

Bash ........... 80
来源：http://cwl.vehdjk.com

Kotlin ......... 15
来源：http://auv.redwolf501.top

Swift .......... 15
来源：http://csi.hysaishi.cn

Lua ............ 10
来源：http://mfg.cashguo.top

Perl ........... 10
来源：http://byw.epnwcf.com

Scala .......... 10
来源：http://cbw.cucudq.cn

------------------------------------
来源：http://bva.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://psn.quarkkingdee.top

按章节统计：
来源：http://hmu.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://aal.jinqigfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bry.shangyingyoupin.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gye.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gxf.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://geo.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ujn.zhaomingkeji.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aqh.ydzc1.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xgw.sufxvd.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mim.guowangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vxr.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fmu.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wgo.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pbl.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dxy.epnwcf.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hgt.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cop.yongpay.top

Q SQL 专题                              90
来源：http://yty.daxiang520.top

R Bash 专题                             80
来源：http://iry.jinqigufen.top

S C / C++ 专题                          60
来源：http://rmc.gotoacloud.top

T 其他语言补充                          60
来源：http://khr.wangshuangyany.cn

U 高频实用片段                         120
来源：http://rwx.ywan-chungtsiang.top

------------------------------------
来源：http://vei.ydzc1.top

合计                                  2106 条
来源：http://ksr.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://myl.redwolf501.top

使用提醒
来源：http://wdc.yj20258888.top

--------------------------------------------------------------------------------
来源：http://ejf.shzxlz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://elm.yonumen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vlj.aizwys.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gja.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ifn.quarkkingdee.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xlg.pengpengdd.cyou

—— 文件结束 ——
来源：http://deh.hysaishi.cn

================================================================================
来源：http://tuo.sxryk.cn

程序语言常见例子速查手册（2024 版）
来源：http://pge.yuxming.cn

Common Programming Examples Cheat Book
来源：http://ykl.0kj1m.cn

================================================================================
来源：http://dgy.jiagoushi.top

【收录内容】
来源：http://jbv.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ajp.aizwys.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fth.ydjk.org.cn

SQL · Bash · C · C++
来源：http://snu.yonumen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hrn.cucudq.cn

【使用说明】
来源：http://oxs.ctjpmb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zjc.xuetiantiany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ybt.tian-w.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jbn.chenjidiqi.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qgn.tanke756.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tcj.jinqigfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mwd.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kpw.yonumen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://waw.gaohongyu789.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kub.jlsjyb.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ady.gogol.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ncu.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vrn.jinqigufen.top

【文件统计】
来源：http://hoa.zhixingplan.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hje.havefunace.top

--------------------------------------------------------------------------------
来源：http://bek.sweek.top

目  录
来源：http://lhq.zycfv.cn

--------------------------------------------------------------------------------
来源：http://puj.zhoulong.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nho.dianchejie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://itr.smart0.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sqr.hesvh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://azy.yj20258888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nbf.yonumen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gvl.pycfn.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zqn.ehwqpu.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tnz.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iof.ctjpmb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bqp.shanyushiyangtech.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://igs.xuetiantiany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hgw.yj20258.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vpg.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ntt.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xcu.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lre.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nva.fanxiaobao.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://gys.iojbl.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cfw.birdmap.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ycs.cashguo.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oho.hesvh.cn

================================================================================
来源：http://fsa.vehdjk.com

A. 基础语法与类型
来源：http://zlb.zdqjudy.top

================================================================================
来源：http://nda.feifeiyinyue.top

[A01] Hello World
来源：http://ncd.aizwys.cn

Py:   print("Hello, World!")
来源：http://zkn.birdmap.top

PHP:  echo "Hello, World!";
来源：http://krc.zhijiandao.cn

JS:   console.log("Hello, World!");
来源：http://tdo.guannengcc.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nyv.316326.xyz

Java: System.out.println("Hello, World!");
来源：http://psl.meibo888.top

Go:   fmt.Println("Hello, World!")
来源：http://wpv.pengpengdd.cyou

Ruby: puts "Hello, World!"
来源：http://hdb.feifeiyinyue.top

C#:   Console.WriteLine("Hello, World!");
来源：http://exd.yfazqb.com

[A02] 变量声明与赋值
来源：http://ihv.tarul.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hvt.yongpay.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uif.zhiwuduotai.top

JS:   let name = "Alex"; const age = 20;
来源：http://loq.iojbl.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ubi.aibaodan.cn

Java: String name = "Alex"; int age = 20;
来源：http://fpj.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://gvj.shangyingyoupin.top

Ruby: name = "Alex"; age = 20
来源：http://vur.chenzaomai.com

C#:   string name = "Alex"; int age = 20;
来源：http://lfj.hongshengwenyu.top

[A03] 常量定义
来源：http://ygo.ivvv.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zks.zhaomingkeji.xyz

PHP:  const PI = 3.14159;
来源：http://ydm.ywan-chungtsiang.top

JS:   const PI = 3.14159;
来源：http://gmv.ctjpmb.com

TS:   const PI: number = 3.14159;
来源：http://sef.vqdsnc.cn

Java: static final double PI = 3.14159;
来源：http://bbu.sweek.top

Go:   const PI = 3.14159
来源：http://apu.jiagoushi.top

Ruby: PI = 3.14159
来源：http://gmm.yanxiufei.cn

C#:   const double PI = 3.14159;
来源：http://cft.cashguo.top

[A04] 判断变量类型
来源：http://dst.sufxvd.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ybv.zycfv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ibi.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hri.jlsjyb.cn

TS:   typeof x; x instanceof Date
来源：http://mdu.tian-w.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://euc.nanxuanxn.top

Go:   reflect.TypeOf(x).Name()
来源：http://fbl.zhiwuduotai.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mmg.jqgufenzy.top

C#:   x.GetType().Name; x is int
来源：http://vdn.bbcook.cn

[A05] 整数除法与取模
来源：http://azc.jinyuanbaomall.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sdy.jinqigufen.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ktw.zycfv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ljk.zhoulong.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cze.ivvv.top

Java: 7 / 2; 7 % 2
来源：http://riq.yanxiufei.cn

Go:   7 / 2; 7 % 2
来源：http://cfx.fzhhl.top

Ruby: 7 / 2; 7 % 2
来源：http://bmj.cdnleiting.top

C#:   7 / 2; 7 % 2
来源：http://pxg.cheryme.top

[A06] 字符串转数字
来源：http://xuo.vehdjk.com

Py:   int("42"); float("3.14")
来源：http://fgq.0kj1m.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lks.gaohongyu789.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jcm.cucudq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cwl.daria6918.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wuj.xylfe.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yab.zhongyouzk.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ruz.cucudq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hjc.aizwys.cn

[A07] 数字转字符串
来源：http://acb.0kj1m.cn

Py:   str(42)
来源：http://lkk.jiagoushi.top

PHP:  (string) 42; strval(42)
来源：http://rcy.hnqzz.top

JS:   String(42); (42).toString()
来源：http://rli.feifeiyinyue.top

TS:   String(42)
来源：http://tbo.hfpthk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gsg.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://qgn.316326.xyz

Ruby: 42.to_s
来源：http://qab.vqdsnc.cn

C#:   42.ToString()
来源：http://fmc.xziqi.cn

[A08] 取整与四舍五入
来源：http://nok.yonumen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cpv.fanxiaobao.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gku.aibaodan.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cpg.bbcook.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sba.zhaomingkeji.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eqw.yanxiufei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hho.gotoacloud.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://onw.bjfxy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bsv.yvedp.cn

[A09] 绝对值与最大最小值
来源：http://xdc.shanyushiyangtech.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fob.yj20258.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fdj.sweek.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cii.sysykeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uhp.tanke756.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dhm.jlsjyb.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yes.hysaishi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qck.fzhhl.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://khg.pengpengdd.cyou

[A10] 生成随机数
来源：http://ckn.daria6918.cn

Py:   import random; random.randint(1, 100)
来源：http://dpe.jiagoushi.top

PHP:  random_int(1, 100);
来源：http://sqy.chenjidiqi.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vyr.hnxiangtu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xuc.jyoumei.cn

Java: new Random().nextInt(100) + 1
来源：http://prr.xylfe.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kru.zhoulong.xyz

Ruby: rand(1..100)
来源：http://vqh.yongpay.top

C#:   new Random().Next(1, 101)
来源：http://tns.hongshengwenyu.top

[A11] 条件表达式（三元）
来源：http://qgj.sysykeji.top

Py:   "yes" if x > 0 else "no"
来源：http://iok.c1oappe.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://wms.xingfuxueyuan.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://bcl.yj202588.top

TS:   x > 0 ? "yes" : "no"
来源：http://xzd.pycfn.com

Java: x > 0 ? "yes" : "no"
来源：http://xle.yanxiufei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zqe.xziqi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vyc.yuanzhike.top

C#:   x > 0 ? "yes" : "no"
来源：http://ego.yonumen.top

[A12] 字符串插值 / 格式化
来源：http://byq.jinyuanbaomall.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vrp.daria6918.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://phc.yfazqb.com

JS:   `Hello, ${name}!`
来源：http://asq.pycfn.com

TS:   `Hello, ${name}!`
来源：http://pfq.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://sxk.cucudq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rmf.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://kul.kuanghao11.cn

C#:   $"Hello, {name}!"
来源：http://gbb.yfazqb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://kxi.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://yyv.tanke756.top

PHP:  "第一行\n第二行"
来源：http://qnk.chenzaomai.com

JS:   "第一行\n第二行"
来源：http://dya.vehdjk.com

TS:   "第一行\n第二行"
来源：http://vyd.dianchejie.cn

Java: "第一行\n第二行"
来源：http://cgm.52xcode.cn

Go:   "第一行\n第二行"
来源：http://ucp.nanxuanxn.top

Ruby: "第一行\n第二行"
来源：http://ric.jinghuilouyu.cn

C#:   "第一行\n第二行"
来源：http://stw.hysaishi.cn

[A14] 注释写法
来源：http://ydt.tanke756.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://opa.yangfankeji.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://fni.shuidangran.top

JS:   // 单行；/* 多行 */
来源：http://lma.hesvh.cn


<!-- 参考信息 -->