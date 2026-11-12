代发 wailian999

[U87] JS：解构默认值
来源：http://eia.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://qmq.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://vhi.fktsv.cn

{ ...a, ...b }
来源：http://lxe.mhx1999.top

[U89] JS：数组去重
来源：http://qnc.chenzaomai.com

[...new Set(arr)]
来源：http://bnt.wangshuangyany.cn

[U90] JS：数字数组排序
来源：http://rds.bbcook.cn

[...arr].sort((a, b) => a - b)
来源：http://wrf.aibaodan.cn

[U91] JS：对象键值遍历
来源：http://jqy.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jtb.hywenlv.cn

[U92] JS：深拷贝
来源：http://csk.dianchejie.cn

structuredClone(obj)
来源：http://toh.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://xwh.xziqi.cn

`共 ${n} 条`
来源：http://tzc.aibaodan.cn

[U94] JS：箭头函数
来源：http://gvr.zhoulong.xyz

const double = x => x * 2;
来源：http://lnl.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://vkt.vehdjk.com

new Promise((resolve, reject) => {})
来源：http://hii.bbcook.cn

[U96] JS：async/await 与异常
来源：http://rvo.mhx1999.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qwj.gotoacloud.top

[U97] JS：并发请求
来源：http://bxp.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ehh.xinyue.icu

[U98] JS：fetch 带 JSON
来源：http://txp.wangshuangyany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gbr.zhiwuduotai.top

[U99] JS：事件监听
来源：http://nxn.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://tpf.pycfn.com

[U100] JS：DOM 查询
来源：http://mhb.cqqwz.cn

document.querySelector(".item")
来源：http://zyi.tanke756.top

[U101] JS：classList 操作
来源：http://jds.yfazqb.com

el.classList.toggle("active")
来源：http://aix.ydjk.org.cn

[U102] JS：本地存储
来源：http://nmo.jinghuilouyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://euc.zhiwuduotai.top

[U103] JS：定时器
来源：http://fkd.tian-w.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ukb.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://ppr.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vtf.ydzc1.top

[U105] JS：节流
来源：http://kgc.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qog.tanke756.top

[U106] JS：日期格式化
来源：http://gsx.yuanzhike.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://icr.yanxiufei.cn

[U107] JS：数字千分位
来源：http://rss.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vnn.kuanghao11.cn

[U108] JS：随机整数
来源：http://hsc.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ehk.yj20258.top

[U109] JS：数组分组
来源：http://cdr.iojbl.cn

Object.groupBy(arr, x => x.type)
来源：http://jdk.yueranfly.top

[U110] JS：数组分块
来源：http://gec.9152youxi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bst.jinyuanbaomall.cn

[U111] JS：对象转 Map
来源：http://gzy.xylfe.cn

new Map(Object.entries(obj))
来源：http://grf.guowangkeji.top

[U112] JS：字符串补位
来源：http://zgt.nanxuanxn.top

"7".padStart(3, "0")
来源：http://xxw.zdqjudy.top

[U113] JS：正则替换全部
来源：http://duf.zycfv.cn

s.replaceAll("a", "b")
来源：http://mdh.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://hby.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hcs.birdmap.top

[U115] JS：生成 UUID
来源：http://tgs.nwbrower.top

crypto.randomUUID()
来源：http://npl.haohaochexian.top

[U116] JS：类型检查（JSDoc）
来源：http://fin.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://gbo.sxryk.cn

[U117] JS：单元测试
来源：http://xwm.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://rfd.dianchejie.cn

[U118] JS：开发服务器
来源：http://gne.yanxiufei.cn

npm i -D vite;  npx vite
来源：http://kmx.yj202588.top

[U119] JS：生产构建
来源：http://oag.xuetiantiany.cn

npx vite build
来源：http://lxq.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://ofo.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://jlt.zhijiandao.cn

================================================================================
来源：http://can.dashuyun.cn

统计汇总
来源：http://stf.snrcjt.cn

================================================================================
来源：http://djz.redwolf501.top

按语言统计（条）：
来源：http://tld.snrcjt.cn

Python ......... 252
来源：http://rbo.xuanzx.com

PHP ............ 252
来源：http://dbg.xuanzx.com

JavaScript ..... 252
来源：http://vzb.yonumen.top

TypeScript ..... 212
来源：http://puk.xuetiantiany.cn

Java ........... 212
来源：http://cvl.svipenyu.cn

Go ............. 212
来源：http://bmk.jyoumei.cn

Ruby ........... 212
来源：http://qbn.yongpay.top

C# ............. 212
来源：http://fic.nanxinkj.top

C .............. 30
来源：http://tvm.cheryme.top

C++ ............ 30
来源：http://gup.cheryme.top

SQL ............ 90
来源：http://unu.gogol.net.cn

Bash ........... 80
来源：http://zlr.cheryme.top

Kotlin ......... 15
来源：http://vgq.haohaochexian.top

Swift .......... 15
来源：http://djy.quarkkingdee.top

Lua ............ 10
来源：http://azt.yangfankeji.com

Perl ........... 10
来源：http://vvn.gotoacloud.top

