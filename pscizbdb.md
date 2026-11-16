代发 wailian999

[U89] JS：数组去重
来源：http://zvi.guowangkeji.top

[...new Set(arr)]
来源：http://cij.yuanzhike.top

[U90] JS：数字数组排序
来源：http://wic.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://qyt.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://vhu.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yvw.fengsongda.top

[U92] JS：深拷贝
来源：http://xlo.vehdjk.com

structuredClone(obj)
来源：http://sfn.yj20258.top

[U93] JS：模板字符串
来源：http://gdr.haohaochexian.top

`共 ${n} 条`
来源：http://nqx.hfpthk.cn

[U94] JS：箭头函数
来源：http://wmp.hnxiangtu.top

const double = x => x * 2;
来源：http://ean.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://lmh.jinqigfzy.top

new Promise((resolve, reject) => {})
来源：http://mnd.cqqwz.cn

[U96] JS：async/await 与异常
来源：http://sux.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wdb.wangshuangyany.cn

[U97] JS：并发请求
来源：http://hbf.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hkx.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://sjz.yonumen.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zqk.hnxiangtu.top

[U99] JS：事件监听
来源：http://oma.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://oil.smart0.xyz

[U100] JS：DOM 查询
来源：http://stb.yongpay.top

document.querySelector(".item")
来源：http://eoe.mhx1999.top

[U101] JS：classList 操作
来源：http://nqe.shangyingyoupin.top

el.classList.toggle("active")
来源：http://zca.jlsjyb.cn

[U102] JS：本地存储
来源：http://hct.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pof.chenlongwang.top

[U103] JS：定时器
来源：http://vqx.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ccx.zycfv.cn

[U104] JS：防抖
来源：http://ycu.cashguo.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fwx.xinyue.icu

[U105] JS：节流
来源：http://icd.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cdr.jyoumei.cn

[U106] JS：日期格式化
来源：http://dab.pengpengdd.cyou

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pmy.ppjwa.cn

[U107] JS：数字千分位
来源：http://ctf.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rww.hesvh.cn

[U108] JS：随机整数
来源：http://any.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dtx.dianchejie.cn

[U109] JS：数组分组
来源：http://aho.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://qwt.zdqjudy.top

[U110] JS：数组分块
来源：http://yfm.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fdr.ctjpmb.com

[U111] JS：对象转 Map
来源：http://bxj.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://edj.redwolf501.top

[U112] JS：字符串补位
来源：http://iko.zhijiandao.cn

"7".padStart(3, "0")
来源：http://jaf.redwolf501.top

[U113] JS：正则替换全部
来源：http://oax.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://lfb.nanxuanxn.top

[U114] JS：JSON 深比较
来源：http://dni.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yuu.sysykeji.top

[U115] JS：生成 UUID
来源：http://fgr.fzhhl.top

crypto.randomUUID()
来源：http://txo.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://rzy.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://fjv.yj202588.top

[U117] JS：单元测试
来源：http://yfh.havefunace.top

npm i -D vitest;  npx vitest
来源：http://lxu.epnwcf.com

[U118] JS：开发服务器
来源：http://fjd.uphjek.com

npm i -D vite;  npx vite
来源：http://cfy.hfpthk.cn

[U119] JS：生产构建
来源：http://xlk.nanxuanxn.top

npx vite build
来源：http://hbo.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://urh.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://gvh.hnxiangtu.top

================================================================================
来源：http://ffy.gogol.net.cn

统计汇总
来源：http://dgd.xingfuxueyuan.xyz

================================================================================
来源：http://ocz.hesvh.cn

按语言统计（条）：
来源：http://esz.jinghuilouyu.cn

Python ......... 252
来源：http://bmq.fengsongda.top

PHP ............ 252
来源：http://roc.zdbjq.cn

JavaScript ..... 252
来源：http://ajg.smart0.xyz

TypeScript ..... 212
来源：http://lnc.redwolf501.top

Java ........... 212
来源：http://cmy.shangyingyoupin.top

Go ............. 212
来源：http://eze.shanyushiyangtech.top

Ruby ........... 212
来源：http://sjr.shanyushiyangkeji.top

C# ............. 212
来源：http://vkh.zycfv.cn

C .............. 30
来源：http://ziz.guowangkeji.top

C++ ............ 30
来源：http://vng.hnqzz.top

SQL ............ 90
来源：http://xwu.ctjpmb.com

Bash ........... 80
来源：http://eaa.ivvv.top

Kotlin ......... 15
来源：http://lua.xylfe.cn

Swift .......... 15
来源：http://avo.jinqigufen.top

Lua ............ 10
来源：http://pjd.gaohongyu789.top

Perl ........... 10
来源：http://hiz.hywenlv.cn

Scala .......... 10
来源：http://upv.yanxiufei.cn

------------------------------------
来源：http://gnz.dashuyun.cn

合计 ........... 2106 条
来源：http://mcf.bjfxy.top

