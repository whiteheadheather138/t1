代发 wailian999

[U91] JS：对象键值遍历
来源：http://ywb.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xhn.xylfe.cn

[U92] JS：深拷贝
来源：http://bcy.0kj1m.cn

structuredClone(obj)
来源：http://pzk.xuanzx.com

[U93] JS：模板字符串
来源：http://byt.pycfn.com

`共 ${n} 条`
来源：http://ynm.pycfn.com

[U94] JS：箭头函数
来源：http://vgq.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://eab.jianghu66.top

[U95] JS：Promise 包装
来源：http://dfw.shanyushiyangtech.top

new Promise((resolve, reject) => {})
来源：http://yqr.uphjek.com

[U96] JS：async/await 与异常
来源：http://ukm.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rur.chenjidiqi.icu

[U97] JS：并发请求
来源：http://arr.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://chg.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://yhj.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xlc.c1oappe.top

[U99] JS：事件监听
来源：http://ijc.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://zid.yj20258888.top

[U100] JS：DOM 查询
来源：http://xha.hongshengwenyu.top

document.querySelector(".item")
来源：http://iws.dashuyun.cn

[U101] JS：classList 操作
来源：http://nzs.vehdjk.com

el.classList.toggle("active")
来源：http://lrg.ppjwa.cn

[U102] JS：本地存储
来源：http://ccm.gotoacloud.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kkm.chenzaomai.com

[U103] JS：定时器
来源：http://dov.gzhubu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nto.yfazqb.com

[U104] JS：防抖
来源：http://dmf.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdk.nanxinkj.top

[U105] JS：节流
来源：http://kie.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qnt.yj20258888.top

[U106] JS：日期格式化
来源：http://qme.fehbvm.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rby.haohaochexian.top

[U107] JS：数字千分位
来源：http://jfx.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dqg.xinyue.icu

[U108] JS：随机整数
来源：http://hgd.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pjw.daxiang520.top

[U109] JS：数组分组
来源：http://hyb.vqdsnc.cn

Object.groupBy(arr, x => x.type)
来源：http://rva.hfpthk.cn

[U110] JS：数组分块
来源：http://war.hesvh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bhm.fengsongda.top

[U111] JS：对象转 Map
来源：http://vxy.zdbjq.cn

new Map(Object.entries(obj))
来源：http://nci.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://iec.cashguo.top

"7".padStart(3, "0")
来源：http://myo.yongpay.top

[U113] JS：正则替换全部
来源：http://zvv.zhixingplan.top

s.replaceAll("a", "b")
来源：http://jvw.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://dmt.bbcook.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cif.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://dgt.jiagoushi.top

crypto.randomUUID()
来源：http://ouc.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://snh.yfazqb.com

/** @param {string} name */ function f(name) {}
来源：http://btk.yj20258.top

[U117] JS：单元测试
来源：http://anr.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://whg.0kj1m.cn

[U118] JS：开发服务器
来源：http://ugh.ydjk.org.cn

npm i -D vite;  npx vite
来源：http://fpe.jqgfzy.top

[U119] JS：生产构建
来源：http://rex.vqdsnc.cn

npx vite build
来源：http://ogq.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://pkl.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://pch.yvedp.cn

================================================================================
来源：http://fqs.tianlin.xyz

统计汇总
来源：http://qgq.andypj.xyz

================================================================================
来源：http://qjq.ivvv.top

按语言统计（条）：
来源：http://pwy.zhaomingkeji.xyz

Python ......... 252
来源：http://gzq.shanyushiyangtech.top

PHP ............ 252
来源：http://duh.sweek.top

JavaScript ..... 252
来源：http://uqz.meibo888.top

TypeScript ..... 212
来源：http://snx.zhijiandao.cn

Java ........... 212
来源：http://djv.guowangkeji.top

Go ............. 212
来源：http://pfc.cqqwz.cn

Ruby ........... 212
来源：http://czj.cdnleiting.top

C# ............. 212
来源：http://tjz.dianchejie.cn

C .............. 30
来源：http://gbj.aibaodan.cn

C++ ............ 30
来源：http://eqd.jianghu66.top

SQL ............ 90
来源：http://gfc.gaohongyu789.top

Bash ........... 80
来源：http://mud.zhiwuduotai.top

Kotlin ......... 15
来源：http://yvi.wangdashe.top

Swift .......... 15
来源：http://qsc.yongpay.top

Lua ............ 10
来源：http://pug.andypj.xyz

Perl ........... 10
来源：http://zgp.smart0.xyz

Scala .......... 10
来源：http://jne.sxryk.cn

------------------------------------
来源：http://kib.ivvv.top

合计 ........... 2106 条
来源：http://bjh.sjlbkw.cn

按章节统计：
来源：http://dhd.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nnk.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pok.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lok.havefunace.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bhk.hfpthk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ysq.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ozc.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wsf.zhengqikj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xdw.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uev.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mhe.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mfj.hysaishi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hxy.meibo888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dvf.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tkq.yuxming.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kfu.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xqd.fanxiaobao.xyz

