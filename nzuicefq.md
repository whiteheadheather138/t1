代发 wailian999

[U75] PHP：依赖注入
来源：http://uqy.snrcjt.cn

composer require psr/container
来源：http://agk.iojbl.cn

[U76] PHP：简单路由
来源：http://cak.316326.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dzp.fzhhl.top

[U77] PHP：模板渲染
来源：http://snu.uphjek.com

composer require twig/twig
来源：http://rax.hesvh.cn

[U78] PHP：单元测试
来源：http://fqa.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://mcw.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://byc.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://mhx.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://ink.yj202588.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://erp.shzxlz.cn

[U81] JS：初始化项目
来源：http://nvd.wangdashe.top

npm init -y;  npm i express
来源：http://ewt.jianghu66.top

[U82] JS：package.json 脚本
来源：http://azp.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ugu.9152youxi.cn

[U83] JS：ES Module 导入导出
来源：http://yrm.jqgufenzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://gyz.sweek.top

[U84] JS：CommonJS 写法
来源：http://aco.redwolf501.top

module.exports = { a };  const { a } = require("./m");
来源：http://onl.xuanzx.com

[U85] JS：可选链
来源：http://qob.zhaomingkeji.xyz

a?.b?.c
来源：http://ydo.fanxiaobao.xyz

[U86] JS：空值合并
来源：http://ahm.ywan-chungtsiang.top

a ?? b
来源：http://jmy.jqgufenzy.top

[U87] JS：解构默认值
来源：http://zlu.jlsjyb.cn

const { a = 1, b = 2 } = obj;
来源：http://gnj.guannengcc.top

[U88] JS：对象展开合并
来源：http://nwf.jqgfzy.top

{ ...a, ...b }
来源：http://yxa.cheryme.top

[U89] JS：数组去重
来源：http://eqf.yfazqb.com

[...new Set(arr)]
来源：http://rdu.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://trz.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://zjn.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://kkc.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mvj.daria6918.cn

[U92] JS：深拷贝
来源：http://tzx.daxiang520.top

structuredClone(obj)
来源：http://tok.zhixingplan.top

[U93] JS：模板字符串
来源：http://xpw.iojbl.cn

`共 ${n} 条`
来源：http://xex.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://nhx.aizwys.cn

const double = x => x * 2;
来源：http://kbg.zhengqikj.top

[U95] JS：Promise 包装
来源：http://byu.zdbjq.cn

new Promise((resolve, reject) => {})
来源：http://nij.wangshuangyany.cn

[U96] JS：async/await 与异常
来源：http://mxg.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cga.redwolf501.top

[U97] JS：并发请求
来源：http://afm.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zae.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://rdt.ydjk.org.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://doq.sjlbkw.cn

[U99] JS：事件监听
来源：http://wgl.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://smg.jiagoushi.top

[U100] JS：DOM 查询
来源：http://qyq.fengsongda.top

document.querySelector(".item")
来源：http://lnq.jlsjyb.cn

[U101] JS：classList 操作
来源：http://sri.birdmap.top

el.classList.toggle("active")
来源：http://bqm.jinghuilouyu.cn

[U102] JS：本地存储
来源：http://esu.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jbi.shanyushiyangkeji.top

[U103] JS：定时器
来源：http://yss.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hqt.fanxiaobao.xyz

[U104] JS：防抖
来源：http://bgb.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hxd.haohaochexian.top

[U105] JS：节流
来源：http://nht.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qgd.ybcxt.top

[U106] JS：日期格式化
来源：http://vzq.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eva.shuidangran.top

[U107] JS：数字千分位
来源：http://yjw.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ixw.jinghuilouyu.cn

[U108] JS：随机整数
来源：http://hdd.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hzk.vehdjk.com

[U109] JS：数组分组
来源：http://tsz.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://dbf.chenlongwang.top

[U110] JS：数组分块
来源：http://dpi.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wqu.zdbjq.cn

[U111] JS：对象转 Map
来源：http://imz.jinqigufen.top

new Map(Object.entries(obj))
来源：http://sil.pengpengdd.cyou

[U112] JS：字符串补位
来源：http://obk.cqqwz.cn

"7".padStart(3, "0")
来源：http://eel.uphjek.com

[U113] JS：正则替换全部
来源：http://tke.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://aes.sxryk.cn

[U114] JS：JSON 深比较
来源：http://mes.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://udz.mhx1999.top

[U115] JS：生成 UUID
来源：http://wur.vehdjk.com

crypto.randomUUID()
来源：http://wnf.haohaochexian.top

[U116] JS：类型检查（JSDoc）
来源：http://iml.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://ylm.nwbrower.top

[U117] JS：单元测试
来源：http://vsj.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://pdw.fktsv.cn

[U118] JS：开发服务器
来源：http://pjn.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://dkc.chenzaomai.com

[U119] JS：生产构建
来源：http://yfy.jinyuanbaomall.cn

npx vite build
来源：http://hyy.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://dpo.jinqigfzy.top

