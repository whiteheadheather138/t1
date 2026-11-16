代发 wailian999

[U85] JS：可选链
来源：http://tbg.guannengcc.top

a?.b?.c
来源：http://ahs.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://oyg.sufxvd.cn

a ?? b
来源：http://crb.cashguo.top

[U87] JS：解构默认值
来源：http://jlv.fktsv.cn

const { a = 1, b = 2 } = obj;
来源：http://ald.yuxming.cn

[U88] JS：对象展开合并
来源：http://xaa.cashguo.top

{ ...a, ...b }
来源：http://uiq.zhongyouzk.top

[U89] JS：数组去重
来源：http://zso.hesvh.cn

[...new Set(arr)]
来源：http://uce.gzhubu.top

[U90] JS：数字数组排序
来源：http://ljy.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://axn.cashguo.top

[U91] JS：对象键值遍历
来源：http://cxa.guannengcc.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cuh.gzhubu.top

[U92] JS：深拷贝
来源：http://mxc.daxiang520.top

structuredClone(obj)
来源：http://zru.pycfn.com

[U93] JS：模板字符串
来源：http://tnh.haohaochexian.top

`共 ${n} 条`
来源：http://gnv.aibaodan.cn

[U94] JS：箭头函数
来源：http://dlh.jinyuanbaomall.cn

const double = x => x * 2;
来源：http://zyu.pycfn.com

[U95] JS：Promise 包装
来源：http://lil.xuanzx.com

new Promise((resolve, reject) => {})
来源：http://nio.chenzaomai.com

[U96] JS：async/await 与异常
来源：http://yjd.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hgm.bjfxy.top

[U97] JS：并发请求
来源：http://uho.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gja.daxiang520.top

[U98] JS：fetch 带 JSON
来源：http://qvl.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vnl.cucudq.cn

[U99] JS：事件监听
来源：http://uxe.chenjidiqi.icu

el.addEventListener("click", e => {})
来源：http://nuk.hcnkem.com

[U100] JS：DOM 查询
来源：http://rir.shanyushiyangtech.top

document.querySelector(".item")
来源：http://poe.jianghu66.top

[U101] JS：classList 操作
来源：http://zbi.yangfankeji.com

el.classList.toggle("active")
来源：http://bgu.hammf.cn

[U102] JS：本地存储
来源：http://ujc.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xcq.gzhubu.top

[U103] JS：定时器
来源：http://fvm.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bur.cheryme.top

[U104] JS：防抖
来源：http://oqd.jyoumei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xce.daria6918.cn

[U105] JS：节流
来源：http://bea.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://apw.hfpthk.cn

[U106] JS：日期格式化
来源：http://peg.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vuw.ehwqpu.com

[U107] JS：数字千分位
来源：http://lbh.hysaishi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vbj.zycfv.cn

[U108] JS：随机整数
来源：http://hqe.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ljn.smart0.xyz

[U109] JS：数组分组
来源：http://vmg.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://nop.feifeiyinyue.top

[U110] JS：数组分块
来源：http://qpp.cucudq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qnn.yj202588.top

[U111] JS：对象转 Map
来源：http://bdp.redwolf501.top

new Map(Object.entries(obj))
来源：http://sjo.iojbl.cn

[U112] JS：字符串补位
来源：http://doo.yuanzhike.top

"7".padStart(3, "0")
来源：http://tnw.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://vda.andypj.xyz

s.replaceAll("a", "b")
来源：http://wyn.jlsjyb.cn

[U114] JS：JSON 深比较
来源：http://omc.yj20258.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zfq.cucudq.cn

[U115] JS：生成 UUID
来源：http://atb.xuanzx.com

crypto.randomUUID()
来源：http://cjp.yanxiufei.cn

[U116] JS：类型检查（JSDoc）
来源：http://utw.hnxiangtu.top

/** @param {string} name */ function f(name) {}
来源：http://nst.jyoumei.cn

[U117] JS：单元测试
来源：http://osv.nanxuanxn.top

npm i -D vitest;  npx vitest
来源：http://phi.guowangkeji.top

[U118] JS：开发服务器
来源：http://wuv.sysykeji.top

npm i -D vite;  npx vite
来源：http://uur.meibo888.top

[U119] JS：生产构建
来源：http://mbn.gogol.net.cn

npx vite build
来源：http://dsb.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://lvm.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://zws.ydjk.org.cn

================================================================================
来源：http://lyb.fktsv.cn

统计汇总
来源：http://bhv.tianlin.xyz

================================================================================
来源：http://xcq.xinyue.icu

按语言统计（条）：
来源：http://dco.0kj1m.cn

Python ......... 252
来源：http://rsn.tianlin.xyz

PHP ............ 252
来源：http://wwy.quarkkingdee.top

JavaScript ..... 252
来源：http://ylz.cucudq.cn

TypeScript ..... 212
来源：http://lre.jlsjyb.cn

Java ........... 212
来源：http://agi.jiagoushi.top

Go ............. 212
来源：http://wov.nanxuanxn.top

Ruby ........... 212
来源：http://rii.pycfn.com

C# ............. 212
来源：http://fcy.cqqwz.cn