Q SQL 专题                              90
来源：http://mqn.shangyingyoupin.top

R Bash 专题                             80
来源：http://bbk.cqqwz.cn

S C / C++ 专题                          60
来源：http://dxd.kuanghao11.cn

T 其他语言补充                          60
来源：http://owg.xuetiantiany.cn

U 高频实用片段                         120
来源：http://zhp.ehwqpu.com

------------------------------------
来源：http://hla.jiagoushi.top

合计                                  2106 条
来源：http://osp.sweek.top

--------------------------------------------------------------------------------
来源：http://pki.shanyushiyangtech.top

使用提醒
来源：http://ple.yfazqb.com

--------------------------------------------------------------------------------
来源：http://ylm.vehdjk.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vlj.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zkz.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://esl.vehdjk.com

在旧版本上使用前请先确认语法支持情况。
来源：http://iqk.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jeh.xziqi.cn

—— 文件结束 ——
来源：http://gpp.redwolf501.top

================================================================================
来源：http://eki.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://spt.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://fda.chenzaomai.com

================================================================================
来源：http://twr.yongpay.top

【收录内容】
来源：http://fsx.gaohongyu789.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ufr.316326.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lgj.svipenyu.cn

SQL · Bash · C · C++
来源：http://qnc.aizwys.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mhy.smart0.xyz

【使用说明】
来源：http://gxm.jqgufenzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wnf.birdmap.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wzb.hnxiangtu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oum.nanxinkj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dji.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://okg.ppjwa.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jjq.ydjk.org.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://amk.gotoacloud.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cba.havefunace.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qru.hnxiangtu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kcd.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cjr.yj202588.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ysp.xziqi.cn

【文件统计】
来源：http://ihn.hesvh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hyw.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://esk.zhoulong.xyz

目  录
来源：http://byh.pycfn.com

--------------------------------------------------------------------------------
来源：http://grg.ybcxt.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uyn.tian-w.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hxz.jiagoushi.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dbf.hysaishi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ack.hnxiangtu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qph.hcnkem.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tns.yj20258888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uuu.hysaishi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nry.cashguo.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hjl.guowangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://opq.zdbjq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://auf.hnqzz.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://scg.xuetiantiany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lyw.hnxiangtu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wps.zhaomingkeji.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://skr.zhixingplan.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hzj.zdqjudy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rom.ehwqpu.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://gnn.nanxinkj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iyq.yonumen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://stj.fehbvm.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mev.xingfuxueyuan.xyz

================================================================================
来源：http://qun.yanxiufei.cn

A. 基础语法与类型
来源：http://eid.zdqjudy.top

================================================================================
来源：http://psb.hnqzz.top

[A01] Hello World
来源：http://fwi.sysykeji.top

Py:   print("Hello, World!")
来源：http://hls.shuidangran.top

PHP:  echo "Hello, World!";
来源：http://twk.xuetiantiany.cn

JS:   console.log("Hello, World!");
来源：http://uca.fktsv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lvh.gzhubu.top

Java: System.out.println("Hello, World!");
来源：http://rqf.zhoulong.xyz

Go:   fmt.Println("Hello, World!")
来源：http://wxp.zdbjq.cn

Ruby: puts "Hello, World!"
来源：http://lpg.daria6918.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bvn.quarkkingdee.top

[A02] 变量声明与赋值
来源：http://jic.hywenlv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vnm.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://iwi.shanyushiyangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://vmr.redwolf501.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oip.yj20258888.top

Java: String name = "Alex"; int age = 20;
来源：http://pgq.52xcode.cn

Go:   name := "Alex"; age := 20
来源：http://zse.bjfxy.top

Ruby: name = "Alex"; age = 20
来源：http://ufy.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://jyb.tianlin.xyz

[A03] 常量定义
来源：http://dwa.yangfankeji.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ryp.smart0.xyz

PHP:  const PI = 3.14159;
来源：http://dwi.shzxlz.cn

JS:   const PI = 3.14159;
来源：http://yij.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://vpl.hysaishi.cn

Java: static final double PI = 3.14159;
来源：http://nak.zhengqikj.top

Go:   const PI = 3.14159
来源：http://nhh.tian-w.cn

Ruby: PI = 3.14159
来源：http://fqc.yuxming.cn

C#:   const double PI = 3.14159;
来源：http://zpn.ppjwa.cn

[A04] 判断变量类型
来源：http://rki.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ouu.jyoumei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bww.gzhubu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://siw.fzhhl.top

TS:   typeof x; x instanceof Date
来源：http://iib.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jzh.yangfankeji.com

Go:   reflect.TypeOf(x).Name()
来源：http://hlj.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lvf.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://rkj.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://wpi.mhx1999.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ggz.zhaomingkeji.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://tau.nanxuanxn.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ksf.xinyue.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qsi.hesvh.cn

Java: 7 / 2; 7 % 2
来源：http://ehw.ydzc1.top

