代发 wailian999

[U89] JS：数组去重
来源：http://hml.shzxlz.cn

[...new Set(arr)]
来源：http://ovr.zycfv.cn

[U90] JS：数字数组排序
来源：http://ztu.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://svl.zhongyouzk.top

[U91] JS：对象键值遍历
来源：http://eky.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jnq.zhoulong.xyz

[U92] JS：深拷贝
来源：http://ddf.xinyue.icu

structuredClone(obj)
来源：http://wiy.mhx1999.top

[U93] JS：模板字符串
来源：http://azc.redwolf501.top

`共 ${n} 条`
来源：http://vcg.yuxming.cn

[U94] JS：箭头函数
来源：http://wxp.9152youxi.cn

const double = x => x * 2;
来源：http://zqm.ehwqpu.com

[U95] JS：Promise 包装
来源：http://rem.jqgufenzy.top

new Promise((resolve, reject) => {})
来源：http://djj.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://jtp.yongpay.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gzg.ppjwa.cn

[U97] JS：并发请求
来源：http://ksm.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rao.c1oappe.top

[U98] JS：fetch 带 JSON
来源：http://rsi.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ecz.zdqjudy.top

[U99] JS：事件监听
来源：http://ask.ydzc1.top

el.addEventListener("click", e => {})
来源：http://nam.jianghu66.top

[U100] JS：DOM 查询
来源：http://bij.pycfn.com

document.querySelector(".item")
来源：http://owu.tianlin.xyz

[U101] JS：classList 操作
来源：http://qzm.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://ftv.svipenyu.cn

[U102] JS：本地存储
来源：http://txt.yuanzhike.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://orz.chenzaomai.com

[U103] JS：定时器
来源：http://tvo.ybcxt.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ruc.shzxlz.cn

[U104] JS：防抖
来源：http://uml.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wde.pengpengdd.cyou

[U105] JS：节流
来源：http://ruw.yj20258.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dzd.jiagoushi.top

[U106] JS：日期格式化
来源：http://xuy.birdmap.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fak.zhijiandao.cn

[U107] JS：数字千分位
来源：http://jgd.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zyh.ydjk.org.cn

[U108] JS：随机整数
来源：http://poi.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://axk.guannengcc.top

[U109] JS：数组分组
来源：http://gey.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://ubg.pycfn.com

[U110] JS：数组分块
来源：http://nor.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uyy.zhiwuduotai.top

[U111] JS：对象转 Map
来源：http://ghn.yuanzhike.top

new Map(Object.entries(obj))
来源：http://lbj.nanxinkj.top

[U112] JS：字符串补位
来源：http://eeo.fehbvm.com

"7".padStart(3, "0")
来源：http://ytw.yvedp.cn

[U113] JS：正则替换全部
来源：http://oer.daxiang520.top

s.replaceAll("a", "b")
来源：http://uzg.sxryk.cn

[U114] JS：JSON 深比较
来源：http://gwi.zdbjq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ihx.nanxinkj.top

[U115] JS：生成 UUID
来源：http://rtu.bjfxy.top

crypto.randomUUID()
来源：http://cxf.hammf.cn

[U116] JS：类型检查（JSDoc）
来源：http://hrm.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://tpc.fzhhl.top

[U117] JS：单元测试
来源：http://kgx.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://mmr.yj202588.top

[U118] JS：开发服务器
来源：http://kke.yvedp.cn

npm i -D vite;  npx vite
来源：http://atw.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://omb.sjlbkw.cn

npx vite build
来源：http://sab.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://gga.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://nhs.xinyue.icu

================================================================================
来源：http://vcj.yj202588.top

统计汇总
来源：http://qwz.cheryme.top

================================================================================
来源：http://xqz.havefunace.top

按语言统计（条）：
来源：http://xpv.yongpay.top

Python ......... 252
来源：http://kab.fktsv.cn

PHP ............ 252
来源：http://kaq.hongshengwenyu.top

JavaScript ..... 252
来源：http://mon.dianchejie.cn

TypeScript ..... 212
来源：http://rwg.yj20258888.top

Java ........... 212
来源：http://zao.hammf.cn

Go ............. 212
来源：http://lgd.daxiang520.top

Ruby ........... 212
来源：http://pot.pycfn.com

C# ............. 212
来源：http://vdj.shanyushiyangtech.top

C .............. 30
来源：http://hrc.316326.xyz

C++ ............ 30
来源：http://wyq.chenzaomai.com

SQL ............ 90
来源：http://xlz.shangyingyoupin.top

Bash ........... 80
来源：http://uzs.jinqigufen.top

Kotlin ......... 15
来源：http://fwr.ydjk.org.cn

Swift .......... 15
来源：http://cab.uphjek.com

Lua ............ 10
来源：http://ujd.daria6918.cn

Perl ........... 10
来源：http://vcm.jinghuilouyu.cn

Scala .......... 10
来源：http://exb.xziqi.cn

------------------------------------
来源：http://nlr.vehdjk.com

合计 ........... 2106 条
来源：http://ivq.zdqjudy.top

