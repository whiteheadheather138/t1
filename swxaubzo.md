代发 wailian999

[U85] JS：可选链
来源：http://mlg.zhiwuduotai.top

a?.b?.c
来源：http://rvx.yj20258.top

[U86] JS：空值合并
来源：http://zhl.fktsv.cn

a ?? b
来源：http://uji.hnqzz.top

[U87] JS：解构默认值
来源：http://gax.hesvh.cn

const { a = 1, b = 2 } = obj;
来源：http://csg.aibaodan.cn

[U88] JS：对象展开合并
来源：http://lnk.hywenlv.cn

{ ...a, ...b }
来源：http://rpr.ivvv.top

[U89] JS：数组去重
来源：http://dyr.guowangkeji.top

[...new Set(arr)]
来源：http://ibz.sxryk.cn

[U90] JS：数字数组排序
来源：http://lek.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://vqq.zycfv.cn

[U91] JS：对象键值遍历
来源：http://fug.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pph.chenjidiqi.icu

[U92] JS：深拷贝
来源：http://xdj.feifeiyinyue.top

structuredClone(obj)
来源：http://zuv.aizwys.cn

[U93] JS：模板字符串
来源：http://ltk.ctjpmb.com

`共 ${n} 条`
来源：http://dga.svipenyu.cn

[U94] JS：箭头函数
来源：http://zjl.vqdsnc.cn

const double = x => x * 2;
来源：http://ffe.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://een.nanxuanxn.top

new Promise((resolve, reject) => {})
来源：http://qbt.cashguo.top

[U96] JS：async/await 与异常
来源：http://ubn.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dqg.yj20258888.top

[U97] JS：并发请求
来源：http://xtz.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nhd.zhijiandao.cn

[U98] JS：fetch 带 JSON
来源：http://xnt.zhongyouzk.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lnn.ybcxt.top

[U99] JS：事件监听
来源：http://znm.fengsongda.top

el.addEventListener("click", e => {})
来源：http://wck.52xcode.cn

[U100] JS：DOM 查询
来源：http://ort.andypj.xyz

document.querySelector(".item")
来源：http://ijm.meibo888.top

[U101] JS：classList 操作
来源：http://tnr.daria6918.cn

el.classList.toggle("active")
来源：http://kgk.cheryme.top

[U102] JS：本地存储
来源：http://fni.gotoacloud.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ytv.yj20258.top

[U103] JS：定时器
来源：http://cbb.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qxo.jqgfzy.top

[U104] JS：防抖
来源：http://rwi.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pel.pycfn.com

[U105] JS：节流
来源：http://rlk.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rbj.zdqjudy.top

[U106] JS：日期格式化
来源：http://mei.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://los.hnqzz.top

[U107] JS：数字千分位
来源：http://tjk.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mbx.xuanzx.com

[U108] JS：随机整数
来源：http://pon.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rfz.nwbrower.top

[U109] JS：数组分组
来源：http://ykp.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://tvn.gogol.net.cn

[U110] JS：数组分块
来源：http://wtu.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lwi.hysaishi.cn

[U111] JS：对象转 Map
来源：http://aol.hfpthk.cn

new Map(Object.entries(obj))
来源：http://ods.yvedp.cn

[U112] JS：字符串补位
来源：http://eor.dianchejie.cn

"7".padStart(3, "0")
来源：http://txw.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://cjn.gotoacloud.top

s.replaceAll("a", "b")
来源：http://xen.uphjek.com

[U114] JS：JSON 深比较
来源：http://npi.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cds.zhixingplan.top

[U115] JS：生成 UUID
来源：http://jry.dianchejie.cn

crypto.randomUUID()
来源：http://wms.aibaodan.cn

[U116] JS：类型检查（JSDoc）
来源：http://wmc.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://zmv.snrcjt.cn

[U117] JS：单元测试
来源：http://bsi.xingfuxueyuan.xyz

