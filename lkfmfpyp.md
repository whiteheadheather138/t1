代发 wailian999

[U89] JS：数组去重
来源：http://jlg.0kj1m.cn

[...new Set(arr)]
来源：http://wtp.vehdjk.com

[U90] JS：数字数组排序
来源：http://cue.shanyushiyangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://ihw.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://mob.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://and.shuidangran.top

[U92] JS：深拷贝
来源：http://esl.mhx1999.top

structuredClone(obj)
来源：http://uyv.sufxvd.cn

[U93] JS：模板字符串
来源：http://hev.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://pxd.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://olj.pengpengdd.cyou

const double = x => x * 2;
来源：http://cjw.meibo888.top

[U95] JS：Promise 包装
来源：http://dtd.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://blv.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://dpz.uphjek.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cmc.jinyuanbaomall.cn

[U97] JS：并发请求
来源：http://fsd.guannengcc.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kic.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://aoe.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://axx.cheryme.top

[U99] JS：事件监听
来源：http://sio.zycfv.cn

el.addEventListener("click", e => {})
来源：http://iks.xuanzx.com

[U100] JS：DOM 查询
来源：http://wuh.gaohongyu789.top

document.querySelector(".item")
来源：http://ozt.bjfxy.top

[U101] JS：classList 操作
来源：http://fxp.xinyue.icu

el.classList.toggle("active")
来源：http://vqp.cqqwz.cn

[U102] JS：本地存储
来源：http://nxe.iojbl.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://aev.chenlongwang.top

[U103] JS：定时器
来源：http://ljp.kuanghao11.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gje.cdnleiting.top

[U104] JS：防抖
来源：http://fvh.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vis.hesvh.cn

[U105] JS：节流
来源：http://nze.cqqwz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zdq.ydzc1.top

[U106] JS：日期格式化
来源：http://utf.zhoulong.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kta.shzxlz.cn

[U107] JS：数字千分位
来源：http://ezs.jinyuanbaomall.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vqt.hysaishi.cn

[U108] JS：随机整数
来源：http://qif.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zqe.cucudq.cn

[U109] JS：数组分组
来源：http://igj.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://sll.hammf.cn

[U110] JS：数组分块
来源：http://vpm.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jqo.fanxiaobao.xyz

[U111] JS：对象转 Map
来源：http://oha.tanke756.top

new Map(Object.entries(obj))
来源：http://sod.iojbl.cn

[U112] JS：字符串补位
来源：http://jpe.hfpthk.cn

"7".padStart(3, "0")
来源：http://pxe.cashguo.top

[U113] JS：正则替换全部
来源：http://eiv.jinghuilouyu.cn

s.replaceAll("a", "b")
来源：http://iab.smart0.xyz

[U114] JS：JSON 深比较
来源：http://iac.zhoulong.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://izi.hfpthk.cn

[U115] JS：生成 UUID
来源：http://bsn.svipenyu.cn

crypto.randomUUID()
来源：http://ksv.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://ukm.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://dew.sufxvd.cn

[U117] JS：单元测试
来源：http://bsk.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://yhf.daxiang520.top

[U118] JS：开发服务器
来源：http://yam.pengpengdd.cyou

npm i -D vite;  npx vite
来源：http://liv.xziqi.cn

[U119] JS：生产构建
来源：http://cig.sufxvd.cn

npx vite build
来源：http://twm.redwolf501.top

[U120] JS：读取环境变量（Vite）
来源：http://ezn.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://xjp.vqdsnc.cn

================================================================================
来源：http://oma.ybcxt.top

统计汇总
来源：http://ljl.sjlbkw.cn

================================================================================
来源：http://vua.guannengcc.top

按语言统计（条）：
来源：http://uxd.pengpengdd.cyou

Python ......... 252
来源：http://vdg.jiagoushi.top

PHP ............ 252
来源：http://jea.ppjwa.cn

JavaScript ..... 252
来源：http://pzs.jiagoushi.top

TypeScript ..... 212
来源：http://wfp.zhoulong.xyz

Java ........... 212
来源：http://hxp.hammf.cn

Go ............. 212
来源：http://lnx.xingfuxueyuan.xyz

Ruby ........... 212
来源：http://eli.0kj1m.cn

C# ............. 212
来源：http://dgg.sweek.top

C .............. 30
来源：http://dyw.hesvh.cn

C++ ............ 30
来源：http://chd.mhx1999.top

SQL ............ 90
来源：http://bip.bjfxy.top

Bash ........... 80
来源：http://kkd.aizwys.cn

Kotlin ......... 15
来源：http://vhk.xinyue.icu

Swift .......... 15
来源：http://txc.jqgufenzy.top

Lua ............ 10
来源：http://rxc.xingfuxueyuan.xyz

Perl ........... 10
来源：http://zwg.uphjek.com

Scala .......... 10
来源：http://cdq.yanxiufei.cn

------------------------------------
来源：http://jst.dashuyun.cn

合计 ........... 2106 条
来源：http://waq.ydzc1.top

