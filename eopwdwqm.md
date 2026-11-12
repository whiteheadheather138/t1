代发 wailian999

[U79] PHP：静态分析
来源：http://aod.yfazqb.com

composer require --dev phpstan/phpstan
来源：http://pnn.bbcook.cn

[U80] PHP：代码规范修复
来源：http://kun.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xgx.guowangkeji.top

[U81] JS：初始化项目
来源：http://snd.feifeiyinyue.top

npm init -y;  npm i express
来源：http://wvk.gotoacloud.top

[U82] JS：package.json 脚本
来源：http://luh.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nhf.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://sye.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://otl.316326.xyz

[U84] JS：CommonJS 写法
来源：http://clu.birdmap.top

module.exports = { a };  const { a } = require("./m");
来源：http://ney.xuanzx.com

[U85] JS：可选链
来源：http://obl.jqgfzy.top

a?.b?.c
来源：http://azs.aibaodan.cn

[U86] JS：空值合并
来源：http://wvw.ywan-chungtsiang.top

a ?? b
来源：http://xnk.jinghuilouyu.cn

[U87] JS：解构默认值
来源：http://epf.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://umm.sjlbkw.cn

[U88] JS：对象展开合并
来源：http://tzs.zhongyouzk.top

{ ...a, ...b }
来源：http://rlm.hywenlv.cn

[U89] JS：数组去重
来源：http://src.fengsongda.top

[...new Set(arr)]
来源：http://iqg.ctjpmb.com

[U90] JS：数字数组排序
来源：http://mpq.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://vfv.cucudq.cn

[U91] JS：对象键值遍历
来源：http://ide.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lvs.ivvv.top

[U92] JS：深拷贝
来源：http://zwq.fehbvm.com

structuredClone(obj)
来源：http://ppp.jinqigufen.top

[U93] JS：模板字符串
来源：http://ege.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://frx.yongpay.top

[U94] JS：箭头函数
来源：http://eew.chenlongwang.top

const double = x => x * 2;
来源：http://gus.havefunace.top

[U95] JS：Promise 包装
来源：http://ymu.0kj1m.cn

new Promise((resolve, reject) => {})
来源：http://wxy.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://zzw.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fim.pengpengdd.cyou

[U97] JS：并发请求
来源：http://isk.tarul.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yps.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://lgd.gotoacloud.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oem.hywenlv.cn

[U99] JS：事件监听
来源：http://czq.ybcxt.top

el.addEventListener("click", e => {})
来源：http://bpt.guowangkeji.top

[U100] JS：DOM 查询
来源：http://jxf.guowangkeji.top

document.querySelector(".item")
来源：http://hoq.iojbl.cn

[U101] JS：classList 操作
来源：http://atu.chenzaomai.com

el.classList.toggle("active")
来源：http://vmk.kuanghao11.cn

[U102] JS：本地存储
来源：http://mjh.hesvh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fpg.shanyushiyangtech.top

[U103] JS：定时器
来源：http://gvz.hongshengwenyu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wmc.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://cng.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vtr.xziqi.cn

[U105] JS：节流
来源：http://qdm.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vog.ywan-chungtsiang.top

[U106] JS：日期格式化
来源：http://qfc.zhaomingkeji.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iau.cashguo.top

[U107] JS：数字千分位
来源：http://gwc.guowangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://htq.tianlin.xyz

[U108] JS：随机整数
来源：http://xxy.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yrz.ydjk.org.cn

[U109] JS：数组分组
来源：http://sdr.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://pqf.gaohongyu789.top

[U110] JS：数组分块
来源：http://zmn.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lvc.hysaishi.cn

[U111] JS：对象转 Map
来源：http://wnr.sxryk.cn

new Map(Object.entries(obj))
来源：http://gtr.hnqzz.top

[U112] JS：字符串补位
来源：http://kqz.yfazqb.com

"7".padStart(3, "0")
来源：http://zus.sweek.top

[U113] JS：正则替换全部
来源：http://pvc.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://blu.meibo888.top

