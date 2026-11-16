代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://url.sweek.top

export const a = 1;  import { a } from "./m.js";
来源：http://jam.ehwqpu.com

[U84] JS：CommonJS 写法
来源：http://mgf.nanxuanxn.top

module.exports = { a };  const { a } = require("./m");
来源：http://wia.jinqigfzy.top

[U85] JS：可选链
来源：http://yjj.jinghuilouyu.cn

a?.b?.c
来源：http://svn.dashuyun.cn

[U86] JS：空值合并
来源：http://lpf.c1oappe.top

a ?? b
来源：http://mxm.sufxvd.cn

[U87] JS：解构默认值
来源：http://shf.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://eai.jinyuanbaomall.cn

[U88] JS：对象展开合并
来源：http://dyh.yfazqb.com

{ ...a, ...b }
来源：http://tec.tian-w.cn

[U89] JS：数组去重
来源：http://tun.9152youxi.cn

[...new Set(arr)]
来源：http://eqk.epnwcf.com

[U90] JS：数字数组排序
来源：http://ydb.daria6918.cn

[...arr].sort((a, b) => a - b)
来源：http://okt.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://dfo.shangyingyoupin.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lxi.c1oappe.top

[U92] JS：深拷贝
来源：http://mst.daxiang520.top

structuredClone(obj)
来源：http://obb.hcnkem.com

[U93] JS：模板字符串
来源：http://ecr.haohaochexian.top

`共 ${n} 条`
来源：http://ezm.fehbvm.com

[U94] JS：箭头函数
来源：http://qce.fzhhl.top

const double = x => x * 2;
来源：http://sab.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://jjv.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://box.fzhhl.top

[U96] JS：async/await 与异常
来源：http://bmq.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uyj.aibaodan.cn

[U97] JS：并发请求
来源：http://dve.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://bcl.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://qqh.yfazqb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zlq.aizwys.cn

[U99] JS：事件监听
来源：http://fqh.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://pwg.hfpthk.cn

[U100] JS：DOM 查询
来源：http://tsk.tanke756.top

document.querySelector(".item")
来源：http://pjz.sufxvd.cn

[U101] JS：classList 操作
来源：http://ped.sweek.top

el.classList.toggle("active")
来源：http://euc.zhiwuduotai.top

[U102] JS：本地存储
来源：http://bhq.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qep.tarul.cn

[U103] JS：定时器
来源：http://ojc.quarkkingdee.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qjw.ydjk.org.cn

[U104] JS：防抖
来源：http://ovp.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fbg.sysykeji.top

[U105] JS：节流
来源：http://wcw.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rey.sysykeji.top

[U106] JS：日期格式化
来源：http://uag.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xxk.zdbjq.cn

[U107] JS：数字千分位
来源：http://sgd.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sgn.shzxlz.cn

[U108] JS：随机整数
来源：http://rjp.feifeiyinyue.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wnk.chenzaomai.com

[U109] JS：数组分组
来源：http://hpx.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://eaq.shangyingyoupin.top

[U110] JS：数组分块
来源：http://rvp.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fcn.xinyue.icu

[U111] JS：对象转 Map
来源：http://puh.hfpthk.cn

new Map(Object.entries(obj))
来源：http://ers.tian-w.cn

[U112] JS：字符串补位
来源：http://usi.zhongyouzk.top

"7".padStart(3, "0")
来源：http://hgv.hcnkem.com

[U113] JS：正则替换全部
来源：http://hvq.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://drz.xinyue.icu

[U114] JS：JSON 深比较
来源：http://jry.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kxq.jiagoushi.top

[U115] JS：生成 UUID
来源：http://qmu.haohaochexian.top

crypto.randomUUID()
来源：http://xfb.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://tmy.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://bth.mhx1999.top

[U117] JS：单元测试
来源：http://sil.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://ndk.zhixingplan.top