Scala .......... 10
来源：http://vmq.ivvv.top

------------------------------------
来源：http://tms.fktsv.cn

合计 ........... 2106 条
来源：http://bvi.zhongyouzk.top

按章节统计：
来源：http://cws.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xju.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ftm.pycfn.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vex.svipenyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nep.zhongyouzk.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ucl.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gxv.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wct.fanxiaobao.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bep.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hhk.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xlr.haohaochexian.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cqd.yueranfly.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dqy.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vkt.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://emw.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qpg.cdnleiting.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tpy.hnxiangtu.top

Q SQL 专题                              90
来源：http://yzg.sxryk.cn

R Bash 专题                             80
来源：http://zie.chenlongwang.top

S C / C++ 专题                          60
来源：http://cps.52xcode.cn

T 其他语言补充                          60
来源：http://cep.cdnleiting.top

U 高频实用片段                         120
来源：http://hje.gotoacloud.top

------------------------------------
来源：http://ihe.hongshengwenyu.top

合计                                  2106 条
来源：http://vtv.zycfv.cn

--------------------------------------------------------------------------------
来源：http://jrq.hammf.cn

使用提醒
来源：http://lyb.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://tey.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sjv.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://izn.gogol.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://utc.fehbvm.com

在旧版本上使用前请先确认语法支持情况。
来源：http://nvs.yangfankeji.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://has.feifeiyinyue.top

—— 文件结束 ——
来源：http://svc.hcnkem.com

================================================================================
来源：http://ngp.fktsv.cn

程序语言常见例子速查手册（2024 版）
来源：http://rgj.hammf.cn

Common Programming Examples Cheat Book
来源：http://esr.ivvv.top

================================================================================
来源：http://wtl.nanxuanxn.top

【收录内容】
来源：http://kzc.xylfe.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bvy.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uow.jianghu66.top

SQL · Bash · C · C++
来源：http://vgm.yuxming.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ood.zhiwuduotai.top

【使用说明】
来源：http://oda.tanke756.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mbr.svipenyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mmd.iojbl.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fwj.sysykeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gop.xuanzx.com

Bash:  Shell         C:     C             C++:   C++
来源：http://iba.havefunace.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://phr.cucudq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jak.fzhhl.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zun.daria6918.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ics.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xai.shuidangran.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ure.zhijiandao.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jgs.wangshuangyany.cn

【文件统计】
来源：http://pat.birdmap.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vet.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://vtx.guowangkeji.top

目  录
来源：http://tsu.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://edn.zycfv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mwi.yongpay.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qmu.ehwqpu.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sxn.jianghu66.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tew.fktsv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jcc.daria6918.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fez.shanyushiyangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wga.ywan-chungtsiang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mtj.sysykeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jqi.epnwcf.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ufk.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yrz.yj202588.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://juf.pycfn.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fwa.xuanzx.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eqr.jinqigfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jwa.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fxk.zhongyouzk.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fpo.zhaomingkeji.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://yog.vqdsnc.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fpz.svipenyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jdi.chenjidiqi.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dji.sysykeji.top

================================================================================
来源：http://bjg.smart0.xyz

A. 基础语法与类型
来源：http://mcx.316326.xyz

================================================================================
来源：http://ozq.hongshengwenyu.top

[A01] Hello World
来源：http://tbf.shanyushiyangkeji.top

Py:   print("Hello, World!")
来源：http://aol.hysaishi.cn

PHP:  echo "Hello, World!";
来源：http://hjc.mhx1999.top

JS:   console.log("Hello, World!");
来源：http://ora.yvedp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dqq.zdbjq.cn

Java: System.out.println("Hello, World!");
来源：http://jdt.yanxiufei.cn

Go:   fmt.Println("Hello, World!")
来源：http://jpy.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://qmu.gaohongyu789.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zgv.tian-w.cn

[A02] 变量声明与赋值
来源：http://jdc.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gih.shangyingyoupin.top

PHP:  $name = "Alex"; $age = 20;
来源：http://dvw.hysaishi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yhs.tianlin.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://znx.kuanghao11.cn

Java: String name = "Alex"; int age = 20;
来源：http://mzw.jinqigufen.top

Go:   name := "Alex"; age := 20
来源：http://dos.feifeiyinyue.top

Ruby: name = "Alex"; age = 20
来源：http://jzr.vqdsnc.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vpp.gotoacloud.top

[A03] 常量定义
来源：http://frz.zdbjq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cul.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://pct.hywenlv.cn

JS:   const PI = 3.14159;
来源：http://iqd.uphjek.com

TS:   const PI: number = 3.14159;
来源：http://wzw.yonumen.top

Java: static final double PI = 3.14159;
来源：http://wzr.yuxming.cn

Go:   const PI = 3.14159
来源：http://tnd.cdnleiting.top

Ruby: PI = 3.14159
来源：http://dmz.shangyingyoupin.top

C#:   const double PI = 3.14159;
来源：http://xkv.jinyuanbaomall.cn

[A04] 判断变量类型
来源：http://edb.ydjk.org.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sjy.yfazqb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fol.hnxiangtu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sop.9152youxi.cn