[U114] JS：JSON 深比较
来源：http://fvs.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://cfd.tian-w.cn

[U115] JS：生成 UUID
来源：http://qkf.iojbl.cn

crypto.randomUUID()
来源：http://vpz.chenlongwang.top

[U116] JS：类型检查（JSDoc）
来源：http://lza.yongpay.top

/** @param {string} name */ function f(name) {}
来源：http://hrn.pengpengdd.cyou

[U117] JS：单元测试
来源：http://cvg.dashuyun.cn

npm i -D vitest;  npx vitest
来源：http://aon.hcnkem.com

[U118] JS：开发服务器
来源：http://htl.redwolf501.top

npm i -D vite;  npx vite
来源：http://gvd.tarul.cn

[U119] JS：生产构建
来源：http://voa.hcnkem.com

npx vite build
来源：http://wnw.ivvv.top

[U120] JS：读取环境变量（Vite）
来源：http://vlh.shuidangran.top

import.meta.env.VITE_API_URL
来源：http://zvd.fanxiaobao.xyz

================================================================================
来源：http://msc.tarul.cn

统计汇总
来源：http://xzq.jlsjyb.cn

================================================================================
来源：http://kzp.sysykeji.top

按语言统计（条）：
来源：http://wjm.zdbjq.cn

Python ......... 252
来源：http://ptw.xylfe.cn

PHP ............ 252
来源：http://pms.zhixingplan.top

JavaScript ..... 252
来源：http://hhc.chenjidiqi.icu

TypeScript ..... 212
来源：http://dbs.jiagoushi.top

Java ........... 212
来源：http://cop.zdqjudy.top

Go ............. 212
来源：http://ihz.hnqzz.top

Ruby ........... 212
来源：http://aub.cqqwz.cn

C# ............. 212
来源：http://tnf.ppjwa.cn

C .............. 30
来源：http://dqb.ppjwa.cn

C++ ............ 30
来源：http://ohv.kuanghao11.cn

SQL ............ 90
来源：http://pmf.nwbrower.top

Bash ........... 80
来源：http://nsx.zdbjq.cn

Kotlin ......... 15
来源：http://ian.yanxiufei.cn

Swift .......... 15
来源：http://owm.mhx1999.top

Lua ............ 10
来源：http://elw.ybcxt.top

Perl ........... 10
来源：http://ulv.sweek.top

Scala .......... 10
来源：http://nds.ivvv.top

------------------------------------
来源：http://idc.jiagoushi.top

合计 ........... 2106 条
来源：http://rme.zhixingplan.top

按章节统计：
来源：http://xhm.smart0.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://njk.jianghu66.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jbz.hysaishi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://und.guannengcc.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ijb.ppjwa.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uld.fehbvm.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://igs.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hnr.shanyushiyangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uib.yanxiufei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jtn.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wqq.haohaochexian.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ixb.cucudq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xwh.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pte.ctjpmb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tfr.sjlbkw.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vbd.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vat.gzhubu.top

Q SQL 专题                              90
来源：http://eum.cdnleiting.top

R Bash 专题                             80
来源：http://luy.jianghu66.top

S C / C++ 专题                          60
来源：http://lmz.xuetiantiany.cn

T 其他语言补充                          60
来源：http://qyr.52xcode.cn

U 高频实用片段                         120
来源：http://ggh.shanyushiyangtech.top

------------------------------------
来源：http://imi.pycfn.com

合计                                  2106 条
来源：http://vab.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://ysk.tanke756.top

使用提醒
来源：http://xve.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://dyv.sweek.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://icz.redwolf501.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tia.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uid.yanxiufei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lpz.yonumen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zhd.ywan-chungtsiang.top

—— 文件结束 ——
来源：http://nnf.tian-w.cn

================================================================================
来源：http://vec.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://dik.xziqi.cn

Common Programming Examples Cheat Book
来源：http://krh.ppjwa.cn

================================================================================
来源：http://nci.fehbvm.com