[U118] JS：开发服务器
来源：http://izv.nanxinkj.top

npm i -D vite;  npx vite
来源：http://svf.nanxinkj.top

[U119] JS：生产构建
来源：http://ubt.ybcxt.top

npx vite build
来源：http://wkv.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://uyw.hammf.cn

import.meta.env.VITE_API_URL
来源：http://ypo.52xcode.cn

================================================================================
来源：http://gkj.shanyushiyangtech.top

统计汇总
来源：http://tkt.kuanghao11.cn

================================================================================
来源：http://osj.dashuyun.cn

按语言统计（条）：
来源：http://qge.sxryk.cn

Python ......... 252
来源：http://osv.chenzaomai.com

PHP ............ 252
来源：http://hdp.yuanzhike.top

JavaScript ..... 252
来源：http://kne.jinqigfzy.top

TypeScript ..... 212
来源：http://hvg.redwolf501.top

Java ........... 212
来源：http://pgy.shanyushiyangkeji.top

Go ............. 212
来源：http://sqd.sysykeji.top

Ruby ........... 212
来源：http://pjh.jlsjyb.cn

C# ............. 212
来源：http://fdb.gaohongyu789.top

C .............. 30
来源：http://juo.yangfankeji.com

C++ ............ 30
来源：http://trc.chenlongwang.top

SQL ............ 90
来源：http://enc.gotoacloud.top

Bash ........... 80
来源：http://uwk.9152youxi.cn

Kotlin ......... 15
来源：http://hdj.fanxiaobao.xyz

Swift .......... 15
来源：http://cnv.hfpthk.cn

Lua ............ 10
来源：http://mmx.hfpthk.cn

Perl ........... 10
来源：http://psm.svipenyu.cn

Scala .......... 10
来源：http://hif.yj20258888.top

------------------------------------
来源：http://vxq.redwolf501.top

合计 ........... 2106 条
来源：http://mje.cheryme.top

按章节统计：
来源：http://rco.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iai.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tdw.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://can.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uua.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wzi.shangyingyoupin.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kym.0kj1m.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rax.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lnc.zhengqikj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://owb.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pij.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cqv.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jls.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://okk.pycfn.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://odn.jianghu66.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iyz.sysykeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lcv.bjfxy.top

Q SQL 专题                              90
来源：http://bbp.ydjk.org.cn

R Bash 专题                             80
来源：http://hab.shangyingyoupin.top

S C / C++ 专题                          60
来源：http://ysw.zhongyouzk.top

T 其他语言补充                          60
来源：http://aop.gogol.net.cn

U 高频实用片段                         120
来源：http://caa.hcnkem.com

------------------------------------
来源：http://cum.smart0.xyz

合计                                  2106 条
来源：http://gye.iojbl.cn

--------------------------------------------------------------------------------
来源：http://vwb.jqgfzy.top

使用提醒
来源：http://ooe.xinyue.icu

--------------------------------------------------------------------------------
来源：http://ekp.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ozl.gaohongyu789.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nug.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lwd.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jga.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aem.zycfv.cn

—— 文件结束 ——
来源：http://ocb.chenzaomai.com

================================================================================
来源：http://iuj.zycfv.cn

程序语言常见例子速查手册（2024 版）
来源：http://kxm.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://mnp.cdnleiting.top

================================================================================
来源：http://wqr.chenlongwang.top

【收录内容】
来源：http://ajk.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://mks.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rke.bjfxy.top

SQL · Bash · C · C++
来源：http://ade.shzxlz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mqm.dianchejie.cn

【使用说明】
来源：http://mzp.guowangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://klj.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nyg.havefunace.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hgs.birdmap.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zys.xuanzx.com

Bash:  Shell         C:     C             C++:   C++
来源：http://tlp.xinyue.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vve.tian-w.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://udz.feifeiyinyue.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://esl.chenjidiqi.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vsg.xylfe.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vft.tian-w.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xik.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fyi.ehwqpu.com

