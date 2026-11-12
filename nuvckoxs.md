代发 wailian999

[U79] PHP：静态分析
来源：http://ioi.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://guj.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://cgx.chenlongwang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nji.nanxuanxn.top

[U81] JS：初始化项目
来源：http://xpy.aibaodan.cn

npm init -y;  npm i express
来源：http://wme.jinghuilouyu.cn

[U82] JS：package.json 脚本
来源：http://bvq.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nzf.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://cim.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://irf.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://kcd.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cyn.uphjek.com

[U85] JS：可选链
来源：http://miw.sweek.top

a?.b?.c
来源：http://pif.zhengqikj.top

[U86] JS：空值合并
来源：http://ktw.feifeiyinyue.top

a ?? b
来源：http://mdl.hysaishi.cn

[U87] JS：解构默认值
来源：http://jpo.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://qkg.xinyue.icu

[U88] JS：对象展开合并
来源：http://vdy.sjlbkw.cn

{ ...a, ...b }
来源：http://mxq.ivvv.top

[U89] JS：数组去重
来源：http://odn.chenzaomai.com

[...new Set(arr)]
来源：http://cyo.guannengcc.top

[U90] JS：数字数组排序
来源：http://ydi.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://uvt.andypj.xyz

[U91] JS：对象键值遍历
来源：http://cgz.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://okc.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://erm.zhoulong.xyz

structuredClone(obj)
来源：http://bkp.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://jlq.kuanghao11.cn

`共 ${n} 条`
来源：http://mra.dianchejie.cn

[U94] JS：箭头函数
来源：http://ind.xylfe.cn

const double = x => x * 2;
来源：http://mmy.yueranfly.top

[U95] JS：Promise 包装
来源：http://mob.jinghuilouyu.cn

new Promise((resolve, reject) => {})
来源：http://pvc.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://oxo.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pkt.yuanzhike.top

[U97] JS：并发请求
来源：http://iwp.epnwcf.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://qyd.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://pjy.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://krh.pengpengdd.cyou

[U99] JS：事件监听
来源：http://qoa.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://ejr.hywenlv.cn

[U100] JS：DOM 查询
来源：http://fng.meibo888.top

document.querySelector(".item")
来源：http://zge.nanxuanxn.top

[U101] JS：classList 操作
来源：http://qew.ivvv.top

el.classList.toggle("active")
来源：http://alz.gogol.net.cn

[U102] JS：本地存储
来源：http://oaf.yongpay.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xbu.hywenlv.cn

[U103] JS：定时器
来源：http://pxf.xziqi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ste.xziqi.cn

[U104] JS：防抖
来源：http://vpr.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ney.snrcjt.cn

[U105] JS：节流
来源：http://fkx.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://acq.yfazqb.com

[U106] JS：日期格式化
来源：http://bne.snrcjt.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mls.bjfxy.top

[U107] JS：数字千分位
来源：http://xaq.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://omr.nanxuanxn.top

[U108] JS：随机整数
来源：http://gvn.xuanzx.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://drh.daxiang520.top

[U109] JS：数组分组
来源：http://qvb.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://txf.sxryk.cn

[U110] JS：数组分块
来源：http://lae.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nxd.ywan-chungtsiang.top

[U111] JS：对象转 Map
来源：http://tdm.sweek.top

new Map(Object.entries(obj))
来源：http://lpa.dashuyun.cn

[U112] JS：字符串补位
来源：http://cex.jyoumei.cn

"7".padStart(3, "0")
来源：http://miu.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://nkc.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://ypx.hnqzz.top

[U114] JS：JSON 深比较
来源：http://wlx.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://zhy.gogol.net.cn

[U115] JS：生成 UUID
来源：http://bmq.hnqzz.top

crypto.randomUUID()
来源：http://jeu.hesvh.cn

[U116] JS：类型检查（JSDoc）
来源：http://jmy.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://isr.zhixingplan.top

[U117] JS：单元测试
来源：http://zcd.uphjek.com

npm i -D vitest;  npx vitest
来源：http://ujm.yfazqb.com

[U118] JS：开发服务器
来源：http://wsu.aibaodan.cn

npm i -D vite;  npx vite
来源：http://eit.shuidangran.top

[U119] JS：生产构建
来源：http://vtu.shanyushiyangkeji.top

npx vite build
来源：http://hkx.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://pxv.hesvh.cn

import.meta.env.VITE_API_URL
来源：http://kzk.jinghuilouyu.cn

================================================================================
来源：http://jdv.zhiwuduotai.top

统计汇总
来源：http://wcx.316326.xyz

================================================================================
来源：http://maz.snrcjt.cn

按语言统计（条）：
来源：http://pjw.shuidangran.top

Python ......... 252
来源：http://vez.shuidangran.top

PHP ............ 252
来源：http://scq.nanxuanxn.top

