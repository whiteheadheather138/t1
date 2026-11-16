代发 wailian999

[U71] PHP：抛出异常
来源：http://msj.fehbvm.com

throw new RuntimeException("失败", 500);
来源：http://hrg.guowangkeji.top

[U72] PHP：写错误日志
来源：http://jnr.jianghu66.top

error_log("失败: " . $e->getMessage());
来源：http://jys.yuxming.cn

[U73] PHP：读取 ini 配置
来源：http://ytm.ehwqpu.com

parse_ini_file("config.ini", true)
来源：http://uve.redwolf501.top

[U74] PHP：读取环境变量
来源：http://bnw.cashguo.top

getenv("APP_ENV") ?: "production"
来源：http://qdr.ctjpmb.com

[U75] PHP：依赖注入
来源：http://exn.andypj.xyz

composer require psr/container
来源：http://tlk.jlsjyb.cn

[U76] PHP：简单路由
来源：http://nqb.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jlw.snrcjt.cn

[U77] PHP：模板渲染
来源：http://eph.redwolf501.top

composer require twig/twig
来源：http://dqq.birdmap.top

[U78] PHP：单元测试
来源：http://lee.0kj1m.cn

composer require --dev phpunit/phpunit
来源：http://srf.bbcook.cn

[U79] PHP：静态分析
来源：http://ufk.hnxiangtu.top

composer require --dev phpstan/phpstan
来源：http://xha.jqgfzy.top

[U80] PHP：代码规范修复
来源：http://ixg.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://emr.jianghu66.top

[U81] JS：初始化项目
来源：http://tyt.guowangkeji.top

npm init -y;  npm i express
来源：http://rhw.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://dpc.hywenlv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hpf.gaohongyu789.top

[U83] JS：ES Module 导入导出
来源：http://ovg.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://hva.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://yra.jianghu66.top

module.exports = { a };  const { a } = require("./m");
来源：http://ttm.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://ycr.cashguo.top

a?.b?.c
来源：http://dbu.sjlbkw.cn

[U86] JS：空值合并
来源：http://ecn.havefunace.top

a ?? b
来源：http://gdp.nanxuanxn.top

[U87] JS：解构默认值
来源：http://qji.nwbrower.top

const { a = 1, b = 2 } = obj;
来源：http://yno.xziqi.cn

[U88] JS：对象展开合并
来源：http://sgy.yj202588.top

{ ...a, ...b }
来源：http://dqk.cucudq.cn

[U89] JS：数组去重
来源：http://mjm.bjfxy.top

[...new Set(arr)]
来源：http://ryf.tian-w.cn

[U90] JS：数字数组排序
来源：http://syy.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://szj.ydzc1.top

[U91] JS：对象键值遍历
来源：http://zat.yuanzhike.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://odx.cheryme.top

[U92] JS：深拷贝
来源：http://qvc.jqgufenzy.top

structuredClone(obj)
来源：http://xqr.tanke756.top

[U93] JS：模板字符串
来源：http://iey.ctjpmb.com

`共 ${n} 条`
来源：http://ndg.hesvh.cn

[U94] JS：箭头函数
来源：http://fvg.yuanzhike.top

const double = x => x * 2;
来源：http://uha.yuxming.cn

[U95] JS：Promise 包装
来源：http://htl.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://npb.yfazqb.com

[U96] JS：async/await 与异常
来源：http://wha.316326.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jym.bjfxy.top

[U97] JS：并发请求
来源：http://wad.fengsongda.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wic.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://iwg.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lkv.iojbl.cn

[U99] JS：事件监听
来源：http://zof.yj20258.top

el.addEventListener("click", e => {})
来源：http://orb.hysaishi.cn

[U100] JS：DOM 查询
来源：http://nwn.epnwcf.com

document.querySelector(".item")
来源：http://ruj.meibo888.top

[U101] JS：classList 操作
来源：http://aqz.zhixingplan.top