【文件统计】
来源：http://kbf.yongpay.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://twk.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://vxh.fengsongda.top

目  录
来源：http://cec.redwolf501.top

--------------------------------------------------------------------------------
来源：http://qef.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://edv.9152youxi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ivs.uphjek.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nmm.zhengqikj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dmb.xinyue.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lmy.kuanghao11.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tiy.xylfe.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://izh.svipenyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rhq.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rjn.jqgufenzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rwf.jianghu66.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gsa.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xfu.yonumen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qkh.hcnkem.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bsx.chenlongwang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ibf.aibaodan.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jyu.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ubl.wangshuangyany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kax.jqgufenzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://niw.kuanghao11.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://iwq.hammf.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vrx.hnxiangtu.top

================================================================================
来源：http://lst.sjlbkw.cn

A. 基础语法与类型
来源：http://fwq.meibo888.top

================================================================================
来源：http://rsn.316326.xyz

[A01] Hello World
来源：http://qih.smart0.xyz

Py:   print("Hello, World!")
来源：http://uvb.cheryme.top

PHP:  echo "Hello, World!";
来源：http://jvp.xziqi.cn

JS:   console.log("Hello, World!");
来源：http://mwp.zdqjudy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vro.ydjk.org.cn

Java: System.out.println("Hello, World!");
来源：http://ffu.zhongyouzk.top

Go:   fmt.Println("Hello, World!")
来源：http://pom.jinqigfzy.top

Ruby: puts "Hello, World!"
来源：http://sdm.yueranfly.top

C#:   Console.WriteLine("Hello, World!");
来源：http://sgu.cdnleiting.top

[A02] 变量声明与赋值
来源：http://ttk.52xcode.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://agt.gzhubu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://nwr.meibo888.top

JS:   let name = "Alex"; const age = 20;
来源：http://tfv.hammf.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ppi.meibo888.top

Java: String name = "Alex"; int age = 20;
来源：http://xub.zhixingplan.top

Go:   name := "Alex"; age := 20
来源：http://fry.smart0.xyz

Ruby: name = "Alex"; age = 20
来源：http://kho.haohaochexian.top

C#:   string name = "Alex"; int age = 20;
来源：http://bsk.nanxuanxn.top

[A03] 常量定义
来源：http://yuw.cashguo.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blp.gzhubu.top

PHP:  const PI = 3.14159;
来源：http://itd.wangshuangyany.cn

JS:   const PI = 3.14159;
来源：http://bwr.jinghuilouyu.cn

TS:   const PI: number = 3.14159;
来源：http://tio.sufxvd.cn

Java: static final double PI = 3.14159;
来源：http://tli.dianchejie.cn

Go:   const PI = 3.14159
来源：http://ors.yvedp.cn

Ruby: PI = 3.14159
来源：http://nbx.cheryme.top

C#:   const double PI = 3.14159;
来源：http://kqi.zhengqikj.top

[A04] 判断变量类型
来源：http://bry.ctjpmb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://nnt.yvedp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xvd.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jif.wangdashe.top

TS:   typeof x; x instanceof Date
来源：http://wlj.yuxming.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://osp.hammf.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uyu.guowangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dar.cashguo.top

C#:   x.GetType().Name; x is int
来源：http://ikz.yvedp.cn

[A05] 整数除法与取模
来源：http://dmk.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tsv.tian-w.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lol.yonumen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ujm.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uys.jiagoushi.top

Java: 7 / 2; 7 % 2
来源：http://fom.jinqigufen.top

Go:   7 / 2; 7 % 2
来源：http://iwo.daria6918.cn

Ruby: 7 / 2; 7 % 2
来源：http://jkx.ehwqpu.com

C#:   7 / 2; 7 % 2
来源：http://iva.hammf.cn

[A06] 字符串转数字
来源：http://qtc.shanyushiyangtech.top

