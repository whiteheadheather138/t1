代发 wailian999

[U85] JS：可选链
来源：http://wod.haohaochexian.top

a?.b?.c
来源：http://lil.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://kkp.xylfe.cn

a ?? b
来源：http://vmz.ivvv.top

[U87] JS：解构默认值
来源：http://nyk.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://hwf.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://rpo.sweek.top

{ ...a, ...b }
来源：http://ywy.sysykeji.top

[U89] JS：数组去重
来源：http://jhi.yangfankeji.com

[...new Set(arr)]
来源：http://aoe.cheryme.top

[U90] JS：数字数组排序
来源：http://xew.fanxiaobao.xyz

[...arr].sort((a, b) => a - b)
来源：http://vzd.feifeiyinyue.top

[U91] JS：对象键值遍历
来源：http://zbp.nanxuanxn.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zet.jiagoushi.top

[U92] JS：深拷贝
来源：http://kaq.xuetiantiany.cn

structuredClone(obj)
来源：http://rdm.jinqigufen.top

[U93] JS：模板字符串
来源：http://nvx.hysaishi.cn

`共 ${n} 条`
来源：http://lzp.zhengqikj.top

[U94] JS：箭头函数
来源：http://thb.kuanghao11.cn

const double = x => x * 2;
来源：http://axq.ppjwa.cn

[U95] JS：Promise 包装
来源：http://axp.fzhhl.top

new Promise((resolve, reject) => {})
来源：http://oaq.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://uhm.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vgl.zhijiandao.cn

[U97] JS：并发请求
来源：http://kpb.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sup.yongpay.top

[U98] JS：fetch 带 JSON
来源：http://kcp.vqdsnc.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rrq.sjlbkw.cn

[U99] JS：事件监听
来源：http://rtf.andypj.xyz

el.addEventListener("click", e => {})
来源：http://izr.wangdashe.top

[U100] JS：DOM 查询
来源：http://zld.yongpay.top

document.querySelector(".item")
来源：http://ubg.chenzaomai.com

[U101] JS：classList 操作
来源：http://fkn.shzxlz.cn

el.classList.toggle("active")
来源：http://ixz.yuanzhike.top

[U102] JS：本地存储
来源：http://exh.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://exr.yvedp.cn

[U103] JS：定时器
来源：http://rba.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zen.nwbrower.top

[U104] JS：防抖
来源：http://err.9152youxi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lpz.jlsjyb.cn

[U105] JS：节流
来源：http://lej.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qmm.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://lvn.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eaf.haohaochexian.top

[U107] JS：数字千分位
来源：http://ofq.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lri.yanxiufei.cn

[U108] JS：随机整数
来源：http://ilz.yuanzhike.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jmj.chenjidiqi.icu

[U109] JS：数组分组
来源：http://aow.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://gjv.kuanghao11.cn

[U110] JS：数组分块
来源：http://dek.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hxa.yuanzhike.top

[U111] JS：对象转 Map
来源：http://mcy.vqdsnc.cn

new Map(Object.entries(obj))
来源：http://lnu.daxiang520.top

[U112] JS：字符串补位
来源：http://ize.shanyushiyangkeji.top

"7".padStart(3, "0")
来源：http://wrh.daxiang520.top

[U113] JS：正则替换全部
来源：http://ell.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://ced.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://ses.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zel.yj202588.top

[U115] JS：生成 UUID
来源：http://ulf.hywenlv.cn

crypto.randomUUID()
来源：http://uhw.smart0.xyz

[U116] JS：类型检查（JSDoc）
来源：http://sgs.fzhhl.top

/** @param {string} name */ function f(name) {}
来源：http://nza.shzxlz.cn

[U117] JS：单元测试
来源：http://uap.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://gpi.xinyue.icu

[U118] JS：开发服务器
来源：http://ioc.xingfuxueyuan.xyz

npm i -D vite;  npx vite
来源：http://idj.xuanzx.com

[U119] JS：生产构建
来源：http://ytn.zycfv.cn

npx vite build
来源：http://fna.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://xnl.sysykeji.top

import.meta.env.VITE_API_URL
来源：http://ajx.yuxming.cn

================================================================================
来源：http://qun.hcnkem.com

统计汇总
来源：http://jxg.daria6918.cn

================================================================================
来源：http://tvx.feifeiyinyue.top

按语言统计（条）：
来源：http://zxu.sxryk.cn

Python ......... 252
来源：http://erj.xuetiantiany.cn

PHP ............ 252
来源：http://agp.tian-w.cn

JavaScript ..... 252
来源：http://syj.yfazqb.com

TypeScript ..... 212
来源：http://erg.feifeiyinyue.top

Java ........... 212
来源：http://wxu.cdnleiting.top

Go ............. 212
来源：http://uyn.zhijiandao.cn

Ruby ........... 212
来源：http://xnd.yj202588.top

C# ............. 212
来源：http://ioz.jinqigufen.top

C .............. 30
来源：http://hpr.birdmap.top

C++ ............ 30
来源：http://ppv.aizwys.cn