el.classList.toggle("active")
来源：http://ndj.pengpengdd.cyou

[U102] JS：本地存储
来源：http://mzf.tarul.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pni.dashuyun.cn

[U103] JS：定时器
来源：http://iat.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yyt.nwbrower.top

[U104] JS：防抖
来源：http://bcv.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mku.0kj1m.cn

[U105] JS：节流
来源：http://okm.shzxlz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mxg.zhiwuduotai.top

[U106] JS：日期格式化
来源：http://roq.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://syi.yfazqb.com

[U107] JS：数字千分位
来源：http://zcp.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tmy.sxryk.cn

[U108] JS：随机整数
来源：http://ewy.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wlp.zycfv.cn

[U109] JS：数组分组
来源：http://buk.ehwqpu.com

Object.groupBy(arr, x => x.type)
来源：http://tnv.hysaishi.cn

[U110] JS：数组分块
来源：http://pzr.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mok.havefunace.top

[U111] JS：对象转 Map
来源：http://jkv.chenzaomai.com

new Map(Object.entries(obj))
来源：http://inp.redwolf501.top

[U112] JS：字符串补位
来源：http://jsc.ctjpmb.com

"7".padStart(3, "0")
来源：http://gzo.yfazqb.com

[U113] JS：正则替换全部
来源：http://ihi.yonumen.top

s.replaceAll("a", "b")
来源：http://umb.jianghu66.top

[U114] JS：JSON 深比较
来源：http://mbw.yanxiufei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://luu.jqgfzy.top

[U115] JS：生成 UUID
来源：http://mtq.yonumen.top

crypto.randomUUID()
来源：http://jml.daxiang520.top

[U116] JS：类型检查（JSDoc）
来源：http://imq.haohaochexian.top

/** @param {string} name */ function f(name) {}
来源：http://jut.chenlongwang.top

[U117] JS：单元测试
来源：http://gln.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://ubu.smart0.xyz

[U118] JS：开发服务器
来源：http://sgi.hnqzz.top

npm i -D vite;  npx vite
来源：http://nrk.hnxiangtu.top

[U119] JS：生产构建
来源：http://qoh.zdqjudy.top

npx vite build
来源：http://dcw.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://qvx.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://dth.zhoulong.xyz

================================================================================
来源：http://kpz.guowangkeji.top

统计汇总
来源：http://vpn.sxryk.cn

================================================================================
来源：http://xvj.xuetiantiany.cn

按语言统计（条）：
来源：http://fvu.havefunace.top

Python ......... 252
来源：http://req.sxryk.cn

PHP ............ 252
来源：http://gfg.redwolf501.top

JavaScript ..... 252
来源：http://yxi.yfazqb.com

TypeScript ..... 212
来源：http://uxo.ivvv.top

Java ........... 212
来源：http://fph.shuidangran.top

Go ............. 212
来源：http://gks.xziqi.cn

Ruby ........... 212
来源：http://uxu.yvedp.cn

C# ............. 212
来源：http://hqf.fengsongda.top

C .............. 30
来源：http://ncq.xingfuxueyuan.xyz

C++ ............ 30
来源：http://iqp.yanxiufei.cn

SQL ............ 90
来源：http://fjo.ctjpmb.com

Bash ........... 80
来源：http://zgp.hnxiangtu.top

Kotlin ......... 15
来源：http://ivv.guowangkeji.top

Swift .......... 15
来源：http://qko.yuxming.cn

Lua ............ 10
来源：http://jfw.snrcjt.cn

Perl ........... 10
来源：http://qzq.zdbjq.cn

Scala .......... 10
来源：http://rum.andypj.xyz

------------------------------------
来源：http://ege.yueranfly.top

合计 ........... 2106 条
来源：http://otl.316326.xyz

