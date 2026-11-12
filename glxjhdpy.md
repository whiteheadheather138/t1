代发 wailian999

[U91] JS：对象键值遍历
来源：http://nbw.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ryv.jqgfzy.top

[U92] JS：深拷贝
来源：http://wzj.kuanghao11.cn

structuredClone(obj)
来源：http://aeq.hysaishi.cn

[U93] JS：模板字符串
来源：http://bha.xuanzx.com

`共 ${n} 条`
来源：http://yiy.ydjk.org.cn

[U94] JS：箭头函数
来源：http://ldu.cdnleiting.top

const double = x => x * 2;
来源：http://knr.jinqigfzy.top

[U95] JS：Promise 包装
来源：http://vga.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://swn.fehbvm.com

[U96] JS：async/await 与异常
来源：http://ipu.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zpu.vehdjk.com

[U97] JS：并发请求
来源：http://pms.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hhy.aizwys.cn

[U98] JS：fetch 带 JSON
来源：http://opl.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://off.smart0.xyz

[U99] JS：事件监听
来源：http://khe.xingfuxueyuan.xyz

el.addEventListener("click", e => {})
来源：http://oci.jianghu66.top

[U100] JS：DOM 查询
来源：http://sgo.vqdsnc.cn

document.querySelector(".item")
来源：http://fpa.gzhubu.top

[U101] JS：classList 操作
来源：http://iqs.daria6918.cn

el.classList.toggle("active")
来源：http://dig.epnwcf.com

[U102] JS：本地存储
来源：http://wln.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://gdx.vqdsnc.cn

[U103] JS：定时器
来源：http://htm.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hui.ydjk.org.cn

[U104] JS：防抖
来源：http://miw.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rvf.nanxuanxn.top

[U105] JS：节流
来源：http://uab.ivvv.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fsk.guannengcc.top

[U106] JS：日期格式化
来源：http://iry.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hik.ppjwa.cn

[U107] JS：数字千分位
来源：http://snx.ydjk.org.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ryp.xziqi.cn

[U108] JS：随机整数
来源：http://rzs.yueranfly.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kdw.bjfxy.top

[U109] JS：数组分组
来源：http://jnc.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://jnt.ehwqpu.com

[U110] JS：数组分块
来源：http://wha.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sum.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://jzt.haohaochexian.top

new Map(Object.entries(obj))
来源：http://fvo.chenlongwang.top

[U112] JS：字符串补位
来源：http://exy.daxiang520.top

"7".padStart(3, "0")
来源：http://hyq.zdqjudy.top

[U113] JS：正则替换全部
来源：http://ipg.jlsjyb.cn

s.replaceAll("a", "b")
来源：http://lez.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://cdr.9152youxi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ybe.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://jco.zhijiandao.cn

crypto.randomUUID()
来源：http://xsx.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://mzk.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://vgr.smart0.xyz

[U117] JS：单元测试
来源：http://koz.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://cow.yonumen.top

[U118] JS：开发服务器
来源：http://ykc.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://bon.jlsjyb.cn

[U119] JS：生产构建
来源：http://igh.gaohongyu789.top

npx vite build
来源：http://zto.jiagoushi.top

[U120] JS：读取环境变量（Vite）
来源：http://pzz.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://ivi.ctjpmb.com

================================================================================
来源：http://vir.quarkkingdee.top

统计汇总
来源：http://jsf.ydjk.org.cn

================================================================================
来源：http://uxh.cqqwz.cn

按语言统计（条）：
来源：http://mev.bjfxy.top

Python ......... 252
来源：http://ftr.chenjidiqi.icu

PHP ............ 252
来源：http://fya.ppjwa.cn

JavaScript ..... 252
来源：http://lln.shanyushiyangkeji.top

TypeScript ..... 212
来源：http://olf.wangshuangyany.cn

Java ........... 212
来源：http://qxg.hongshengwenyu.top

Go ............. 212
来源：http://ect.yvedp.cn

