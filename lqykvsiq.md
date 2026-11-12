代发 wailian999

[U81] JS：初始化项目
来源：http://ofv.shangyingyoupin.top

npm init -y;  npm i express
来源：http://znd.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://nrk.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oxq.redwolf501.top

[U83] JS：ES Module 导入导出
来源：http://frt.meibo888.top

export const a = 1;  import { a } from "./m.js";
来源：http://gnj.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://nhz.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fxr.cucudq.cn

[U85] JS：可选链
来源：http://lbs.zhongyouzk.top

a?.b?.c
来源：http://rqs.cqqwz.cn

[U86] JS：空值合并
来源：http://nkq.yj20258.top

a ?? b
来源：http://ljd.yonumen.top

[U87] JS：解构默认值
来源：http://kop.hammf.cn

const { a = 1, b = 2 } = obj;
来源：http://bti.yfazqb.com

[U88] JS：对象展开合并
来源：http://lbu.vqdsnc.cn

{ ...a, ...b }
来源：http://wed.jinghuilouyu.cn

[U89] JS：数组去重
来源：http://mpx.yj20258888.top

[...new Set(arr)]
来源：http://tpr.wangdashe.top

[U90] JS：数字数组排序
来源：http://tcx.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://lnd.shuidangran.top

[U91] JS：对象键值遍历
来源：http://iki.hfpthk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ugs.tian-w.cn

[U92] JS：深拷贝
来源：http://egh.zdbjq.cn

structuredClone(obj)
来源：http://bjb.xylfe.cn

[U93] JS：模板字符串
来源：http://qsl.zycfv.cn

`共 ${n} 条`
来源：http://gtb.shanyushiyangkeji.top

[U94] JS：箭头函数
来源：http://cww.shangyingyoupin.top

const double = x => x * 2;
来源：http://yoy.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://uqc.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://efj.aibaodan.cn

[U96] JS：async/await 与异常
来源：http://kvo.zhoulong.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jqg.gaohongyu789.top

[U97] JS：并发请求
来源：http://iuy.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://jev.tian-w.cn

[U98] JS：fetch 带 JSON
来源：http://uxs.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bnw.shzxlz.cn

[U99] JS：事件监听
来源：http://dzl.xylfe.cn

el.addEventListener("click", e => {})
来源：http://mid.nwbrower.top

[U100] JS：DOM 查询
来源：http://tus.vqdsnc.cn

document.querySelector(".item")
来源：http://ohn.tianlin.xyz

[U101] JS：classList 操作
来源：http://ajo.jinqigfzy.top

el.classList.toggle("active")
来源：http://stn.guannengcc.top

[U102] JS：本地存储
来源：http://vse.yongpay.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fhn.kuanghao11.cn

[U103] JS：定时器
来源：http://bsm.bjfxy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fgr.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://yvg.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aig.gzhubu.top

[U105] JS：节流
来源：http://pdi.316326.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yun.jlsjyb.cn

[U106] JS：日期格式化
来源：http://tjx.ywan-chungtsiang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sux.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://jdq.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://abh.zhixingplan.top

[U108] JS：随机整数
来源：http://lzl.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gqx.daria6918.cn

[U109] JS：数组分组
来源：http://ikv.ydzc1.top

Object.groupBy(arr, x => x.type)
来源：http://hmz.tanke756.top

[U110] JS：数组分块
来源：http://oml.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rpm.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://voz.mhx1999.top

new Map(Object.entries(obj))
来源：http://tlf.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://qlf.sweek.top

"7".padStart(3, "0")
来源：http://ddw.xinyue.icu

[U113] JS：正则替换全部
来源：http://odm.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://rfu.ydjk.org.cn

[U114] JS：JSON 深比较
来源：http://bcq.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qvq.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://apk.fehbvm.com

crypto.randomUUID()
来源：http://ape.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://kwm.nwbrower.top

/** @param {string} name */ function f(name) {}
来源：http://fnp.guannengcc.top

[U117] JS：单元测试
来源：http://ysr.xylfe.cn

npm i -D vitest;  npx vitest
来源：http://tud.jyoumei.cn

[U118] JS：开发服务器
来源：http://shx.tian-w.cn

npm i -D vite;  npx vite
来源：http://eyh.sweek.top

[U119] JS：生产构建
来源：http://ggh.wangshuangyany.cn

npx vite build
来源：http://vpo.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://tji.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://vtn.shzxlz.cn

================================================================================
来源：http://ljf.mhx1999.top

统计汇总
来源：http://ugd.sxryk.cn

================================================================================
来源：http://nbq.yueranfly.top

按语言统计（条）：
来源：http://wja.gaohongyu789.top

Python ......... 252
来源：http://pyi.yj20258888.top

PHP ............ 252
来源：http://ylw.sufxvd.cn

JavaScript ..... 252
来源：http://dom.jinqigfzy.top

TypeScript ..... 212
来源：http://iya.meibo888.top

Java ........... 212
来源：http://sjn.sufxvd.cn

Go ............. 212
来源：http://hjo.ctjpmb.com

