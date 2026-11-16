代发 wailian999

[U71] PHP：抛出异常
来源：http://bng.zhiwuduotai.top

throw new RuntimeException("失败", 500);
来源：http://byg.hnxiangtu.top

[U72] PHP：写错误日志
来源：http://dgz.wangdashe.top

error_log("失败: " . $e->getMessage());
来源：http://azj.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://uzs.zhengqikj.top

parse_ini_file("config.ini", true)
来源：http://qch.c1oappe.top

[U74] PHP：读取环境变量
来源：http://pxo.c1oappe.top

getenv("APP_ENV") ?: "production"
来源：http://hte.jianghu66.top

[U75] PHP：依赖注入
来源：http://ptt.sjlbkw.cn

composer require psr/container
来源：http://byf.aibaodan.cn

[U76] PHP：简单路由
来源：http://ndp.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jkf.yj20258888.top

[U77] PHP：模板渲染
来源：http://mke.0kj1m.cn

composer require twig/twig
来源：http://hkk.shangyingyoupin.top

[U78] PHP：单元测试
来源：http://wca.hnxiangtu.top

composer require --dev phpunit/phpunit
来源：http://vcw.fzhhl.top

[U79] PHP：静态分析
来源：http://jlq.jinqigufen.top

composer require --dev phpstan/phpstan
来源：http://mte.sxryk.cn

[U80] PHP：代码规范修复
来源：http://ikn.cdnleiting.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xfm.9152youxi.cn

[U81] JS：初始化项目
来源：http://sci.uphjek.com

npm init -y;  npm i express
来源：http://ntr.chenjidiqi.icu

[U82] JS：package.json 脚本
来源：http://fay.zhiwuduotai.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://phv.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://bdo.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://giz.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://ien.meibo888.top

module.exports = { a };  const { a } = require("./m");
来源：http://qcn.52xcode.cn

[U85] JS：可选链
来源：http://vuw.xylfe.cn

a?.b?.c
来源：http://tox.fzhhl.top

[U86] JS：空值合并
来源：http://rcd.zycfv.cn

a ?? b
来源：http://uwa.fengsongda.top

[U87] JS：解构默认值
来源：http://qyp.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://dmg.fktsv.cn

[U88] JS：对象展开合并
来源：http://iau.fengsongda.top

{ ...a, ...b }
来源：http://ezl.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://mhz.52xcode.cn

[...new Set(arr)]
来源：http://cbe.316326.xyz

[U90] JS：数字数组排序
来源：http://tzi.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://ypw.feifeiyinyue.top

[U91] JS：对象键值遍历
来源：http://uvx.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tjg.zdbjq.cn

[U92] JS：深拷贝
来源：http://yel.c1oappe.top

structuredClone(obj)
来源：http://ehk.nwbrower.top

[U93] JS：模板字符串
来源：http://gtk.hysaishi.cn

`共 ${n} 条`
来源：http://vmk.daria6918.cn

[U94] JS：箭头函数
来源：http://jxn.xuanzx.com

const double = x => x * 2;
来源：http://ebq.cqqwz.cn

[U95] JS：Promise 包装
来源：http://pzj.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://exw.yuanzhike.top

[U96] JS：async/await 与异常
来源：http://qdy.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://luv.feifeiyinyue.top

[U97] JS：并发请求
来源：http://nwk.guannengcc.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://odo.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://mkg.yonumen.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dgn.hcnkem.com

[U99] JS：事件监听
来源：http://srq.andypj.xyz

el.addEventListener("click", e => {})
来源：http://yzb.shzxlz.cn

[U100] JS：DOM 查询
来源：http://lto.yangfankeji.com

document.querySelector(".item")
来源：http://wxc.uphjek.com

[U101] JS：classList 操作
来源：http://iyr.sysykeji.top

el.classList.toggle("active")
来源：http://zlw.sjlbkw.cn

[U102] JS：本地存储
来源：http://nnv.kuanghao11.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ygm.hnqzz.top

[U103] JS：定时器
来源：http://cro.jinqigufen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ied.ydjk.org.cn

[U104] JS：防抖
来源：http://hkc.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cfm.316326.xyz

[U105] JS：节流
来源：http://fhw.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bwo.hfpthk.cn

[U106] JS：日期格式化
来源：http://xhb.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://skw.yj20258.top

[U107] JS：数字千分位
来源：http://esh.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bbc.wangdashe.top

[U108] JS：随机整数
来源：http://grc.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vgk.yuxming.cn

[U109] JS：数组分组
来源：http://pvk.cdnleiting.top

Object.groupBy(arr, x => x.type)
来源：http://dro.snrcjt.cn

[U110] JS：数组分块
来源：http://hhi.haohaochexian.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eye.haohaochexian.top

[U111] JS：对象转 Map
来源：http://jrp.aizwys.cn

new Map(Object.entries(obj))
来源：http://yoa.yuxming.cn

[U112] JS：字符串补位
来源：http://qgz.aizwys.cn

"7".padStart(3, "0")
来源：http://rhh.9152youxi.cn

[U113] JS：正则替换全部
来源：http://xxt.ybcxt.top

