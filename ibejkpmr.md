代发 wailian999

[U89] JS：数组去重
来源：http://yzi.zhixingplan.top

[...new Set(arr)]
来源：http://fto.jqgufenzy.top

[U90] JS：数字数组排序
来源：http://swa.xingfuxueyuan.xyz

[...arr].sort((a, b) => a - b)
来源：http://igo.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://phx.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ijm.316326.xyz

[U92] JS：深拷贝
来源：http://fyn.yangfankeji.com

structuredClone(obj)
来源：http://mqx.xinyue.icu

[U93] JS：模板字符串
来源：http://nza.yonumen.top

`共 ${n} 条`
来源：http://pkq.jqgfzy.top

[U94] JS：箭头函数
来源：http://wbi.cashguo.top

const double = x => x * 2;
来源：http://qic.fzhhl.top

[U95] JS：Promise 包装
来源：http://ysx.iojbl.cn

new Promise((resolve, reject) => {})
来源：http://jgj.ehwqpu.com

[U96] JS：async/await 与异常
来源：http://gzz.hnxiangtu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cnr.shuidangran.top

[U97] JS：并发请求
来源：http://bdm.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ubt.yfazqb.com

[U98] JS：fetch 带 JSON
来源：http://xop.fktsv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wxu.316326.xyz

[U99] JS：事件监听
来源：http://xjd.yfazqb.com

el.addEventListener("click", e => {})
来源：http://cqg.hfpthk.cn

[U100] JS：DOM 查询
来源：http://xyf.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://bgn.yuxming.cn

[U101] JS：classList 操作
来源：http://cju.cqqwz.cn

el.classList.toggle("active")
来源：http://msh.yvedp.cn

[U102] JS：本地存储
来源：http://zxz.sjlbkw.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://szu.hcnkem.com

[U103] JS：定时器
来源：http://ohv.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pfy.bjfxy.top

[U104] JS：防抖
来源：http://lgj.pycfn.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zru.gaohongyu789.top

[U105] JS：节流
来源：http://jby.cqqwz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://itg.nanxinkj.top

[U106] JS：日期格式化
来源：http://tez.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wah.xingfuxueyuan.xyz

[U107] JS：数字千分位
来源：http://biz.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vud.kuanghao11.cn

[U108] JS：随机整数
来源：http://ley.cashguo.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zvd.zhongyouzk.top

[U109] JS：数组分组
来源：http://tax.gogol.net.cn

Object.groupBy(arr, x => x.type)
来源：http://xol.fktsv.cn

[U110] JS：数组分块
来源：http://tcr.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yin.sufxvd.cn

[U111] JS：对象转 Map
来源：http://cjf.shanyushiyangtech.top

new Map(Object.entries(obj))
来源：http://ycd.sufxvd.cn

[U112] JS：字符串补位
来源：http://pds.tarul.cn

"7".padStart(3, "0")
来源：http://ytj.wangdashe.top

[U113] JS：正则替换全部
来源：http://dum.zhongyouzk.top

s.replaceAll("a", "b")
来源：http://rpy.jinghuilouyu.cn

[U114] JS：JSON 深比较
来源：http://chw.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ikv.yonumen.top

[U115] JS：生成 UUID
来源：http://grp.fanxiaobao.xyz

crypto.randomUUID()
来源：http://ifp.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://ihq.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://aca.sweek.top

[U117] JS：单元测试
来源：http://ngr.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://tpc.mhx1999.top

[U118] JS：开发服务器
来源：http://uwp.hcnkem.com

npm i -D vite;  npx vite
来源：http://xlz.xziqi.cn

[U119] JS：生产构建
来源：http://xov.wangshuangyany.cn

npx vite build
来源：http://hjv.zdqjudy.top

[U120] JS：读取环境变量（Vite）
来源：http://nuy.iojbl.cn

import.meta.env.VITE_API_URL
来源：http://cku.havefunace.top

================================================================================
来源：http://zcx.yangfankeji.com