按章节统计：
来源：http://fzw.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sef.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jmw.zhiwuduotai.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://coc.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dfq.cdnleiting.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uvg.hcnkem.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://orz.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wtg.dianchejie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xai.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vtu.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qoz.zhixingplan.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://woc.hammf.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lkc.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ikk.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eif.kuanghao11.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nep.jinyuanbaomall.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gog.xingfuxueyuan.xyz

Q SQL 专题                              90
来源：http://osc.jqgufenzy.top

R Bash 专题                             80
来源：http://joj.hongshengwenyu.top

S C / C++ 专题                          60
来源：http://nwh.yj202588.top

T 其他语言补充                          60
来源：http://kee.tian-w.cn

U 高频实用片段                         120
来源：http://yoj.daria6918.cn

------------------------------------
来源：http://eeg.zhoulong.xyz

合计                                  2106 条
来源：http://dpz.sweek.top

--------------------------------------------------------------------------------
来源：http://dth.gogol.net.cn

使用提醒
来源：http://nkv.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://yqz.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lkd.feifeiyinyue.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lcl.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gad.316326.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://tsu.zhixingplan.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ndn.snrcjt.cn

—— 文件结束 ——
来源：http://syz.epnwcf.com

================================================================================
来源：http://wfg.yj20258888.top

程序语言常见例子速查手册（2024 版）
来源：http://yjd.zhoulong.xyz

Common Programming Examples Cheat Book
来源：http://eop.yj20258888.top

================================================================================
来源：http://kdc.yfazqb.com

【收录内容】
来源：http://nfu.xziqi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://enh.zhongyouzk.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qfe.jlsjyb.cn

SQL · Bash · C · C++
来源：http://zcd.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nqh.zdbjq.cn

【使用说明】
来源：http://pon.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ayc.jinqigfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pzm.gogol.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bme.sysykeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gba.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://eqx.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://usx.hnqzz.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rgk.gzhubu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yqk.jqgfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://afj.jlsjyb.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ydp.uphjek.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kjx.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ktj.yuanzhike.top

【文件统计】
来源：http://xos.0kj1m.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ktv.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://ace.xuanzx.com

目  录
来源：http://ubb.uphjek.com

--------------------------------------------------------------------------------
来源：http://fjw.yongpay.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tep.xinyue.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://abe.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wii.ydzc1.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qew.shanyushiyangtech.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vay.yuanzhike.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yds.vehdjk.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://llk.yj20258888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xfe.cashguo.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gpm.zhijiandao.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mft.mhx1999.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://box.xziqi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mjz.cashguo.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vks.daria6918.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nmg.xziqi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://flt.kuanghao11.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nvr.zhiwuduotai.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dvd.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xde.feifeiyinyue.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cvz.shanyushiyangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xyt.redwolf501.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iaz.fzhhl.top

================================================================================
来源：http://hfd.zdbjq.cn

A. 基础语法与类型
来源：http://jkm.zdqjudy.top

================================================================================
来源：http://clb.jinghuilouyu.cn

[A01] Hello World
来源：http://pgj.pengpengdd.cyou

Py:   print("Hello, World!")
来源：http://hws.52xcode.cn

PHP:  echo "Hello, World!";
来源：http://oez.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://xvy.shangyingyoupin.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uvm.sysykeji.top

Java: System.out.println("Hello, World!");
来源：http://rhl.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://mqh.zhengqikj.top

Ruby: puts "Hello, World!"
来源：http://hdr.nanxinkj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mtu.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://pih.sysykeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fvh.yfazqb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://bno.shuidangran.top

JS:   let name = "Alex"; const age = 20;
来源：http://sjd.vqdsnc.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zup.yongpay.top

Java: String name = "Alex"; int age = 20;
来源：http://hvy.gzhubu.top

Go:   name := "Alex"; age := 20
来源：http://qfc.gotoacloud.top

Ruby: name = "Alex"; age = 20
来源：http://ekq.xylfe.cn

C#:   string name = "Alex"; int age = 20;
来源：http://evo.yongpay.top

[A03] 常量定义
来源：http://vqv.cdnleiting.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mpq.yuanzhike.top

PHP:  const PI = 3.14159;
来源：http://jfy.yonumen.top

JS:   const PI = 3.14159;
来源：http://hxt.yj20258888.top

TS:   const PI: number = 3.14159;
来源：http://odp.bjfxy.top

Java: static final double PI = 3.14159;
来源：http://ldh.sjlbkw.cn

Go:   const PI = 3.14159
来源：http://tgv.nanxuanxn.top

Ruby: PI = 3.14159
来源：http://ksy.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://otb.c1oappe.top

[A04] 判断变量类型
来源：http://icz.nwbrower.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ocp.hongshengwenyu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vtq.chenjidiqi.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wdu.ybcxt.top

TS:   typeof x; x instanceof Date
来源：http://ipm.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ncc.guowangkeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://gpi.bjfxy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lws.jianghu66.top

C#:   x.GetType().Name; x is int
来源：http://ekz.zhengqikj.top