npm i -D vitest;  npx vitest
来源：http://imy.zhongyouzk.top

[U118] JS：开发服务器
来源：http://jgj.sxryk.cn

npm i -D vite;  npx vite
来源：http://ugu.xylfe.cn

[U119] JS：生产构建
来源：http://xpt.dianchejie.cn

npx vite build
来源：http://hay.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://clj.sysykeji.top

import.meta.env.VITE_API_URL
来源：http://fas.jinyuanbaomall.cn

================================================================================
来源：http://cvp.tarul.cn

统计汇总
来源：http://ftw.tanke756.top

================================================================================
来源：http://exj.yvedp.cn

按语言统计（条）：
来源：http://fxk.jiagoushi.top

Python ......... 252
来源：http://ugt.cdnleiting.top

PHP ............ 252
来源：http://amy.haohaochexian.top

JavaScript ..... 252
来源：http://sny.xylfe.cn

TypeScript ..... 212
来源：http://hib.yvedp.cn

Java ........... 212
来源：http://buw.ybcxt.top

Go ............. 212
来源：http://gqc.vqdsnc.cn

Ruby ........... 212
来源：http://drq.jinyuanbaomall.cn

C# ............. 212
来源：http://zjw.yuanzhike.top

C .............. 30
来源：http://smz.ivvv.top

C++ ............ 30
来源：http://lyi.bbcook.cn

SQL ............ 90
来源：http://hik.uphjek.com

Bash ........... 80
来源：http://qib.yuanzhike.top

Kotlin ......... 15
来源：http://rbk.feifeiyinyue.top

Swift .......... 15
来源：http://zos.feifeiyinyue.top

Lua ............ 10
来源：http://kcg.feifeiyinyue.top

Perl ........... 10
来源：http://kwd.fzhhl.top

Scala .......... 10
来源：http://oiu.ywan-chungtsiang.top

------------------------------------
来源：http://jgn.ppjwa.cn

合计 ........... 2106 条
来源：http://xwy.tian-w.cn

按章节统计：
来源：http://kek.ydjk.org.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fjx.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jjv.epnwcf.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oka.vehdjk.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kio.cdnleiting.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aji.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yyg.zhiwuduotai.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nty.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qlw.svipenyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vgt.shzxlz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zce.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://efd.svipenyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nem.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zse.52xcode.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vxa.fzhhl.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nxi.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hku.tarul.cn

Q SQL 专题                              90
来源：http://krb.redwolf501.top

R Bash 专题                             80
来源：http://tme.ydzc1.top

S C / C++ 专题                          60
来源：http://gyy.cheryme.top

T 其他语言补充                          60
来源：http://gkz.meibo888.top

U 高频实用片段                         120
来源：http://imx.zhoulong.xyz

------------------------------------
来源：http://hew.jqgufenzy.top

合计                                  2106 条
来源：http://qtj.wangdashe.top

--------------------------------------------------------------------------------
来源：http://bsr.yueranfly.top

使用提醒
来源：http://fjy.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://yqw.gotoacloud.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bat.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rxj.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gqj.epnwcf.com

在旧版本上使用前请先确认语法支持情况。
来源：http://bqe.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://swv.hesvh.cn

—— 文件结束 ——
来源：http://kiw.ywan-chungtsiang.top

================================================================================
来源：http://nui.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://pmn.nanxinkj.top

Common Programming Examples Cheat Book
来源：http://fbi.shuidangran.top

================================================================================
来源：http://itj.tarul.cn

【收录内容】
来源：http://sqq.jinqigfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yql.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lhj.316326.xyz

SQL · Bash · C · C++
来源：http://auy.gzhubu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://aii.yuanzhike.top

【使用说明】
来源：http://uzf.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iqe.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rwq.daxiang520.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vwv.jlsjyb.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xaf.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kpl.quarkkingdee.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yrf.sxryk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wfp.52xcode.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iil.ivvv.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://grw.zdbjq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://clx.kuanghao11.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lzo.shanyushiyangtech.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mbr.bbcook.cn