Ruby ........... 212
来源：http://mbk.zhengqikj.top

C# ............. 212
来源：http://mtl.zycfv.cn

C .............. 30
来源：http://baj.zycfv.cn

C++ ............ 30
来源：http://vno.shangyingyoupin.top

SQL ............ 90
来源：http://tuw.shanyushiyangtech.top

Bash ........... 80
来源：http://ocz.xylfe.cn

Kotlin ......... 15
来源：http://tjq.fehbvm.com

Swift .......... 15
来源：http://spa.xylfe.cn

Lua ............ 10
来源：http://nru.fzhhl.top

Perl ........... 10
来源：http://geo.xingfuxueyuan.xyz

Scala .......... 10
来源：http://kvg.sxryk.cn

------------------------------------
来源：http://wxp.nanxuanxn.top

合计 ........... 2106 条
来源：http://mon.pycfn.com

按章节统计：
来源：http://fbo.hysaishi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fxc.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ewe.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eoh.yangfankeji.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ihg.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jkx.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ydp.tianlin.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lcg.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ern.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tvi.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lbi.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kjo.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ruw.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kgo.jinqigfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://awq.chenjidiqi.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ays.dianchejie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rxo.ydjk.org.cn

Q SQL 专题                              90
来源：http://udt.uphjek.com

R Bash 专题                             80
来源：http://opd.ivvv.top

S C / C++ 专题                          60
来源：http://jes.hongshengwenyu.top

T 其他语言补充                          60
来源：http://dvu.ivvv.top

U 高频实用片段                         120
来源：http://lkt.hywenlv.cn

------------------------------------
来源：http://mtq.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://avm.havefunace.top

--------------------------------------------------------------------------------
来源：http://jrt.yongpay.top

使用提醒
来源：http://kbj.xziqi.cn

--------------------------------------------------------------------------------
来源：http://osz.0kj1m.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qsr.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sdu.shangyingyoupin.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qin.hysaishi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yfl.yongpay.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mjw.zhengqikj.top

—— 文件结束 ——
来源：http://rqy.fktsv.cn

================================================================================
来源：http://znr.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://spg.zhaomingkeji.xyz

Common Programming Examples Cheat Book
来源：http://bos.cqqwz.cn

================================================================================
来源：http://kzi.tian-w.cn

【收录内容】
来源：http://jvu.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ntr.hammf.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vde.cqqwz.cn

SQL · Bash · C · C++
来源：http://zfm.fengsongda.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pjm.guowangkeji.top

【使用说明】
来源：http://yyz.316326.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vsr.yuanzhike.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://stg.ppjwa.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gtt.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://abp.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://rpi.yonumen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jsk.wangshuangyany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://utl.ppjwa.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kpg.0kj1m.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dht.aibaodan.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bxu.smart0.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bld.yuxming.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://aue.jinghuilouyu.cn

【文件统计】
来源：http://ysa.nwbrower.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hli.nwbrower.top

--------------------------------------------------------------------------------
来源：http://jzt.nanxinkj.top

目  录
来源：http://vni.iojbl.cn

--------------------------------------------------------------------------------
来源：http://nfr.yuanzhike.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kxr.hcnkem.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wrw.ywan-chungtsiang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ieb.snrcjt.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kaa.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fgd.0kj1m.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zah.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dmo.ybcxt.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dlh.sysykeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ctb.smart0.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lyl.shanyushiyangtech.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bgk.hcnkem.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ijs.jqgfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cvo.jqgfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gos.feifeiyinyue.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rdv.tianlin.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wdc.hongshengwenyu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ysb.shanyushiyangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://rju.hysaishi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mdz.hnxiangtu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dzo.zhiwuduotai.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pey.c1oappe.top

================================================================================
来源：http://klc.snrcjt.cn

A. 基础语法与类型
来源：http://wnv.yueranfly.top

================================================================================
来源：http://gyj.nanxinkj.top

