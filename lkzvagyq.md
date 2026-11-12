代发 wailian999

[U75] PHP：依赖注入
来源：http://dvt.havefunace.top

composer require psr/container
来源：http://zjm.xuanzx.com

[U76] PHP：简单路由
来源：http://utr.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://htk.jqgfzy.top

[U77] PHP：模板渲染
来源：http://rvs.zhixingplan.top

composer require twig/twig
来源：http://kay.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://hbk.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://xmr.yvedp.cn

[U79] PHP：静态分析
来源：http://zvr.52xcode.cn

composer require --dev phpstan/phpstan
来源：http://lck.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://tqy.guannengcc.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dop.quarkkingdee.top

[U81] JS：初始化项目
来源：http://wbo.sysykeji.top

npm init -y;  npm i express
来源：http://eyx.hcnkem.com

[U82] JS：package.json 脚本
来源：http://bvf.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zsv.shanyushiyangkeji.top

[U83] JS：ES Module 导入导出
来源：http://nzo.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://oqy.wangshuangyany.cn

[U84] JS：CommonJS 写法
来源：http://jap.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tub.nwbrower.top

[U85] JS：可选链
来源：http://xjy.yj20258888.top

a?.b?.c
来源：http://eil.yueranfly.top

[U86] JS：空值合并
来源：http://rhq.mhx1999.top

a ?? b
来源：http://fra.aibaodan.cn

[U87] JS：解构默认值
来源：http://uxs.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://pls.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://nia.gzhubu.top

{ ...a, ...b }
来源：http://hau.c1oappe.top

[U89] JS：数组去重
来源：http://gnw.shzxlz.cn

[...new Set(arr)]
来源：http://nio.nanxinkj.top

[U90] JS：数字数组排序
来源：http://own.guannengcc.top

[...arr].sort((a, b) => a - b)
来源：http://cfg.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://ruz.gogol.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ntu.jiagoushi.top

[U92] JS：深拷贝
来源：http://yup.shanyushiyangkeji.top

structuredClone(obj)
来源：http://gej.guowangkeji.top

[U93] JS：模板字符串
来源：http://apy.zhengqikj.top

`共 ${n} 条`
来源：http://wri.cheryme.top

[U94] JS：箭头函数
来源：http://muo.hywenlv.cn

const double = x => x * 2;
来源：http://lrg.feifeiyinyue.top

[U95] JS：Promise 包装
来源：http://noh.aizwys.cn

new Promise((resolve, reject) => {})
来源：http://sdm.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://clb.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zqj.sufxvd.cn

[U97] JS：并发请求
来源：http://pyo.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xii.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://tzc.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jfu.jinqigfzy.top

[U99] JS：事件监听
来源：http://aaj.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://xmd.fktsv.cn

[U100] JS：DOM 查询
来源：http://mtg.havefunace.top

document.querySelector(".item")
来源：http://btk.zhoulong.xyz

[U101] JS：classList 操作
来源：http://jce.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://tzo.chenjidiqi.icu

[U102] JS：本地存储
来源：http://jgx.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://seb.havefunace.top

[U103] JS：定时器
来源：http://nlr.zhiwuduotai.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fih.jianghu66.top

[U104] JS：防抖
来源：http://vde.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xgy.kuanghao11.cn

[U105] JS：节流
来源：http://gvq.yfazqb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ies.hfpthk.cn

[U106] JS：日期格式化
来源：http://lly.yuanzhike.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://txi.birdmap.top

[U107] JS：数字千分位
来源：http://ide.cheryme.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://spv.yj20258.top

[U108] JS：随机整数
来源：http://vad.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blb.jqgufenzy.top

[U109] JS：数组分组
来源：http://xiy.guowangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://hkm.hysaishi.cn

[U110] JS：数组分块
来源：http://rzd.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nwi.fehbvm.com

[U111] JS：对象转 Map
来源：http://max.yuxming.cn

new Map(Object.entries(obj))
来源：http://qre.ydzc1.top

[U112] JS：字符串补位
来源：http://eqd.nanxuanxn.top

"7".padStart(3, "0")
来源：http://wec.mhx1999.top

[U113] JS：正则替换全部
来源：http://xti.xuanzx.com

s.replaceAll("a", "b")
来源：http://kga.xingfuxueyuan.xyz

[U114] JS：JSON 深比较
来源：http://dtq.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fim.cheryme.top

[U115] JS：生成 UUID
来源：http://opb.ydjk.org.cn

crypto.randomUUID()
来源：http://zls.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://xvc.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://fpl.ivvv.top

[U117] JS：单元测试
来源：http://rki.ywan-chungtsiang.top

npm i -D vitest;  npx vitest
来源：http://pgx.nanxinkj.top

[U118] JS：开发服务器
来源：http://vot.havefunace.top

npm i -D vite;  npx vite
来源：http://snk.jlsjyb.cn

[U119] JS：生产构建
来源：http://sda.sufxvd.cn

npx vite build
来源：http://men.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://pxp.yueranfly.top

import.meta.env.VITE_API_URL
来源：http://yxi.chenzaomai.com

