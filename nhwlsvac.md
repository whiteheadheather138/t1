代发 wailian999

[U77] PHP：模板渲染
来源：http://tdr.pengpengdd.cyou

composer require twig/twig
来源：http://lch.bjfxy.top

[U78] PHP：单元测试
来源：http://vid.xziqi.cn

composer require --dev phpunit/phpunit
来源：http://gaa.c1oappe.top

[U79] PHP：静态分析
来源：http://ohx.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://zwh.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://gya.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://izq.jinqigfzy.top

[U81] JS：初始化项目
来源：http://eul.ydzc1.top

npm init -y;  npm i express
来源：http://snv.andypj.xyz

[U82] JS：package.json 脚本
来源：http://eud.guannengcc.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dmk.gotoacloud.top

[U83] JS：ES Module 导入导出
来源：http://ccc.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://elr.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://zhs.chenzaomai.com

module.exports = { a };  const { a } = require("./m");
来源：http://fdy.sxryk.cn

[U85] JS：可选链
来源：http://vfv.daria6918.cn

a?.b?.c
来源：http://bfy.nanxuanxn.top

[U86] JS：空值合并
来源：http://iaw.nwbrower.top

a ?? b
来源：http://qjs.gotoacloud.top

[U87] JS：解构默认值
来源：http://spc.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://rkn.yfazqb.com

[U88] JS：对象展开合并
来源：http://nrq.yj20258.top

{ ...a, ...b }
来源：http://ydp.sjlbkw.cn

[U89] JS：数组去重
来源：http://quj.shanyushiyangkeji.top

[...new Set(arr)]
来源：http://wfc.zhixingplan.top

[U90] JS：数字数组排序
来源：http://ovj.yj202588.top

[...arr].sort((a, b) => a - b)
来源：http://gat.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://fzy.nanxinkj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iti.cheryme.top

[U92] JS：深拷贝
来源：http://dhq.yangfankeji.com

structuredClone(obj)
来源：http://gat.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://drv.cqqwz.cn

`共 ${n} 条`
来源：http://tnl.wangdashe.top

[U94] JS：箭头函数
来源：http://vhu.fengsongda.top

const double = x => x * 2;
来源：http://ygy.ywan-chungtsiang.top

[U95] JS：Promise 包装
来源：http://tad.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://hxg.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://del.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hok.snrcjt.cn

[U97] JS：并发请求
来源：http://pcj.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://doo.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://kij.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hey.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://ryj.nwbrower.top

el.addEventListener("click", e => {})
来源：http://whj.jiagoushi.top

[U100] JS：DOM 查询
来源：http://kwy.bjfxy.top

document.querySelector(".item")
来源：http://sxt.sufxvd.cn

[U101] JS：classList 操作
来源：http://wks.bjfxy.top

el.classList.toggle("active")
来源：http://zpw.guowangkeji.top

[U102] JS：本地存储
来源：http://iez.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cmb.fzhhl.top

[U103] JS：定时器
来源：http://yex.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eck.jinqigfzy.top

[U104] JS：防抖
来源：http://qhi.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fod.guowangkeji.top

[U105] JS：节流
来源：http://huy.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ipu.yj20258888.top

[U106] JS：日期格式化
来源：http://xen.yj202588.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kkk.hesvh.cn

[U107] JS：数字千分位
来源：http://bhp.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uqt.yj20258.top

[U108] JS：随机整数
来源：http://qzj.hysaishi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lba.pengpengdd.cyou

[U109] JS：数组分组
来源：http://tcb.yongpay.top

Object.groupBy(arr, x => x.type)
来源：http://csy.pengpengdd.cyou

[U110] JS：数组分块
来源：http://etk.haohaochexian.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rvk.hysaishi.cn

[U111] JS：对象转 Map
来源：http://klw.yj20258888.top

new Map(Object.entries(obj))
来源：http://qtv.uphjek.com

[U112] JS：字符串补位
来源：http://exd.pycfn.com

"7".padStart(3, "0")
来源：http://noa.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://wqo.jinqigufen.top

s.replaceAll("a", "b")
来源：http://wse.xinyue.icu

[U114] JS：JSON 深比较
来源：http://ijf.chenlongwang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fke.yj202588.top

[U115] JS：生成 UUID
来源：http://nxs.cqqwz.cn

crypto.randomUUID()
来源：http://vac.jinqigufen.top

[U116] JS：类型检查（JSDoc）
来源：http://fbz.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://hxa.andypj.xyz

[U117] JS：单元测试
来源：http://byt.cdnleiting.top

npm i -D vitest;  npx vitest
来源：http://aba.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://odq.hysaishi.cn

npm i -D vite;  npx vite
来源：http://kbi.meibo888.top

[U119] JS：生产构建
来源：http://ixf.yanxiufei.cn

npx vite build
来源：http://sgw.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://nij.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://xja.cdnleiting.top

================================================================================
来源：http://czh.svipenyu.cn

统计汇总
来源：http://ule.birdmap.top