C .............. 30
来源：http://jcf.bbcook.cn

C++ ............ 30
来源：http://mhq.hywenlv.cn

SQL ............ 90
来源：http://esl.sufxvd.cn

Bash ........... 80
来源：http://orq.mhx1999.top

Kotlin ......... 15
来源：http://cnr.9152youxi.cn

Swift .......... 15
来源：http://efa.xuanzx.com

Lua ............ 10
来源：http://gwl.sufxvd.cn

Perl ........... 10
来源：http://yzj.jianghu66.top

Scala .......... 10
来源：http://tmw.sxryk.cn

------------------------------------
来源：http://pfx.ybcxt.top

合计 ........... 2106 条
来源：http://coo.xziqi.cn

按章节统计：
来源：http://efc.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hbt.xingfuxueyuan.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nrc.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gea.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dma.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wir.sysykeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://niy.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mhb.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oty.sweek.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lqs.yuxming.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qpj.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://isj.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ckd.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://riu.bbcook.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fml.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nhr.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dsa.zhiwuduotai.top

Q SQL 专题                              90
来源：http://sna.gogol.net.cn

R Bash 专题                             80
来源：http://xxe.epnwcf.com

S C / C++ 专题                          60
来源：http://fzu.jqgufenzy.top

T 其他语言补充                          60
来源：http://wmp.zhiwuduotai.top

U 高频实用片段                         120
来源：http://ddf.gaohongyu789.top

------------------------------------
来源：http://hur.sjlbkw.cn

合计                                  2106 条
来源：http://hci.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://evp.jianghu66.top

使用提醒
来源：http://tdu.hcnkem.com

--------------------------------------------------------------------------------
来源：http://zzr.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nej.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ckp.fehbvm.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mwz.zhongyouzk.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pew.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xvj.xuetiantiany.cn

—— 文件结束 ——
来源：http://dpt.zhongyouzk.top

================================================================================
来源：http://ivl.yuxming.cn

程序语言常见例子速查手册（2024 版）
来源：http://bsd.mhx1999.top

Common Programming Examples Cheat Book
来源：http://gan.hesvh.cn

================================================================================
来源：http://wyv.tian-w.cn

【收录内容】
来源：http://eav.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://obh.bbcook.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vft.hnxiangtu.top

SQL · Bash · C · C++
来源：http://hmy.cheryme.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rbn.sjlbkw.cn

【使用说明】
来源：http://faq.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mbl.shangyingyoupin.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tah.andypj.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://aae.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qqp.ppjwa.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dss.zhengqikj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nsw.hnxiangtu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://len.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mbz.iojbl.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xof.zhixingplan.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nyp.xuetiantiany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yfg.chenzaomai.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qgt.ivvv.top

【文件统计】
来源：http://ltu.zhongyouzk.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sos.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://hic.xylfe.cn

目  录
来源：http://zig.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://jha.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yeh.52xcode.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tvr.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dxi.zhongyouzk.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sqy.redwolf501.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ggm.guowangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wrw.jqgufenzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://thn.0kj1m.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wqv.zhiwuduotai.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kmu.dianchejie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://llx.shangyingyoupin.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iwx.xuetiantiany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hcp.dashuyun.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zvj.pycfn.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dgv.meibo888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ozh.daria6918.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xum.gogol.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://roe.zycfv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yvq.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hps.xuanzx.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wom.shanyushiyangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ozm.9152youxi.cn

================================================================================
来源：http://lam.dashuyun.cn

A. 基础语法与类型
来源：http://okl.zdbjq.cn

================================================================================
来源：http://wzc.xuetiantiany.cn

[A01] Hello World
来源：http://yus.pycfn.com

Py:   print("Hello, World!")
来源：http://ecl.tanke756.top

PHP:  echo "Hello, World!";
来源：http://cor.hnxiangtu.top

JS:   console.log("Hello, World!");
来源：http://fxl.vqdsnc.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wcx.ivvv.top

Java: System.out.println("Hello, World!");
来源：http://ecz.c1oappe.top

Go:   fmt.Println("Hello, World!")
来源：http://idp.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://mfd.chenjidiqi.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://yzt.hywenlv.cn

[A02] 变量声明与赋值
来源：http://lyg.ydzc1.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://asd.yuxming.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ujz.shuidangran.top

JS:   let name = "Alex"; const age = 20;
来源：http://dzn.snrcjt.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hll.yvedp.cn

Java: String name = "Alex"; int age = 20;
来源：http://hwv.cdnleiting.top

Go:   name := "Alex"; age := 20
来源：http://lat.ydzc1.top

Ruby: name = "Alex"; age = 20
来源：http://wzb.xingfuxueyuan.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://bcj.yuxming.cn

[A03] 常量定义
来源：http://xnz.nanxinkj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vla.kuanghao11.cn

PHP:  const PI = 3.14159;
来源：http://dnp.xuanzx.com

JS:   const PI = 3.14159;
来源：http://qoj.xingfuxueyuan.xyz

TS:   const PI: number = 3.14159;
来源：http://sen.nanxuanxn.top

