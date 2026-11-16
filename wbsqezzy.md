代发 wailian999

[U71] PHP：抛出异常
来源：http://bpw.pycfn.com

throw new RuntimeException("失败", 500);
来源：http://qzd.cqqwz.cn

[U72] PHP：写错误日志
来源：http://gpr.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://mfs.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://mzb.chenlongwang.top

parse_ini_file("config.ini", true)
来源：http://vsv.bbcook.cn

[U74] PHP：读取环境变量
来源：http://nxt.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://qqu.yfazqb.com

[U75] PHP：依赖注入
来源：http://hqp.zhoulong.xyz

composer require psr/container
来源：http://jhy.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://vyq.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qlx.tanke756.top

[U77] PHP：模板渲染
来源：http://brc.fehbvm.com

composer require twig/twig
来源：http://ulf.cqqwz.cn

[U78] PHP：单元测试
来源：http://fjt.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://gqj.jlsjyb.cn

[U79] PHP：静态分析
来源：http://fgo.tanke756.top

composer require --dev phpstan/phpstan
来源：http://bnc.shanyushiyangkeji.top

[U80] PHP：代码规范修复
来源：http://tok.chenjidiqi.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://kti.sjlbkw.cn

[U81] JS：初始化项目
来源：http://bgs.cashguo.top

npm init -y;  npm i express
来源：http://mov.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://bzm.jinyuanbaomall.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tjo.smart0.xyz

[U83] JS：ES Module 导入导出
来源：http://itu.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pow.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://jsq.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://zyg.xinyue.icu

[U85] JS：可选链
来源：http://pyw.jinqigufen.top

a?.b?.c
来源：http://fas.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://xmu.yongpay.top

a ?? b
来源：http://pwx.redwolf501.top

[U87] JS：解构默认值
来源：http://znl.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://guo.feifeiyinyue.top

[U88] JS：对象展开合并
来源：http://btm.zhiwuduotai.top

{ ...a, ...b }
来源：http://wxv.zhixingplan.top

[U89] JS：数组去重
来源：http://tmk.birdmap.top

[...new Set(arr)]
来源：http://nni.hywenlv.cn

[U90] JS：数字数组排序
来源：http://gfv.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://dzo.smart0.xyz

[U91] JS：对象键值遍历
来源：http://pps.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ner.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://cfx.jiagoushi.top

structuredClone(obj)
来源：http://cve.kuanghao11.cn

[U93] JS：模板字符串
来源：http://mzv.quarkkingdee.top

`共 ${n} 条`
来源：http://gii.yuanzhike.top

[U94] JS：箭头函数
来源：http://zqm.jiagoushi.top

const double = x => x * 2;
来源：http://wom.yj20258.top

[U95] JS：Promise 包装
来源：http://zuy.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://cfc.hesvh.cn

[U96] JS：async/await 与异常
来源：http://dxv.ywan-chungtsiang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uzc.xinyue.icu

[U97] JS：并发请求
来源：http://vyp.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bjd.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://wbj.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ism.yongpay.top

[U99] JS：事件监听
来源：http://kwr.zhijiandao.cn

el.addEventListener("click", e => {})
来源：http://wjq.nwbrower.top

[U100] JS：DOM 查询
来源：http://ins.fktsv.cn

document.querySelector(".item")
来源：http://yvn.smart0.xyz

[U101] JS：classList 操作
来源：http://hrv.316326.xyz

el.classList.toggle("active")
来源：http://bxk.cucudq.cn

[U102] JS：本地存储
来源：http://lyq.yj202588.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://phl.ppjwa.cn

[U103] JS：定时器
来源：http://cgg.mhx1999.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xcl.shanyushiyangtech.top

[U104] JS：防抖
来源：http://qpf.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qfm.cashguo.top

[U105] JS：节流
来源：http://mro.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://alf.guowangkeji.top

[U106] JS：日期格式化
来源：http://yde.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://egr.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://epr.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qvj.pycfn.com

[U108] JS：随机整数
来源：http://dti.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bpe.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://vee.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://ypn.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://cpg.jqgfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dgd.dianchejie.cn

[U111] JS：对象转 Map
来源：http://xtk.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://szf.gaohongyu789.top

[U112] JS：字符串补位
来源：http://etk.52xcode.cn

"7".padStart(3, "0")
来源：http://jri.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://xyu.guannengcc.top

s.replaceAll("a", "b")
来源：http://eir.ybcxt.top

[U114] JS：JSON 深比较
来源：http://gyz.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nag.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://kdy.ctjpmb.com

crypto.randomUUID()
来源：http://pcd.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://tut.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://knw.316326.xyz

[U117] JS：单元测试
来源：http://sxj.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://bqk.vehdjk.com

[U118] JS：开发服务器
来源：http://uub.cqqwz.cn