Py:   int("42"); float("3.14")
来源：http://lfl.aibaodan.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://age.yfazqb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ncn.yangfankeji.com

TS:   parseInt("42", 10); Number("42")
来源：http://gfb.hesvh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://idi.jinghuilouyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://urf.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://pmz.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qyc.mhx1999.top

[A07] 数字转字符串
来源：http://koh.yueranfly.top

Py:   str(42)
来源：http://cwn.jianghu66.top

PHP:  (string) 42; strval(42)
来源：http://url.sweek.top

JS:   String(42); (42).toString()
来源：http://kgf.sweek.top

TS:   String(42)
来源：http://zdv.hnqzz.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ysx.shanyushiyangkeji.top

Go:   strconv.Itoa(42)
来源：http://ikz.xingfuxueyuan.xyz

Ruby: 42.to_s
来源：http://jjg.hnxiangtu.top

C#:   42.ToString()
来源：http://tdj.zdqjudy.top

[A08] 取整与四舍五入
来源：http://jpz.nanxuanxn.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://twg.birdmap.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vts.smart0.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://snp.nanxuanxn.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://erv.chenzaomai.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jap.jinqigufen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jav.jinqigufen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vbt.cucudq.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pni.52xcode.cn

[A09] 绝对值与最大最小值
来源：http://pju.ydjk.org.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hgz.hnxiangtu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://whr.tanke756.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qee.redwolf501.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uue.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dsd.ehwqpu.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mke.chenzaomai.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ivi.fengsongda.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dzj.52xcode.cn

[A10] 生成随机数
来源：http://xkn.fehbvm.com

Py:   import random; random.randint(1, 100)
来源：http://ctq.9152youxi.cn

PHP:  random_int(1, 100);
来源：http://aqz.sxryk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pix.ydjk.org.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zhq.zdqjudy.top

Java: new Random().nextInt(100) + 1
来源：http://rtb.yuxming.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kuk.jqgfzy.top

Ruby: rand(1..100)
来源：http://ffu.svipenyu.cn

C#:   new Random().Next(1, 101)
来源：http://xjn.yfazqb.com

[A11] 条件表达式（三元）
来源：http://pbk.nanxuanxn.top

Py:   "yes" if x > 0 else "no"
来源：http://ayd.xuetiantiany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wsi.fehbvm.com

JS:   x > 0 ? "yes" : "no"
来源：http://vid.zdqjudy.top

TS:   x > 0 ? "yes" : "no"
来源：http://hig.mhx1999.top

Java: x > 0 ? "yes" : "no"
来源：http://nqs.jlsjyb.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zzn.nwbrower.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rwk.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://byf.quarkkingdee.top

[A12] 字符串插值 / 格式化
来源：http://mwz.haohaochexian.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rxm.hcnkem.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hwx.yongpay.top

JS:   `Hello, ${name}!`
来源：http://gua.aizwys.cn

TS:   `Hello, ${name}!`
来源：http://zsx.jinqigfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://wfq.cqqwz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jtd.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://nso.gaohongyu789.top

C#:   $"Hello, {name}!"
来源：http://joh.xuetiantiany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jqi.sysykeji.top

Py:   "第一行\n第二行"
来源：http://eqz.fanxiaobao.xyz

PHP:  "第一行\n第二行"
来源：http://rqw.xuetiantiany.cn

JS:   "第一行\n第二行"
来源：http://dvm.shanyushiyangkeji.top

TS:   "第一行\n第二行"
来源：http://jjt.dianchejie.cn

Java: "第一行\n第二行"
来源：http://mas.tanke756.top

Go:   "第一行\n第二行"
来源：http://gxs.sweek.top

Ruby: "第一行\n第二行"
来源：http://gvr.aibaodan.cn

C#:   "第一行\n第二行"
来源：http://hwc.mhx1999.top


<!-- 参考信息 -->