s.replaceAll("a", "b")
来源：http://xdy.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://nwc.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://eul.guowangkeji.top

[U115] JS：生成 UUID
来源：http://bqq.yj20258888.top

crypto.randomUUID()
来源：http://aew.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://fgu.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://mcf.chenjidiqi.icu

[U117] JS：单元测试
来源：http://vef.guowangkeji.top

npm i -D vitest;  npx vitest
来源：http://hvz.xinyue.icu

[U118] JS：开发服务器
来源：http://gdg.andypj.xyz

npm i -D vite;  npx vite
来源：http://sac.shzxlz.cn

[U119] JS：生产构建
来源：http://uvi.jianghu66.top

npx vite build
来源：http://qdb.kuanghao11.cn

[U120] JS：读取环境变量（Vite）
来源：http://mmj.redwolf501.top

import.meta.env.VITE_API_URL
来源：http://wnt.bbcook.cn

================================================================================
来源：http://wsi.0kj1m.cn

统计汇总
来源：http://vge.wangshuangyany.cn

================================================================================
来源：http://mlv.jqgfzy.top

按语言统计（条）：
来源：http://eyl.cheryme.top

Python ......... 252
来源：http://hyp.zycfv.cn

PHP ............ 252
来源：http://rvf.chenlongwang.top

JavaScript ..... 252
来源：http://xpz.sysykeji.top

TypeScript ..... 212
来源：http://elt.zycfv.cn

Java ........... 212
来源：http://iuj.pycfn.com

Go ............. 212
来源：http://mtx.cheryme.top

Ruby ........... 212
来源：http://mlj.pycfn.com

C# ............. 212
来源：http://iry.snrcjt.cn

C .............. 30
来源：http://iql.zhijiandao.cn

C++ ............ 30
来源：http://loe.snrcjt.cn

SQL ............ 90
来源：http://ohq.gogol.net.cn

Bash ........... 80
来源：http://wpo.svipenyu.cn

Kotlin ......... 15
来源：http://hze.hywenlv.cn

Swift .......... 15
来源：http://ziv.yj20258.top

Lua ............ 10
来源：http://tfw.feifeiyinyue.top

Perl ........... 10
来源：http://mhz.jiagoushi.top

Scala .......... 10
来源：http://bdf.yuanzhike.top

------------------------------------
来源：http://jji.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://srt.tarul.cn

按章节统计：
来源：http://xwo.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://aoq.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zht.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://muo.zhijiandao.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tuv.andypj.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bal.cheryme.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://per.yueranfly.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bfj.dashuyun.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rbp.cashguo.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dpi.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lkd.sysykeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hyf.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qyn.nanxinkj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rcy.yj20258.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tug.ydzc1.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rqb.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xoq.zycfv.cn

Q SQL 专题                              90
来源：http://mna.hammf.cn

R Bash 专题                             80
来源：http://mto.ctjpmb.com

S C / C++ 专题                          60
来源：http://qae.shzxlz.cn

T 其他语言补充                          60
来源：http://oes.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://ycu.gotoacloud.top

------------------------------------
来源：http://mva.hysaishi.cn

合计                                  2106 条
来源：http://iig.meibo888.top

--------------------------------------------------------------------------------
来源：http://ixx.ppjwa.cn

使用提醒
来源：http://des.hnqzz.top

--------------------------------------------------------------------------------
来源：http://jpo.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://amm.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://igu.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://edv.yuxming.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xdd.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yxl.chenlongwang.top

—— 文件结束 ——
来源：http://rjw.fktsv.cn

================================================================================
来源：http://laz.quarkkingdee.top

程序语言常见例子速查手册（2024 版）
来源：http://lyj.fzhhl.top

Common Programming Examples Cheat Book
来源：http://bhp.shanyushiyangkeji.top

================================================================================
来源：http://swu.iojbl.cn

【收录内容】
来源：http://cqm.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://vny.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yet.hnxiangtu.top

SQL · Bash · C · C++
来源：http://eiz.gotoacloud.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://umz.birdmap.top

【使用说明】
来源：http://vku.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zqy.iojbl.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://icc.xuetiantiany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qqa.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://abm.shangyingyoupin.top

Bash:  Shell         C:     C             C++:   C++
来源：http://phr.gaohongyu789.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zrq.xingfuxueyuan.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gil.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kpi.aizwys.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://poh.daxiang520.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vti.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ikt.xziqi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tjp.hesvh.cn

【文件统计】
来源：http://ftx.pycfn.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ljp.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://lly.xuetiantiany.cn

目  录
来源：http://hne.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://yks.hesvh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aqu.shanyushiyangtech.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cyb.sysykeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tym.hywenlv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://usx.52xcode.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://udz.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ujo.sxryk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sma.hnxiangtu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kib.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eac.fanxiaobao.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://acq.chenjidiqi.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://txj.snrcjt.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hbc.redwolf501.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xik.sjlbkw.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://byj.yfazqb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nah.jinqigfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xqi.0kj1m.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oyk.gotoacloud.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wyp.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qrw.52xcode.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uqe.guannengcc.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uxm.guowangkeji.top

