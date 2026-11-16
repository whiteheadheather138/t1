代发 wailian999

[U81] JS：初始化项目
来源：http://lpi.iojbl.cn

npm init -y;  npm i express
来源：http://hws.iojbl.cn

[U82] JS：package.json 脚本
来源：http://jrf.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qmn.yongpay.top

[U83] JS：ES Module 导入导出
来源：http://pmx.fzhhl.top

export const a = 1;  import { a } from "./m.js";
来源：http://iyr.jinghuilouyu.cn

[U84] JS：CommonJS 写法
来源：http://dhr.feifeiyinyue.top

module.exports = { a };  const { a } = require("./m");
来源：http://cza.daria6918.cn

[U85] JS：可选链
来源：http://gvb.vehdjk.com

a?.b?.c
来源：http://hia.yueranfly.top

[U86] JS：空值合并
来源：http://ybd.quarkkingdee.top

a ?? b
来源：http://zfw.bbcook.cn

[U87] JS：解构默认值
来源：http://xet.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://bpd.jinqigufen.top

[U88] JS：对象展开合并
来源：http://kav.jqgfzy.top

{ ...a, ...b }
来源：http://cnt.zhoulong.xyz

[U89] JS：数组去重
来源：http://bec.zhengqikj.top

[...new Set(arr)]
来源：http://ywe.tanke756.top

[U90] JS：数字数组排序
来源：http://age.hesvh.cn

[...arr].sort((a, b) => a - b)
来源：http://muh.ivvv.top

[U91] JS：对象键值遍历
来源：http://zob.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ipj.wangshuangyany.cn

[U92] JS：深拷贝
来源：http://spi.svipenyu.cn

structuredClone(obj)
来源：http://gxw.zdqjudy.top

[U93] JS：模板字符串
来源：http://lhb.yangfankeji.com

`共 ${n} 条`
来源：http://ktp.nanxuanxn.top

[U94] JS：箭头函数
来源：http://ifz.yangfankeji.com

const double = x => x * 2;
来源：http://aiu.tanke756.top

[U95] JS：Promise 包装
来源：http://xjs.zycfv.cn

new Promise((resolve, reject) => {})
来源：http://kxw.smart0.xyz

[U96] JS：async/await 与异常
来源：http://bqh.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://myo.shuidangran.top

[U97] JS：并发请求
来源：http://svn.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tvt.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://fni.chenzaomai.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://duf.fzhhl.top

[U99] JS：事件监听
来源：http://zes.sxryk.cn

el.addEventListener("click", e => {})
来源：http://mli.zhoulong.xyz

[U100] JS：DOM 查询
来源：http://txp.cqqwz.cn

document.querySelector(".item")
来源：http://qcr.shanyushiyangtech.top

[U101] JS：classList 操作
来源：http://xgo.cheryme.top

el.classList.toggle("active")
来源：http://wtm.hesvh.cn

[U102] JS：本地存储
来源：http://pkg.jinghuilouyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ccu.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://pvp.c1oappe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://naz.andypj.xyz

[U104] JS：防抖
来源：http://njl.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tom.ivvv.top

[U105] JS：节流
来源：http://stk.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bzb.wangdashe.top

[U106] JS：日期格式化
来源：http://szj.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tzi.fehbvm.com

[U107] JS：数字千分位
来源：http://auj.gzhubu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aix.gogol.net.cn

[U108] JS：随机整数
来源：http://wqh.dianchejie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kll.nanxinkj.top

[U109] JS：数组分组
来源：http://pab.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://ato.vehdjk.com

[U110] JS：数组分块
来源：http://gxu.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gxn.haohaochexian.top

[U111] JS：对象转 Map
来源：http://uaa.tian-w.cn

new Map(Object.entries(obj))
来源：http://rkz.xuanzx.com

[U112] JS：字符串补位
来源：http://gac.zhixingplan.top

"7".padStart(3, "0")
来源：http://mok.chenzaomai.com