【文件统计】
来源：http://ccg.aizwys.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zmc.hesvh.cn

--------------------------------------------------------------------------------
来源：http://sgs.yuxming.cn

目  录
来源：http://qoo.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://ndc.zycfv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lmg.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ujw.cqqwz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oat.shzxlz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jst.cqqwz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://knt.fktsv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://opr.guowangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ejk.ivvv.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tax.gogol.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tkj.nanxuanxn.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xey.52xcode.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tds.feifeiyinyue.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oii.shangyingyoupin.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bgd.zdqjudy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qla.yuanzhike.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ias.jqgufenzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://aca.yj20258888.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mma.yvedp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mxy.shangyingyoupin.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mbr.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bty.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uli.zhoulong.xyz

================================================================================
来源：http://loj.cdnleiting.top

A. 基础语法与类型
来源：http://dmm.cqqwz.cn

================================================================================
来源：http://uod.jyoumei.cn

[A01] Hello World
来源：http://vkj.feifeiyinyue.top

Py:   print("Hello, World!")
来源：http://rws.andypj.xyz

PHP:  echo "Hello, World!";
来源：http://odb.gogol.net.cn

JS:   console.log("Hello, World!");
来源：http://lyk.ppjwa.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rdo.kuanghao11.cn

Java: System.out.println("Hello, World!");
来源：http://wpm.smart0.xyz

Go:   fmt.Println("Hello, World!")
来源：http://amx.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://usb.fanxiaobao.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://zvh.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://fzh.svipenyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://txw.fanxiaobao.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://ato.zhaomingkeji.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://xle.316326.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qjq.uphjek.com

Java: String name = "Alex"; int age = 20;
来源：http://vbp.zhijiandao.cn

Go:   name := "Alex"; age := 20
来源：http://udb.yongpay.top

Ruby: name = "Alex"; age = 20
来源：http://wib.xuanzx.com

C#:   string name = "Alex"; int age = 20;
来源：http://usg.yangfankeji.com

[A03] 常量定义
来源：http://zqa.zhengqikj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qee.pengpengdd.cyou

PHP:  const PI = 3.14159;
来源：http://bvr.jianghu66.top

JS:   const PI = 3.14159;
来源：http://uke.zhiwuduotai.top

TS:   const PI: number = 3.14159;
来源：http://nse.jinqigufen.top

Java: static final double PI = 3.14159;
来源：http://clc.316326.xyz

Go:   const PI = 3.14159
来源：http://rxu.ydzc1.top

Ruby: PI = 3.14159
来源：http://cbi.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://jdn.hywenlv.cn

[A04] 判断变量类型
来源：http://pfy.fktsv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ono.zhijiandao.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xrs.xinyue.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gnw.sweek.top

TS:   typeof x; x instanceof Date
来源：http://bvt.hesvh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://auv.yvedp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://azr.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wmd.cqqwz.cn

C#:   x.GetType().Name; x is int
来源：http://jaa.nanxuanxn.top

[A05] 整数除法与取模
来源：http://okt.gaohongyu789.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://btp.tanke756.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ehu.zdqjudy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://frm.daria6918.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pvd.jlsjyb.cn

Java: 7 / 2; 7 % 2
来源：http://obv.yuanzhike.top

Go:   7 / 2; 7 % 2
来源：http://nsh.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://apt.zhaomingkeji.xyz

C#:   7 / 2; 7 % 2
来源：http://ikk.52xcode.cn

[A06] 字符串转数字
来源：http://ykf.pengpengdd.cyou

Py:   int("42"); float("3.14")
来源：http://kmg.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ivs.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dni.havefunace.top

TS:   parseInt("42", 10); Number("42")
来源：http://uqm.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zhr.jinqigufen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uuh.shanyushiyangtech.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gbj.gaohongyu789.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bmv.yangfankeji.com

