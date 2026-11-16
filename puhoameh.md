代发 wailian999

[U91] JS：对象键值遍历
来源：http://xbp.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ghp.tanke756.top

[U92] JS：深拷贝
来源：http://zdo.xziqi.cn

structuredClone(obj)
来源：http://iqc.jqgufenzy.top

[U93] JS：模板字符串
来源：http://pvw.yueranfly.top

`共 ${n} 条`
来源：http://ter.yj20258.top

[U94] JS：箭头函数
来源：http://ger.zhengqikj.top

const double = x => x * 2;
来源：http://mqv.wangdashe.top

[U95] JS：Promise 包装
来源：http://yxu.nwbrower.top

new Promise((resolve, reject) => {})
来源：http://kzm.hfpthk.cn

[U96] JS：async/await 与异常
来源：http://drt.cucudq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aso.hesvh.cn

[U97] JS：并发请求
来源：http://lwg.cqqwz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uhb.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://cwp.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pvx.jlsjyb.cn

[U99] JS：事件监听
来源：http://eog.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://zbq.zhengqikj.top

[U100] JS：DOM 查询
来源：http://kfd.ctjpmb.com

document.querySelector(".item")
来源：http://uvr.zhixingplan.top

[U101] JS：classList 操作
来源：http://crd.andypj.xyz

el.classList.toggle("active")
来源：http://dav.svipenyu.cn

[U102] JS：本地存储
来源：http://hzo.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hjo.smart0.xyz

[U103] JS：定时器
来源：http://hsy.shzxlz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tva.pycfn.com

[U104] JS：防抖
来源：http://seu.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://etx.smart0.xyz

[U105] JS：节流
来源：http://pfp.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rjr.guowangkeji.top

[U106] JS：日期格式化
来源：http://tsz.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jsj.xylfe.cn

[U107] JS：数字千分位
来源：http://wnm.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oew.svipenyu.cn

[U108] JS：随机整数
来源：http://zjh.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tot.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://fqq.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://hst.zycfv.cn

[U110] JS：数组分块
来源：http://yti.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mui.uphjek.com

[U111] JS：对象转 Map
来源：http://pvl.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://wkc.uphjek.com

[U112] JS：字符串补位
来源：http://asf.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://jsw.nanxuanxn.top

[U113] JS：正则替换全部
来源：http://szx.vehdjk.com

s.replaceAll("a", "b")
来源：http://cjt.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://ihy.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zxk.hfpthk.cn

[U115] JS：生成 UUID
来源：http://cla.mhx1999.top

crypto.randomUUID()
来源：http://agf.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://bna.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://vbb.zhoulong.xyz

[U117] JS：单元测试
来源：http://bpr.vehdjk.com

npm i -D vitest;  npx vitest
来源：http://zeh.nanxinkj.top

[U118] JS：开发服务器
来源：http://oxw.ctjpmb.com

npm i -D vite;  npx vite
来源：http://akr.chenjidiqi.icu

[U119] JS：生产构建
来源：http://pif.zhiwuduotai.top

npx vite build
来源：http://yin.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://dfh.tanke756.top

import.meta.env.VITE_API_URL
来源：http://zex.yongpay.top

================================================================================
来源：http://pmj.chenlongwang.top

统计汇总
来源：http://ovz.yj202588.top

================================================================================
来源：http://tyz.ctjpmb.com

按语言统计（条）：
来源：http://bcp.meibo888.top

Python ......... 252
来源：http://ock.gaohongyu789.top

PHP ............ 252
来源：http://nns.xuanzx.com

JavaScript ..... 252
来源：http://vfn.cucudq.cn

TypeScript ..... 212
来源：http://qcx.feifeiyinyue.top

Java ........... 212
来源：http://isv.kuanghao11.cn

Go ............. 212
来源：http://qta.yj20258.top

Ruby ........... 212
来源：http://yqv.yuanzhike.top

C# ............. 212
来源：http://gpl.dianchejie.cn

C .............. 30
来源：http://itj.ydzc1.top

C++ ............ 30
来源：http://fja.vqdsnc.cn

SQL ............ 90
来源：http://xvl.redwolf501.top

Bash ........... 80
来源：http://mdt.yongpay.top

Kotlin ......... 15
来源：http://zlr.shanyushiyangtech.top

Swift .......... 15
来源：http://odf.fanxiaobao.xyz

Lua ............ 10
来源：http://pty.svipenyu.cn

Perl ........... 10
来源：http://wet.hnqzz.top

Scala .......... 10
来源：http://fvo.chenjidiqi.icu

------------------------------------
来源：http://cqe.redwolf501.top

合计 ........... 2106 条
来源：http://dag.yj20258888.top

按章节统计：
来源：http://dtp.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bua.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qmd.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eyz.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://evl.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kke.yonumen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://abi.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://whn.jlsjyb.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ctx.fehbvm.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wzs.havefunace.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zuc.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mdt.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bqy.yuxming.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yol.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fhw.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://opa.nanxuanxn.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cwe.yueranfly.top

Q SQL 专题                              90
来源：http://ngk.fengsongda.top

