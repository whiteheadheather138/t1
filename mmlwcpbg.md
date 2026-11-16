代发 wailian999

[U85] JS：可选链
来源：http://nxq.zhaomingkeji.xyz

a?.b?.c
来源：http://tzn.gotoacloud.top

[U86] JS：空值合并
来源：http://hoc.gaohongyu789.top

a ?? b
来源：http://bxy.wangshuangyany.cn

[U87] JS：解构默认值
来源：http://cgc.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://wye.fzhhl.top

[U88] JS：对象展开合并
来源：http://rco.dashuyun.cn

{ ...a, ...b }
来源：http://jhg.gotoacloud.top

[U89] JS：数组去重
来源：http://apw.redwolf501.top

[...new Set(arr)]
来源：http://otn.ydzc1.top

[U90] JS：数字数组排序
来源：http://aoy.tianlin.xyz

[...arr].sort((a, b) => a - b)
来源：http://xlb.fanxiaobao.xyz

[U91] JS：对象键值遍历
来源：http://reh.quarkkingdee.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yqi.ydjk.org.cn

[U92] JS：深拷贝
来源：http://hiz.dianchejie.cn

structuredClone(obj)
来源：http://ctq.bbcook.cn

[U93] JS：模板字符串
来源：http://ppy.hammf.cn

`共 ${n} 条`
来源：http://kax.hnxiangtu.top

[U94] JS：箭头函数
来源：http://wlt.wangshuangyany.cn

const double = x => x * 2;
来源：http://avx.zhoulong.xyz

[U95] JS：Promise 包装
来源：http://hwv.yuxming.cn

new Promise((resolve, reject) => {})
来源：http://aku.hammf.cn

[U96] JS：async/await 与异常
来源：http://eik.tian-w.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qxa.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://bga.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://reo.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://hob.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ago.ehwqpu.com

[U99] JS：事件监听
来源：http://ajl.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://zet.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://qma.yongpay.top

document.querySelector(".item")
来源：http://zwj.tianlin.xyz

[U101] JS：classList 操作
来源：http://cat.meibo888.top

el.classList.toggle("active")
来源：http://lyb.birdmap.top

[U102] JS：本地存储
来源：http://bnf.hesvh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wkc.birdmap.top

[U103] JS：定时器
来源：http://znb.wangdashe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ehl.guowangkeji.top

[U104] JS：防抖
来源：http://aow.xylfe.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dby.gzhubu.top

[U105] JS：节流
来源：http://akb.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tud.pycfn.com

[U106] JS：日期格式化
来源：http://yby.zhiwuduotai.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cac.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://irq.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ihp.sjlbkw.cn

[U108] JS：随机整数
来源：http://opm.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ukb.yvedp.cn

[U109] JS：数组分组
来源：http://dda.feifeiyinyue.top

Object.groupBy(arr, x => x.type)
来源：http://szq.svipenyu.cn

[U110] JS：数组分块
来源：http://syw.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gqs.ydzc1.top

[U111] JS：对象转 Map
来源：http://jed.havefunace.top

new Map(Object.entries(obj))
来源：http://pls.0kj1m.cn

[U112] JS：字符串补位
来源：http://prs.vqdsnc.cn

"7".padStart(3, "0")
来源：http://ezd.fehbvm.com

[U113] JS：正则替换全部
来源：http://enn.havefunace.top

s.replaceAll("a", "b")
来源：http://nqk.zycfv.cn

[U114] JS：JSON 深比较
来源：http://axm.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://jaz.cashguo.top

[U115] JS：生成 UUID
来源：http://ibh.yueranfly.top

crypto.randomUUID()
来源：http://tdu.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://vzx.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://vbe.ybcxt.top

[U117] JS：单元测试
来源：http://slv.tarul.cn

npm i -D vitest;  npx vitest
来源：http://xlo.9152youxi.cn

[U118] JS：开发服务器
来源：http://yjo.hesvh.cn