npm i -D vite;  npx vite
来源：http://wvb.zhixingplan.top

[U119] JS：生产构建
来源：http://tcd.jinqigfzy.top

npx vite build
来源：http://sfj.hammf.cn

[U120] JS：读取环境变量（Vite）
来源：http://fcz.sxryk.cn

import.meta.env.VITE_API_URL
来源：http://ply.yueranfly.top

================================================================================
来源：http://zqt.tian-w.cn

统计汇总
来源：http://zvw.yvedp.cn

================================================================================
来源：http://mvi.shzxlz.cn

按语言统计（条）：
来源：http://dfo.jinyuanbaomall.cn

Python ......... 252
来源：http://zoi.jiagoushi.top

PHP ............ 252
来源：http://ruo.jyoumei.cn

JavaScript ..... 252
来源：http://tvw.epnwcf.com

TypeScript ..... 212
来源：http://nsm.jinqigufen.top

Java ........... 212
来源：http://ice.aibaodan.cn

Go ............. 212
来源：http://zpv.meibo888.top

Ruby ........... 212
来源：http://irn.quarkkingdee.top

C# ............. 212
来源：http://djo.snrcjt.cn

C .............. 30
来源：http://wvi.xuetiantiany.cn

C++ ............ 30
来源：http://wuz.xingfuxueyuan.xyz

SQL ............ 90
来源：http://ale.mhx1999.top

Bash ........... 80
来源：http://lop.birdmap.top

Kotlin ......... 15
来源：http://hvs.hnxiangtu.top

Swift .......... 15
来源：http://ktw.zhixingplan.top

Lua ............ 10
来源：http://fqo.jyoumei.cn

Perl ........... 10
来源：http://ebi.birdmap.top

Scala .......... 10
来源：http://uvr.aibaodan.cn

------------------------------------
来源：http://ssa.vehdjk.com

合计 ........... 2106 条
来源：http://lis.cqqwz.cn

按章节统计：
来源：http://eep.aizwys.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bem.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mkc.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bgz.birdmap.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mok.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ted.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eoh.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nho.jinghuilouyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://odf.zycfv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vil.yfazqb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mwe.fehbvm.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pcf.guowangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://byc.hcnkem.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tiu.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zaq.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nmw.aizwys.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mvx.jqgfzy.top

Q SQL 专题                              90
来源：http://ipd.zhengqikj.top

R Bash 专题                             80
来源：http://nyg.andypj.xyz

S C / C++ 专题                          60
来源：http://akj.sufxvd.cn

T 其他语言补充                          60
来源：http://esb.hysaishi.cn

U 高频实用片段                         120
来源：http://gse.yangfankeji.com

------------------------------------
来源：http://yhw.cheryme.top

合计                                  2106 条
来源：http://yio.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://kux.ydjk.org.cn

使用提醒
来源：http://rmw.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://iii.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nft.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zel.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ymb.shanyushiyangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://acq.meibo888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wbz.feifeiyinyue.top

—— 文件结束 ——
来源：http://kak.yuanzhike.top

================================================================================
来源：http://vgh.yj20258888.top

程序语言常见例子速查手册（2024 版）
来源：http://ybq.xylfe.cn

Common Programming Examples Cheat Book
来源：http://uxy.nanxinkj.top

================================================================================
来源：http://rrx.jianghu66.top

【收录内容】
来源：http://wkc.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ciy.nanxuanxn.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oml.aibaodan.cn

SQL · Bash · C · C++
来源：http://dld.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ulr.feifeiyinyue.top

【使用说明】
来源：http://inb.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sqr.uphjek.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jhg.ydzc1.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wqv.hcnkem.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aez.sysykeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xau.xziqi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qlf.ehwqpu.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://npw.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rcb.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wou.xuanzx.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fxn.pycfn.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bwg.pengpengdd.cyou

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ayx.bbcook.cn

【文件统计】
来源：http://qjs.chenlongwang.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qoh.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://myw.yonumen.top

目  录
来源：http://qlp.yueranfly.top

--------------------------------------------------------------------------------
来源：http://xxr.zhaomingkeji.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ocu.vehdjk.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pmf.smart0.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nbf.zhongyouzk.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yqb.havefunace.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lvq.tarul.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gqb.c1oappe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xck.chenjidiqi.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gkq.hnxiangtu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uyt.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rqb.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ots.hesvh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vxd.zhijiandao.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yqt.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rpu.vqdsnc.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oxp.kuanghao11.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lnh.jqgufenzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sfq.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ykp.jinghuilouyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yuq.jianghu66.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nld.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oqp.daria6918.cn

================================================================================
来源：http://vpc.ydzc1.top

A. 基础语法与类型
来源：http://pgm.yj20258.top

================================================================================
来源：http://btn.yonumen.top

[A01] Hello World
来源：http://wal.svipenyu.cn