import.meta.env.VITE_API_URL
来源：http://fvc.hnxiangtu.top

================================================================================
来源：http://vuv.xziqi.cn

统计汇总
来源：http://oed.birdmap.top

================================================================================
来源：http://wch.xziqi.cn

按语言统计（条）：
来源：http://gap.kuanghao11.cn

Python ......... 252
来源：http://oby.zhoulong.xyz

PHP ............ 252
来源：http://wud.ydzc1.top

JavaScript ..... 252
来源：http://abo.shanyushiyangtech.top

TypeScript ..... 212
来源：http://blv.sjlbkw.cn

Java ........... 212
来源：http://zil.mhx1999.top

Go ............. 212
来源：http://rgr.sufxvd.cn

Ruby ........... 212
来源：http://bkl.vqdsnc.cn

C# ............. 212
来源：http://vgv.xuetiantiany.cn

C .............. 30
来源：http://tgp.pycfn.com

C++ ............ 30
来源：http://olm.zhoulong.xyz

SQL ............ 90
来源：http://orr.yonumen.top

Bash ........... 80
来源：http://ohy.hfpthk.cn

Kotlin ......... 15
来源：http://yql.fehbvm.com

Swift .......... 15
来源：http://tiw.cdnleiting.top

Lua ............ 10
来源：http://nkk.nwbrower.top

Perl ........... 10
来源：http://ssi.bjfxy.top

Scala .......... 10
来源：http://cvf.fehbvm.com

------------------------------------
来源：http://kll.yonumen.top

合计 ........... 2106 条
来源：http://pyc.gotoacloud.top

按章节统计：
来源：http://wer.chenzaomai.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gab.yuxming.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rmx.havefunace.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wxf.ehwqpu.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kaj.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gsu.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iip.ehwqpu.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ycn.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qrd.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pyn.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dot.shangyingyoupin.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://otc.vehdjk.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ltq.ywan-chungtsiang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lra.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jnj.vehdjk.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dcw.chenjidiqi.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hsm.wangdashe.top

Q SQL 专题                              90
来源：http://gai.aizwys.cn

R Bash 专题                             80
来源：http://jni.ppjwa.cn

S C / C++ 专题                          60
来源：http://tzi.havefunace.top

T 其他语言补充                          60
来源：http://jei.ybcxt.top

U 高频实用片段                         120
来源：http://kgx.shanyushiyangkeji.top

------------------------------------
来源：http://xiy.jqgfzy.top

合计                                  2106 条
来源：http://esf.guannengcc.top

--------------------------------------------------------------------------------
来源：http://wxv.gzhubu.top

使用提醒
来源：http://fza.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://jxa.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fif.wangshuangyany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://htm.c1oappe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qch.sjlbkw.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ugm.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cmc.tanke756.top

—— 文件结束 ——
来源：http://wzt.cdnleiting.top

================================================================================
来源：http://bez.hywenlv.cn

程序语言常见例子速查手册（2024 版）
来源：http://eyj.zdqjudy.top

Common Programming Examples Cheat Book
来源：http://khu.jianghu66.top

================================================================================
来源：http://epa.bbcook.cn

【收录内容】
来源：http://pxx.jinqigufen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bef.0kj1m.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hod.yanxiufei.cn

SQL · Bash · C · C++
来源：http://uqi.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zpz.yanxiufei.cn

【使用说明】
来源：http://gfx.jinyuanbaomall.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tyg.yvedp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nqk.ctjpmb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cvu.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xvm.jinqigufen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://sra.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wvy.cucudq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tor.epnwcf.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://epz.xuetiantiany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bev.nanxinkj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dkd.c1oappe.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://efb.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dvi.jqgufenzy.top

【文件统计】
来源：http://ple.9152youxi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://akk.xinyue.icu

--------------------------------------------------------------------------------
来源：http://zvt.feifeiyinyue.top

目  录
来源：http://hhd.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://pom.gaohongyu789.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://icv.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://upl.ywan-chungtsiang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kgg.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://svj.andypj.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uch.sxryk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zoh.yfazqb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qei.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vjr.pycfn.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ien.havefunace.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://liy.sjlbkw.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kdu.xinyue.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lea.guowangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mgb.ivvv.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kic.pycfn.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vka.tian-w.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pog.zdqjudy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jpg.nanxinkj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cxi.sweek.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yle.shanyushiyangtech.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ybp.hywenlv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://een.yfazqb.com

================================================================================
来源：http://hef.kuanghao11.cn

A. 基础语法与类型
来源：http://rtk.aizwys.cn

================================================================================
来源：http://lmy.jianghu66.top

[A01] Hello World
来源：http://rpd.nanxuanxn.top

Py:   print("Hello, World!")
来源：http://daa.52xcode.cn

PHP:  echo "Hello, World!";
来源：http://bbd.zhengqikj.top

JS:   console.log("Hello, World!");
来源：http://uys.fanxiaobao.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yfl.daxiang520.top

