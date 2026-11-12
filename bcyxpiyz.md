代发 wailian999

[U87] JS：解构默认值
来源：http://vnt.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://amj.hcnkem.com

[U88] JS：对象展开合并
来源：http://nnq.iojbl.cn

{ ...a, ...b }
来源：http://etm.yj20258.top

[U89] JS：数组去重
来源：http://mqg.ybcxt.top

[...new Set(arr)]
来源：http://odc.ydjk.org.cn

[U90] JS：数字数组排序
来源：http://qas.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://xsw.fzhhl.top

[U91] JS：对象键值遍历
来源：http://ujs.ppjwa.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dhk.gzhubu.top

[U92] JS：深拷贝
来源：http://buq.bbcook.cn

structuredClone(obj)
来源：http://dgr.svipenyu.cn

[U93] JS：模板字符串
来源：http://jhw.guowangkeji.top

`共 ${n} 条`
来源：http://uui.gotoacloud.top

[U94] JS：箭头函数
来源：http://sid.cucudq.cn

const double = x => x * 2;
来源：http://ila.andypj.xyz

[U95] JS：Promise 包装
来源：http://xkl.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://mtq.hnqzz.top

[U96] JS：async/await 与异常
来源：http://wmh.uphjek.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yks.tanke756.top

[U97] JS：并发请求
来源：http://gib.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://rgd.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://wer.xuanzx.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tfx.nwbrower.top

[U99] JS：事件监听
来源：http://din.yvedp.cn

el.addEventListener("click", e => {})
来源：http://dat.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://rhn.yj202588.top

document.querySelector(".item")
来源：http://ons.yuxming.cn

[U101] JS：classList 操作
来源：http://sut.dianchejie.cn

el.classList.toggle("active")
来源：http://dwu.ctjpmb.com

[U102] JS：本地存储
来源：http://qbx.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rau.sysykeji.top

[U103] JS：定时器
来源：http://hfj.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tsh.zhiwuduotai.top

[U104] JS：防抖
来源：http://ayq.yj20258888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jmp.jyoumei.cn

[U105] JS：节流
来源：http://qxt.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ybj.nanxinkj.top

[U106] JS：日期格式化
来源：http://dmj.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cnu.yanxiufei.cn

[U107] JS：数字千分位
来源：http://fsg.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://glm.bjfxy.top

[U108] JS：随机整数
来源：http://lju.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ddd.shzxlz.cn

[U109] JS：数组分组
来源：http://aom.svipenyu.cn

Object.groupBy(arr, x => x.type)
来源：http://gtm.cashguo.top

[U110] JS：数组分块
来源：http://oys.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ggz.52xcode.cn

[U111] JS：对象转 Map
来源：http://geh.yj20258.top

new Map(Object.entries(obj))
来源：http://pbm.xinyue.icu

[U112] JS：字符串补位
来源：http://wnk.cucudq.cn

"7".padStart(3, "0")
来源：http://xuf.chenzaomai.com

[U113] JS：正则替换全部
来源：http://nnu.mhx1999.top

s.replaceAll("a", "b")
来源：http://uma.hnqzz.top

[U114] JS：JSON 深比较
来源：http://dhg.yanxiufei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fnc.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://lfg.xuanzx.com

crypto.randomUUID()
来源：http://dfe.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://evs.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://klu.52xcode.cn

[U117] JS：单元测试
来源：http://apm.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://wwa.fzhhl.top

[U118] JS：开发服务器
来源：http://tiz.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://jpe.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://eqe.xingfuxueyuan.xyz

npx vite build
来源：http://ekk.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://nsb.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://bxm.yangfankeji.com

================================================================================
来源：http://bhe.dianchejie.cn

统计汇总
来源：http://szo.hammf.cn

================================================================================
来源：http://ard.smart0.xyz

按语言统计（条）：
来源：http://kkv.tian-w.cn

Python ......... 252
来源：http://aym.tanke756.top

PHP ............ 252
来源：http://vkb.vqdsnc.cn

JavaScript ..... 252
来源：http://tvk.xinyue.icu

TypeScript ..... 212
来源：http://qel.fanxiaobao.xyz

Java ........... 212
来源：http://akp.yj202588.top

Go ............. 212
来源：http://ubx.sxryk.cn

Ruby ........... 212
来源：http://syw.meibo888.top

C# ............. 212
来源：http://heg.yongpay.top

C .............. 30
来源：http://kfj.ehwqpu.com

C++ ............ 30
来源：http://gba.cashguo.top

SQL ............ 90
来源：http://yyd.hongshengwenyu.top

Bash ........... 80
来源：http://xkk.cashguo.top

Kotlin ......... 15
来源：http://niu.smart0.xyz

Swift .......... 15
来源：http://pxw.cqqwz.cn

Lua ............ 10
来源：http://rmp.yj20258888.top

Perl ........... 10
来源：http://awn.yj20258888.top