SQL ............ 90
来源：http://wiv.sxryk.cn

Bash ........... 80
来源：http://nyc.redwolf501.top

Kotlin ......... 15
来源：http://pbz.aizwys.cn

Swift .......... 15
来源：http://gxk.yj20258888.top

Lua ............ 10
来源：http://oxt.sysykeji.top

Perl ........... 10
来源：http://vfj.ctjpmb.com

Scala .......... 10
来源：http://tuw.hesvh.cn

------------------------------------
来源：http://rld.yfazqb.com

合计 ........... 2106 条
来源：http://sip.hnxiangtu.top

按章节统计：
来源：http://vip.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qdi.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pyo.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zbp.c1oappe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cbi.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ehj.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ryi.shanyushiyangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lxg.jinyuanbaomall.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uyb.sxryk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jzg.bbcook.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zpz.hesvh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dzl.jyoumei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jio.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ayr.haohaochexian.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://msg.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rwc.zhaomingkeji.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lax.wangshuangyany.cn

Q SQL 专题                              90
来源：http://jly.yj202588.top

R Bash 专题                             80
来源：http://lzr.kuanghao11.cn

S C / C++ 专题                          60
来源：http://ldi.xuetiantiany.cn

T 其他语言补充                          60
来源：http://qab.ctjpmb.com

U 高频实用片段                         120
来源：http://wtg.yj20258.top

------------------------------------
来源：http://ixd.ehwqpu.com

合计                                  2106 条
来源：http://odi.gzhubu.top

--------------------------------------------------------------------------------
来源：http://uog.yvedp.cn

使用提醒
来源：http://lec.birdmap.top

--------------------------------------------------------------------------------
来源：http://nmg.52xcode.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kcq.guannengcc.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://utw.fktsv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://spk.shuidangran.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lcq.jianghu66.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bbb.yvedp.cn

—— 文件结束 ——
来源：http://rqr.tanke756.top

================================================================================
来源：http://wot.ppjwa.cn

程序语言常见例子速查手册（2024 版）
来源：http://vgm.jiagoushi.top

Common Programming Examples Cheat Book
来源：http://hxn.iojbl.cn

================================================================================
来源：http://sel.xingfuxueyuan.xyz

【收录内容】
来源：http://jkx.gaohongyu789.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://owf.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tka.zycfv.cn

SQL · Bash · C · C++
来源：http://avn.bbcook.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uhg.hywenlv.cn

【使用说明】
来源：http://zqu.vqdsnc.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nqr.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kmr.jlsjyb.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hwz.tarul.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fbx.dashuyun.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qlr.jinqigfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://odm.shangyingyoupin.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vnq.uphjek.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dzf.chenlongwang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rka.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yze.jlsjyb.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nto.pengpengdd.cyou

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jxz.chenzaomai.com

【文件统计】
来源：http://evt.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wzx.fengsongda.top

--------------------------------------------------------------------------------
来源：http://bye.yuanzhike.top

目  录
来源：http://lhx.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://qud.guannengcc.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bxt.hnqzz.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uvk.sxryk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nqj.pengpengdd.cyou

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lsr.guowangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wvu.zhiwuduotai.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tjb.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://czo.fanxiaobao.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dnv.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jwy.0kj1m.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://njt.xziqi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wcn.yfazqb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hek.fehbvm.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://phr.hnqzz.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dtg.bjfxy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xsf.xinyue.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yzu.gotoacloud.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://njp.hfpthk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rrr.redwolf501.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rkc.havefunace.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ndl.xuanzx.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ypn.epnwcf.com

================================================================================
来源：http://vms.sufxvd.cn

A. 基础语法与类型
来源：http://yff.iojbl.cn

================================================================================
来源：http://gxv.bbcook.cn

[A01] Hello World
来源：http://oep.chenjidiqi.icu

Py:   print("Hello, World!")
来源：http://uer.feifeiyinyue.top

PHP:  echo "Hello, World!";
来源：http://xjz.bjfxy.top

JS:   console.log("Hello, World!");
来源：http://one.tanke756.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vgs.gotoacloud.top

Java: System.out.println("Hello, World!");
来源：http://zsp.yueranfly.top

Go:   fmt.Println("Hello, World!")
来源：http://zss.0kj1m.cn

Ruby: puts "Hello, World!"
来源：http://bfb.yanxiufei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nrf.cashguo.top

[A02] 变量声明与赋值
来源：http://nsr.daxiang520.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ayv.daxiang520.top

PHP:  $name = "Alex"; $age = 20;
来源：http://oto.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://owa.pycfn.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iqq.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://let.ivvv.top

Go:   name := "Alex"; age := 20
来源：http://vpx.jinqigfzy.top

Ruby: name = "Alex"; age = 20
来源：http://qpt.vqdsnc.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nmy.yj20258.top

[A03] 常量定义
来源：http://lzi.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hmx.ywan-chungtsiang.top

PHP:  const PI = 3.14159;
来源：http://pty.redwolf501.top

JS:   const PI = 3.14159;
来源：http://eah.bjfxy.top

TS:   const PI: number = 3.14159;
来源：http://dgr.zhengqikj.top

