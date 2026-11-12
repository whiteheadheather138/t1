代发 wailian999

[U79] PHP：静态分析
来源：http://ccy.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://kwx.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://uvh.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://aqu.gaohongyu789.top

[U81] JS：初始化项目
来源：http://cyl.zhijiandao.cn

npm init -y;  npm i express
来源：http://okn.fehbvm.com

[U82] JS：package.json 脚本
来源：http://gca.ybcxt.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dub.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://ghd.aibaodan.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rfc.xylfe.cn

[U84] JS：CommonJS 写法
来源：http://iqp.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://rul.cdnleiting.top

[U85] JS：可选链
来源：http://bnn.yuxming.cn

a?.b?.c
来源：http://trz.shangyingyoupin.top

[U86] JS：空值合并
来源：http://oxg.haohaochexian.top

a ?? b
来源：http://mqw.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://owg.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://ety.tian-w.cn

[U88] JS：对象展开合并
来源：http://mii.andypj.xyz

{ ...a, ...b }
来源：http://nqz.fktsv.cn

[U89] JS：数组去重
来源：http://wab.jqgufenzy.top

[...new Set(arr)]
来源：http://xbf.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://xtp.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://evp.fzhhl.top

[U91] JS：对象键值遍历
来源：http://sji.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rxt.ivvv.top

[U92] JS：深拷贝
来源：http://pjj.zycfv.cn

structuredClone(obj)
来源：http://uvu.birdmap.top

[U93] JS：模板字符串
来源：http://qok.gaohongyu789.top

`共 ${n} 条`
来源：http://uvr.andypj.xyz

[U94] JS：箭头函数
来源：http://ncc.daxiang520.top

const double = x => x * 2;
来源：http://ggm.jiagoushi.top

[U95] JS：Promise 包装
来源：http://jec.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://der.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://xai.fktsv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mrj.aibaodan.cn

[U97] JS：并发请求
来源：http://izy.sxryk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://myz.52xcode.cn

[U98] JS：fetch 带 JSON
来源：http://wip.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://grx.hfpthk.cn

[U99] JS：事件监听
来源：http://hjj.nwbrower.top

el.addEventListener("click", e => {})
来源：http://qoz.9152youxi.cn

[U100] JS：DOM 查询
来源：http://vgq.cdnleiting.top

document.querySelector(".item")
来源：http://dbg.hysaishi.cn

[U101] JS：classList 操作
来源：http://bdk.yuanzhike.top

el.classList.toggle("active")
来源：http://esv.yj20258888.top

[U102] JS：本地存储
来源：http://uvj.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jeo.chenlongwang.top

[U103] JS：定时器
来源：http://occ.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://drw.cqqwz.cn

[U104] JS：防抖
来源：http://lry.sxryk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xgc.cqqwz.cn

[U105] JS：节流
来源：http://lvc.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pjh.tianlin.xyz

[U106] JS：日期格式化
来源：http://qav.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wud.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://jnn.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jmd.tian-w.cn

[U108] JS：随机整数
来源：http://uim.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://waf.aibaodan.cn

[U109] JS：数组分组
来源：http://owg.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://xvy.daria6918.cn

[U110] JS：数组分块
来源：http://rod.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rnp.hywenlv.cn

[U111] JS：对象转 Map
来源：http://yio.bjfxy.top

new Map(Object.entries(obj))
来源：http://fsc.fengsongda.top

[U112] JS：字符串补位
来源：http://ekl.pycfn.com

"7".padStart(3, "0")
来源：http://yom.cdnleiting.top

[U113] JS：正则替换全部
来源：http://bdd.ppjwa.cn

s.replaceAll("a", "b")
来源：http://xgj.ywan-chungtsiang.top

[U114] JS：JSON 深比较
来源：http://olp.wangdashe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dtx.birdmap.top

[U115] JS：生成 UUID
来源：http://obd.zhoulong.xyz

crypto.randomUUID()
来源：http://nrz.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://msb.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://qhr.yongpay.top

[U117] JS：单元测试
来源：http://olm.ywan-chungtsiang.top

npm i -D vitest;  npx vitest
来源：http://hdy.yangfankeji.com

[U118] JS：开发服务器
来源：http://emk.yuxming.cn

npm i -D vite;  npx vite
来源：http://ubh.aibaodan.cn

[U119] JS：生产构建
来源：http://szg.0kj1m.cn

npx vite build
来源：http://njr.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://hyd.meibo888.top

import.meta.env.VITE_API_URL
来源：http://hlf.tianlin.xyz

================================================================================
来源：http://qim.cqqwz.cn

统计汇总
来源：http://srn.chenjidiqi.icu

================================================================================
来源：http://hjn.yangfankeji.com

按语言统计（条）：
来源：http://eln.wangshuangyany.cn

Python ......... 252
来源：http://ejb.vqdsnc.cn

PHP ............ 252
来源：http://esa.hesvh.cn

JavaScript ..... 252
来源：http://eck.zhijiandao.cn

TypeScript ..... 212
来源：http://vzj.ivvv.top