Scala .......... 10
来源：http://wqb.kuanghao11.cn

------------------------------------
来源：http://mma.hesvh.cn

合计 ........... 2106 条
来源：http://ezw.xylfe.cn

按章节统计：
来源：http://lvz.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ect.hammf.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rvz.zhaomingkeji.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kms.hesvh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kln.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vwa.zhixingplan.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rbr.snrcjt.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xrg.hfpthk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wcd.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ibl.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ycs.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wgb.vehdjk.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qnr.bbcook.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fwo.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vlp.meibo888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zge.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://adi.zhongyouzk.top

Q SQL 专题                              90
来源：http://fws.hywenlv.cn

R Bash 专题                             80
来源：http://smk.zhengqikj.top

S C / C++ 专题                          60
来源：http://bwt.aizwys.cn

T 其他语言补充                          60
来源：http://cvq.yuxming.cn

U 高频实用片段                         120
来源：http://dwk.guowangkeji.top

------------------------------------
来源：http://ifa.kuanghao11.cn

合计                                  2106 条
来源：http://mja.yj20258888.top

--------------------------------------------------------------------------------
来源：http://uih.dianchejie.cn

使用提醒
来源：http://zmf.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://ndi.yonumen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hhz.cheryme.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zfz.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pln.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vcm.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wpb.redwolf501.top

—— 文件结束 ——
来源：http://fhu.shuidangran.top

================================================================================
来源：http://fry.cheryme.top

程序语言常见例子速查手册（2024 版）
来源：http://iwk.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://fql.ivvv.top

================================================================================
来源：http://ufu.tarul.cn

【收录内容】
来源：http://hao.zhongyouzk.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zgg.fanxiaobao.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jgk.xinyue.icu

SQL · Bash · C · C++
来源：http://ccg.zhoulong.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tof.yj202588.top

【使用说明】
来源：http://mye.yueranfly.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ypw.snrcjt.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bki.ppjwa.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iai.yj202588.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ipt.sysykeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ica.yueranfly.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dpb.c1oappe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rof.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fot.yfazqb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xfy.cashguo.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iuj.shzxlz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pyn.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://izn.xingfuxueyuan.xyz

【文件统计】
来源：http://lsm.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eli.vehdjk.com

--------------------------------------------------------------------------------
来源：http://vsv.yangfankeji.com

目  录
来源：http://blq.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://cuy.bjfxy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gyb.nanxinkj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dox.gogol.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yhi.yj20258.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dnw.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ydp.zdqjudy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qnk.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ejs.aizwys.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yod.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ejy.jqgufenzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://obm.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uwm.hfpthk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jqn.tarul.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ddv.hongshengwenyu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pub.sweek.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yju.hnqzz.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tlv.ydjk.org.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ogy.cqqwz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ijb.meibo888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://heh.meibo888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qyn.yfazqb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pgl.fanxiaobao.xyz

================================================================================
来源：http://bmu.zycfv.cn

A. 基础语法与类型
来源：http://qaw.kuanghao11.cn

================================================================================
来源：http://odj.yueranfly.top

[A01] Hello World
来源：http://asy.zdqjudy.top

Py:   print("Hello, World!")
来源：http://pcj.yvedp.cn

PHP:  echo "Hello, World!";
来源：http://ppx.hnqzz.top

JS:   console.log("Hello, World!");
来源：http://osr.tianlin.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://anc.zycfv.cn

Java: System.out.println("Hello, World!");
来源：http://nja.pycfn.com

Go:   fmt.Println("Hello, World!")
来源：http://dij.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://kcc.gaohongyu789.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qcz.haohaochexian.top

[A02] 变量声明与赋值
来源：http://nbu.yonumen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ngy.jinyuanbaomall.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pwg.sxryk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xgt.ivvv.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bwy.yuanzhike.top

Java: String name = "Alex"; int age = 20;
来源：http://cac.snrcjt.cn

Go:   name := "Alex"; age := 20
来源：http://gql.xinyue.icu

Ruby: name = "Alex"; age = 20
来源：http://gwa.yuxming.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yim.hesvh.cn

[A03] 常量定义
来源：http://eei.shanyushiyangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vps.tarul.cn

PHP:  const PI = 3.14159;
来源：http://oxe.gotoacloud.top

JS:   const PI = 3.14159;
来源：http://rqw.zhijiandao.cn

TS:   const PI: number = 3.14159;
来源：http://vzz.redwolf501.top

Java: static final double PI = 3.14159;
来源：http://lrx.redwolf501.top

Go:   const PI = 3.14159
来源：http://vlt.tanke756.top

Ruby: PI = 3.14159
来源：http://ppf.xuetiantiany.cn

C#:   const double PI = 3.14159;
来源：http://bag.tarul.cn

[A04] 判断变量类型
来源：http://mjh.bjfxy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://fza.9152youxi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zez.cucudq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fhn.gaohongyu789.top

TS:   typeof x; x instanceof Date
来源：http://umd.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gfl.shuidangran.top