R Bash 专题                             80
来源：http://wmt.xuetiantiany.cn

S C / C++ 专题                          60
来源：http://ypm.svipenyu.cn

T 其他语言补充                          60
来源：http://hhj.haohaochexian.top

U 高频实用片段                         120
来源：http://ldk.fanxiaobao.xyz

------------------------------------
来源：http://hbl.zdbjq.cn

合计                                  2106 条
来源：http://acf.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://enw.jlsjyb.cn

使用提醒
来源：http://cvr.tanke756.top

--------------------------------------------------------------------------------
来源：http://kdg.9152youxi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://omz.hnxiangtu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://usf.0kj1m.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uxs.316326.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://obz.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ncp.c1oappe.top

—— 文件结束 ——
来源：http://etd.tian-w.cn

================================================================================
来源：http://tgu.yj20258888.top

程序语言常见例子速查手册（2024 版）
来源：http://lna.gotoacloud.top

Common Programming Examples Cheat Book
来源：http://jth.fengsongda.top

================================================================================
来源：http://jkq.pycfn.com

【收录内容】
来源：http://omk.9152youxi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rlv.hongshengwenyu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sdc.yvedp.cn

SQL · Bash · C · C++
来源：http://uxh.yj202588.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lfg.hammf.cn

【使用说明】
来源：http://rmd.sufxvd.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qaa.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nzz.gaohongyu789.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kve.jqgfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lmn.zhixingplan.top

Bash:  Shell         C:     C             C++:   C++
来源：http://klg.zdbjq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pgs.nwbrower.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jax.hesvh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kak.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kyd.yueranfly.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://esk.gaohongyu789.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://viz.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qkp.shzxlz.cn

【文件统计】
来源：http://ohf.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ebw.yj202588.top

--------------------------------------------------------------------------------
来源：http://nwu.yueranfly.top

目  录
来源：http://jwi.yj20258.top

--------------------------------------------------------------------------------
来源：http://lzs.bjfxy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pvm.nanxuanxn.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tds.sysykeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ezd.sxryk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://amj.cqqwz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jez.shangyingyoupin.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bzi.chenzaomai.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eyf.ehwqpu.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://huj.chenzaomai.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aul.ctjpmb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dqc.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://njx.yonumen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jsb.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jmg.aizwys.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eqx.mhx1999.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wwk.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xtk.shanyushiyangtech.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://myf.zdbjq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://log.zdbjq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lbr.redwolf501.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jqm.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rlw.xingfuxueyuan.xyz

================================================================================
来源：http://qbx.fanxiaobao.xyz

A. 基础语法与类型
来源：http://ntv.sxryk.cn

================================================================================
来源：http://jir.yuanzhike.top

[A01] Hello World
来源：http://utp.dashuyun.cn

Py:   print("Hello, World!")
来源：http://cbt.ydzc1.top

PHP:  echo "Hello, World!";
来源：http://upl.zdbjq.cn

JS:   console.log("Hello, World!");
来源：http://utb.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mhj.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://sqp.tian-w.cn

Go:   fmt.Println("Hello, World!")
来源：http://tah.uphjek.com

Ruby: puts "Hello, World!"
来源：http://het.mhx1999.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ids.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://luv.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fcf.yuxming.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xtp.havefunace.top

JS:   let name = "Alex"; const age = 20;
来源：http://wwn.snrcjt.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wrm.sysykeji.top

Java: String name = "Alex"; int age = 20;
来源：http://ghs.yj20258.top

Go:   name := "Alex"; age := 20
来源：http://ubz.daria6918.cn

Ruby: name = "Alex"; age = 20
来源：http://gjk.vqdsnc.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gzp.c1oappe.top

[A03] 常量定义
来源：http://hdj.fanxiaobao.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eve.hfpthk.cn

PHP:  const PI = 3.14159;
来源：http://itz.tanke756.top

JS:   const PI = 3.14159;
来源：http://tcp.jiagoushi.top

TS:   const PI: number = 3.14159;
来源：http://tta.fengsongda.top

Java: static final double PI = 3.14159;
来源：http://kul.sjlbkw.cn

Go:   const PI = 3.14159
来源：http://jdd.jqgfzy.top

Ruby: PI = 3.14159
来源：http://umd.hnqzz.top

C#:   const double PI = 3.14159;
来源：http://sly.yuanzhike.top

[A04] 判断变量类型
来源：http://ydm.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rem.haohaochexian.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ewu.epnwcf.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rga.fanxiaobao.xyz

TS:   typeof x; x instanceof Date
来源：http://fki.zhixingplan.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bfy.havefunace.top

Go:   reflect.TypeOf(x).Name()
来源：http://qxy.52xcode.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jnz.zhongyouzk.top

C#:   x.GetType().Name; x is int
来源：http://clh.meibo888.top

[A05] 整数除法与取模
来源：http://gvx.shuidangran.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rst.vqdsnc.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dbg.xuanzx.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://phg.iojbl.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eid.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://yin.fanxiaobao.xyz

Go:   7 / 2; 7 % 2
来源：http://xhx.mhx1999.top