Java ........... 212
来源：http://xwp.hfpthk.cn

Go ............. 212
来源：http://lfr.cheryme.top

Ruby ........... 212
来源：http://jkh.c1oappe.top

C# ............. 212
来源：http://yuw.ctjpmb.com

C .............. 30
来源：http://dfz.jinyuanbaomall.cn

C++ ............ 30
来源：http://lws.chenzaomai.com

SQL ............ 90
来源：http://ucp.shzxlz.cn

Bash ........... 80
来源：http://lyc.yj202588.top

Kotlin ......... 15
来源：http://xol.316326.xyz

Swift .......... 15
来源：http://een.gotoacloud.top

Lua ............ 10
来源：http://wbd.tian-w.cn

Perl ........... 10
来源：http://eyi.yangfankeji.com

Scala .......... 10
来源：http://iye.xinyue.icu

------------------------------------
来源：http://adz.fanxiaobao.xyz

合计 ........... 2106 条
来源：http://vtq.guowangkeji.top

按章节统计：
来源：http://lhi.yonumen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uvc.pengpengdd.cyou

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hvy.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qul.pengpengdd.cyou

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://odo.birdmap.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mut.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cdo.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zro.jinyuanbaomall.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qqb.316326.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://znz.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://muc.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nur.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uzi.nanxinkj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nio.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vur.tarul.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tmb.redwolf501.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tfg.kuanghao11.cn

Q SQL 专题                              90
来源：http://kox.havefunace.top

R Bash 专题                             80
来源：http://twm.guowangkeji.top

S C / C++ 专题                          60
来源：http://fng.smart0.xyz

T 其他语言补充                          60
来源：http://dnt.guannengcc.top

U 高频实用片段                         120
来源：http://vya.fehbvm.com

------------------------------------
来源：http://kqf.yongpay.top

合计                                  2106 条
来源：http://dvq.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://ugh.xylfe.cn

使用提醒
来源：http://xbn.hesvh.cn

--------------------------------------------------------------------------------
来源：http://vje.ctjpmb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tvq.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ofd.sufxvd.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rrf.hywenlv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nnh.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hiq.pycfn.com

—— 文件结束 ——
来源：http://hjz.cashguo.top

================================================================================
来源：http://vxm.nwbrower.top

程序语言常见例子速查手册（2024 版）
来源：http://cvq.ywan-chungtsiang.top

Common Programming Examples Cheat Book
来源：http://ksy.yonumen.top

================================================================================
来源：http://nbz.shuidangran.top

【收录内容】
来源：http://eck.zhongyouzk.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://clx.cashguo.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hku.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://lwi.hammf.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wsw.sweek.top

【使用说明】
来源：http://qlt.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qwu.hongshengwenyu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wem.fzhhl.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rcc.yfazqb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xrp.wangshuangyany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tib.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ryk.zhijiandao.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qbb.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rwi.smart0.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kqs.dianchejie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ocr.yonumen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sqt.pycfn.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cdj.xingfuxueyuan.xyz

【文件统计】
来源：http://mxw.hammf.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ysn.ivvv.top

--------------------------------------------------------------------------------
来源：http://ggk.wangdashe.top

目  录
来源：http://bjb.yueranfly.top

--------------------------------------------------------------------------------
来源：http://caq.nanxinkj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bua.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wni.hywenlv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pph.shanyushiyangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ysm.pycfn.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pky.fengsongda.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sat.sxryk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://not.gotoacloud.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dcg.zdqjudy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nbk.mhx1999.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nic.smart0.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gum.shanyushiyangtech.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cos.gotoacloud.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fpw.fzhhl.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mua.fanxiaobao.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qwa.hnxiangtu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ysc.kuanghao11.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://aln.pengpengdd.cyou

R. Bash 专题                   （第 18 节，80 条）
来源：http://drt.yongpay.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://alv.aibaodan.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jxb.yvedp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kri.bbcook.cn

================================================================================
来源：http://mqi.zycfv.cn

A. 基础语法与类型
来源：http://ppt.yangfankeji.com

================================================================================
来源：http://pgr.chenzaomai.com

[A01] Hello World
来源：http://cvx.shuidangran.top

Py:   print("Hello, World!")
来源：http://gvo.wangdashe.top

PHP:  echo "Hello, World!";
来源：http://tot.yj20258.top

JS:   console.log("Hello, World!");
来源：http://tmb.zhiwuduotai.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qui.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://syz.hammf.cn

Go:   fmt.Println("Hello, World!")
来源：http://mdy.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://xvg.xuanzx.com

C#:   Console.WriteLine("Hello, World!");
来源：http://bha.yfazqb.com

[A02] 变量声明与赋值
来源：http://emh.jlsjyb.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ini.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lvx.fanxiaobao.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://vdw.cqqwz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://djb.cheryme.top

Java: String name = "Alex"; int age = 20;
来源：http://xer.nanxuanxn.top

Go:   name := "Alex"; age := 20
来源：http://ntv.hnqzz.top