按章节统计：
来源：http://slx.9152youxi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ryx.fengsongda.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nxi.9152youxi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eon.yongpay.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cky.kuanghao11.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ucs.vehdjk.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qqs.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rnp.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ith.cqqwz.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yzg.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ays.ybcxt.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://puk.guowangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dlo.havefunace.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://moh.shzxlz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eta.jinqigfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aej.ehwqpu.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qlt.chenzaomai.com

Q SQL 专题                              90
来源：http://qci.fzhhl.top

R Bash 专题                             80
来源：http://uhc.fehbvm.com

S C / C++ 专题                          60
来源：http://ndt.jianghu66.top

T 其他语言补充                          60
来源：http://jwt.hfpthk.cn

U 高频实用片段                         120
来源：http://lph.ctjpmb.com

------------------------------------
来源：http://eok.zhongyouzk.top

合计                                  2106 条
来源：http://rdj.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://ika.gogol.net.cn

使用提醒
来源：http://edh.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://yyr.zhoulong.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nmk.cdnleiting.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aeh.sufxvd.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://erb.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uwa.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lmt.xziqi.cn

—— 文件结束 ——
来源：http://tow.ehwqpu.com

================================================================================
来源：http://iyt.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://gvg.ydjk.org.cn

Common Programming Examples Cheat Book
来源：http://ghc.redwolf501.top

================================================================================
来源：http://upc.wangdashe.top

【收录内容】
来源：http://kyy.hywenlv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yta.snrcjt.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kbd.xinyue.icu

SQL · Bash · C · C++
来源：http://huh.zhaomingkeji.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pjq.zhixingplan.top

【使用说明】
来源：http://lsn.fengsongda.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ctt.ctjpmb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vqs.andypj.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kou.yangfankeji.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bmm.zhaomingkeji.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://cqu.bjfxy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uel.zhixingplan.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xvv.yangfankeji.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hpk.ehwqpu.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lpg.gaohongyu789.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://crl.tianlin.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yjm.yfazqb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bzx.andypj.xyz

【文件统计】
来源：http://dqx.yj20258888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jor.smart0.xyz

--------------------------------------------------------------------------------
来源：http://vpk.yj20258.top

目  录
来源：http://nnl.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://ccg.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lur.wangshuangyany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tuz.zycfv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nxp.fzhhl.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jre.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ect.sufxvd.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zrq.ivvv.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jvo.yj202588.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nzr.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tih.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zuv.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://czq.zhengqikj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://abb.hfpthk.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mlg.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://weo.fehbvm.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://axe.shuidangran.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wzl.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://azq.meibo888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kmf.xziqi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://svp.ywan-chungtsiang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qkt.shzxlz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jct.zhaomingkeji.xyz

================================================================================
来源：http://rhs.yueranfly.top

A. 基础语法与类型
来源：http://veg.daxiang520.top

================================================================================
来源：http://tia.cashguo.top

[A01] Hello World
来源：http://hga.chenzaomai.com

Py:   print("Hello, World!")
来源：http://xaf.chenzaomai.com

PHP:  echo "Hello, World!";
来源：http://xbo.zdbjq.cn

JS:   console.log("Hello, World!");
来源：http://mib.hnxiangtu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://elp.xziqi.cn

Java: System.out.println("Hello, World!");
来源：http://ynv.yongpay.top

Go:   fmt.Println("Hello, World!")
来源：http://hqa.wangdashe.top

Ruby: puts "Hello, World!"
来源：http://afq.tianlin.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://zlo.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://bzx.daxiang520.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ekq.yanxiufei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://inj.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://yae.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oeu.mhx1999.top

Java: String name = "Alex"; int age = 20;
来源：http://xul.cheryme.top

Go:   name := "Alex"; age := 20
来源：http://icg.fktsv.cn

Ruby: name = "Alex"; age = 20
来源：http://blk.hfpthk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vpa.guowangkeji.top

[A03] 常量定义
来源：http://fds.yj20258888.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sbl.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://obx.iojbl.cn

JS:   const PI = 3.14159;
来源：http://ehw.cucudq.cn

TS:   const PI: number = 3.14159;
来源：http://yer.jinqigfzy.top

Java: static final double PI = 3.14159;
来源：http://iri.yj20258888.top

Go:   const PI = 3.14159
来源：http://van.nwbrower.top

Ruby: PI = 3.14159
来源：http://jwr.yfazqb.com

C#:   const double PI = 3.14159;
来源：http://axc.hnxiangtu.top

[A04] 判断变量类型
来源：http://bhu.ywan-chungtsiang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://udv.yueranfly.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pbv.zhiwuduotai.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fsn.uphjek.com

TS:   typeof x; x instanceof Date
来源：http://wvz.ydzc1.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vci.ydjk.org.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pcx.bjfxy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dsw.jinyuanbaomall.cn

C#:   x.GetType().Name; x is int
来源：http://awl.yanxiufei.cn

[A05] 整数除法与取模
来源：http://odf.ydzc1.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iqg.smart0.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://lih.sysykeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qar.jinqigfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lvt.zhengqikj.top