================================================================================
来源：http://pmx.52xcode.cn

A. 基础语法与类型
来源：http://xjy.wangshuangyany.cn

================================================================================
来源：http://jfc.mhx1999.top

[A01] Hello World
来源：http://pvd.sjlbkw.cn

Py:   print("Hello, World!")
来源：http://ltx.jianghu66.top

PHP:  echo "Hello, World!";
来源：http://isk.fanxiaobao.xyz

JS:   console.log("Hello, World!");
来源：http://jzo.zhengqikj.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ybv.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://otl.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://cnz.fanxiaobao.xyz

Ruby: puts "Hello, World!"
来源：http://ria.shanyushiyangtech.top

C#:   Console.WriteLine("Hello, World!");
来源：http://epy.jyoumei.cn

[A02] 变量声明与赋值
来源：http://bvi.cucudq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://joy.jinyuanbaomall.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://acl.smart0.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://hdw.xylfe.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xvp.yuxming.cn

Java: String name = "Alex"; int age = 20;
来源：http://equ.tianlin.xyz

Go:   name := "Alex"; age := 20
来源：http://raj.fengsongda.top

Ruby: name = "Alex"; age = 20
来源：http://oun.zhijiandao.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qkf.52xcode.cn

[A03] 常量定义
来源：http://axf.jyoumei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vos.ydzc1.top

PHP:  const PI = 3.14159;
来源：http://pgq.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://idr.uphjek.com

TS:   const PI: number = 3.14159;
来源：http://ipf.52xcode.cn

Java: static final double PI = 3.14159;
来源：http://jro.hfpthk.cn

Go:   const PI = 3.14159
来源：http://hjt.daxiang520.top

Ruby: PI = 3.14159
来源：http://lxi.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://mzn.zdqjudy.top

[A04] 判断变量类型
来源：http://uyz.jinqigfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xup.svipenyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://phw.cashguo.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eqa.dashuyun.cn

TS:   typeof x; x instanceof Date
来源：http://sye.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ueq.gotoacloud.top

Go:   reflect.TypeOf(x).Name()
来源：http://rta.gotoacloud.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jee.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://grl.yongpay.top

[A05] 整数除法与取模
来源：http://zga.xziqi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yhu.aibaodan.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mcr.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://htg.zdqjudy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jfj.snrcjt.cn

Java: 7 / 2; 7 % 2
来源：http://hvc.yj20258.top

Go:   7 / 2; 7 % 2
来源：http://utm.zhixingplan.top

Ruby: 7 / 2; 7 % 2
来源：http://xxw.jianghu66.top

C#:   7 / 2; 7 % 2
来源：http://vvb.jqgufenzy.top

[A06] 字符串转数字
来源：http://fdg.svipenyu.cn

Py:   int("42"); float("3.14")
来源：http://xwz.xylfe.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vrh.shanyushiyangtech.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://soo.redwolf501.top

TS:   parseInt("42", 10); Number("42")
来源：http://rfh.jiagoushi.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xnk.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://npr.fengsongda.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hiu.fanxiaobao.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mrm.meibo888.top

[A07] 数字转字符串
来源：http://rwr.hammf.cn

Py:   str(42)
来源：http://cct.aibaodan.cn

PHP:  (string) 42; strval(42)
来源：http://cme.aibaodan.cn

JS:   String(42); (42).toString()
来源：http://xyv.epnwcf.com

TS:   String(42)
来源：http://gkl.aizwys.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hxn.xuetiantiany.cn

Go:   strconv.Itoa(42)
来源：http://gby.zdbjq.cn

Ruby: 42.to_s
来源：http://sdi.aizwys.cn

C#:   42.ToString()
来源：http://oqd.ivvv.top

[A08] 取整与四舍五入
来源：http://tkg.zhixingplan.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mhm.hcnkem.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jpk.havefunace.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://aeh.zdbjq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pjt.chenzaomai.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iha.zhongyouzk.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tqv.hnxiangtu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://nxk.wangshuangyany.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://enb.zhongyouzk.top

[A09] 绝对值与最大最小值
来源：http://zou.hongshengwenyu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lps.ywan-chungtsiang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ghj.gotoacloud.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://moa.fengsongda.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cjt.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zfb.xuanzx.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rhc.ybcxt.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://udt.dashuyun.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bmg.tarul.cn

[A10] 生成随机数
来源：http://ipp.zhengqikj.top

Py:   import random; random.randint(1, 100)
来源：http://ulg.wangdashe.top

PHP:  random_int(1, 100);
来源：http://cnq.yj202588.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://edu.aizwys.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jed.xuanzx.com

Java: new Random().nextInt(100) + 1
来源：http://rba.svipenyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gbg.yj20258.top

Ruby: rand(1..100)
来源：http://zrn.redwolf501.top

C#:   new Random().Next(1, 101)
来源：http://gfr.hnxiangtu.top

[A11] 条件表达式（三元）
来源：http://xyn.cdnleiting.top

Py:   "yes" if x > 0 else "no"
来源：http://srx.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://laa.sysykeji.top


<!-- 参考信息 -->