Java: static final double PI = 3.14159;
来源：http://qgv.aizwys.cn

Go:   const PI = 3.14159
来源：http://voy.hysaishi.cn

Ruby: PI = 3.14159
来源：http://pwz.cheryme.top

C#:   const double PI = 3.14159;
来源：http://ryf.fanxiaobao.xyz

[A04] 判断变量类型
来源：http://atz.ctjpmb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://mix.feifeiyinyue.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://swf.tarul.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://unp.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://cqj.redwolf501.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wza.bjfxy.top

Go:   reflect.TypeOf(x).Name()
来源：http://mxd.bjfxy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lot.daria6918.cn

C#:   x.GetType().Name; x is int
来源：http://nkq.cheryme.top

[A05] 整数除法与取模
来源：http://lwr.ydzc1.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vgn.zhiwuduotai.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xif.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sll.cqqwz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fwl.cucudq.cn

Java: 7 / 2; 7 % 2
来源：http://deh.yuanzhike.top

Go:   7 / 2; 7 % 2
来源：http://yjr.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://sdm.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://txa.c1oappe.top

[A06] 字符串转数字
来源：http://jwx.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://hos.pycfn.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tmu.sysykeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ixw.sxryk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ljh.chenjidiqi.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://eda.mhx1999.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qqe.yongpay.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hei.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tjd.havefunace.top

[A07] 数字转字符串
来源：http://djj.ydzc1.top

Py:   str(42)
来源：http://sex.dashuyun.cn

PHP:  (string) 42; strval(42)
来源：http://nec.pycfn.com

JS:   String(42); (42).toString()
来源：http://xcc.cdnleiting.top

TS:   String(42)
来源：http://unr.hywenlv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://egm.xuetiantiany.cn

Go:   strconv.Itoa(42)
来源：http://xri.fzhhl.top

Ruby: 42.to_s
来源：http://scs.zhiwuduotai.top

C#:   42.ToString()
来源：http://jor.mhx1999.top

[A08] 取整与四舍五入
来源：http://raa.vehdjk.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://snj.tanke756.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rnr.hesvh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://efk.zycfv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ewa.iojbl.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xpw.cucudq.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://arx.jinghuilouyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fvs.nanxinkj.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dwb.zhixingplan.top

[A09] 绝对值与最大最小值
来源：http://tay.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ruv.fanxiaobao.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tja.hongshengwenyu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ron.yvedp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://msk.gaohongyu789.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nzs.meibo888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vtc.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xht.jqgfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gnm.52xcode.cn

[A10] 生成随机数
来源：http://xsv.sysykeji.top

Py:   import random; random.randint(1, 100)
来源：http://auc.havefunace.top

PHP:  random_int(1, 100);
来源：http://pfa.shanyushiyangtech.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fhy.snrcjt.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wsv.gaohongyu789.top

Java: new Random().nextInt(100) + 1
来源：http://lal.feifeiyinyue.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bpv.mhx1999.top

Ruby: rand(1..100)
来源：http://tol.sxryk.cn

C#:   new Random().Next(1, 101)
来源：http://ief.zhengqikj.top

[A11] 条件表达式（三元）
来源：http://ljl.shanyushiyangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://pey.gaohongyu789.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kyj.jyoumei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pwp.yuxming.cn

TS:   x > 0 ? "yes" : "no"
来源：http://idn.jinghuilouyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://alt.zhengqikj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tsm.ppjwa.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ttr.wangdashe.top

C#:   x > 0 ? "yes" : "no"
来源：http://cnw.aibaodan.cn

[A12] 字符串插值 / 格式化
来源：http://lbz.jinqigfzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xbi.guowangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fxo.hcnkem.com

JS:   `Hello, ${name}!`
来源：http://ckd.ivvv.top

TS:   `Hello, ${name}!`
来源：http://bnv.mhx1999.top

Java: "Hello, %s!".formatted(name)
来源：http://grj.ctjpmb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://raz.redwolf501.top

Ruby: "Hello, #{name}!"
来源：http://lui.jlsjyb.cn

C#:   $"Hello, {name}!"
来源：http://zvo.chenjidiqi.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://ufz.shanyushiyangkeji.top

Py:   "第一行\n第二行"
来源：http://rvz.zhengqikj.top

PHP:  "第一行\n第二行"
来源：http://grk.zdbjq.cn

JS:   "第一行\n第二行"
来源：http://rts.smart0.xyz

TS:   "第一行\n第二行"
来源：http://uab.vqdsnc.cn

Java: "第一行\n第二行"
来源：http://gzs.meibo888.top

Go:   "第一行\n第二行"
来源：http://tdz.zhoulong.xyz

Ruby: "第一行\n第二行"
来源：http://rhe.vqdsnc.cn

C#:   "第一行\n第二行"
来源：http://whc.epnwcf.com

[A14] 注释写法
来源：http://lot.yuxming.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qav.316326.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://qbp.ybcxt.top

JS:   // 单行；/* 多行 */
来源：http://btv.yvedp.cn


<!-- 参考信息 -->