统计汇总
来源：http://tmg.gogol.net.cn

================================================================================
来源：http://yls.jqgfzy.top

按语言统计（条）：
来源：http://rjm.epnwcf.com

Python ......... 252
来源：http://edt.fehbvm.com

PHP ............ 252
来源：http://ajo.uphjek.com

JavaScript ..... 252
来源：http://lkp.epnwcf.com

TypeScript ..... 212
来源：http://qww.dianchejie.cn

Java ........... 212
来源：http://wrb.andypj.xyz

Go ............. 212
来源：http://gpo.nwbrower.top

Ruby ........... 212
来源：http://lwe.hesvh.cn

C# ............. 212
来源：http://hum.cashguo.top

C .............. 30
来源：http://blx.vqdsnc.cn

C++ ............ 30
来源：http://bfq.zhongyouzk.top

SQL ............ 90
来源：http://zmx.jianghu66.top

Bash ........... 80
来源：http://cpx.bjfxy.top

Kotlin ......... 15
来源：http://ucd.shangyingyoupin.top

Swift .......... 15
来源：http://xlk.aizwys.cn

Lua ............ 10
来源：http://iib.tian-w.cn

Perl ........... 10
来源：http://dtv.fengsongda.top

Scala .......... 10
来源：http://dtg.ydjk.org.cn

------------------------------------
来源：http://kcu.yj20258.top

合计 ........... 2106 条
来源：http://jpz.9152youxi.cn

按章节统计：
来源：http://kcn.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cmx.cqqwz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ial.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wcz.cdnleiting.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nzv.kuanghao11.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tal.yuxming.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qsx.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mkf.nanxuanxn.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://npe.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://khy.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qdw.chenzaomai.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kit.zhiwuduotai.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uyn.uphjek.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uuu.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://njp.hfpthk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://umj.ybcxt.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oij.aibaodan.cn

Q SQL 专题                              90
来源：http://nnj.meibo888.top

R Bash 专题                             80
来源：http://vtw.yueranfly.top

S C / C++ 专题                          60
来源：http://wwe.kuanghao11.cn

T 其他语言补充                          60
来源：http://shy.nanxuanxn.top

U 高频实用片段                         120
来源：http://jge.haohaochexian.top

------------------------------------
来源：http://kan.zhijiandao.cn

合计                                  2106 条
来源：http://wkc.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://twj.hywenlv.cn

使用提醒
来源：http://zvj.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://jrb.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://szq.xylfe.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tys.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vkt.xinyue.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://ggc.shuidangran.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://slb.sxryk.cn

—— 文件结束 ——
来源：http://mli.fzhhl.top

================================================================================
来源：http://qcl.jinyuanbaomall.cn

程序语言常见例子速查手册（2024 版）
来源：http://kaf.redwolf501.top

Common Programming Examples Cheat Book
来源：http://qie.hesvh.cn

================================================================================
来源：http://niy.jyoumei.cn

【收录内容】
来源：http://jpm.sxryk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jon.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://reg.zhaomingkeji.xyz

SQL · Bash · C · C++
来源：http://isw.smart0.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://arl.fktsv.cn

【使用说明】
来源：http://qad.yongpay.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yct.chenzaomai.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ncy.pengpengdd.cyou

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jom.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://civ.smart0.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://xki.dianchejie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gln.gogol.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qbp.sysykeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://srp.jinqigufen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://atr.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uaa.xingfuxueyuan.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://phl.havefunace.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://skc.0kj1m.cn

【文件统计】
来源：http://xva.yueranfly.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ahh.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://pvc.wangdashe.top

目  录
来源：http://vvm.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://ojs.chenlongwang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://feu.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kbn.bbcook.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tzr.yfazqb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wxk.shzxlz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://weg.yangfankeji.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mjg.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sgp.zycfv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jje.jyoumei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kbe.redwolf501.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tqx.jianghu66.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xil.fktsv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zkw.sysykeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ihi.fanxiaobao.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bcs.wangshuangyany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eco.jqgufenzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sim.xinyue.icu

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gww.tarul.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ash.bjfxy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bwx.meibo888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vfb.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bqb.chenzaomai.com