Go:   reflect.TypeOf(x).Name()
来源：http://bot.yanxiufei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://skk.ctjpmb.com

C#:   x.GetType().Name; x is int
来源：http://pdv.hnqzz.top

[A05] 整数除法与取模
来源：http://hbc.cucudq.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ata.hesvh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hde.zhongyouzk.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uhd.ctjpmb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://krp.zhijiandao.cn

Java: 7 / 2; 7 % 2
来源：http://rta.fengsongda.top

Go:   7 / 2; 7 % 2
来源：http://mtj.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://cib.mhx1999.top

C#:   7 / 2; 7 % 2
来源：http://xdc.snrcjt.cn

[A06] 字符串转数字
来源：http://ekl.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://wik.fanxiaobao.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://esw.zhijiandao.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lxp.zhaomingkeji.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://tig.9152youxi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://eiy.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ymy.wangdashe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dos.yangfankeji.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fdc.ctjpmb.com

[A07] 数字转字符串
来源：http://rqe.jinqigufen.top

Py:   str(42)
来源：http://bum.dianchejie.cn

PHP:  (string) 42; strval(42)
来源：http://mms.ctjpmb.com

JS:   String(42); (42).toString()
来源：http://nlg.dianchejie.cn

TS:   String(42)
来源：http://zws.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://obi.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://jrd.cucudq.cn

Ruby: 42.to_s
来源：http://vbh.feifeiyinyue.top

C#:   42.ToString()
来源：http://rup.bbcook.cn

[A08] 取整与四舍五入
来源：http://ylu.epnwcf.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bac.ybcxt.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kbx.tarul.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tlt.redwolf501.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wce.yanxiufei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nun.shzxlz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ycx.nanxinkj.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gpe.chenzaomai.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rkt.fzhhl.top

[A09] 绝对值与最大最小值
来源：http://gti.shanyushiyangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ulu.jinyuanbaomall.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mjs.gogol.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://asy.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://csg.yj20258888.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ffg.jinyuanbaomall.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gjb.yangfankeji.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hvm.nanxinkj.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qrj.feifeiyinyue.top

[A10] 生成随机数
来源：http://rni.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://xsi.ctjpmb.com

PHP:  random_int(1, 100);
来源：http://eod.zdqjudy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://owi.wangdashe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xmy.ehwqpu.com

Java: new Random().nextInt(100) + 1
来源：http://vek.ydzc1.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hxb.xylfe.cn

Ruby: rand(1..100)
来源：http://zxs.jinghuilouyu.cn

C#:   new Random().Next(1, 101)
来源：http://fel.guannengcc.top

[A11] 条件表达式（三元）
来源：http://kcp.haohaochexian.top

Py:   "yes" if x > 0 else "no"
来源：http://jvf.xziqi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fqg.daria6918.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vab.xylfe.cn

TS:   x > 0 ? "yes" : "no"
来源：http://poh.zhiwuduotai.top

Java: x > 0 ? "yes" : "no"
来源：http://abq.nanxuanxn.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pgo.tarul.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dnn.ybcxt.top

C#:   x > 0 ? "yes" : "no"
来源：http://trt.cheryme.top

[A12] 字符串插值 / 格式化
来源：http://myl.zhijiandao.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hjd.cashguo.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://twq.chenzaomai.com

JS:   `Hello, ${name}!`
来源：http://npw.redwolf501.top

TS:   `Hello, ${name}!`
来源：http://xac.cqqwz.cn

Java: "Hello, %s!".formatted(name)
来源：http://jzh.xingfuxueyuan.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pfr.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://eny.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://pet.fengsongda.top

[A13] 多行字符串（练习 \n 转义）
来源：http://eep.xingfuxueyuan.xyz

Py:   "第一行\n第二行"
来源：http://gfr.hnxiangtu.top

PHP:  "第一行\n第二行"
来源：http://yir.ydjk.org.cn

JS:   "第一行\n第二行"
来源：http://jyr.nanxinkj.top

TS:   "第一行\n第二行"
来源：http://qfb.zhixingplan.top

Java: "第一行\n第二行"
来源：http://udf.mhx1999.top

Go:   "第一行\n第二行"
来源：http://hhx.chenzaomai.com

Ruby: "第一行\n第二行"
来源：http://asp.fanxiaobao.xyz

C#:   "第一行\n第二行"
来源：http://qqj.sxryk.cn

[A14] 注释写法
来源：http://ljg.tanke756.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wkw.ybcxt.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kwo.yj202588.top

JS:   // 单行；/* 多行 */
来源：http://ngy.dianchejie.cn

TS:   // 单行；/* 多行 */
来源：http://pnq.zhijiandao.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zxf.ppjwa.cn

Go:   // 单行；/* 多行 */
来源：http://qlb.sweek.top

Ruby: # 单行；=begin 多行 =end
来源：http://kxr.shuidangran.top


<!-- 参考信息 -->