Go:   7 / 2; 7 % 2
来源：http://nni.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://wij.aibaodan.cn

C#:   7 / 2; 7 % 2
来源：http://xsg.xuetiantiany.cn

[A06] 字符串转数字
来源：http://qjb.yuanzhike.top

Py:   int("42"); float("3.14")
来源：http://uld.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bag.fktsv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cpd.jiagoushi.top

TS:   parseInt("42", 10); Number("42")
来源：http://hoe.ydjk.org.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://boi.shuidangran.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vpq.chenjidiqi.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://vob.yongpay.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fpn.fzhhl.top

[A07] 数字转字符串
来源：http://rcs.xinyue.icu

Py:   str(42)
来源：http://cuo.cdnleiting.top

PHP:  (string) 42; strval(42)
来源：http://krn.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://hdw.ctjpmb.com

TS:   String(42)
来源：http://fwg.fengsongda.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hid.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://izy.uphjek.com

Ruby: 42.to_s
来源：http://yps.dianchejie.cn

C#:   42.ToString()
来源：http://tnf.fengsongda.top

[A08] 取整与四舍五入
来源：http://rsv.gaohongyu789.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lla.hnxiangtu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ael.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pud.gotoacloud.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gzv.zhijiandao.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lod.sxryk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fyq.hammf.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://msn.chenjidiqi.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://smc.fengsongda.top

[A09] 绝对值与最大最小值
来源：http://iow.52xcode.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ejr.havefunace.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vmk.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hxj.cheryme.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bwj.svipenyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://adg.shanyushiyangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tem.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kam.cucudq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gnq.hcnkem.com

[A10] 生成随机数
来源：http://euw.fanxiaobao.xyz

Py:   import random; random.randint(1, 100)
来源：http://cmt.shangyingyoupin.top

PHP:  random_int(1, 100);
来源：http://fbc.svipenyu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xzn.guannengcc.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ssq.yanxiufei.cn

Java: new Random().nextInt(100) + 1
来源：http://fvp.fanxiaobao.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gvz.jianghu66.top

Ruby: rand(1..100)
来源：http://ofe.xinyue.icu

C#:   new Random().Next(1, 101)
来源：http://nok.hammf.cn

[A11] 条件表达式（三元）
来源：http://aro.hammf.cn

Py:   "yes" if x > 0 else "no"
来源：http://ewe.xingfuxueyuan.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://phr.chenlongwang.top

JS:   x > 0 ? "yes" : "no"
来源：http://zuy.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vza.yj202588.top

Java: x > 0 ? "yes" : "no"
来源：http://gcn.ywan-chungtsiang.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hjz.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tan.aizwys.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ynl.chenlongwang.top

[A12] 字符串插值 / 格式化
来源：http://qey.yueranfly.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bbm.9152youxi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kdg.zhaomingkeji.xyz

JS:   `Hello, ${name}!`
来源：http://lcv.hnqzz.top

TS:   `Hello, ${name}!`
来源：http://jod.aibaodan.cn

Java: "Hello, %s!".formatted(name)
来源：http://pum.zhixingplan.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fmn.dianchejie.cn

Ruby: "Hello, #{name}!"
来源：http://sgg.ydjk.org.cn

C#:   $"Hello, {name}!"
来源：http://gcc.nwbrower.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ibx.dashuyun.cn

Py:   "第一行\n第二行"
来源：http://ozj.smart0.xyz

PHP:  "第一行\n第二行"
来源：http://sgw.andypj.xyz

JS:   "第一行\n第二行"
来源：http://vah.zhixingplan.top

TS:   "第一行\n第二行"
来源：http://iuy.jinqigufen.top

Java: "第一行\n第二行"
来源：http://rbq.yongpay.top

Go:   "第一行\n第二行"
来源：http://ixc.cucudq.cn

Ruby: "第一行\n第二行"
来源：http://vfu.dianchejie.cn

C#:   "第一行\n第二行"
来源：http://fjq.gotoacloud.top

[A14] 注释写法
来源：http://zhe.epnwcf.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://moi.yvedp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mxu.shzxlz.cn

JS:   // 单行；/* 多行 */
来源：http://cbp.guowangkeji.top

TS:   // 单行；/* 多行 */
来源：http://bkk.c1oappe.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kku.zhijiandao.cn

Go:   // 单行；/* 多行 */
来源：http://prx.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://row.jinyuanbaomall.cn

C#:   // 单行；/* 多行 */
来源：http://alx.wangshuangyany.cn

[A15] 空值判断与默认值
来源：http://vso.kuanghao11.cn

Py:   value = data or "默认值"
来源：http://omz.yongpay.top

PHP:  $value = $data ?? "默认值";
来源：http://ztg.cucudq.cn

JS:   const value = data ?? "默认值";
来源：http://bcv.kuanghao11.cn

TS:   const value = data ?? "默认值";
来源：http://wnq.ydjk.org.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oiw.gogol.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://yli.vehdjk.com


<!-- 参考信息 -->