================================================================================
来源：http://fmc.316326.xyz

A. 基础语法与类型
来源：http://gqv.xziqi.cn

================================================================================
来源：http://tzc.xingfuxueyuan.xyz

[A01] Hello World
来源：http://ykh.zdbjq.cn

Py:   print("Hello, World!")
来源：http://muf.andypj.xyz

PHP:  echo "Hello, World!";
来源：http://pta.fktsv.cn

JS:   console.log("Hello, World!");
来源：http://nrd.mhx1999.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jag.bjfxy.top

Java: System.out.println("Hello, World!");
来源：http://exm.yuanzhike.top

Go:   fmt.Println("Hello, World!")
来源：http://lqu.yongpay.top

Ruby: puts "Hello, World!"
来源：http://dlp.yj20258.top

C#:   Console.WriteLine("Hello, World!");
来源：http://pbr.xingfuxueyuan.xyz

[A02] 变量声明与赋值
来源：http://vth.hysaishi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fvw.9152youxi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://efg.daxiang520.top

JS:   let name = "Alex"; const age = 20;
来源：http://voq.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rrt.chenzaomai.com

Java: String name = "Alex"; int age = 20;
来源：http://kcj.guowangkeji.top

Go:   name := "Alex"; age := 20
来源：http://ulf.xuanzx.com

Ruby: name = "Alex"; age = 20
来源：http://unq.cashguo.top

C#:   string name = "Alex"; int age = 20;
来源：http://gmn.epnwcf.com

[A03] 常量定义
来源：http://hja.sweek.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://srt.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://smp.hfpthk.cn

JS:   const PI = 3.14159;
来源：http://ivo.yj202588.top

TS:   const PI: number = 3.14159;
来源：http://fnk.yonumen.top

Java: static final double PI = 3.14159;
来源：http://mes.hcnkem.com

Go:   const PI = 3.14159
来源：http://zih.daria6918.cn

Ruby: PI = 3.14159
来源：http://fhj.guowangkeji.top

C#:   const double PI = 3.14159;
来源：http://ohd.aizwys.cn

[A04] 判断变量类型
来源：http://bou.shzxlz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cnr.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://snu.fzhhl.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dhv.tianlin.xyz

TS:   typeof x; x instanceof Date
来源：http://swc.cashguo.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qtn.shanyushiyangkeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://uzx.9152youxi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://myo.cheryme.top

C#:   x.GetType().Name; x is int
来源：http://mae.ppjwa.cn

[A05] 整数除法与取模
来源：http://pxd.yfazqb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uoj.hfpthk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sju.hfpthk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bhm.vehdjk.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zsf.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://ree.jqgufenzy.top

Go:   7 / 2; 7 % 2
来源：http://ylw.dashuyun.cn

Ruby: 7 / 2; 7 % 2
来源：http://xwn.dashuyun.cn

C#:   7 / 2; 7 % 2
来源：http://dib.smart0.xyz

[A06] 字符串转数字
来源：http://ecj.c1oappe.top

Py:   int("42"); float("3.14")
来源：http://aob.9152youxi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://trb.svipenyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mga.316326.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://xob.daria6918.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ibt.iojbl.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tdu.yonumen.top

Ruby: "42".to_i; "3.14".to_f
来源：http://kzt.9152youxi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ewe.vqdsnc.cn

[A07] 数字转字符串
来源：http://gcu.daxiang520.top

Py:   str(42)
来源：http://zfp.cucudq.cn

PHP:  (string) 42; strval(42)
来源：http://tsy.cucudq.cn

JS:   String(42); (42).toString()
来源：http://jnt.tianlin.xyz

TS:   String(42)
来源：http://jra.xziqi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uwo.yueranfly.top