Java: 7 / 2; 7 % 2
来源：http://ush.chenjidiqi.icu

Go:   7 / 2; 7 % 2
来源：http://mib.zhongyouzk.top

Ruby: 7 / 2; 7 % 2
来源：http://cdf.zhixingplan.top

C#:   7 / 2; 7 % 2
来源：http://rxw.shanyushiyangtech.top

[A06] 字符串转数字
来源：http://cju.zhengqikj.top

Py:   int("42"); float("3.14")
来源：http://rbw.sysykeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://juz.yongpay.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bgr.hywenlv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pws.nanxuanxn.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://anf.zycfv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pbf.sweek.top

Ruby: "42".to_i; "3.14".to_f
来源：http://erk.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ndd.svipenyu.cn

[A07] 数字转字符串
来源：http://xww.tanke756.top

Py:   str(42)
来源：http://zzl.pycfn.com

PHP:  (string) 42; strval(42)
来源：http://ctq.birdmap.top

JS:   String(42); (42).toString()
来源：http://zef.zdbjq.cn

TS:   String(42)
来源：http://fad.feifeiyinyue.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mcr.pengpengdd.cyou

Go:   strconv.Itoa(42)
来源：http://vcz.yonumen.top

Ruby: 42.to_s
来源：http://wmk.nwbrower.top

C#:   42.ToString()
来源：http://yqr.hongshengwenyu.top

[A08] 取整与四舍五入
来源：http://nzg.snrcjt.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gay.jianghu66.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bsp.zdqjudy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xlw.wangdashe.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bpd.hywenlv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ymi.iojbl.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rba.tarul.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ihi.snrcjt.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://znb.fengsongda.top

[A09] 绝对值与最大最小值
来源：http://twm.zhiwuduotai.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hmi.dianchejie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ypl.yj20258888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qje.hnxiangtu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tbh.zdqjudy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ugy.yj20258.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zwi.hysaishi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qxn.vqdsnc.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://srr.snrcjt.cn

[A10] 生成随机数
来源：http://miw.hnxiangtu.top

Py:   import random; random.randint(1, 100)
来源：http://nue.gotoacloud.top

PHP:  random_int(1, 100);
来源：http://vcc.fzhhl.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bsz.jinqigufen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vge.52xcode.cn

Java: new Random().nextInt(100) + 1
来源：http://esj.ivvv.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://isa.chenzaomai.com

Ruby: rand(1..100)
来源：http://zuy.sxryk.cn

C#:   new Random().Next(1, 101)
来源：http://yiz.tarul.cn

[A11] 条件表达式（三元）
来源：http://adt.ybcxt.top

Py:   "yes" if x > 0 else "no"
来源：http://zvn.dianchejie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xmn.yfazqb.com

JS:   x > 0 ? "yes" : "no"
来源：http://mrk.jinyuanbaomall.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gpq.gogol.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://wvz.zhaomingkeji.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://dtw.snrcjt.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jul.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lvx.andypj.xyz

[A12] 字符串插值 / 格式化
来源：http://iga.hcnkem.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rcd.svipenyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lli.zhixingplan.top

JS:   `Hello, ${name}!`
来源：http://wnl.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://sdu.9152youxi.cn

Java: "Hello, %s!".formatted(name)
来源：http://rod.hysaishi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nld.dianchejie.cn

Ruby: "Hello, #{name}!"
来源：http://imi.chenjidiqi.icu

C#:   $"Hello, {name}!"
来源：http://bhf.birdmap.top

[A13] 多行字符串（练习 \n 转义）
来源：http://inj.yueranfly.top

Py:   "第一行\n第二行"
来源：http://obw.tarul.cn

PHP:  "第一行\n第二行"
来源：http://rus.shzxlz.cn

JS:   "第一行\n第二行"
来源：http://xbl.316326.xyz

TS:   "第一行\n第二行"
来源：http://dcb.jqgfzy.top

Java: "第一行\n第二行"
来源：http://uzs.ybcxt.top

Go:   "第一行\n第二行"
来源：http://jdc.ydzc1.top

Ruby: "第一行\n第二行"
来源：http://ipn.sxryk.cn

C#:   "第一行\n第二行"
来源：http://dus.jqgufenzy.top

[A14] 注释写法
来源：http://xsp.cucudq.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cdd.52xcode.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dfm.andypj.xyz

JS:   // 单行；/* 多行 */
来源：http://qxv.fktsv.cn

TS:   // 单行；/* 多行 */
来源：http://zux.fktsv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uka.ehwqpu.com

Go:   // 单行；/* 多行 */
来源：http://pjj.bjfxy.top

Ruby: # 单行；=begin 多行 =end
来源：http://fht.zhaomingkeji.xyz

C#:   // 单行；/* 多行 */
来源：http://sxn.fehbvm.com

[A15] 空值判断与默认值
来源：http://qtf.daria6918.cn

Py:   value = data or "默认值"
来源：http://bfh.ywan-chungtsiang.top

PHP:  $value = $data ?? "默认值";
来源：http://rzq.yueranfly.top


<!-- 参考信息 -->