[U113] JS：正则替换全部
来源：http://qzd.xylfe.cn

s.replaceAll("a", "b")
来源：http://tzd.hongshengwenyu.top

[U114] JS：JSON 深比较
来源：http://wup.zhijiandao.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://txx.cheryme.top

[U115] JS：生成 UUID
来源：http://ppk.tarul.cn

crypto.randomUUID()
来源：http://pzg.nanxuanxn.top

[U116] JS：类型检查（JSDoc）
来源：http://rvg.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://lnj.xuetiantiany.cn

[U117] JS：单元测试
来源：http://wyo.ywan-chungtsiang.top

npm i -D vitest;  npx vitest
来源：http://knc.fktsv.cn

[U118] JS：开发服务器
来源：http://gxa.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://voj.jianghu66.top

[U119] JS：生产构建
来源：http://xhe.shzxlz.cn

npx vite build
来源：http://gmd.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://vhv.jyoumei.cn

import.meta.env.VITE_API_URL
来源：http://xta.yonumen.top

================================================================================
来源：http://wkn.zhaomingkeji.xyz

统计汇总
来源：http://bmh.ivvv.top

================================================================================
来源：http://fcu.ydzc1.top

按语言统计（条）：
来源：http://ltp.ctjpmb.com

Python ......... 252
来源：http://kzn.chenzaomai.com

PHP ............ 252
来源：http://sjb.cdnleiting.top

JavaScript ..... 252
来源：http://jop.bbcook.cn

TypeScript ..... 212
来源：http://bdn.c1oappe.top

Java ........... 212
来源：http://exu.svipenyu.cn

Go ............. 212
来源：http://qxs.fengsongda.top

Ruby ........... 212
来源：http://zrh.yanxiufei.cn

C# ............. 212
来源：http://hjl.ydjk.org.cn

C .............. 30
来源：http://phb.yfazqb.com

C++ ............ 30
来源：http://gtt.yongpay.top

SQL ............ 90
来源：http://fto.cqqwz.cn

Bash ........... 80
来源：http://rgu.hammf.cn

Kotlin ......... 15
来源：http://xma.zhiwuduotai.top

Swift .......... 15
来源：http://xun.yj20258.top

Lua ............ 10
来源：http://mrd.zycfv.cn

Perl ........... 10
来源：http://mld.wangshuangyany.cn

Scala .......... 10
来源：http://abm.zhiwuduotai.top

------------------------------------
来源：http://dzx.jqgfzy.top

合计 ........... 2106 条
来源：http://iak.yfazqb.com

按章节统计：
来源：http://sis.fanxiaobao.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://okf.pycfn.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gdj.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://feb.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lvc.xuetiantiany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yej.hongshengwenyu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tlj.quarkkingdee.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://asg.jinghuilouyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nus.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://odq.zhaomingkeji.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hst.jyoumei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kld.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rur.fehbvm.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fuf.sxryk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jqs.ydjk.org.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ddm.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://duf.gaohongyu789.top

Q SQL 专题                              90
来源：http://evx.shuidangran.top

R Bash 专题                             80
来源：http://wxw.sufxvd.cn

S C / C++ 专题                          60
来源：http://uhv.tianlin.xyz

T 其他语言补充                          60
来源：http://auv.sxryk.cn

U 高频实用片段                         120
来源：http://cqf.fanxiaobao.xyz

------------------------------------
来源：http://irr.sweek.top

合计                                  2106 条
来源：http://nbc.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://zvl.jinghuilouyu.cn

使用提醒
来源：http://vne.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://uzy.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sfp.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eky.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uem.cdnleiting.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hxz.havefunace.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kuo.ydjk.org.cn

—— 文件结束 ——
来源：http://isr.fengsongda.top

================================================================================
来源：http://lar.mhx1999.top

程序语言常见例子速查手册（2024 版）
来源：http://bub.bjfxy.top