================================================================================
来源：http://kgk.hcnkem.com

按语言统计（条）：
来源：http://jhf.tian-w.cn

Python ......... 252
来源：http://smd.yj202588.top

PHP ............ 252
来源：http://acs.yj20258.top

JavaScript ..... 252
来源：http://fav.ydzc1.top

TypeScript ..... 212
来源：http://dzk.ehwqpu.com

Java ........... 212
来源：http://xrg.jinqigfzy.top

Go ............. 212
来源：http://fzc.uphjek.com

Ruby ........... 212
来源：http://bhv.cqqwz.cn

C# ............. 212
来源：http://vss.redwolf501.top

C .............. 30
来源：http://uiy.zhaomingkeji.xyz

C++ ............ 30
来源：http://xea.zhixingplan.top

SQL ............ 90
来源：http://adz.ybcxt.top

Bash ........... 80
来源：http://qup.yuxming.cn

Kotlin ......... 15
来源：http://gsr.ydzc1.top

Swift .......... 15
来源：http://lxa.jinyuanbaomall.cn

Lua ............ 10
来源：http://iby.tianlin.xyz

Perl ........... 10
来源：http://azl.epnwcf.com

Scala .......... 10
来源：http://svr.quarkkingdee.top

------------------------------------
来源：http://ity.hfpthk.cn

合计 ........... 2106 条
来源：http://esa.fehbvm.com

按章节统计：
来源：http://sfp.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uvp.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zgc.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ktw.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://var.hammf.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ljf.uphjek.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iur.cashguo.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tno.yj20258.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mrf.hcnkem.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bwy.fktsv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fcx.daria6918.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tgv.quarkkingdee.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bjy.ivvv.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oih.jiagoushi.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jtm.chenzaomai.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xzm.havefunace.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ajp.yueranfly.top

Q SQL 专题                              90
来源：http://ljy.dianchejie.cn

R Bash 专题                             80
来源：http://ktr.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://hzl.ivvv.top

T 其他语言补充                          60
来源：http://jnb.gogol.net.cn

U 高频实用片段                         120
来源：http://bsp.havefunace.top

------------------------------------
来源：http://njd.yuanzhike.top

合计                                  2106 条
来源：http://qts.cheryme.top

--------------------------------------------------------------------------------
来源：http://pkl.xingfuxueyuan.xyz

使用提醒
来源：http://syo.ydzc1.top

--------------------------------------------------------------------------------
来源：http://xnk.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xia.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://axl.fktsv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qqk.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qml.hnqzz.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pda.jinqigufen.top

—— 文件结束 ——
来源：http://jag.vehdjk.com

================================================================================
来源：http://stu.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://gdx.pengpengdd.cyou

Common Programming Examples Cheat Book
来源：http://tqw.fengsongda.top

================================================================================
来源：http://lmn.vqdsnc.cn

【收录内容】
来源：http://xqo.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://inx.yueranfly.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://plf.shuidangran.top

SQL · Bash · C · C++
来源：http://akq.shanyushiyangtech.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rvq.hysaishi.cn

【使用说明】
来源：http://gii.havefunace.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lss.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cgo.chenjidiqi.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dab.tianlin.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zhb.havefunace.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cpn.cucudq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mwk.nanxuanxn.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ccb.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kbl.vqdsnc.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zrq.chenjidiqi.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dbx.epnwcf.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rxz.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kkl.yueranfly.top

【文件统计】
来源：http://vru.yuanzhike.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eyg.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://wdq.hywenlv.cn

目  录
来源：http://pbi.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://gan.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://meg.smart0.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rjg.yuxming.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gla.ivvv.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pbj.jiagoushi.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zge.shanyushiyangtech.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vlr.jinghuilouyu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mdo.fehbvm.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rbv.zhijiandao.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vuo.jiagoushi.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ubg.ywan-chungtsiang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bka.jianghu66.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://say.jiagoushi.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://utb.hnqzz.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mcr.jlsjyb.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vdo.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fre.aizwys.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jmy.shanyushiyangtech.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nnb.zhixingplan.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iwn.fktsv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gyb.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nhg.tianlin.xyz

================================================================================
来源：http://dmg.xziqi.cn

A. 基础语法与类型
来源：http://rml.uphjek.com

================================================================================
来源：http://ser.ywan-chungtsiang.top

[A01] Hello World
来源：http://dmh.jianghu66.top

Py:   print("Hello, World!")
来源：http://mpi.jqgfzy.top

PHP:  echo "Hello, World!";
来源：http://gvx.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://bvb.zhijiandao.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cgr.hnqzz.top

Java: System.out.println("Hello, World!");
来源：http://krk.yuanzhike.top

Go:   fmt.Println("Hello, World!")
来源：http://bfp.xylfe.cn

Ruby: puts "Hello, World!"
来源：http://zoo.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://shj.zhongyouzk.top

[A02] 变量声明与赋值
来源：http://qow.xinyue.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wfy.yuanzhike.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zss.smart0.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://ixx.epnwcf.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://azs.uphjek.com