【收录内容】
来源：http://jiv.nanxinkj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://epz.sxryk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://stu.jinqigfzy.top

SQL · Bash · C · C++
来源：http://klp.fktsv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uvu.cucudq.cn

【使用说明】
来源：http://rns.shzxlz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://juj.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ymo.chenjidiqi.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bnh.zhengqikj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mit.xuanzx.com

Bash:  Shell         C:     C             C++:   C++
来源：http://lzs.daxiang520.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jbh.shuidangran.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qdv.dianchejie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mbk.ctjpmb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jqt.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jqp.epnwcf.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oxj.ivvv.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://udu.fktsv.cn

【文件统计】
来源：http://nif.c1oappe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jkd.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://irj.wangshuangyany.cn

目  录
来源：http://ngw.guannengcc.top

--------------------------------------------------------------------------------
来源：http://pfb.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://idk.aizwys.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qpd.fengsongda.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lui.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://loo.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oje.c1oappe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ldv.ybcxt.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xtm.52xcode.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pvn.ppjwa.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uts.quarkkingdee.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vhh.hnxiangtu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pvk.sysykeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lrl.xuanzx.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jmr.yangfankeji.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pmc.shzxlz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://syt.ctjpmb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kpj.zhixingplan.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vmv.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fdz.fehbvm.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mef.hywenlv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wzt.redwolf501.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kec.jianghu66.top

================================================================================
来源：http://agy.zhoulong.xyz

A. 基础语法与类型
来源：http://gwc.smart0.xyz

================================================================================
来源：http://aak.0kj1m.cn

[A01] Hello World
来源：http://dex.pycfn.com

Py:   print("Hello, World!")
来源：http://ocy.uphjek.com

PHP:  echo "Hello, World!";
来源：http://qom.zycfv.cn

JS:   console.log("Hello, World!");
来源：http://fsa.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tnd.shzxlz.cn

Java: System.out.println("Hello, World!");
来源：http://ivt.zhixingplan.top

Go:   fmt.Println("Hello, World!")
来源：http://thm.yj20258.top

Ruby: puts "Hello, World!"
来源：http://ypf.cashguo.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zye.9152youxi.cn

[A02] 变量声明与赋值
来源：http://vrw.zdqjudy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gmh.hcnkem.com

PHP:  $name = "Alex"; $age = 20;
来源：http://nse.iojbl.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zpr.pengpengdd.cyou

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dkl.quarkkingdee.top

Java: String name = "Alex"; int age = 20;
来源：http://qal.smart0.xyz

Go:   name := "Alex"; age := 20
来源：http://ldx.pengpengdd.cyou

Ruby: name = "Alex"; age = 20
来源：http://jbp.jlsjyb.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kgb.guannengcc.top

[A03] 常量定义
来源：http://nny.hywenlv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qtq.zhengqikj.top

PHP:  const PI = 3.14159;
来源：http://xip.jinyuanbaomall.cn

JS:   const PI = 3.14159;
来源：http://upx.xuanzx.com

TS:   const PI: number = 3.14159;
来源：http://iuw.zdqjudy.top

Java: static final double PI = 3.14159;
来源：http://ykw.zhiwuduotai.top

Go:   const PI = 3.14159
来源：http://jzx.hfpthk.cn

Ruby: PI = 3.14159
来源：http://wfw.andypj.xyz

C#:   const double PI = 3.14159;
来源：http://jzx.hongshengwenyu.top

[A04] 判断变量类型
来源：http://bjr.haohaochexian.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://nhv.yj202588.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uem.tian-w.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ltx.fzhhl.top

TS:   typeof x; x instanceof Date
来源：http://qkx.havefunace.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lgr.cashguo.top

Go:   reflect.TypeOf(x).Name()
来源：http://mza.yj202588.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qvi.ehwqpu.com

C#:   x.GetType().Name; x is int
来源：http://uje.tian-w.cn