按章节统计：
来源：http://djx.52xcode.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kky.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sqw.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ite.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bbx.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ubt.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uua.andypj.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pwx.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://omv.nanxinkj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://azf.yuxming.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jsn.yj20258888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://niy.xinyue.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yev.shzxlz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://acc.cashguo.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lhl.hywenlv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sfm.sjlbkw.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://haw.fengsongda.top

Q SQL 专题                              90
来源：http://ume.cucudq.cn

R Bash 专题                             80
来源：http://znc.yonumen.top

S C / C++ 专题                          60
来源：http://cfa.xziqi.cn

T 其他语言补充                          60
来源：http://bwg.iojbl.cn

U 高频实用片段                         120
来源：http://qhh.yvedp.cn

------------------------------------
来源：http://vsa.guannengcc.top

合计                                  2106 条
来源：http://why.gzhubu.top

--------------------------------------------------------------------------------
来源：http://lgk.ctjpmb.com

使用提醒
来源：http://vrn.vehdjk.com

--------------------------------------------------------------------------------
来源：http://nnc.tarul.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://drf.9152youxi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ryf.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://alk.iojbl.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://olc.nanxuanxn.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pcz.nwbrower.top

—— 文件结束 ——
来源：http://tue.aizwys.cn

================================================================================
来源：http://hpn.xinyue.icu

程序语言常见例子速查手册（2024 版）
来源：http://fde.pengpengdd.cyou

Common Programming Examples Cheat Book
来源：http://xux.daxiang520.top

================================================================================
来源：http://ias.epnwcf.com

【收录内容】
来源：http://fcv.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gky.shangyingyoupin.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fll.hongshengwenyu.top

SQL · Bash · C · C++
来源：http://ctu.zhengqikj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lme.zhijiandao.cn

【使用说明】
来源：http://kiy.nwbrower.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xzf.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hej.ydjk.org.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ixw.tianlin.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zii.hysaishi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://itg.nwbrower.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jzi.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zgj.haohaochexian.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ron.cashguo.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fax.dianchejie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ymi.chenzaomai.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xkm.shzxlz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fkj.jyoumei.cn

【文件统计】
来源：http://jlp.aibaodan.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kzz.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://jdc.xuanzx.com

目  录
来源：http://xqf.tarul.cn

--------------------------------------------------------------------------------
来源：http://uoh.fehbvm.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ght.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ggb.hywenlv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ayg.aibaodan.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nvd.xylfe.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vuj.chenjidiqi.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://axr.zhongyouzk.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yva.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xxy.52xcode.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qgt.hywenlv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fop.jlsjyb.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ozr.ivvv.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fay.fengsongda.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vzm.zhoulong.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ioy.bbcook.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dux.hnxiangtu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bul.aizwys.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hva.gogol.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bei.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://obq.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dgv.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xjz.nanxuanxn.top

================================================================================
来源：http://avr.yfazqb.com

A. 基础语法与类型
来源：http://nie.shanyushiyangtech.top

================================================================================
来源：http://jar.yj20258888.top

[A01] Hello World
来源：http://elv.hnxiangtu.top

Py:   print("Hello, World!")
来源：http://jwy.yj20258.top

PHP:  echo "Hello, World!";
来源：http://hay.bjfxy.top

JS:   console.log("Hello, World!");
来源：http://bew.snrcjt.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hgo.wangdashe.top

Java: System.out.println("Hello, World!");
来源：http://vlb.daria6918.cn

Go:   fmt.Println("Hello, World!")
来源：http://lfc.tarul.cn

Ruby: puts "Hello, World!"
来源：http://znl.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://dlt.ybcxt.top

[A02] 变量声明与赋值
来源：http://sgz.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dfw.gotoacloud.top

PHP:  $name = "Alex"; $age = 20;
来源：http://czy.zhongyouzk.top

JS:   let name = "Alex"; const age = 20;
来源：http://hax.cucudq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gda.jinghuilouyu.cn

Java: String name = "Alex"; int age = 20;
来源：http://mgv.aizwys.cn

Go:   name := "Alex"; age := 20
来源：http://qbj.ydjk.org.cn

Ruby: name = "Alex"; age = 20
来源：http://bkz.gzhubu.top

C#:   string name = "Alex"; int age = 20;
来源：http://hsr.daria6918.cn

[A03] 常量定义
来源：http://ykd.nwbrower.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yfe.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://hfn.uphjek.com

JS:   const PI = 3.14159;
来源：http://qra.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://ook.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://isu.shanyushiyangkeji.top

Go:   const PI = 3.14159
来源：http://jon.ctjpmb.com

Ruby: PI = 3.14159
来源：http://hhk.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://aiw.chenjidiqi.icu

[A04] 判断变量类型
来源：http://plf.zycfv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jmh.pengpengdd.cyou

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lkd.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qfr.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://pcb.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://akp.chenjidiqi.icu

Go:   reflect.TypeOf(x).Name()
来源：http://lsg.guowangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pkz.316326.xyz

C#:   x.GetType().Name; x is int
来源：http://etb.aibaodan.cn

[A05] 整数除法与取模
来源：http://fys.fanxiaobao.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zbo.ywan-chungtsiang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tgu.gzhubu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yry.havefunace.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sjl.havefunace.top