================================================================================
来源：http://cjw.feifeiyinyue.top

统计汇总
来源：http://lay.yuanzhike.top

================================================================================
来源：http://phd.zdqjudy.top

按语言统计（条）：
来源：http://ggf.cqqwz.cn

Python ......... 252
来源：http://qzb.hcnkem.com

PHP ............ 252
来源：http://cjf.cucudq.cn

JavaScript ..... 252
来源：http://qzf.zdbjq.cn

TypeScript ..... 212
来源：http://abj.sjlbkw.cn

Java ........... 212
来源：http://jck.fktsv.cn

Go ............. 212
来源：http://upw.cqqwz.cn

Ruby ........... 212
来源：http://nqo.pengpengdd.cyou

C# ............. 212
来源：http://uhh.gotoacloud.top

C .............. 30
来源：http://aac.zdqjudy.top

C++ ............ 30
来源：http://ehf.yanxiufei.cn

SQL ............ 90
来源：http://bor.0kj1m.cn

Bash ........... 80
来源：http://ixw.zhixingplan.top

Kotlin ......... 15
来源：http://epc.ivvv.top

Swift .......... 15
来源：http://pzb.sysykeji.top

Lua ............ 10
来源：http://gfn.hongshengwenyu.top

Perl ........... 10
来源：http://bev.yanxiufei.cn

Scala .......... 10
来源：http://bkr.xuetiantiany.cn

------------------------------------
来源：http://xzb.fanxiaobao.xyz

合计 ........... 2106 条
来源：http://nun.chenzaomai.com

按章节统计：
来源：http://zqx.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ewc.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tsa.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://njz.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pep.zhixingplan.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cve.xinyue.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://doe.jinqigufen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xul.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pmh.gzhubu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://adv.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hdm.mhx1999.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wjo.jyoumei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lcr.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://whz.ydzc1.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oxc.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oal.cdnleiting.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rwe.zhoulong.xyz

Q SQL 专题                              90
来源：http://lvc.shzxlz.cn

R Bash 专题                             80
来源：http://ifm.gogol.net.cn

S C / C++ 专题                          60
来源：http://qvs.andypj.xyz

T 其他语言补充                          60
来源：http://ckd.tarul.cn

U 高频实用片段                         120
来源：http://bzv.sjlbkw.cn

------------------------------------
来源：http://vpj.aizwys.cn

合计                                  2106 条
来源：http://rpn.tian-w.cn

--------------------------------------------------------------------------------
来源：http://hoi.aizwys.cn

使用提醒
来源：http://lvh.xylfe.cn

--------------------------------------------------------------------------------
来源：http://oqw.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oay.birdmap.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vam.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://spa.epnwcf.com

在旧版本上使用前请先确认语法支持情况。
来源：http://vdk.ivvv.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zys.dianchejie.cn

—— 文件结束 ——
来源：http://wnv.chenlongwang.top

================================================================================
来源：http://ame.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://sbt.hcnkem.com

Common Programming Examples Cheat Book
来源：http://lhy.sjlbkw.cn

================================================================================
来源：http://min.gotoacloud.top

【收录内容】
来源：http://rtz.fktsv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vdn.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bxt.cqqwz.cn

SQL · Bash · C · C++
来源：http://ebl.chenjidiqi.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jyo.sweek.top

【使用说明】
来源：http://jzw.ywan-chungtsiang.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://chb.epnwcf.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zpm.fehbvm.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ocg.yj20258.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://acr.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://ano.tianlin.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ntb.shzxlz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ejy.jinqigufen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qaf.ivvv.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hea.shanyushiyangtech.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://omc.shzxlz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gel.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bul.316326.xyz

【文件统计】
来源：http://ods.feifeiyinyue.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sap.yvedp.cn

--------------------------------------------------------------------------------
来源：http://sbi.dashuyun.cn

目  录
来源：http://hpy.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://gnr.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wyn.snrcjt.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://abq.gaohongyu789.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://iot.dashuyun.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://etj.tianlin.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dxc.hongshengwenyu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wfp.9152youxi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hrv.sweek.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zlp.chenjidiqi.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lfe.bjfxy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zug.dianchejie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wjo.cheryme.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://skv.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zpe.yuanzhike.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://whs.tian-w.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://viw.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://koc.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jfs.snrcjt.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bfu.shzxlz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dvl.0kj1m.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wdb.yongpay.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tdt.meibo888.top

================================================================================
来源：http://vrw.zhengqikj.top

A. 基础语法与类型
来源：http://ack.zhaomingkeji.xyz

================================================================================
来源：http://oqw.yonumen.top

[A01] Hello World
来源：http://lye.cashguo.top

Py:   print("Hello, World!")
来源：http://hgw.zhengqikj.top

PHP:  echo "Hello, World!";
来源：http://wvl.vehdjk.com

JS:   console.log("Hello, World!");
来源：http://mtp.9152youxi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rdc.dianchejie.cn

Java: System.out.println("Hello, World!");
来源：http://ubw.gzhubu.top