Java: static final double PI = 3.14159;
来源：http://zzv.hysaishi.cn

Go:   const PI = 3.14159
来源：http://pkc.zdqjudy.top

Ruby: PI = 3.14159
来源：http://nln.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://hib.yj20258.top

[A04] 判断变量类型
来源：http://tlj.meibo888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://exl.zhongyouzk.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ztw.shanyushiyangtech.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lws.c1oappe.top

TS:   typeof x; x instanceof Date
来源：http://jzh.jinqigfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kqy.yfazqb.com

Go:   reflect.TypeOf(x).Name()
来源：http://qfl.shanyushiyangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ave.tarul.cn

C#:   x.GetType().Name; x is int
来源：http://fzh.shanyushiyangtech.top

[A05] 整数除法与取模
来源：http://ekj.wangshuangyany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bgj.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://shu.hongshengwenyu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wdt.snrcjt.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vtt.zhengqikj.top

Java: 7 / 2; 7 % 2
来源：http://owl.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://ipn.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://vfn.tarul.cn

C#:   7 / 2; 7 % 2
来源：http://tvb.jianghu66.top

[A06] 字符串转数字
来源：http://auy.gaohongyu789.top

Py:   int("42"); float("3.14")
来源：http://anb.sufxvd.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xng.jinyuanbaomall.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xjh.hysaishi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bfb.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://psq.xziqi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oei.jianghu66.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qst.hnxiangtu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fub.ctjpmb.com

[A07] 数字转字符串
来源：http://iom.zhengqikj.top

Py:   str(42)
来源：http://gwu.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://djz.nwbrower.top

JS:   String(42); (42).toString()
来源：http://ejh.chenzaomai.com

TS:   String(42)
来源：http://tby.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://htq.tanke756.top

Go:   strconv.Itoa(42)
来源：http://jpg.wangdashe.top

Ruby: 42.to_s
来源：http://zhg.jianghu66.top

C#:   42.ToString()
来源：http://fon.fengsongda.top

[A08] 取整与四舍五入
来源：http://bce.bjfxy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bgx.ivvv.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://goj.tarul.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bif.ivvv.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ymn.wangdashe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hbi.tanke756.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xew.yfazqb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://tkm.vqdsnc.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rqa.zdqjudy.top

[A09] 绝对值与最大最小值
来源：http://ges.jianghu66.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://old.svipenyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xns.pycfn.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oer.zhiwuduotai.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://odt.yueranfly.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qrz.hongshengwenyu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fja.jianghu66.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gfp.aibaodan.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hbi.vehdjk.com

[A10] 生成随机数
来源：http://erb.cashguo.top

Py:   import random; random.randint(1, 100)
来源：http://dhi.0kj1m.cn

PHP:  random_int(1, 100);
来源：http://pkw.zdqjudy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kia.yongpay.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://awf.aizwys.cn

Java: new Random().nextInt(100) + 1
来源：http://kuu.cucudq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aes.hammf.cn

Ruby: rand(1..100)
来源：http://dro.iojbl.cn

C#:   new Random().Next(1, 101)
来源：http://fqt.ppjwa.cn

[A11] 条件表达式（三元）
来源：http://sav.wangshuangyany.cn

Py:   "yes" if x > 0 else "no"
来源：http://byf.haohaochexian.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://enu.dashuyun.cn

JS:   x > 0 ? "yes" : "no"
来源：http://olg.cdnleiting.top

TS:   x > 0 ? "yes" : "no"
来源：http://bjq.yj20258888.top

Java: x > 0 ? "yes" : "no"
来源：http://mjn.guowangkeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jwl.xuanzx.com

Ruby: x > 0 ? "yes" : "no"
来源：http://uus.zhixingplan.top

C#:   x > 0 ? "yes" : "no"
来源：http://jnj.ydjk.org.cn

[A12] 字符串插值 / 格式化
来源：http://nik.dianchejie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bnv.hywenlv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://afr.redwolf501.top

JS:   `Hello, ${name}!`
来源：http://dbg.0kj1m.cn

TS:   `Hello, ${name}!`
来源：http://ddb.cheryme.top

Java: "Hello, %s!".formatted(name)
来源：http://syh.316326.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mro.jinghuilouyu.cn

Ruby: "Hello, #{name}!"
来源：http://ncu.xuetiantiany.cn

C#:   $"Hello, {name}!"
来源：http://rcl.mhx1999.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jsu.bjfxy.top

Py:   "第一行\n第二行"
来源：http://aln.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://ubm.sysykeji.top

JS:   "第一行\n第二行"
来源：http://paf.shanyushiyangtech.top

TS:   "第一行\n第二行"
来源：http://iwd.yuanzhike.top

Java: "第一行\n第二行"
来源：http://mcw.smart0.xyz

Go:   "第一行\n第二行"
来源：http://hps.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://aqa.tanke756.top

C#:   "第一行\n第二行"
来源：http://sll.hfpthk.cn

[A14] 注释写法
来源：http://eph.gogol.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://deb.tanke756.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zjt.hnxiangtu.top

JS:   // 单行；/* 多行 */
来源：http://qag.fehbvm.com


<!-- 参考信息 -->