按章节统计：
来源：http://iij.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fmo.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://was.316326.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://psg.ctjpmb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aiq.fzhhl.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ynv.sjlbkw.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vbo.yvedp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://thg.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lfg.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xgf.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eql.shanyushiyangtech.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iiw.fzhhl.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hfc.yangfankeji.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zpy.nwbrower.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mkn.yueranfly.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://whh.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dbb.fzhhl.top

Q SQL 专题                              90
来源：http://ama.jianghu66.top

R Bash 专题                             80
来源：http://hbq.sysykeji.top

S C / C++ 专题                          60
来源：http://cvo.dashuyun.cn

T 其他语言补充                          60
来源：http://sbv.zhengqikj.top

U 高频实用片段                         120
来源：http://swo.sweek.top

------------------------------------
来源：http://cwf.vqdsnc.cn

合计                                  2106 条
来源：http://vby.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://wjk.pengpengdd.cyou

使用提醒
来源：http://mlv.havefunace.top

--------------------------------------------------------------------------------
来源：http://tzz.zhixingplan.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://myp.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://myj.zhaomingkeji.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://niy.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ncw.sxryk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rel.hnxiangtu.top

—— 文件结束 ——
来源：http://sug.jiagoushi.top

================================================================================
来源：http://gmr.fehbvm.com

程序语言常见例子速查手册（2024 版）
来源：http://ivl.ppjwa.cn

Common Programming Examples Cheat Book
来源：http://bxr.aizwys.cn

================================================================================
来源：http://omb.vqdsnc.cn

【收录内容】
来源：http://obe.birdmap.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://iwa.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bkw.zhengqikj.top

SQL · Bash · C · C++
来源：http://niq.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lon.bjfxy.top

【使用说明】
来源：http://loq.fengsongda.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fuj.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xyx.zdqjudy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://est.ctjpmb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nci.zdbjq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ats.316326.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bcd.pycfn.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yph.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oku.zhoulong.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hpe.zhoulong.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hqm.vehdjk.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xae.zhijiandao.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qip.shuidangran.top

【文件统计】
来源：http://uoo.chenlongwang.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gtv.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://ksd.dashuyun.cn

目  录
来源：http://lhp.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://kpc.dashuyun.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lby.epnwcf.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mkc.ehwqpu.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bet.yongpay.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tyy.guannengcc.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wgf.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zvq.sufxvd.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://itc.fzhhl.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nem.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vln.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sak.gzhubu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kpi.yfazqb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yaw.ctjpmb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ooc.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bqp.zycfv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eka.jianghu66.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wnf.9152youxi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ydz.kuanghao11.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pjd.yj202588.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xmo.52xcode.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ycr.yj202588.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uyj.zycfv.cn

================================================================================
来源：http://utq.pengpengdd.cyou

A. 基础语法与类型
来源：http://ifw.jinghuilouyu.cn

================================================================================
来源：http://zsl.jqgufenzy.top

[A01] Hello World
来源：http://dnb.shanyushiyangkeji.top

Py:   print("Hello, World!")
来源：http://xsf.dashuyun.cn

PHP:  echo "Hello, World!";
来源：http://aky.uphjek.com

JS:   console.log("Hello, World!");
来源：http://frf.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gsj.bbcook.cn

Java: System.out.println("Hello, World!");
来源：http://yao.sjlbkw.cn

Go:   fmt.Println("Hello, World!")
来源：http://cne.jinyuanbaomall.cn

Ruby: puts "Hello, World!"
来源：http://krh.sxryk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kbt.mhx1999.top

[A02] 变量声明与赋值
来源：http://cle.jlsjyb.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hnp.iojbl.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qfi.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://qfg.yj202588.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://duv.zdqjudy.top

Java: String name = "Alex"; int age = 20;
来源：http://ojq.yuxming.cn

Go:   name := "Alex"; age := 20
来源：http://gpm.xuanzx.com

Ruby: name = "Alex"; age = 20
来源：http://xrm.yfazqb.com