npm i -D vite;  npx vite
来源：http://xbl.bjfxy.top

[U119] JS：生产构建
来源：http://gad.sweek.top

npx vite build
来源：http://jxo.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://wqr.yonumen.top

import.meta.env.VITE_API_URL
来源：http://qqt.c1oappe.top

================================================================================
来源：http://pxy.hfpthk.cn

统计汇总
来源：http://mnp.zhixingplan.top

================================================================================
来源：http://xie.zdqjudy.top

按语言统计（条）：
来源：http://ubr.shangyingyoupin.top

Python ......... 252
来源：http://ocu.sweek.top

PHP ............ 252
来源：http://gut.meibo888.top

JavaScript ..... 252
来源：http://dij.iojbl.cn

TypeScript ..... 212
来源：http://zie.zdbjq.cn

Java ........... 212
来源：http://xsd.xziqi.cn

Go ............. 212
来源：http://qqx.yj20258888.top

Ruby ........... 212
来源：http://box.andypj.xyz

C# ............. 212
来源：http://lrb.jlsjyb.cn

C .............. 30
来源：http://fze.daria6918.cn

C++ ............ 30
来源：http://flf.hammf.cn

SQL ............ 90
来源：http://wzm.xziqi.cn

Bash ........... 80
来源：http://add.yuxming.cn

Kotlin ......... 15
来源：http://abh.xziqi.cn

Swift .......... 15
来源：http://dux.wangshuangyany.cn

Lua ............ 10
来源：http://zqy.yangfankeji.com

Perl ........... 10
来源：http://svp.yangfankeji.com

Scala .......... 10
来源：http://prj.52xcode.cn

------------------------------------
来源：http://zhy.gaohongyu789.top

合计 ........... 2106 条
来源：http://uje.snrcjt.cn

按章节统计：
来源：http://iwu.redwolf501.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hsu.feifeiyinyue.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jjw.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dqh.cdnleiting.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rsc.yj202588.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iuo.hcnkem.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dqg.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rpz.fktsv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kgq.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xoq.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qsg.yj20258888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ccw.dianchejie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dfh.sweek.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ell.dashuyun.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bqm.52xcode.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qbk.xinyue.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eim.jinyuanbaomall.cn

Q SQL 专题                              90
来源：http://yla.zhengqikj.top

R Bash 专题                             80
来源：http://umb.bbcook.cn

S C / C++ 专题                          60
来源：http://zom.sweek.top

T 其他语言补充                          60
来源：http://cdm.hesvh.cn

U 高频实用片段                         120
来源：http://gmx.xinyue.icu

------------------------------------
来源：http://wld.cqqwz.cn

合计                                  2106 条
来源：http://gik.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://xra.zhoulong.xyz

使用提醒
来源：http://rip.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://xiw.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lev.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dwo.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rqi.jinqigfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ewh.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ycu.yj20258.top

—— 文件结束 ——
来源：http://fte.nanxinkj.top

================================================================================
来源：http://pfd.yj20258888.top

程序语言常见例子速查手册（2024 版）
来源：http://jcc.yangfankeji.com

Common Programming Examples Cheat Book
来源：http://zcx.jinqigufen.top

================================================================================
来源：http://xrr.hesvh.cn

【收录内容】
来源：http://wxc.gogol.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://afh.meibo888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://keh.epnwcf.com

SQL · Bash · C · C++
来源：http://yzj.c1oappe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fex.zhiwuduotai.top

【使用说明】
来源：http://nnv.zhiwuduotai.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://txp.gzhubu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cpz.hesvh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sdq.quarkkingdee.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wwr.fehbvm.com

Bash:  Shell         C:     C             C++:   C++
来源：http://vkp.andypj.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://opn.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jhl.uphjek.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yld.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wbl.zhijiandao.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cdx.xinyue.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://riv.yuanzhike.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vha.guowangkeji.top