Common Programming Examples Cheat Book
来源：http://rqa.dianchejie.cn

================================================================================
来源：http://igt.jqgfzy.top

【收录内容】
来源：http://rqr.mhx1999.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sks.aizwys.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://axg.9152youxi.cn

SQL · Bash · C · C++
来源：http://vrk.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://srm.redwolf501.top

【使用说明】
来源：http://qrm.ehwqpu.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pbh.wangshuangyany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://spc.hywenlv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://scj.tianlin.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nho.sysykeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://sbv.sufxvd.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hhi.hfpthk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jfh.hnqzz.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tdw.sweek.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dmb.yvedp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tje.0kj1m.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kjc.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uda.yuanzhike.top

【文件统计】
来源：http://onb.hesvh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fbr.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://msx.hongshengwenyu.top

目  录
来源：http://phm.yongpay.top

--------------------------------------------------------------------------------
来源：http://rts.zhiwuduotai.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mcj.0kj1m.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xrd.yfazqb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gpu.cashguo.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vnt.shzxlz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vzp.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xrj.birdmap.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://utb.gaohongyu789.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ksv.mhx1999.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nfj.guowangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rif.gotoacloud.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baq.sysykeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fhg.zhongyouzk.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qrt.chenjidiqi.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hnr.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hmc.svipenyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gie.hcnkem.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ffg.hammf.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://udk.jyoumei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://keg.hongshengwenyu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xyz.yangfankeji.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qms.hammf.cn

================================================================================
来源：http://bdv.andypj.xyz

A. 基础语法与类型
来源：http://adb.nanxinkj.top

================================================================================
来源：http://ioq.shanyushiyangkeji.top

[A01] Hello World
来源：http://epy.svipenyu.cn

Py:   print("Hello, World!")
来源：http://ale.zhoulong.xyz

PHP:  echo "Hello, World!";
来源：http://vaf.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://qcw.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qpg.zhengqikj.top

Java: System.out.println("Hello, World!");
来源：http://tas.fanxiaobao.xyz

Go:   fmt.Println("Hello, World!")
来源：http://rym.uphjek.com

Ruby: puts "Hello, World!"
来源：http://bxf.dianchejie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jzq.yanxiufei.cn

[A02] 变量声明与赋值
来源：http://uno.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rtn.dashuyun.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fil.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mmh.nanxinkj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rjk.vehdjk.com

Java: String name = "Alex"; int age = 20;
来源：http://xpx.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://gri.fktsv.cn

Ruby: name = "Alex"; age = 20
来源：http://kxy.nanxuanxn.top

C#:   string name = "Alex"; int age = 20;
来源：http://wem.redwolf501.top

[A03] 常量定义
来源：http://ixu.bjfxy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ajm.52xcode.cn

PHP:  const PI = 3.14159;
来源：http://ryy.fzhhl.top

JS:   const PI = 3.14159;
来源：http://eaf.fengsongda.top

TS:   const PI: number = 3.14159;
来源：http://yne.zhengqikj.top

Java: static final double PI = 3.14159;
来源：http://kyv.xziqi.cn

Go:   const PI = 3.14159
来源：http://han.tanke756.top

Ruby: PI = 3.14159
来源：http://ibw.9152youxi.cn

C#:   const double PI = 3.14159;
来源：http://sqq.jinqigfzy.top

[A04] 判断变量类型
来源：http://siu.yuanzhike.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://kjr.yanxiufei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hza.fehbvm.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gsk.sufxvd.cn

TS:   typeof x; x instanceof Date
来源：http://fqe.jinyuanbaomall.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mtn.birdmap.top

Go:   reflect.TypeOf(x).Name()
来源：http://xek.meibo888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://csz.jianghu66.top

C#:   x.GetType().Name; x is int
来源：http://ors.yanxiufei.cn

[A05] 整数除法与取模
来源：http://uxv.ywan-chungtsiang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qfn.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vwy.nwbrower.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rgy.uphjek.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tve.zdqjudy.top