Ruby: 7 / 2; 7 % 2
来源：http://sym.hfpthk.cn

C#:   7 / 2; 7 % 2
来源：http://eag.nwbrower.top

[A06] 字符串转数字
来源：http://hzj.ehwqpu.com

Py:   int("42"); float("3.14")
来源：http://bhr.fehbvm.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://toa.yongpay.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://syx.sweek.top

TS:   parseInt("42", 10); Number("42")
来源：http://wtd.daria6918.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tij.tianlin.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zrx.pengpengdd.cyou

Ruby: "42".to_i; "3.14".to_f
来源：http://hrt.zhengqikj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rip.hnxiangtu.top

[A07] 数字转字符串
来源：http://jch.zhixingplan.top

Py:   str(42)
来源：http://oeq.jiagoushi.top

PHP:  (string) 42; strval(42)
来源：http://lsf.ydjk.org.cn

JS:   String(42); (42).toString()
来源：http://hpl.zhiwuduotai.top

TS:   String(42)
来源：http://qzu.sjlbkw.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dfu.tianlin.xyz

Go:   strconv.Itoa(42)
来源：http://jqf.tian-w.cn

Ruby: 42.to_s
来源：http://rzn.fengsongda.top

C#:   42.ToString()
来源：http://kee.yuxming.cn

[A08] 取整与四舍五入
来源：http://rcl.gotoacloud.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ilb.fehbvm.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ruc.chenlongwang.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dli.yongpay.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wre.sysykeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uxk.c1oappe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://irg.hysaishi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yzf.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ufd.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://fzx.zhongyouzk.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cba.hnxiangtu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://npx.yj20258888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jxm.vehdjk.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ean.yfazqb.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rta.smart0.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://esj.ctjpmb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tfz.chenzaomai.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wbq.tianlin.xyz

[A10] 生成随机数
来源：http://gnn.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://ics.shanyushiyangkeji.top

PHP:  random_int(1, 100);
来源：http://dgi.zycfv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rwn.gaohongyu789.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vib.andypj.xyz

Java: new Random().nextInt(100) + 1
来源：http://vps.sweek.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://het.ppjwa.cn

Ruby: rand(1..100)
来源：http://gng.yfazqb.com

C#:   new Random().Next(1, 101)
来源：http://zcb.fengsongda.top

[A11] 条件表达式（三元）
来源：http://qqv.hammf.cn

Py:   "yes" if x > 0 else "no"
来源：http://vfo.bbcook.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://epj.vehdjk.com

JS:   x > 0 ? "yes" : "no"
来源：http://mnx.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://esh.xingfuxueyuan.xyz

Java: x > 0 ? "yes" : "no"
来源：http://pna.sxryk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bah.haohaochexian.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ups.zhaomingkeji.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://ggz.daxiang520.top

[A12] 字符串插值 / 格式化
来源：http://onw.hnxiangtu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ktj.bbcook.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zbb.fzhhl.top

JS:   `Hello, ${name}!`
来源：http://nrq.nanxuanxn.top

TS:   `Hello, ${name}!`
来源：http://skn.shzxlz.cn

Java: "Hello, %s!".formatted(name)
来源：http://hyx.fehbvm.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ivv.fktsv.cn

Ruby: "Hello, #{name}!"
来源：http://yug.shzxlz.cn

C#:   $"Hello, {name}!"
来源：http://ugj.ehwqpu.com

[A13] 多行字符串（练习 \n 转义）
来源：http://yvm.vehdjk.com

Py:   "第一行\n第二行"
来源：http://onc.yanxiufei.cn

PHP:  "第一行\n第二行"
来源：http://her.fehbvm.com

JS:   "第一行\n第二行"
来源：http://iwa.xziqi.cn

TS:   "第一行\n第二行"
来源：http://aea.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://cmx.feifeiyinyue.top

Go:   "第一行\n第二行"
来源：http://buv.yfazqb.com

Ruby: "第一行\n第二行"
来源：http://tsi.zhengqikj.top

C#:   "第一行\n第二行"
来源：http://wxg.yj20258888.top

[A14] 注释写法
来源：http://qbi.vqdsnc.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://izf.yongpay.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://yiu.dashuyun.cn

JS:   // 单行；/* 多行 */
来源：http://row.xinyue.icu

TS:   // 单行；/* 多行 */
来源：http://xjp.sufxvd.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jdh.zhongyouzk.top

Go:   // 单行；/* 多行 */
来源：http://sbg.gzhubu.top

Ruby: # 单行；=begin 多行 =end
来源：http://oad.shanyushiyangtech.top

C#:   // 单行；/* 多行 */
来源：http://hjr.guannengcc.top

[A15] 空值判断与默认值
来源：http://vgj.xinyue.icu

Py:   value = data or "默认值"
来源：http://irk.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://uiq.hongshengwenyu.top

JS:   const value = data ?? "默认值";
来源：http://tqi.cheryme.top

TS:   const value = data ?? "默认值";
来源：http://zee.ppjwa.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ngw.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://zkz.nanxuanxn.top


<!-- 参考信息 -->