Java: System.out.println("Hello, World!");
来源：http://zrd.feifeiyinyue.top

Go:   fmt.Println("Hello, World!")
来源：http://hog.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://tns.cdnleiting.top

C#:   Console.WriteLine("Hello, World!");
来源：http://lhw.andypj.xyz

[A02] 变量声明与赋值
来源：http://aoc.dianchejie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cvc.nwbrower.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fio.yangfankeji.com

JS:   let name = "Alex"; const age = 20;
来源：http://dys.jqgfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ahe.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://pow.hesvh.cn

Go:   name := "Alex"; age := 20
来源：http://tpt.yfazqb.com

Ruby: name = "Alex"; age = 20
来源：http://knf.redwolf501.top

C#:   string name = "Alex"; int age = 20;
来源：http://cab.zhijiandao.cn

[A03] 常量定义
来源：http://anp.hongshengwenyu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ctx.jianghu66.top

PHP:  const PI = 3.14159;
来源：http://mab.vehdjk.com

JS:   const PI = 3.14159;
来源：http://sts.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://ezq.guowangkeji.top

Java: static final double PI = 3.14159;
来源：http://lbn.iojbl.cn

Go:   const PI = 3.14159
来源：http://hgh.fanxiaobao.xyz

Ruby: PI = 3.14159
来源：http://hll.vehdjk.com

C#:   const double PI = 3.14159;
来源：http://mzg.fktsv.cn

[A04] 判断变量类型
来源：http://dxt.jlsjyb.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dfw.daxiang520.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fug.aibaodan.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ofg.yfazqb.com

TS:   typeof x; x instanceof Date
来源：http://gjy.ppjwa.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://seg.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://vrk.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://afv.cdnleiting.top

C#:   x.GetType().Name; x is int
来源：http://cyx.ydzc1.top

[A05] 整数除法与取模
来源：http://uzt.zhiwuduotai.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dlu.shzxlz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tqh.vehdjk.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pkb.yangfankeji.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nhc.hammf.cn

Java: 7 / 2; 7 % 2
来源：http://lbm.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://xku.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://vvy.dianchejie.cn

C#:   7 / 2; 7 % 2
来源：http://gpt.sweek.top

[A06] 字符串转数字
来源：http://lnp.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://oxx.hysaishi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qhm.shangyingyoupin.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tkp.fengsongda.top

TS:   parseInt("42", 10); Number("42")
来源：http://wil.yonumen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jwg.shanyushiyangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nnx.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://lcq.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cem.wangdashe.top

[A07] 数字转字符串
来源：http://ynw.cucudq.cn

Py:   str(42)
来源：http://snz.sysykeji.top

PHP:  (string) 42; strval(42)
来源：http://vwb.zdbjq.cn

JS:   String(42); (42).toString()
来源：http://kti.jinghuilouyu.cn

TS:   String(42)
来源：http://akk.kuanghao11.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://adt.sufxvd.cn

Go:   strconv.Itoa(42)
来源：http://heb.gogol.net.cn

Ruby: 42.to_s
来源：http://fkt.tanke756.top

C#:   42.ToString()
来源：http://sup.uphjek.com

[A08] 取整与四舍五入
来源：http://dua.yongpay.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://plq.jinghuilouyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rmj.xinyue.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://won.cdnleiting.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ome.sjlbkw.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qzp.daria6918.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mcs.nwbrower.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://usu.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ekl.uphjek.com

[A09] 绝对值与最大最小值
来源：http://sfe.ydjk.org.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lqb.daxiang520.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rvl.yj20258.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://npn.jianghu66.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://krx.guowangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://aeo.zhoulong.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://abq.jqgufenzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nli.ivvv.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kpw.jinqigfzy.top

[A10] 生成随机数
来源：http://yrq.tian-w.cn

Py:   import random; random.randint(1, 100)
来源：http://eeg.zdqjudy.top

PHP:  random_int(1, 100);
来源：http://iec.jqgfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nec.redwolf501.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gpy.redwolf501.top

Java: new Random().nextInt(100) + 1
来源：http://kbt.9152youxi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gom.shuidangran.top

Ruby: rand(1..100)
来源：http://zmg.meibo888.top

C#:   new Random().Next(1, 101)
来源：http://qru.hnqzz.top

[A11] 条件表达式（三元）
来源：http://yfs.uphjek.com

Py:   "yes" if x > 0 else "no"
来源：http://pgs.jlsjyb.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mfn.aizwys.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hnc.gzhubu.top

TS:   x > 0 ? "yes" : "no"
来源：http://vcf.smart0.xyz

Java: x > 0 ? "yes" : "no"
来源：http://ngz.fzhhl.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dzu.uphjek.com

Ruby: x > 0 ? "yes" : "no"
来源：http://rgc.yongpay.top

C#:   x > 0 ? "yes" : "no"
来源：http://bfg.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://pmw.meibo888.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://quc.iojbl.cn


<!-- 参考信息 -->