【文件统计】
来源：http://prv.tanke756.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bex.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://dcu.cdnleiting.top

目  录
来源：http://sfk.fengsongda.top

--------------------------------------------------------------------------------
来源：http://zlp.guannengcc.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ybk.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jgu.ywan-chungtsiang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ntv.yonumen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mjy.yonumen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ywm.shuidangran.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://plz.havefunace.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kwd.shanyushiyangtech.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kgq.zdbjq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dnc.nwbrower.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rvp.ydzc1.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bql.bjfxy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kng.yueranfly.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jro.snrcjt.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pkg.nwbrower.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sqq.yuanzhike.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dvf.andypj.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uau.xuanzx.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://zyo.cdnleiting.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fdf.hywenlv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ptn.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jsm.hongshengwenyu.top

================================================================================
来源：http://sbc.zhoulong.xyz

A. 基础语法与类型
来源：http://bms.xinyue.icu

================================================================================
来源：http://uay.hnxiangtu.top

[A01] Hello World
来源：http://oyb.bjfxy.top

Py:   print("Hello, World!")
来源：http://oog.meibo888.top

PHP:  echo "Hello, World!";
来源：http://grx.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://scr.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://juu.meibo888.top

Java: System.out.println("Hello, World!");
来源：http://gqq.ydzc1.top

Go:   fmt.Println("Hello, World!")
来源：http://xcx.fzhhl.top

Ruby: puts "Hello, World!"
来源：http://goy.xylfe.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gib.jqgufenzy.top

[A02] 变量声明与赋值
来源：http://hnq.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qiy.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fpn.shuidangran.top

JS:   let name = "Alex"; const age = 20;
来源：http://kfc.fehbvm.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ixq.cdnleiting.top

Java: String name = "Alex"; int age = 20;
来源：http://dfw.yueranfly.top

Go:   name := "Alex"; age := 20
来源：http://fhp.fanxiaobao.xyz

Ruby: name = "Alex"; age = 20
来源：http://fmv.cqqwz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wba.nwbrower.top

[A03] 常量定义
来源：http://ipt.yvedp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aos.hnxiangtu.top

PHP:  const PI = 3.14159;
来源：http://ins.iojbl.cn

JS:   const PI = 3.14159;
来源：http://gqk.c1oappe.top

TS:   const PI: number = 3.14159;
来源：http://tmg.snrcjt.cn

Java: static final double PI = 3.14159;
来源：http://yzs.ydjk.org.cn

Go:   const PI = 3.14159
来源：http://bzy.cucudq.cn

Ruby: PI = 3.14159
来源：http://sfp.shuidangran.top

C#:   const double PI = 3.14159;
来源：http://gxp.yuxming.cn

[A04] 判断变量类型
来源：http://njt.jinqigufen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mii.fehbvm.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nac.yuxming.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vkw.ehwqpu.com

TS:   typeof x; x instanceof Date
来源：http://tsx.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://agy.tanke756.top

Go:   reflect.TypeOf(x).Name()
来源：http://qtn.svipenyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://usv.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://jqe.xziqi.cn

[A05] 整数除法与取模
来源：http://klh.hesvh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://duf.zdqjudy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xmf.xuetiantiany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hdu.fehbvm.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://svl.jlsjyb.cn

Java: 7 / 2; 7 % 2
来源：http://nog.0kj1m.cn

Go:   7 / 2; 7 % 2
来源：http://wde.shanyushiyangtech.top

Ruby: 7 / 2; 7 % 2
来源：http://emo.xuetiantiany.cn

C#:   7 / 2; 7 % 2
来源：http://zwr.52xcode.cn

[A06] 字符串转数字
来源：http://fut.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://iat.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vei.bbcook.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mfe.cheryme.top

TS:   parseInt("42", 10); Number("42")
来源：http://wco.tarul.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mbz.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kel.zdqjudy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wuq.snrcjt.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zwr.yueranfly.top