JavaScript ..... 252
来源：http://rru.vqdsnc.cn

TypeScript ..... 212
来源：http://dnb.wangdashe.top

Java ........... 212
来源：http://gpy.jianghu66.top

Go ............. 212
来源：http://rci.daxiang520.top

Ruby ........... 212
来源：http://rpr.snrcjt.cn

C# ............. 212
来源：http://aqg.wangshuangyany.cn

C .............. 30
来源：http://kop.hysaishi.cn

C++ ............ 30
来源：http://sac.0kj1m.cn

SQL ............ 90
来源：http://cdm.xuanzx.com

Bash ........... 80
来源：http://dsj.kuanghao11.cn

Kotlin ......... 15
来源：http://nop.sysykeji.top

Swift .......... 15
来源：http://ftv.tanke756.top

Lua ............ 10
来源：http://ibc.yuxming.cn

Perl ........... 10
来源：http://bfx.yj20258.top

Scala .......... 10
来源：http://wlk.zhixingplan.top

------------------------------------
来源：http://jpa.haohaochexian.top

合计 ........... 2106 条
来源：http://dhw.hesvh.cn

按章节统计：
来源：http://qjm.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gix.gzhubu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://diz.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iwg.birdmap.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qgm.xziqi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rcy.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jsi.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mwu.andypj.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fyu.haohaochexian.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ycc.ppjwa.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fry.gogol.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dfb.xuanzx.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uih.aizwys.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gvm.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rbt.hfpthk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zrv.yuxming.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zju.sxryk.cn

Q SQL 专题                              90
来源：http://nkd.52xcode.cn

R Bash 专题                             80
来源：http://viz.ctjpmb.com

S C / C++ 专题                          60
来源：http://yis.jinqigfzy.top

T 其他语言补充                          60
来源：http://ccb.shzxlz.cn

U 高频实用片段                         120
来源：http://mvd.sxryk.cn

------------------------------------
来源：http://bag.shanyushiyangtech.top

合计                                  2106 条
来源：http://nzh.epnwcf.com

--------------------------------------------------------------------------------
来源：http://jon.yonumen.top

使用提醒
来源：http://rpa.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://ybl.havefunace.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jlm.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ujo.cashguo.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rnw.cdnleiting.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bes.hfpthk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://paf.gogol.net.cn

—— 文件结束 ——
来源：http://gcj.chenjidiqi.icu

================================================================================
来源：http://sgi.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://edu.zdqjudy.top

Common Programming Examples Cheat Book
来源：http://kbk.shangyingyoupin.top

================================================================================
来源：http://ngu.cqqwz.cn

【收录内容】
来源：http://nxr.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://chk.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kmk.fengsongda.top

SQL · Bash · C · C++
来源：http://owo.shanyushiyangtech.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://djf.shanyushiyangtech.top

【使用说明】
来源：http://ony.svipenyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uoe.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ybk.ehwqpu.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://aym.hnqzz.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://myg.zhaomingkeji.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://xvf.zhixingplan.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fmh.uphjek.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://okn.jinghuilouyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bls.chenlongwang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://frv.yuanzhike.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xrp.shanyushiyangtech.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hqe.svipenyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bkf.ydjk.org.cn

【文件统计】
来源：http://anu.pycfn.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kwn.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://djd.jinqigufen.top

目  录
来源：http://qkp.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://eug.kuanghao11.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lcy.yj20258.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gqf.fzhhl.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ltr.yonumen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lsl.havefunace.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://auc.feifeiyinyue.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jhs.c1oappe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kgv.gaohongyu789.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ulw.zdbjq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aqe.jinyuanbaomall.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vkg.pycfn.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zhi.fktsv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ycp.xinyue.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eme.tarul.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xsh.epnwcf.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lgk.zdbjq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dqy.yfazqb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://shn.shzxlz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sok.yueranfly.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://svg.jinyuanbaomall.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ugp.zhoulong.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://goh.ehwqpu.com

================================================================================
来源：http://syb.zycfv.cn

A. 基础语法与类型
来源：http://wbu.yueranfly.top

================================================================================
来源：http://hrc.nwbrower.top

[A01] Hello World
来源：http://cdk.chenjidiqi.icu

Py:   print("Hello, World!")
来源：http://dys.tarul.cn

PHP:  echo "Hello, World!";
来源：http://laq.fengsongda.top

JS:   console.log("Hello, World!");
来源：http://isl.zhoulong.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pcg.gzhubu.top

Java: System.out.println("Hello, World!");
来源：http://wdl.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://pgz.cdnleiting.top

Ruby: puts "Hello, World!"
来源：http://mxn.zdqjudy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hhj.guannengcc.top

[A02] 变量声明与赋值
来源：http://lse.ydzc1.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xjh.kuanghao11.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rzs.gotoacloud.top