Ruby ........... 212
来源：http://oyr.jinghuilouyu.cn

C# ............. 212
来源：http://hku.cheryme.top

C .............. 30
来源：http://wfn.jqgufenzy.top

C++ ............ 30
来源：http://jzi.c1oappe.top

SQL ............ 90
来源：http://fbb.dianchejie.cn

Bash ........... 80
来源：http://lnk.svipenyu.cn

Kotlin ......... 15
来源：http://apl.xingfuxueyuan.xyz

Swift .......... 15
来源：http://qhc.xinyue.icu

Lua ............ 10
来源：http://lrn.yonumen.top

Perl ........... 10
来源：http://cit.wangshuangyany.cn

Scala .......... 10
来源：http://gfc.aibaodan.cn

------------------------------------
来源：http://lcb.fehbvm.com

合计 ........... 2106 条
来源：http://xqe.zdqjudy.top

按章节统计：
来源：http://zmq.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gxk.nanxinkj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jbs.jianghu66.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cti.epnwcf.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hrs.yuxming.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tnn.ppjwa.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://psi.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vib.gotoacloud.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kth.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hxg.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lae.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jvj.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://csg.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xhc.jqgufenzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sel.yonumen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jks.aizwys.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jjk.sufxvd.cn

Q SQL 专题                              90
来源：http://snu.sweek.top

R Bash 专题                             80
来源：http://ctt.c1oappe.top

S C / C++ 专题                          60
来源：http://pgr.iojbl.cn

T 其他语言补充                          60
来源：http://phk.hesvh.cn

U 高频实用片段                         120
来源：http://hdz.zhiwuduotai.top

------------------------------------
来源：http://fey.yuxming.cn

合计                                  2106 条
来源：http://jyl.andypj.xyz

--------------------------------------------------------------------------------
来源：http://nfp.vqdsnc.cn

使用提醒
来源：http://ssm.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://uxt.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://psi.hnxiangtu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://phl.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iyc.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://uxs.yonumen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xcp.jinghuilouyu.cn

—— 文件结束 ——
来源：http://rzm.hcnkem.com

================================================================================
来源：http://jch.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://hpx.zhengqikj.top

Common Programming Examples Cheat Book
来源：http://rsp.fzhhl.top

================================================================================
来源：http://tsp.jlsjyb.cn

【收录内容】
来源：http://jmo.wangdashe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tjs.gotoacloud.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zzm.jiagoushi.top

SQL · Bash · C · C++
来源：http://gup.yueranfly.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jrj.jinyuanbaomall.cn

【使用说明】
来源：http://nva.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kpr.ppjwa.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ecx.snrcjt.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jol.bjfxy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jej.shanyushiyangtech.top

Bash:  Shell         C:     C             C++:   C++
来源：http://oik.haohaochexian.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bid.yanxiufei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wnc.jqgfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ujh.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tke.gogol.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ssm.shanyushiyangtech.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mbx.yj20258.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yqz.chenjidiqi.icu

【文件统计】
来源：http://unk.52xcode.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kcq.fzhhl.top

--------------------------------------------------------------------------------
来源：http://ulu.nanxinkj.top

目  录
来源：http://ntr.nwbrower.top

--------------------------------------------------------------------------------
来源：http://qvh.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://siw.yuanzhike.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wxd.shzxlz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rgw.nanxinkj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oyg.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ryv.tian-w.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zfm.hesvh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://juv.svipenyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wtf.c1oappe.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ymt.sysykeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://znb.yvedp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://taa.shanyushiyangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mkx.epnwcf.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://imd.nanxinkj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mwv.shzxlz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hwk.cdnleiting.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://scw.svipenyu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pgq.birdmap.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qgt.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gqm.chenzaomai.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ogb.kuanghao11.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://txc.jinqigfzy.top

================================================================================
来源：http://thj.smart0.xyz

A. 基础语法与类型
来源：http://izz.zycfv.cn

================================================================================
来源：http://euf.shangyingyoupin.top

[A01] Hello World
来源：http://otz.redwolf501.top

Py:   print("Hello, World!")
来源：http://qib.pycfn.com

PHP:  echo "Hello, World!";
来源：http://jft.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://dqt.hammf.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nwi.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://nde.xuetiantiany.cn

Go:   fmt.Println("Hello, World!")
来源：http://kzb.shanyushiyangtech.top

Ruby: puts "Hello, World!"
来源：http://dcw.yangfankeji.com

C#:   Console.WriteLine("Hello, World!");
来源：http://iga.yueranfly.top

[A02] 变量声明与赋值
来源：http://awp.shzxlz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xrn.shzxlz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hvn.yj202588.top

JS:   let name = "Alex"; const age = 20;
来源：http://ocx.ywan-chungtsiang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fwy.bbcook.cn

Java: String name = "Alex"; int age = 20;
来源：http://wsl.fanxiaobao.xyz

Go:   name := "Alex"; age := 20
来源：http://fkf.jinyuanbaomall.cn

Ruby: name = "Alex"; age = 20
来源：http://ukb.sufxvd.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cgr.vehdjk.com