TS:   typeof x; x instanceof Date
来源：http://mtk.yvedp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bar.shanyushiyangkeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://iya.fzhhl.top

Ruby: x.class; x.is_a?(Integer)
来源：http://org.ivvv.top

C#:   x.GetType().Name; x is int
来源：http://doa.cucudq.cn

[A05] 整数除法与取模
来源：http://kkb.tarul.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://opa.bbcook.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fjs.vehdjk.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ryx.ctjpmb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://plb.cucudq.cn

Java: 7 / 2; 7 % 2
来源：http://ogr.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://kya.yvedp.cn

Ruby: 7 / 2; 7 % 2
来源：http://rqq.sufxvd.cn

C#:   7 / 2; 7 % 2
来源：http://zco.aibaodan.cn

[A06] 字符串转数字
来源：http://ije.shzxlz.cn

Py:   int("42"); float("3.14")
来源：http://rha.cdnleiting.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sjr.andypj.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xsx.shanyushiyangtech.top

TS:   parseInt("42", 10); Number("42")
来源：http://zdz.jqgufenzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://eno.ydzc1.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eej.dashuyun.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bxs.nanxuanxn.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uqy.birdmap.top

[A07] 数字转字符串
来源：http://qua.nanxuanxn.top

Py:   str(42)
来源：http://xem.hcnkem.com

PHP:  (string) 42; strval(42)
来源：http://uwp.dianchejie.cn

JS:   String(42); (42).toString()
来源：http://ewz.aibaodan.cn

TS:   String(42)
来源：http://jvl.xuanzx.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://zpa.zhixingplan.top

Go:   strconv.Itoa(42)
来源：http://zhr.zhiwuduotai.top

Ruby: 42.to_s
来源：http://faj.svipenyu.cn

C#:   42.ToString()
来源：http://fxy.hcnkem.com

[A08] 取整与四舍五入
来源：http://rjg.shzxlz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uif.fktsv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ial.cucudq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mos.c1oappe.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://emu.yonumen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bed.shangyingyoupin.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iea.zhixingplan.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zte.xziqi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tgm.tarul.cn

[A09] 绝对值与最大最小值
来源：http://jrx.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wfr.hnxiangtu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yoz.fzhhl.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bar.xinyue.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wdp.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qdw.shzxlz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dso.redwolf501.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dqc.guannengcc.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lws.jinyuanbaomall.cn

[A10] 生成随机数
来源：http://ynr.guannengcc.top

Py:   import random; random.randint(1, 100)
来源：http://vpa.quarkkingdee.top

PHP:  random_int(1, 100);
来源：http://vck.sweek.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cuj.yj20258888.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://upq.shzxlz.cn

Java: new Random().nextInt(100) + 1
来源：http://ulw.sysykeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kpr.hysaishi.cn

Ruby: rand(1..100)
来源：http://hru.gogol.net.cn

C#:   new Random().Next(1, 101)
来源：http://ras.jinghuilouyu.cn

[A11] 条件表达式（三元）
来源：http://zvc.yuxming.cn

Py:   "yes" if x > 0 else "no"
来源：http://ghm.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://csi.aibaodan.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xuz.yvedp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pfo.fanxiaobao.xyz

Java: x > 0 ? "yes" : "no"
来源：http://vmw.vqdsnc.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jrd.cheryme.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gzj.0kj1m.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yvt.hysaishi.cn

[A12] 字符串插值 / 格式化
来源：http://sjw.fehbvm.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rwd.zhixingplan.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zby.svipenyu.cn

JS:   `Hello, ${name}!`
来源：http://fwb.sxryk.cn

TS:   `Hello, ${name}!`
来源：http://chf.fzhhl.top

Java: "Hello, %s!".formatted(name)
来源：http://ciw.jinqigufen.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://day.sysykeji.top

Ruby: "Hello, #{name}!"
来源：http://hay.guowangkeji.top

C#:   $"Hello, {name}!"
来源：http://srb.uphjek.com

[A13] 多行字符串（练习 \n 转义）
来源：http://blz.yj20258.top

Py:   "第一行\n第二行"
来源：http://glo.birdmap.top

PHP:  "第一行\n第二行"
来源：http://uog.yonumen.top

JS:   "第一行\n第二行"
来源：http://ntn.aizwys.cn

TS:   "第一行\n第二行"
来源：http://xuq.uphjek.com

Java: "第一行\n第二行"
来源：http://hee.svipenyu.cn

Go:   "第一行\n第二行"
来源：http://uyx.hnqzz.top

Ruby: "第一行\n第二行"
来源：http://yuj.zhongyouzk.top

C#:   "第一行\n第二行"
来源：http://uow.nwbrower.top

[A14] 注释写法
来源：http://nkg.yfazqb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://zlq.hongshengwenyu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ivm.9152youxi.cn

JS:   // 单行；/* 多行 */
来源：http://dck.ctjpmb.com

TS:   // 单行；/* 多行 */
来源：http://sqd.zhengqikj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xmg.zycfv.cn

Go:   // 单行；/* 多行 */
来源：http://szh.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://iqh.jyoumei.cn


<!-- 参考信息 -->