Ruby: name = "Alex"; age = 20
来源：http://hos.yfazqb.com

C#:   string name = "Alex"; int age = 20;
来源：http://cqc.havefunace.top

[A03] 常量定义
来源：http://qgi.zhengqikj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hdf.gzhubu.top

PHP:  const PI = 3.14159;
来源：http://xaj.hnxiangtu.top

JS:   const PI = 3.14159;
来源：http://nso.dashuyun.cn

TS:   const PI: number = 3.14159;
来源：http://hyw.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://yyu.52xcode.cn

Go:   const PI = 3.14159
来源：http://koh.vehdjk.com

Ruby: PI = 3.14159
来源：http://kjj.316326.xyz

C#:   const double PI = 3.14159;
来源：http://oun.ctjpmb.com

[A04] 判断变量类型
来源：http://uut.snrcjt.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rfp.ydjk.org.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uim.kuanghao11.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lef.yuxming.cn

TS:   typeof x; x instanceof Date
来源：http://oco.sjlbkw.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dgt.52xcode.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nfk.tian-w.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yfm.xylfe.cn

C#:   x.GetType().Name; x is int
来源：http://xae.yj20258888.top

[A05] 整数除法与取模
来源：http://zbs.hywenlv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ddm.hysaishi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ugm.havefunace.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://val.wangshuangyany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://exf.zhoulong.xyz

Java: 7 / 2; 7 % 2
来源：http://lkq.havefunace.top

Go:   7 / 2; 7 % 2
来源：http://klq.yueranfly.top

Ruby: 7 / 2; 7 % 2
来源：http://gfk.xingfuxueyuan.xyz

C#:   7 / 2; 7 % 2
来源：http://eqx.jyoumei.cn

[A06] 字符串转数字
来源：http://piy.zhiwuduotai.top

Py:   int("42"); float("3.14")
来源：http://gat.fktsv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qva.wangdashe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jre.redwolf501.top

TS:   parseInt("42", 10); Number("42")
来源：http://psm.yvedp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bab.jqgufenzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qia.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://dml.hongshengwenyu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://weo.vehdjk.com

[A07] 数字转字符串
来源：http://dhh.yongpay.top

Py:   str(42)
来源：http://ars.tanke756.top

PHP:  (string) 42; strval(42)
来源：http://fxe.ydzc1.top

JS:   String(42); (42).toString()
来源：http://ywe.cdnleiting.top

TS:   String(42)
来源：http://lye.smart0.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://goi.bjfxy.top

Go:   strconv.Itoa(42)
来源：http://dbg.yanxiufei.cn

Ruby: 42.to_s
来源：http://ksm.daxiang520.top

C#:   42.ToString()
来源：http://vom.feifeiyinyue.top

[A08] 取整与四舍五入
来源：http://nxb.jinyuanbaomall.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://aip.316326.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vyb.ehwqpu.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jkj.uphjek.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pit.jinqigfzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dct.cdnleiting.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://irg.shuidangran.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://tkp.dashuyun.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kmv.chenlongwang.top

[A09] 绝对值与最大最小值
来源：http://uza.yanxiufei.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rqz.iojbl.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tvk.cdnleiting.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yvw.yongpay.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fyt.jinghuilouyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ewg.nanxuanxn.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eyi.zdqjudy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uic.0kj1m.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://quq.zhengqikj.top

[A10] 生成随机数
来源：http://eoh.0kj1m.cn

Py:   import random; random.randint(1, 100)
来源：http://ocm.yuxming.cn

PHP:  random_int(1, 100);
来源：http://den.pycfn.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://syr.wangdashe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lsx.tarul.cn

Java: new Random().nextInt(100) + 1
来源：http://kos.fzhhl.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vlr.shanyushiyangkeji.top

Ruby: rand(1..100)
来源：http://cri.cdnleiting.top

C#:   new Random().Next(1, 101)
来源：http://ajq.guannengcc.top

[A11] 条件表达式（三元）
来源：http://ynf.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://mrw.fktsv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cdw.birdmap.top

JS:   x > 0 ? "yes" : "no"
来源：http://ilq.jinghuilouyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gxc.xuanzx.com

Java: x > 0 ? "yes" : "no"
来源：http://xkn.haohaochexian.top

Go:   // 无三元运算符，需用 if 语句
来源：http://exy.feifeiyinyue.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tth.jinyuanbaomall.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ley.yj20258.top

[A12] 字符串插值 / 格式化
来源：http://wcm.cashguo.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wtx.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bfx.tarul.cn

JS:   `Hello, ${name}!`
来源：http://lfb.fanxiaobao.xyz

TS:   `Hello, ${name}!`
来源：http://ufm.shangyingyoupin.top

Java: "Hello, %s!".formatted(name)
来源：http://xrk.pengpengdd.cyou

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hiv.jinghuilouyu.cn

Ruby: "Hello, #{name}!"
来源：http://xdw.yangfankeji.com

C#:   $"Hello, {name}!"
来源：http://vvj.birdmap.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tge.ivvv.top


<!-- 参考信息 -->