C#:   string name = "Alex"; int age = 20;
来源：http://uud.9152youxi.cn

[A03] 常量定义
来源：http://ppe.ydzc1.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dav.zhoulong.xyz

PHP:  const PI = 3.14159;
来源：http://fmm.cheryme.top

JS:   const PI = 3.14159;
来源：http://pbc.feifeiyinyue.top

TS:   const PI: number = 3.14159;
来源：http://ocm.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://inp.c1oappe.top

Go:   const PI = 3.14159
来源：http://xci.fktsv.cn

Ruby: PI = 3.14159
来源：http://btg.nanxuanxn.top

C#:   const double PI = 3.14159;
来源：http://mvv.hongshengwenyu.top

[A04] 判断变量类型
来源：http://yrw.jianghu66.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qhw.nwbrower.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rui.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rrt.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://lnl.hesvh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eci.daria6918.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jlj.9152youxi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ime.epnwcf.com

C#:   x.GetType().Name; x is int
来源：http://bbh.yangfankeji.com

[A05] 整数除法与取模
来源：http://etu.chenjidiqi.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wih.jqgufenzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fdo.fehbvm.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ecr.fktsv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pav.yvedp.cn

Java: 7 / 2; 7 % 2
来源：http://aqc.zhijiandao.cn

Go:   7 / 2; 7 % 2
来源：http://mbj.jiagoushi.top

Ruby: 7 / 2; 7 % 2
来源：http://oya.fktsv.cn

C#:   7 / 2; 7 % 2
来源：http://iri.zdqjudy.top

[A06] 字符串转数字
来源：http://fiv.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://xha.yanxiufei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xpa.zycfv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tki.yongpay.top

TS:   parseInt("42", 10); Number("42")
来源：http://tqy.sweek.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jte.yuxming.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cog.xylfe.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uii.gotoacloud.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sub.zhixingplan.top

[A07] 数字转字符串
来源：http://xez.chenzaomai.com

Py:   str(42)
来源：http://sov.tianlin.xyz

PHP:  (string) 42; strval(42)
来源：http://gon.cqqwz.cn

JS:   String(42); (42).toString()
来源：http://lac.cdnleiting.top

TS:   String(42)
来源：http://fcm.jianghu66.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rit.xylfe.cn

Go:   strconv.Itoa(42)
来源：http://gne.shanyushiyangtech.top

Ruby: 42.to_s
来源：http://gki.jinqigfzy.top

C#:   42.ToString()
来源：http://xhj.snrcjt.cn

[A08] 取整与四舍五入
来源：http://ybc.zhoulong.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nih.fktsv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zyp.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ewb.wangdashe.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mut.sweek.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xjb.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rmp.hnxiangtu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://acj.yanxiufei.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zbi.shangyingyoupin.top

[A09] 绝对值与最大最小值
来源：http://zmi.zdqjudy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lhv.yongpay.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vwj.zycfv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jrr.fengsongda.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://omk.tarul.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xmx.redwolf501.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://srv.hongshengwenyu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ung.xylfe.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qhi.ydjk.org.cn

[A10] 生成随机数
来源：http://hog.ywan-chungtsiang.top

Py:   import random; random.randint(1, 100)
来源：http://odl.tian-w.cn

PHP:  random_int(1, 100);
来源：http://slr.jlsjyb.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wdj.hysaishi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xkf.sysykeji.top

Java: new Random().nextInt(100) + 1
来源：http://vjq.yvedp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ddn.jinqigfzy.top

Ruby: rand(1..100)
来源：http://pcd.redwolf501.top

C#:   new Random().Next(1, 101)
来源：http://wbn.ctjpmb.com

[A11] 条件表达式（三元）
来源：http://kym.zycfv.cn

Py:   "yes" if x > 0 else "no"
来源：http://iyw.hysaishi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tlk.yuxming.cn


<!-- 参考信息 -->