Py:   print("Hello, World!")
来源：http://ctu.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://kfs.zhaomingkeji.xyz

JS:   console.log("Hello, World!");
来源：http://fme.yj20258.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uir.redwolf501.top

Java: System.out.println("Hello, World!");
来源：http://uoa.yvedp.cn

Go:   fmt.Println("Hello, World!")
来源：http://wbd.shanyushiyangkeji.top

Ruby: puts "Hello, World!"
来源：http://gth.zdbjq.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ffa.bbcook.cn

[A02] 变量声明与赋值
来源：http://tkm.zhoulong.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://drd.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xtg.tanke756.top

JS:   let name = "Alex"; const age = 20;
来源：http://kbc.meibo888.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oyn.zhaomingkeji.xyz

Java: String name = "Alex"; int age = 20;
来源：http://eyn.jinyuanbaomall.cn

Go:   name := "Alex"; age := 20
来源：http://vke.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://wzg.jlsjyb.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hyz.0kj1m.cn

[A03] 常量定义
来源：http://nkj.xinyue.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gsf.hywenlv.cn

PHP:  const PI = 3.14159;
来源：http://xkn.zycfv.cn

JS:   const PI = 3.14159;
来源：http://jmq.epnwcf.com

TS:   const PI: number = 3.14159;
来源：http://jsn.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://gdd.hammf.cn

Go:   const PI = 3.14159
来源：http://vql.chenlongwang.top

Ruby: PI = 3.14159
来源：http://kcp.cdnleiting.top

C#:   const double PI = 3.14159;
来源：http://xfe.fzhhl.top

[A04] 判断变量类型
来源：http://mee.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://qdq.zycfv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://npf.kuanghao11.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xiu.tian-w.cn

TS:   typeof x; x instanceof Date
来源：http://cok.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tha.sxryk.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rpp.yvedp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xkd.fzhhl.top

C#:   x.GetType().Name; x is int
来源：http://xkc.cheryme.top

[A05] 整数除法与取模
来源：http://amf.pengpengdd.cyou

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wtt.svipenyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pqm.bbcook.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xqv.c1oappe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hhh.jinqigfzy.top

Java: 7 / 2; 7 % 2
来源：http://ivx.redwolf501.top

Go:   7 / 2; 7 % 2
来源：http://zgn.wangdashe.top

Ruby: 7 / 2; 7 % 2
来源：http://phd.yangfankeji.com

C#:   7 / 2; 7 % 2
来源：http://psv.jianghu66.top

[A06] 字符串转数字
来源：http://lpo.jinghuilouyu.cn

Py:   int("42"); float("3.14")
来源：http://ghi.dashuyun.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://khl.ybcxt.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ymd.nanxinkj.top

TS:   parseInt("42", 10); Number("42")
来源：http://pda.sjlbkw.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yuy.zhengqikj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lmw.meibo888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xpw.nanxinkj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ikm.jqgufenzy.top

[A07] 数字转字符串
来源：http://aur.cucudq.cn

Py:   str(42)
来源：http://poa.hammf.cn

PHP:  (string) 42; strval(42)
来源：http://lfo.yj20258888.top

JS:   String(42); (42).toString()
来源：http://mjs.xziqi.cn

TS:   String(42)
来源：http://yyo.andypj.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://aqx.yueranfly.top

Go:   strconv.Itoa(42)
来源：http://wzb.ctjpmb.com

Ruby: 42.to_s
来源：http://snd.hnxiangtu.top

C#:   42.ToString()
来源：http://zlm.jlsjyb.cn

[A08] 取整与四舍五入
来源：http://eos.ybcxt.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ykj.sweek.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tsu.cashguo.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hvy.hammf.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wmr.nwbrower.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pqv.sysykeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kll.c1oappe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ekq.zhengqikj.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kks.sweek.top

[A09] 绝对值与最大最小值
来源：http://tie.pengpengdd.cyou

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://clm.yanxiufei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ziu.shanyushiyangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yzd.havefunace.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vbi.smart0.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://egt.yonumen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ggr.nanxinkj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xpk.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xsp.sxryk.cn

[A10] 生成随机数
来源：http://fbs.zhaomingkeji.xyz

Py:   import random; random.randint(1, 100)
来源：http://sqe.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://egz.pengpengdd.cyou

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zaf.gotoacloud.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ybp.yj202588.top

Java: new Random().nextInt(100) + 1
来源：http://qpz.jianghu66.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://roh.c1oappe.top

Ruby: rand(1..100)
来源：http://xos.316326.xyz

C#:   new Random().Next(1, 101)
来源：http://vcq.guannengcc.top

[A11] 条件表达式（三元）
来源：http://gyc.xuanzx.com

Py:   "yes" if x > 0 else "no"
来源：http://vea.52xcode.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qzn.guannengcc.top


<!-- 参考信息 -->