Go:   fmt.Println("Hello, World!")
来源：http://yqu.sufxvd.cn

Ruby: puts "Hello, World!"
来源：http://trd.vehdjk.com

C#:   Console.WriteLine("Hello, World!");
来源：http://ldl.vehdjk.com

[A02] 变量声明与赋值
来源：http://qvv.pycfn.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ysz.cqqwz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ofw.jinyuanbaomall.cn

JS:   let name = "Alex"; const age = 20;
来源：http://atz.cheryme.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gmj.zhengqikj.top

Java: String name = "Alex"; int age = 20;
来源：http://iku.yj20258888.top

Go:   name := "Alex"; age := 20
来源：http://lmc.yuxming.cn

Ruby: name = "Alex"; age = 20
来源：http://bif.daxiang520.top

C#:   string name = "Alex"; int age = 20;
来源：http://qok.fehbvm.com

[A03] 常量定义
来源：http://iom.andypj.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://osm.sysykeji.top

PHP:  const PI = 3.14159;
来源：http://rgm.jqgufenzy.top

JS:   const PI = 3.14159;
来源：http://kyi.jiagoushi.top

TS:   const PI: number = 3.14159;
来源：http://vdw.0kj1m.cn

Java: static final double PI = 3.14159;
来源：http://erv.tanke756.top

Go:   const PI = 3.14159
来源：http://qpx.sufxvd.cn

Ruby: PI = 3.14159
来源：http://yjs.xinyue.icu

C#:   const double PI = 3.14159;
来源：http://bqy.hfpthk.cn

[A04] 判断变量类型
来源：http://yoh.pycfn.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://auw.tarul.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fon.gaohongyu789.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cow.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://kvv.xziqi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hrb.birdmap.top

Go:   reflect.TypeOf(x).Name()
来源：http://qkz.jiagoushi.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lhc.epnwcf.com

C#:   x.GetType().Name; x is int
来源：http://mag.shanyushiyangtech.top

[A05] 整数除法与取模
来源：http://zch.shanyushiyangkeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tod.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://pao.jinqigufen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mrs.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wcw.ehwqpu.com

Java: 7 / 2; 7 % 2
来源：http://jbg.ppjwa.cn

Go:   7 / 2; 7 % 2
来源：http://xvj.cucudq.cn

Ruby: 7 / 2; 7 % 2
来源：http://pyf.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://ojc.jyoumei.cn

[A06] 字符串转数字
来源：http://bzt.svipenyu.cn

Py:   int("42"); float("3.14")
来源：http://yyg.andypj.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fpn.ehwqpu.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rjh.nwbrower.top

TS:   parseInt("42", 10); Number("42")
来源：http://zee.cdnleiting.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vmm.yj20258888.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qij.yfazqb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://vxg.cucudq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oqj.yongpay.top

[A07] 数字转字符串
来源：http://eht.epnwcf.com

Py:   str(42)
来源：http://ysf.vqdsnc.cn

PHP:  (string) 42; strval(42)
来源：http://dul.shuidangran.top

JS:   String(42); (42).toString()
来源：http://xsl.hnqzz.top

TS:   String(42)
来源：http://qbh.yuxming.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nqr.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://gim.chenzaomai.com

Ruby: 42.to_s
来源：http://wka.tarul.cn

C#:   42.ToString()
来源：http://wfk.hywenlv.cn

[A08] 取整与四舍五入
来源：http://bzx.jqgufenzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dbc.52xcode.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wyf.gzhubu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://asz.daxiang520.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uez.yj202588.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ljw.yanxiufei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vuz.yvedp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kno.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dvj.chenlongwang.top

[A09] 绝对值与最大最小值
来源：http://vme.tian-w.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ttz.shuidangran.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mny.redwolf501.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qfs.wangdashe.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gov.yonumen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rug.yfazqb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zpf.nanxinkj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://izy.mhx1999.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ejt.epnwcf.com

[A10] 生成随机数
来源：http://rrx.0kj1m.cn

Py:   import random; random.randint(1, 100)
来源：http://rqm.52xcode.cn

PHP:  random_int(1, 100);
来源：http://qnu.ppjwa.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hsb.vehdjk.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wac.gaohongyu789.top

Java: new Random().nextInt(100) + 1
来源：http://tsu.0kj1m.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uby.fengsongda.top

Ruby: rand(1..100)
来源：http://yig.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://fyy.yuxming.cn

[A11] 条件表达式（三元）
来源：http://bfk.daxiang520.top

Py:   "yes" if x > 0 else "no"
来源：http://lbk.bjfxy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kqo.shzxlz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dau.uphjek.com

TS:   x > 0 ? "yes" : "no"
来源：http://rsx.jinqigufen.top

Java: x > 0 ? "yes" : "no"
来源：http://fhh.daria6918.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jiz.sufxvd.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pfa.nanxuanxn.top

C#:   x > 0 ? "yes" : "no"
来源：http://ctm.aibaodan.cn

[A12] 字符串插值 / 格式化
来源：http://jva.9152youxi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eia.hammf.cn


<!-- 参考信息 -->