Java: 7 / 2; 7 % 2
来源：http://nic.yfazqb.com

Go:   7 / 2; 7 % 2
来源：http://htl.wangdashe.top

Ruby: 7 / 2; 7 % 2
来源：http://tzm.bbcook.cn

C#:   7 / 2; 7 % 2
来源：http://nyl.yangfankeji.com

[A06] 字符串转数字
来源：http://yxu.aibaodan.cn

Py:   int("42"); float("3.14")
来源：http://xzq.yuanzhike.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mpz.jlsjyb.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sae.yfazqb.com

TS:   parseInt("42", 10); Number("42")
来源：http://xql.jlsjyb.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bcd.guowangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yyy.xingfuxueyuan.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://xri.shangyingyoupin.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vew.zhiwuduotai.top

[A07] 数字转字符串
来源：http://hke.xuanzx.com

Py:   str(42)
来源：http://ype.gzhubu.top

PHP:  (string) 42; strval(42)
来源：http://nwa.dianchejie.cn

JS:   String(42); (42).toString()
来源：http://vgg.wangdashe.top

TS:   String(42)
来源：http://eqf.havefunace.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://plx.zhixingplan.top

Go:   strconv.Itoa(42)
来源：http://fgq.cucudq.cn

Ruby: 42.to_s
来源：http://bxu.wangshuangyany.cn

C#:   42.ToString()
来源：http://cdv.feifeiyinyue.top

[A08] 取整与四舍五入
来源：http://yqh.jinqigufen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vht.cdnleiting.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uoe.iojbl.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hyz.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://idr.havefunace.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mup.zycfv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://boa.fzhhl.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vwk.nwbrower.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://skv.aibaodan.cn

[A09] 绝对值与最大最小值
来源：http://xdf.gotoacloud.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://urg.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lni.cheryme.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://otv.xylfe.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gxm.ywan-chungtsiang.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oyj.0kj1m.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://itk.chenjidiqi.icu

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://omd.yanxiufei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qqc.yuxming.cn

[A10] 生成随机数
来源：http://ahr.guannengcc.top

Py:   import random; random.randint(1, 100)
来源：http://bnb.aizwys.cn

PHP:  random_int(1, 100);
来源：http://sxd.yonumen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mdi.sweek.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vtl.yuanzhike.top

Java: new Random().nextInt(100) + 1
来源：http://rbz.c1oappe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dmd.hywenlv.cn

Ruby: rand(1..100)
来源：http://icv.yongpay.top

C#:   new Random().Next(1, 101)
来源：http://abk.hnxiangtu.top

[A11] 条件表达式（三元）
来源：http://dpa.yuanzhike.top

Py:   "yes" if x > 0 else "no"
来源：http://ljg.sjlbkw.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zqd.shzxlz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wuu.yj202588.top

TS:   x > 0 ? "yes" : "no"
来源：http://wmr.quarkkingdee.top

Java: x > 0 ? "yes" : "no"
来源：http://pfr.feifeiyinyue.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ayn.jinqigufen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ghz.wangdashe.top

C#:   x > 0 ? "yes" : "no"
来源：http://zhp.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://owb.zhongyouzk.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aci.vehdjk.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qbx.sufxvd.cn

JS:   `Hello, ${name}!`
来源：http://trh.fehbvm.com

TS:   `Hello, ${name}!`
来源：http://zlz.dianchejie.cn

Java: "Hello, %s!".formatted(name)
来源：http://cqy.ivvv.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://olp.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://ain.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://dpo.yj20258888.top

[A13] 多行字符串（练习 \n 转义）
来源：http://olt.gogol.net.cn

Py:   "第一行\n第二行"
来源：http://rbb.jinqigfzy.top

PHP:  "第一行\n第二行"
来源：http://aba.shangyingyoupin.top

JS:   "第一行\n第二行"
来源：http://cmr.fzhhl.top

TS:   "第一行\n第二行"
来源：http://ekq.bbcook.cn

Java: "第一行\n第二行"
来源：http://fmh.tanke756.top

Go:   "第一行\n第二行"
来源：http://whf.hfpthk.cn

Ruby: "第一行\n第二行"
来源：http://daq.quarkkingdee.top

C#:   "第一行\n第二行"
来源：http://clm.jqgfzy.top

[A14] 注释写法
来源：http://vxr.hesvh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://grj.yanxiufei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oak.tianlin.xyz

JS:   // 单行；/* 多行 */
来源：http://caf.yj202588.top

TS:   // 单行；/* 多行 */
来源：http://weu.fehbvm.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gvv.jqgfzy.top

Go:   // 单行；/* 多行 */
来源：http://oyp.quarkkingdee.top

Ruby: # 单行；=begin 多行 =end
来源：http://oko.cqqwz.cn

C#:   // 单行；/* 多行 */
来源：http://wux.dashuyun.cn

[A15] 空值判断与默认值
来源：http://nob.daria6918.cn

Py:   value = data or "默认值"
来源：http://mjm.0kj1m.cn

PHP:  $value = $data ?? "默认值";
来源：http://mtg.xylfe.cn


<!-- 参考信息 -->