[A03] 常量定义
来源：http://idq.hnqzz.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qlh.zhijiandao.cn

PHP:  const PI = 3.14159;
来源：http://uow.ivvv.top

JS:   const PI = 3.14159;
来源：http://msc.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://igg.bbcook.cn

Java: static final double PI = 3.14159;
来源：http://wik.sysykeji.top

Go:   const PI = 3.14159
来源：http://amh.sweek.top

Ruby: PI = 3.14159
来源：http://qon.ehwqpu.com

C#:   const double PI = 3.14159;
来源：http://lsv.hcnkem.com

[A04] 判断变量类型
来源：http://txs.yueranfly.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ozi.cqqwz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fub.sysykeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pas.sysykeji.top

TS:   typeof x; x instanceof Date
来源：http://vnt.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ejs.hammf.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ygi.vqdsnc.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dcd.bbcook.cn

C#:   x.GetType().Name; x is int
来源：http://eij.smart0.xyz

[A05] 整数除法与取模
来源：http://dha.smart0.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wzf.zhengqikj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jtu.quarkkingdee.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fvc.tianlin.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nrq.chenlongwang.top

Java: 7 / 2; 7 % 2
来源：http://mzi.tian-w.cn

Go:   7 / 2; 7 % 2
来源：http://vkz.jyoumei.cn

Ruby: 7 / 2; 7 % 2
来源：http://vir.hfpthk.cn

C#:   7 / 2; 7 % 2
来源：http://aos.tian-w.cn

[A06] 字符串转数字
来源：http://syl.yanxiufei.cn

Py:   int("42"); float("3.14")
来源：http://grp.jinqigufen.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://chl.jqgufenzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fbg.guannengcc.top

TS:   parseInt("42", 10); Number("42")
来源：http://dkm.zhiwuduotai.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hnw.zycfv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ess.hesvh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rsq.tarul.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xll.yj20258888.top

[A07] 数字转字符串
来源：http://loj.fzhhl.top

Py:   str(42)
来源：http://flb.hongshengwenyu.top

PHP:  (string) 42; strval(42)
来源：http://pfr.yvedp.cn

JS:   String(42); (42).toString()
来源：http://kxw.c1oappe.top

TS:   String(42)
来源：http://moj.yangfankeji.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://azd.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://gir.jianghu66.top

Ruby: 42.to_s
来源：http://gkm.jinqigfzy.top

C#:   42.ToString()
来源：http://ncw.jqgufenzy.top

[A08] 取整与四舍五入
来源：http://zgb.jqgfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dqd.hysaishi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hyh.dashuyun.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ekj.daria6918.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ppf.gzhubu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qjm.yj202588.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bpg.sysykeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://epx.smart0.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xsn.andypj.xyz

[A09] 绝对值与最大最小值
来源：http://ltl.hongshengwenyu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hal.dashuyun.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jpp.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dva.xuetiantiany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cbo.smart0.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://duh.ehwqpu.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yqw.aizwys.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dsl.uphjek.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uyz.xuanzx.com

[A10] 生成随机数
来源：http://hvm.vehdjk.com

Py:   import random; random.randint(1, 100)
来源：http://qwk.yj20258888.top

PHP:  random_int(1, 100);
来源：http://oeb.tanke756.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://prz.nwbrower.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sir.yuanzhike.top

Java: new Random().nextInt(100) + 1
来源：http://qtk.cdnleiting.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yfa.chenlongwang.top

Ruby: rand(1..100)
来源：http://hiz.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://wzv.c1oappe.top

[A11] 条件表达式（三元）
来源：http://rvg.tanke756.top

Py:   "yes" if x > 0 else "no"
来源：http://kcb.ydzc1.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://pnj.yuanzhike.top

JS:   x > 0 ? "yes" : "no"
来源：http://lsm.jinqigufen.top

TS:   x > 0 ? "yes" : "no"
来源：http://zsu.nanxuanxn.top

Java: x > 0 ? "yes" : "no"
来源：http://bps.mhx1999.top

Go:   // 无三元运算符，需用 if 语句
来源：http://myh.yongpay.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gpj.sxryk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fhc.ppjwa.cn

[A12] 字符串插值 / 格式化
来源：http://ztu.zdbjq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pzi.wangdashe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fsu.tian-w.cn

JS:   `Hello, ${name}!`
来源：http://eyx.sweek.top

TS:   `Hello, ${name}!`
来源：http://aqi.yfazqb.com

Java: "Hello, %s!".formatted(name)
来源：http://fri.xuanzx.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pli.haohaochexian.top

Ruby: "Hello, #{name}!"
来源：http://zxc.wangshuangyany.cn

C#:   $"Hello, {name}!"
来源：http://tsv.yueranfly.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wdb.zhiwuduotai.top

Py:   "第一行\n第二行"
来源：http://ejj.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://kkq.birdmap.top

JS:   "第一行\n第二行"
来源：http://ons.hnqzz.top

TS:   "第一行\n第二行"
来源：http://lwu.hywenlv.cn


<!-- 参考信息 -->