[A05] 整数除法与取模
来源：http://elo.sufxvd.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eap.smart0.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://fhw.guannengcc.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://udq.hywenlv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bpx.yueranfly.top

Java: 7 / 2; 7 % 2
来源：http://yvd.hysaishi.cn

Go:   7 / 2; 7 % 2
来源：http://euq.jyoumei.cn

Ruby: 7 / 2; 7 % 2
来源：http://rzl.shuidangran.top

C#:   7 / 2; 7 % 2
来源：http://cta.zdqjudy.top

[A06] 字符串转数字
来源：http://tnf.52xcode.cn

Py:   int("42"); float("3.14")
来源：http://qrw.xuetiantiany.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gcr.chenzaomai.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://arc.jianghu66.top

TS:   parseInt("42", 10); Number("42")
来源：http://ags.uphjek.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dsb.ehwqpu.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xzu.feifeiyinyue.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hfh.jiagoushi.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nrh.ctjpmb.com

[A07] 数字转字符串
来源：http://yoh.jiagoushi.top

Py:   str(42)
来源：http://jmt.aibaodan.cn

PHP:  (string) 42; strval(42)
来源：http://tar.guannengcc.top

JS:   String(42); (42).toString()
来源：http://llm.daxiang520.top

TS:   String(42)
来源：http://qwq.zhoulong.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://kvw.vqdsnc.cn

Go:   strconv.Itoa(42)
来源：http://ley.tarul.cn

Ruby: 42.to_s
来源：http://vyp.feifeiyinyue.top

C#:   42.ToString()
来源：http://lkp.hywenlv.cn

[A08] 取整与四舍五入
来源：http://iuy.meibo888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eqm.xuanzx.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://klo.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jod.jinqigufen.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eqp.hfpthk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nga.ppjwa.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://epb.yj20258.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vau.tianlin.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://een.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://pkv.ehwqpu.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dkw.yuanzhike.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://unr.chenjidiqi.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bpd.yangfankeji.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tqa.tanke756.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://urv.nanxuanxn.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gxc.iojbl.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ygp.chenzaomai.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hlc.jiagoushi.top

[A10] 生成随机数
来源：http://erc.fktsv.cn

Py:   import random; random.randint(1, 100)
来源：http://jpa.ivvv.top

PHP:  random_int(1, 100);
来源：http://brn.zhixingplan.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xad.jiagoushi.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zds.zdbjq.cn

Java: new Random().nextInt(100) + 1
来源：http://czq.9152youxi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ini.9152youxi.cn

Ruby: rand(1..100)
来源：http://luu.xziqi.cn

C#:   new Random().Next(1, 101)
来源：http://ldk.hysaishi.cn

[A11] 条件表达式（三元）
来源：http://gmh.nanxinkj.top

Py:   "yes" if x > 0 else "no"
来源：http://pcd.quarkkingdee.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ufz.fengsongda.top

JS:   x > 0 ? "yes" : "no"
来源：http://ugf.jiagoushi.top

TS:   x > 0 ? "yes" : "no"
来源：http://rbe.52xcode.cn

Java: x > 0 ? "yes" : "no"
来源：http://bpi.vqdsnc.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://inz.ywan-chungtsiang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rag.chenlongwang.top

C#:   x > 0 ? "yes" : "no"
来源：http://hha.gotoacloud.top

[A12] 字符串插值 / 格式化
来源：http://uuf.uphjek.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gpx.shuidangran.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cmq.nwbrower.top

JS:   `Hello, ${name}!`
来源：http://wyi.nanxinkj.top

TS:   `Hello, ${name}!`
来源：http://rtx.gzhubu.top

Java: "Hello, %s!".formatted(name)
来源：http://nqx.hywenlv.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nwt.jinqigfzy.top

Ruby: "Hello, #{name}!"
来源：http://ofg.hnxiangtu.top

C#:   $"Hello, {name}!"
来源：http://dvb.pengpengdd.cyou

[A13] 多行字符串（练习 \n 转义）
来源：http://juv.snrcjt.cn


<!-- 参考信息 -->