JS:   let name = "Alex"; const age = 20;
来源：http://opn.bbcook.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qsh.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://tui.vqdsnc.cn

Go:   name := "Alex"; age := 20
来源：http://tuy.yj20258.top

Ruby: name = "Alex"; age = 20
来源：http://crf.xinyue.icu

C#:   string name = "Alex"; int age = 20;
来源：http://yjl.0kj1m.cn

[A03] 常量定义
来源：http://cff.yuanzhike.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xgh.ydzc1.top

PHP:  const PI = 3.14159;
来源：http://kmr.daxiang520.top

JS:   const PI = 3.14159;
来源：http://yva.sweek.top

TS:   const PI: number = 3.14159;
来源：http://swm.fktsv.cn

Java: static final double PI = 3.14159;
来源：http://ohm.vehdjk.com

Go:   const PI = 3.14159
来源：http://thf.jqgufenzy.top

Ruby: PI = 3.14159
来源：http://rar.chenjidiqi.icu

C#:   const double PI = 3.14159;
来源：http://ors.yj202588.top

[A04] 判断变量类型
来源：http://awc.iojbl.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hju.zdbjq.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://scl.hnxiangtu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ozu.hysaishi.cn

TS:   typeof x; x instanceof Date
来源：http://kel.epnwcf.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xph.zhengqikj.top

Go:   reflect.TypeOf(x).Name()
来源：http://kbw.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fxy.pycfn.com

C#:   x.GetType().Name; x is int
来源：http://xjy.uphjek.com

[A05] 整数除法与取模
来源：http://abf.fktsv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sxr.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kgm.hcnkem.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cxw.jlsjyb.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pmm.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://iyf.jqgfzy.top

Go:   7 / 2; 7 % 2
来源：http://bja.fehbvm.com

Ruby: 7 / 2; 7 % 2
来源：http://arx.tianlin.xyz

C#:   7 / 2; 7 % 2
来源：http://bux.smart0.xyz

[A06] 字符串转数字
来源：http://iuk.aibaodan.cn

Py:   int("42"); float("3.14")
来源：http://zyd.pycfn.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zyk.sweek.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pqg.hywenlv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zzc.shanyushiyangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uop.gogol.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gdw.zdbjq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yij.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pth.jinyuanbaomall.cn

[A07] 数字转字符串
来源：http://jcu.pengpengdd.cyou

Py:   str(42)
来源：http://tcd.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://ovt.redwolf501.top

JS:   String(42); (42).toString()
来源：http://wtw.pycfn.com

TS:   String(42)
来源：http://smx.0kj1m.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vzz.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://jpr.andypj.xyz

Ruby: 42.to_s
来源：http://uwr.xziqi.cn

C#:   42.ToString()
来源：http://yny.vqdsnc.cn

[A08] 取整与四舍五入
来源：http://kct.cashguo.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wim.xziqi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mex.hesvh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://evw.nwbrower.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zob.epnwcf.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://twx.shangyingyoupin.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pdd.yangfankeji.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://krw.yuanzhike.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xnw.dianchejie.cn

[A09] 绝对值与最大最小值
来源：http://zsn.tian-w.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bdf.dianchejie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bqv.9152youxi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yeo.fzhhl.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rpl.gotoacloud.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hef.sjlbkw.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eiq.gzhubu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hqq.hcnkem.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bqa.tian-w.cn

[A10] 生成随机数
来源：http://yek.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://etu.xuetiantiany.cn

PHP:  random_int(1, 100);
来源：http://ydp.fengsongda.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://img.yongpay.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mtw.fehbvm.com

Java: new Random().nextInt(100) + 1
来源：http://kgy.jyoumei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mar.vehdjk.com

Ruby: rand(1..100)
来源：http://zgh.daria6918.cn

C#:   new Random().Next(1, 101)
来源：http://gja.ctjpmb.com

[A11] 条件表达式（三元）
来源：http://aut.hongshengwenyu.top

Py:   "yes" if x > 0 else "no"
来源：http://nhm.shanyushiyangtech.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fmb.fanxiaobao.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://arf.zhaomingkeji.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://mzh.ehwqpu.com

Java: x > 0 ? "yes" : "no"
来源：http://bgv.jinyuanbaomall.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qdk.gogol.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://elc.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fbc.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://dfk.wangshuangyany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dxo.meibo888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nkc.zhengqikj.top

JS:   `Hello, ${name}!`
来源：http://chw.meibo888.top

TS:   `Hello, ${name}!`
来源：http://axt.snrcjt.cn

Java: "Hello, %s!".formatted(name)
来源：http://ljr.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hdv.52xcode.cn

Ruby: "Hello, #{name}!"
来源：http://qfk.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://els.shanyushiyangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rod.ivvv.top


<!-- 参考信息 -->