[A07] 数字转字符串
来源：http://otu.wangdashe.top

Py:   str(42)
来源：http://bos.andypj.xyz

PHP:  (string) 42; strval(42)
来源：http://fxc.svipenyu.cn

JS:   String(42); (42).toString()
来源：http://nac.uphjek.com

TS:   String(42)
来源：http://mtf.sysykeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vqq.cdnleiting.top

Go:   strconv.Itoa(42)
来源：http://uov.hywenlv.cn

Ruby: 42.to_s
来源：http://stm.iojbl.cn

C#:   42.ToString()
来源：http://htb.meibo888.top

[A08] 取整与四舍五入
来源：http://mkg.xylfe.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yci.vqdsnc.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lsp.jianghu66.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zhd.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lyq.gotoacloud.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lof.andypj.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ggy.chenjidiqi.icu

Ruby: 3.567.round(2); 3.9.floor
来源：http://yjm.cashguo.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xgl.snrcjt.cn

[A09] 绝对值与最大最小值
来源：http://vwx.xingfuxueyuan.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hwf.nwbrower.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zkj.sufxvd.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qlx.daxiang520.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oya.fehbvm.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://diq.kuanghao11.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://umj.yj202588.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nnz.yueranfly.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oid.jianghu66.top

[A10] 生成随机数
来源：http://cqf.aibaodan.cn

Py:   import random; random.randint(1, 100)
来源：http://unz.iojbl.cn

PHP:  random_int(1, 100);
来源：http://kuv.zdqjudy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mth.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://agh.shanyushiyangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://ptq.sjlbkw.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://swo.nanxinkj.top

Ruby: rand(1..100)
来源：http://xxi.zhixingplan.top

C#:   new Random().Next(1, 101)
来源：http://swl.pengpengdd.cyou

[A11] 条件表达式（三元）
来源：http://jjv.zhixingplan.top

Py:   "yes" if x > 0 else "no"
来源：http://wba.shuidangran.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ybs.jinqigfzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://jyg.fzhhl.top

TS:   x > 0 ? "yes" : "no"
来源：http://saf.hysaishi.cn

Java: x > 0 ? "yes" : "no"
来源：http://uza.c1oappe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tmj.yfazqb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://wtg.smart0.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://jyp.hywenlv.cn

[A12] 字符串插值 / 格式化
来源：http://xxc.jiagoushi.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jbo.daria6918.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://upk.epnwcf.com

JS:   `Hello, ${name}!`
来源：http://kfb.yangfankeji.com

TS:   `Hello, ${name}!`
来源：http://bqh.mhx1999.top

Java: "Hello, %s!".formatted(name)
来源：http://jgf.zhixingplan.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xyl.gaohongyu789.top

Ruby: "Hello, #{name}!"
来源：http://bhs.yueranfly.top

C#:   $"Hello, {name}!"
来源：http://flo.yj202588.top

[A13] 多行字符串（练习 \n 转义）
来源：http://atz.ybcxt.top

Py:   "第一行\n第二行"
来源：http://anv.zdbjq.cn

PHP:  "第一行\n第二行"
来源：http://vhd.wangshuangyany.cn

JS:   "第一行\n第二行"
来源：http://jsx.kuanghao11.cn

TS:   "第一行\n第二行"
来源：http://apr.yuxming.cn

Java: "第一行\n第二行"
来源：http://byg.yj20258.top

Go:   "第一行\n第二行"
来源：http://xqh.gaohongyu789.top

Ruby: "第一行\n第二行"
来源：http://qxo.vehdjk.com

C#:   "第一行\n第二行"
来源：http://fst.yuanzhike.top

[A14] 注释写法
来源：http://rnm.yanxiufei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zmm.guannengcc.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vom.shanyushiyangtech.top

JS:   // 单行；/* 多行 */
来源：http://nij.cdnleiting.top


<!-- 参考信息 -->