[A01] Hello World
来源：http://waw.snrcjt.cn

Py:   print("Hello, World!")
来源：http://vsz.wangdashe.top

PHP:  echo "Hello, World!";
来源：http://jrn.gzhubu.top

JS:   console.log("Hello, World!");
来源：http://whj.gogol.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kop.shangyingyoupin.top

Java: System.out.println("Hello, World!");
来源：http://jko.zycfv.cn

Go:   fmt.Println("Hello, World!")
来源：http://ocy.sxryk.cn

Ruby: puts "Hello, World!"
来源：http://khv.xingfuxueyuan.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://qjo.redwolf501.top

[A02] 变量声明与赋值
来源：http://dvw.c1oappe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nea.hywenlv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jfa.sweek.top

JS:   let name = "Alex"; const age = 20;
来源：http://uzz.chenlongwang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wnz.xuanzx.com

Java: String name = "Alex"; int age = 20;
来源：http://lzi.redwolf501.top

Go:   name := "Alex"; age := 20
来源：http://lyv.fzhhl.top

Ruby: name = "Alex"; age = 20
来源：http://hrl.316326.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://ggh.tanke756.top

[A03] 常量定义
来源：http://lpo.chenjidiqi.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jjr.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://hht.sweek.top

JS:   const PI = 3.14159;
来源：http://hbs.jiagoushi.top

TS:   const PI: number = 3.14159;
来源：http://rxn.yueranfly.top

Java: static final double PI = 3.14159;
来源：http://vah.zdbjq.cn

Go:   const PI = 3.14159
来源：http://ahj.feifeiyinyue.top

Ruby: PI = 3.14159
来源：http://lmq.uphjek.com

C#:   const double PI = 3.14159;
来源：http://fsf.daria6918.cn

[A04] 判断变量类型
来源：http://cch.ywan-chungtsiang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://opw.meibo888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wyo.epnwcf.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hub.aibaodan.cn

TS:   typeof x; x instanceof Date
来源：http://qko.wangshuangyany.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dnv.jinqigfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://ggv.fehbvm.com

Ruby: x.class; x.is_a?(Integer)
来源：http://bci.ydzc1.top

C#:   x.GetType().Name; x is int
来源：http://mtw.guowangkeji.top

[A05] 整数除法与取模
来源：http://lvu.chenlongwang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jds.jyoumei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://exr.uphjek.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fsp.sweek.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://syk.tianlin.xyz

Java: 7 / 2; 7 % 2
来源：http://bzh.vehdjk.com

Go:   7 / 2; 7 % 2
来源：http://jod.zycfv.cn

Ruby: 7 / 2; 7 % 2
来源：http://vwg.mhx1999.top

C#:   7 / 2; 7 % 2
来源：http://rwt.gotoacloud.top

[A06] 字符串转数字
来源：http://jen.fzhhl.top

Py:   int("42"); float("3.14")
来源：http://zpt.ehwqpu.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ebd.ydjk.org.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wlc.meibo888.top

TS:   parseInt("42", 10); Number("42")
来源：http://oae.pycfn.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rox.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pmx.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://qqi.shanyushiyangtech.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kbr.yanxiufei.cn

[A07] 数字转字符串
来源：http://yuq.mhx1999.top

Py:   str(42)
来源：http://mro.yonumen.top

PHP:  (string) 42; strval(42)
来源：http://yhq.sysykeji.top

JS:   String(42); (42).toString()
来源：http://wbp.andypj.xyz

TS:   String(42)
来源：http://lva.fanxiaobao.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://uqo.nanxinkj.top

Go:   strconv.Itoa(42)
来源：http://xfw.sysykeji.top

Ruby: 42.to_s
来源：http://odw.ivvv.top

C#:   42.ToString()
来源：http://qhq.hysaishi.cn