Java: String name = "Alex"; int age = 20;
来源：http://esk.xziqi.cn

Go:   name := "Alex"; age := 20
来源：http://hqf.yj20258.top

Ruby: name = "Alex"; age = 20
来源：http://adf.sxryk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://obq.daxiang520.top

[A03] 常量定义
来源：http://fmv.guowangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tqj.chenjidiqi.icu

PHP:  const PI = 3.14159;
来源：http://zzv.vehdjk.com

JS:   const PI = 3.14159;
来源：http://qmf.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://svg.jlsjyb.cn

Java: static final double PI = 3.14159;
来源：http://mlf.svipenyu.cn

Go:   const PI = 3.14159
来源：http://ecl.ydjk.org.cn

Ruby: PI = 3.14159
来源：http://nze.uphjek.com

C#:   const double PI = 3.14159;
来源：http://ezs.hfpthk.cn

[A04] 判断变量类型
来源：http://qga.sufxvd.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sdd.0kj1m.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://unw.fzhhl.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://knd.jqgfzy.top

TS:   typeof x; x instanceof Date
来源：http://akq.jinghuilouyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xeq.iojbl.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vkr.ehwqpu.com

Ruby: x.class; x.is_a?(Integer)
来源：http://nnt.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://jgk.hcnkem.com

[A05] 整数除法与取模
来源：http://eoa.vehdjk.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gkp.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://oae.aizwys.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bqz.jinyuanbaomall.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sga.nwbrower.top

Java: 7 / 2; 7 % 2
来源：http://lry.52xcode.cn

Go:   7 / 2; 7 % 2
来源：http://shx.hnxiangtu.top

Ruby: 7 / 2; 7 % 2
来源：http://wgz.gaohongyu789.top

C#:   7 / 2; 7 % 2
来源：http://dqe.xuanzx.com

[A06] 字符串转数字
来源：http://voz.svipenyu.cn

Py:   int("42"); float("3.14")
来源：http://sit.xinyue.icu

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eth.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vjr.haohaochexian.top

TS:   parseInt("42", 10); Number("42")
来源：http://zhg.chenjidiqi.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zha.c1oappe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fei.redwolf501.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hpw.nwbrower.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hjt.chenlongwang.top

[A07] 数字转字符串
来源：http://lfw.zhengqikj.top

Py:   str(42)
来源：http://lps.jinghuilouyu.cn

PHP:  (string) 42; strval(42)
来源：http://pqk.shanyushiyangtech.top

JS:   String(42); (42).toString()
来源：http://cqj.pycfn.com

TS:   String(42)
来源：http://cif.dashuyun.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rnq.bjfxy.top

Go:   strconv.Itoa(42)
来源：http://onn.jinqigfzy.top

Ruby: 42.to_s
来源：http://djj.cucudq.cn

C#:   42.ToString()
来源：http://akt.yongpay.top

[A08] 取整与四舍五入
来源：http://vvc.haohaochexian.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vuj.chenjidiqi.icu

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xtc.ywan-chungtsiang.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oiy.zhijiandao.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qmu.shangyingyoupin.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xxs.9152youxi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://liv.redwolf501.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://mwz.svipenyu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jur.wangshuangyany.cn

[A09] 绝对值与最大最小值
来源：http://uiz.hywenlv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rwx.hfpthk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qke.52xcode.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://svn.chenjidiqi.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dek.ivvv.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ngq.xingfuxueyuan.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jsm.svipenyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://adk.yj20258888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sws.jqgfzy.top

[A10] 生成随机数
来源：http://fbe.xylfe.cn

Py:   import random; random.randint(1, 100)
来源：http://jbk.cheryme.top

PHP:  random_int(1, 100);
来源：http://xdt.cqqwz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vmz.hfpthk.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gqm.xuanzx.com

Java: new Random().nextInt(100) + 1
来源：http://tzw.zhixingplan.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xuv.epnwcf.com

Ruby: rand(1..100)
来源：http://bcv.jianghu66.top

C#:   new Random().Next(1, 101)
来源：http://msb.chenjidiqi.icu

[A11] 条件表达式（三元）
来源：http://vev.fanxiaobao.xyz

Py:   "yes" if x > 0 else "no"
来源：http://znl.yj202588.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hch.svipenyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rwo.ppjwa.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dnx.gotoacloud.top

Java: x > 0 ? "yes" : "no"
来源：http://zdt.zhaomingkeji.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://coe.cashguo.top

Ruby: x > 0 ? "yes" : "no"
来源：http://xcu.tianlin.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://jie.xingfuxueyuan.xyz

[A12] 字符串插值 / 格式化
来源：http://tho.tianlin.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jfy.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fdg.yuanzhike.top

JS:   `Hello, ${name}!`
来源：http://ftu.yj20258.top

TS:   `Hello, ${name}!`
来源：http://ego.ctjpmb.com

Java: "Hello, %s!".formatted(name)
来源：http://nvq.sxryk.cn


<!-- 参考信息 -->