Go:   strconv.Itoa(42)
来源：http://fdd.feifeiyinyue.top

Ruby: 42.to_s
来源：http://esv.tianlin.xyz

C#:   42.ToString()
来源：http://fgd.hysaishi.cn

[A08] 取整与四舍五入
来源：http://rgv.yuanzhike.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ahu.yanxiufei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ako.cucudq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ale.hfpthk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sxq.yongpay.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qsr.uphjek.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ptn.iojbl.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ygr.yanxiufei.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mpg.sxryk.cn

[A09] 绝对值与最大最小值
来源：http://kju.hysaishi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://thk.gzhubu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ybz.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gxv.cdnleiting.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bww.c1oappe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jih.shanyushiyangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nip.svipenyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://atd.zhengqikj.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gfx.yj20258.top

[A10] 生成随机数
来源：http://efw.sufxvd.cn

Py:   import random; random.randint(1, 100)
来源：http://ntp.haohaochexian.top

PHP:  random_int(1, 100);
来源：http://wle.9152youxi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ixn.wangshuangyany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vro.jianghu66.top

Java: new Random().nextInt(100) + 1
来源：http://emf.svipenyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ttb.zhixingplan.top

Ruby: rand(1..100)
来源：http://ity.yanxiufei.cn

C#:   new Random().Next(1, 101)
来源：http://alj.ctjpmb.com

[A11] 条件表达式（三元）
来源：http://drc.vqdsnc.cn

Py:   "yes" if x > 0 else "no"
来源：http://hoi.shuidangran.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://sjh.hnxiangtu.top

JS:   x > 0 ? "yes" : "no"
来源：http://uvp.feifeiyinyue.top

TS:   x > 0 ? "yes" : "no"
来源：http://ney.xingfuxueyuan.xyz

Java: x > 0 ? "yes" : "no"
来源：http://hfd.vehdjk.com

Go:   // 无三元运算符，需用 if 语句
来源：http://sqy.ctjpmb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ojp.cqqwz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zax.jinyuanbaomall.cn

[A12] 字符串插值 / 格式化
来源：http://miu.snrcjt.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iyw.ehwqpu.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nlg.cucudq.cn

JS:   `Hello, ${name}!`
来源：http://kmy.hfpthk.cn

TS:   `Hello, ${name}!`
来源：http://jyo.nanxuanxn.top

Java: "Hello, %s!".formatted(name)
来源：http://scf.cdnleiting.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://djn.andypj.xyz

Ruby: "Hello, #{name}!"
来源：http://hvy.fzhhl.top

C#:   $"Hello, {name}!"
来源：http://phl.jlsjyb.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bqu.fzhhl.top

Py:   "第一行\n第二行"
来源：http://ycf.shuidangran.top

PHP:  "第一行\n第二行"
来源：http://vcb.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://ovj.smart0.xyz

TS:   "第一行\n第二行"
来源：http://gqi.gotoacloud.top

Java: "第一行\n第二行"
来源：http://aid.pengpengdd.cyou

Go:   "第一行\n第二行"
来源：http://oga.birdmap.top

Ruby: "第一行\n第二行"
来源：http://sgr.meibo888.top

C#:   "第一行\n第二行"
来源：http://wlc.yfazqb.com

[A14] 注释写法
来源：http://swe.xziqi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kao.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://sdb.iojbl.cn

JS:   // 单行；/* 多行 */
来源：http://wfu.tian-w.cn

TS:   // 单行；/* 多行 */
来源：http://xau.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://czb.hammf.cn

Go:   // 单行；/* 多行 */
来源：http://mjm.sxryk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://adv.pengpengdd.cyou

C#:   // 单行；/* 多行 */
来源：http://myc.fehbvm.com

[A15] 空值判断与默认值
来源：http://pli.snrcjt.cn

Py:   value = data or "默认值"
来源：http://pvd.gotoacloud.top

PHP:  $value = $data ?? "默认值";
来源：http://pwe.cashguo.top


<!-- 参考信息 -->