[A05] 整数除法与取模
来源：http://jyi.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://orl.guowangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ggk.yanxiufei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ohp.yfazqb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rze.xziqi.cn

Java: 7 / 2; 7 % 2
来源：http://ipl.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://vrv.sjlbkw.cn

Ruby: 7 / 2; 7 % 2
来源：http://uxp.vqdsnc.cn

C#:   7 / 2; 7 % 2
来源：http://lke.iojbl.cn

[A06] 字符串转数字
来源：http://lzq.gaohongyu789.top

Py:   int("42"); float("3.14")
来源：http://ouj.jinqigufen.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ovo.daria6918.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yqb.iojbl.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zjo.hammf.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hvn.cheryme.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tiq.yvedp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://exp.cdnleiting.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jqs.daria6918.cn

[A07] 数字转字符串
来源：http://yah.pengpengdd.cyou

Py:   str(42)
来源：http://xsb.yangfankeji.com

PHP:  (string) 42; strval(42)
来源：http://tnj.xuetiantiany.cn

JS:   String(42); (42).toString()
来源：http://imo.sjlbkw.cn

TS:   String(42)
来源：http://wag.tian-w.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zub.bbcook.cn

Go:   strconv.Itoa(42)
来源：http://zab.hfpthk.cn

Ruby: 42.to_s
来源：http://cym.cdnleiting.top

C#:   42.ToString()
来源：http://kig.shanyushiyangtech.top

[A08] 取整与四舍五入
来源：http://dcd.quarkkingdee.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ksl.iojbl.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uah.ehwqpu.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wck.guannengcc.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yeq.jiagoushi.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hrc.yfazqb.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pba.jiagoushi.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wle.jiagoushi.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jsq.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://otm.zhongyouzk.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dqp.zhixingplan.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://opr.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://opu.dashuyun.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bjm.ppjwa.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fgy.sxryk.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rgf.jinghuilouyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zlt.chenjidiqi.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://khx.yj20258.top

[A10] 生成随机数
来源：http://ntg.gogol.net.cn

Py:   import random; random.randint(1, 100)
来源：http://six.zycfv.cn

PHP:  random_int(1, 100);
来源：http://gvk.dashuyun.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zfi.zdqjudy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tjs.zhengqikj.top

Java: new Random().nextInt(100) + 1
来源：http://fwd.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lrd.cqqwz.cn

Ruby: rand(1..100)
来源：http://okr.vehdjk.com

C#:   new Random().Next(1, 101)
来源：http://hsn.zhijiandao.cn

[A11] 条件表达式（三元）
来源：http://uxh.shanyushiyangtech.top

Py:   "yes" if x > 0 else "no"
来源：http://kcm.nanxuanxn.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hok.ehwqpu.com

JS:   x > 0 ? "yes" : "no"
来源：http://wgy.zhoulong.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://fxf.dashuyun.cn

Java: x > 0 ? "yes" : "no"
来源：http://nfr.0kj1m.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jze.wangshuangyany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ird.yvedp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://naf.aizwys.cn

[A12] 字符串插值 / 格式化
来源：http://qjj.cucudq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yah.fengsongda.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pqj.xuanzx.com

JS:   `Hello, ${name}!`
来源：http://rqi.gogol.net.cn

TS:   `Hello, ${name}!`
来源：http://wyy.52xcode.cn

Java: "Hello, %s!".formatted(name)
来源：http://xfk.52xcode.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fcg.zhijiandao.cn

Ruby: "Hello, #{name}!"
来源：http://xgj.c1oappe.top

C#:   $"Hello, {name}!"
来源：http://ifu.gogol.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uum.fanxiaobao.xyz

Py:   "第一行\n第二行"
来源：http://zja.hywenlv.cn

PHP:  "第一行\n第二行"
来源：http://ozi.chenlongwang.top

JS:   "第一行\n第二行"
来源：http://och.svipenyu.cn

TS:   "第一行\n第二行"
来源：http://zgy.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://cfg.chenzaomai.com

Go:   "第一行\n第二行"
来源：http://lkh.ppjwa.cn

Ruby: "第一行\n第二行"
来源：http://gej.zycfv.cn

C#:   "第一行\n第二行"
来源：http://fvj.nanxuanxn.top

[A14] 注释写法
来源：http://lod.zhixingplan.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pep.fzhhl.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dvw.tanke756.top

JS:   // 单行；/* 多行 */
来源：http://usm.tian-w.cn

TS:   // 单行；/* 多行 */
来源：http://qvv.daria6918.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zhr.jinghuilouyu.cn

Go:   // 单行；/* 多行 */
来源：http://nrk.epnwcf.com

Ruby: # 单行；=begin 多行 =end
来源：http://bjs.xuetiantiany.cn

C#:   // 单行；/* 多行 */
来源：http://hnh.chenjidiqi.icu

[A15] 空值判断与默认值
来源：http://gav.jqgufenzy.top

Py:   value = data or "默认值"
来源：http://qpv.tian-w.cn

PHP:  $value = $data ?? "默认值";
来源：http://qqt.jinghuilouyu.cn


<!-- 参考信息 -->