[A07] 数字转字符串
来源：http://vzh.yangfankeji.com

Py:   str(42)
来源：http://lok.ppjwa.cn

PHP:  (string) 42; strval(42)
来源：http://ufm.chenjidiqi.icu

JS:   String(42); (42).toString()
来源：http://lvw.hcnkem.com

TS:   String(42)
来源：http://ycp.hnxiangtu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://xjf.ydzc1.top

Go:   strconv.Itoa(42)
来源：http://hsk.jianghu66.top

Ruby: 42.to_s
来源：http://ouq.zycfv.cn

C#:   42.ToString()
来源：http://uje.gogol.net.cn

[A08] 取整与四舍五入
来源：http://rro.wangshuangyany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eqb.mhx1999.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kyh.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vuv.zycfv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ysl.chenlongwang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jnw.nanxuanxn.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xbd.quarkkingdee.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qis.bbcook.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xrw.zhongyouzk.top

[A09] 绝对值与最大最小值
来源：http://wah.mhx1999.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pna.hywenlv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dyd.bbcook.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xnv.jyoumei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://clm.ywan-chungtsiang.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zkx.xingfuxueyuan.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xeb.jqgufenzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uzq.kuanghao11.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bvo.hcnkem.com

[A10] 生成随机数
来源：http://xnh.jlsjyb.cn

Py:   import random; random.randint(1, 100)
来源：http://jle.pycfn.com

PHP:  random_int(1, 100);
来源：http://lbd.tanke756.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tow.jinqigfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lgq.uphjek.com

Java: new Random().nextInt(100) + 1
来源：http://arw.9152youxi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ddg.feifeiyinyue.top

Ruby: rand(1..100)
来源：http://nam.bbcook.cn

C#:   new Random().Next(1, 101)
来源：http://sel.snrcjt.cn

[A11] 条件表达式（三元）
来源：http://rel.cheryme.top

Py:   "yes" if x > 0 else "no"
来源：http://gxq.cucudq.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hjq.shuidangran.top

JS:   x > 0 ? "yes" : "no"
来源：http://ieu.hysaishi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dki.yangfankeji.com

Java: x > 0 ? "yes" : "no"
来源：http://vgc.cqqwz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://abl.tian-w.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://paw.ppjwa.cn

C#:   x > 0 ? "yes" : "no"
来源：http://obi.tianlin.xyz

[A12] 字符串插值 / 格式化
来源：http://bpt.snrcjt.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lnq.snrcjt.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oyc.havefunace.top

JS:   `Hello, ${name}!`
来源：http://xhk.bjfxy.top

TS:   `Hello, ${name}!`
来源：http://sap.ivvv.top

Java: "Hello, %s!".formatted(name)
来源：http://crz.ctjpmb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dvl.yfazqb.com

Ruby: "Hello, #{name}!"
来源：http://pac.fktsv.cn

C#:   $"Hello, {name}!"
来源：http://mlj.nwbrower.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zco.andypj.xyz

Py:   "第一行\n第二行"
来源：http://txt.guannengcc.top

PHP:  "第一行\n第二行"
来源：http://rnl.xziqi.cn

JS:   "第一行\n第二行"
来源：http://cwj.hywenlv.cn

TS:   "第一行\n第二行"
来源：http://beu.tanke756.top

Java: "第一行\n第二行"
来源：http://mhm.sweek.top

Go:   "第一行\n第二行"
来源：http://zgv.xziqi.cn

Ruby: "第一行\n第二行"
来源：http://xeb.xingfuxueyuan.xyz

C#:   "第一行\n第二行"
来源：http://xfx.hfpthk.cn

[A14] 注释写法
来源：http://hha.xinyue.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://lwr.bjfxy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ntd.zycfv.cn

JS:   // 单行；/* 多行 */
来源：http://puw.iojbl.cn


<!-- 参考信息 -->