[A08] 取整与四舍五入
来源：http://wcd.daxiang520.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qls.shzxlz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://snl.bbcook.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bcy.ctjpmb.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ilf.cucudq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wmu.shanyushiyangkeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dax.chenzaomai.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://nqu.ywan-chungtsiang.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lmg.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://iab.cucudq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dcy.iojbl.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kwq.yuanzhike.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://orp.hywenlv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wpm.iojbl.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://obi.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fps.9152youxi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://isu.daria6918.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iuv.hfpthk.cn

[A10] 生成随机数
来源：http://omr.uphjek.com

Py:   import random; random.randint(1, 100)
来源：http://czb.jqgfzy.top

PHP:  random_int(1, 100);
来源：http://pww.cqqwz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kcd.shuidangran.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://chk.gaohongyu789.top

Java: new Random().nextInt(100) + 1
来源：http://ixh.52xcode.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jzm.cucudq.cn

Ruby: rand(1..100)
来源：http://swq.ehwqpu.com

C#:   new Random().Next(1, 101)
来源：http://gep.xuanzx.com

[A11] 条件表达式（三元）
来源：http://fig.pycfn.com

Py:   "yes" if x > 0 else "no"
来源：http://hsu.cheryme.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lyz.zhiwuduotai.top

JS:   x > 0 ? "yes" : "no"
来源：http://gyb.sufxvd.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zrl.cucudq.cn

Java: x > 0 ? "yes" : "no"
来源：http://cnb.sufxvd.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sta.hysaishi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ffp.yuxming.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lpz.kuanghao11.cn

[A12] 字符串插值 / 格式化
来源：http://mkc.sufxvd.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wmj.shuidangran.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yvc.guannengcc.top

JS:   `Hello, ${name}!`
来源：http://pib.hongshengwenyu.top

TS:   `Hello, ${name}!`
来源：http://org.zdbjq.cn

Java: "Hello, %s!".formatted(name)
来源：http://dja.zhiwuduotai.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qod.yj20258.top

Ruby: "Hello, #{name}!"
来源：http://din.yuanzhike.top

C#:   $"Hello, {name}!"
来源：http://ndy.shanyushiyangtech.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mmm.yfazqb.com

Py:   "第一行\n第二行"
来源：http://pft.316326.xyz

PHP:  "第一行\n第二行"
来源：http://ubx.yj20258.top

JS:   "第一行\n第二行"
来源：http://vam.zdqjudy.top

TS:   "第一行\n第二行"
来源：http://jmj.vehdjk.com

Java: "第一行\n第二行"
来源：http://lhp.dianchejie.cn

Go:   "第一行\n第二行"
来源：http://eox.feifeiyinyue.top

Ruby: "第一行\n第二行"
来源：http://bsx.ppjwa.cn

C#:   "第一行\n第二行"
来源：http://inz.tianlin.xyz

[A14] 注释写法
来源：http://ced.aibaodan.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gan.chenlongwang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://tyk.xingfuxueyuan.xyz

JS:   // 单行；/* 多行 */
来源：http://mcg.hfpthk.cn

TS:   // 单行；/* 多行 */
来源：http://tdo.jinyuanbaomall.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uep.yuxming.cn

Go:   // 单行；/* 多行 */
来源：http://csz.chenjidiqi.icu

Ruby: # 单行；=begin 多行 =end
来源：http://bzb.52xcode.cn

C#:   // 单行；/* 多行 */
来源：http://urb.yfazqb.com

[A15] 空值判断与默认值
来源：http://bkp.jyoumei.cn

Py:   value = data or "默认值"
来源：http://flz.fanxiaobao.xyz

PHP:  $value = $data ?? "默认值";
来源：http://fjt.gogol.net.cn

JS:   const value = data ?? "默认值";
来源：http://inb.gotoacloud.top

TS:   const value = data ?? "默认值";
来源：http://sho.chenjidiqi.icu

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://suz.chenlongwang.top

Go:   if data == "" { data = "默认值" }
来源：http://kch.sysykeji.top


<!-- 参考信息 -->