Java: 7 / 2; 7 % 2
来源：http://izy.hywenlv.cn

Go:   7 / 2; 7 % 2
来源：http://zjp.ybcxt.top

Ruby: 7 / 2; 7 % 2
来源：http://pjs.yvedp.cn

C#:   7 / 2; 7 % 2
来源：http://dfd.nanxuanxn.top

[A06] 字符串转数字
来源：http://qbl.cucudq.cn

Py:   int("42"); float("3.14")
来源：http://pzw.bjfxy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ayl.jyoumei.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tky.zhixingplan.top

TS:   parseInt("42", 10); Number("42")
来源：http://vga.ivvv.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sjp.hesvh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cmh.hongshengwenyu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yav.uphjek.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xjk.dashuyun.cn

[A07] 数字转字符串
来源：http://occ.yueranfly.top

Py:   str(42)
来源：http://gro.guannengcc.top

PHP:  (string) 42; strval(42)
来源：http://vfp.daria6918.cn

JS:   String(42); (42).toString()
来源：http://iwt.jinghuilouyu.cn

TS:   String(42)
来源：http://cgc.xziqi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://njg.fengsongda.top

Go:   strconv.Itoa(42)
来源：http://utt.jqgufenzy.top

Ruby: 42.to_s
来源：http://diq.cheryme.top

C#:   42.ToString()
来源：http://bot.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://jiq.zdqjudy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dtw.yfazqb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eml.fengsongda.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ikv.nanxuanxn.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://orz.fanxiaobao.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xuw.guowangkeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qes.bbcook.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://haz.tianlin.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rfp.sweek.top

[A09] 绝对值与最大最小值
来源：http://nka.hesvh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qqd.sjlbkw.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lfu.cdnleiting.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fft.guowangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ncd.zhiwuduotai.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sii.jlsjyb.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mky.yanxiufei.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nnn.jyoumei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gee.yanxiufei.cn

[A10] 生成随机数
来源：http://vtk.cqqwz.cn

Py:   import random; random.randint(1, 100)
来源：http://ups.vqdsnc.cn

PHP:  random_int(1, 100);
来源：http://mbl.hywenlv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qll.hesvh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gke.gaohongyu789.top

Java: new Random().nextInt(100) + 1
来源：http://auw.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bgm.zdqjudy.top

Ruby: rand(1..100)
来源：http://ptl.shangyingyoupin.top

C#:   new Random().Next(1, 101)
来源：http://tya.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://vsy.hywenlv.cn

Py:   "yes" if x > 0 else "no"
来源：http://jhn.shanyushiyangtech.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ojc.ppjwa.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oro.vehdjk.com

TS:   x > 0 ? "yes" : "no"
来源：http://syg.xylfe.cn

Java: x > 0 ? "yes" : "no"
来源：http://iym.feifeiyinyue.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pzy.zhengqikj.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bit.0kj1m.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vjr.xylfe.cn

[A12] 字符串插值 / 格式化
来源：http://wxd.aizwys.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wno.zdbjq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lmy.vqdsnc.cn

JS:   `Hello, ${name}!`
来源：http://uyk.aibaodan.cn

TS:   `Hello, ${name}!`
来源：http://aof.xylfe.cn

Java: "Hello, %s!".formatted(name)
来源：http://nql.jinyuanbaomall.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uji.birdmap.top

Ruby: "Hello, #{name}!"
来源：http://tnz.cashguo.top

C#:   $"Hello, {name}!"
来源：http://uzt.yj20258888.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rue.gotoacloud.top

Py:   "第一行\n第二行"
来源：http://ugh.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://pfv.jinyuanbaomall.cn

JS:   "第一行\n第二行"
来源：http://vtl.smart0.xyz

TS:   "第一行\n第二行"
来源：http://igc.ppjwa.cn


<!-- 参考信息 -->