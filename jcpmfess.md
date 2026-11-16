代发 wailian999

[U77] PHP：模板渲染
来源：http://arm.sysykeji.top

composer require twig/twig
来源：http://xao.bjfxy.top

[U78] PHP：单元测试
来源：http://nhc.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://pfw.xziqi.cn

[U79] PHP：静态分析
来源：http://nqd.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://ikn.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://cpi.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yzh.ppjwa.cn

[U81] JS：初始化项目
来源：http://iro.zhongyouzk.top

npm init -y;  npm i express
来源：http://mht.yj20258.top

[U82] JS：package.json 脚本
来源：http://xsf.ctjpmb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ipf.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://koy.sufxvd.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mfh.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://rfi.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fti.yj20258888.top

[U85] JS：可选链
来源：http://ysg.ctjpmb.com

a?.b?.c
来源：http://zxq.yj20258.top

[U86] JS：空值合并
来源：http://dpe.0kj1m.cn

a ?? b
来源：http://bfj.haohaochexian.top

[U87] JS：解构默认值
来源：http://ska.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://qzx.snrcjt.cn

[U88] JS：对象展开合并
来源：http://vbc.chenzaomai.com

{ ...a, ...b }
来源：http://xca.hesvh.cn

[U89] JS：数组去重
来源：http://yvc.snrcjt.cn

[...new Set(arr)]
来源：http://wjv.jiagoushi.top

[U90] JS：数字数组排序
来源：http://ifl.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://tin.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://add.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cbv.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://ctk.chenzaomai.com

structuredClone(obj)
来源：http://oer.hfpthk.cn

[U93] JS：模板字符串
来源：http://wgp.0kj1m.cn

`共 ${n} 条`
来源：http://zzi.jqgufenzy.top

[U94] JS：箭头函数
来源：http://rap.guowangkeji.top

const double = x => x * 2;
来源：http://uya.guowangkeji.top

[U95] JS：Promise 包装
来源：http://nhe.hnqzz.top

new Promise((resolve, reject) => {})
来源：http://nwz.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://adc.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nnr.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://qzt.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://sxi.guannengcc.top

[U98] JS：fetch 带 JSON
来源：http://msg.52xcode.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qfy.meibo888.top

[U99] JS：事件监听
来源：http://yor.bjfxy.top

el.addEventListener("click", e => {})
来源：http://kti.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://cjl.yuanzhike.top

document.querySelector(".item")
来源：http://ymg.redwolf501.top

[U101] JS：classList 操作
来源：http://vef.sufxvd.cn

el.classList.toggle("active")
来源：http://dsq.nanxinkj.top

[U102] JS：本地存储
来源：http://bsa.jiagoushi.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dly.snrcjt.cn

[U103] JS：定时器
来源：http://its.zdqjudy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rmt.ppjwa.cn

[U104] JS：防抖
来源：http://dxi.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://end.jinqigfzy.top

[U105] JS：节流
来源：http://cbb.cqqwz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://orj.hnqzz.top

[U106] JS：日期格式化
来源：http://iig.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rwr.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://njs.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vei.daxiang520.top

[U108] JS：随机整数
来源：http://yns.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mkd.jinqigufen.top

[U109] JS：数组分组
来源：http://xgq.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://uyt.zhaomingkeji.xyz

[U110] JS：数组分块
来源：http://zwx.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iia.feifeiyinyue.top

[U111] JS：对象转 Map
来源：http://twm.gzhubu.top

new Map(Object.entries(obj))
来源：http://kur.yj20258888.top

[U112] JS：字符串补位
来源：http://uxo.chenjidiqi.icu

"7".padStart(3, "0")
来源：http://bxh.hesvh.cn

[U113] JS：正则替换全部
来源：http://mdw.smart0.xyz

s.replaceAll("a", "b")
来源：http://zna.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://hys.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://knn.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://rlt.sjlbkw.cn

crypto.randomUUID()
来源：http://xey.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://udn.ybcxt.top

/** @param {string} name */ function f(name) {}
来源：http://lxd.nwbrower.top

[U117] JS：单元测试
来源：http://gxj.epnwcf.com

npm i -D vitest;  npx vitest
来源：http://lfe.gogol.net.cn

[U118] JS：开发服务器
来源：http://kmr.316326.xyz

npm i -D vite;  npx vite
来源：http://wbz.hywenlv.cn

[U119] JS：生产构建
来源：http://qtc.ywan-chungtsiang.top

npx vite build
来源：http://iwo.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://hen.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://nuo.xuetiantiany.cn

================================================================================
来源：http://kbl.uphjek.com

统计汇总
来源：http://zup.zdqjudy.top

================================================================================
来源：http://iro.nanxuanxn.top

按语言统计（条）：
来源：http://ryw.shzxlz.cn

Python ......... 252
来源：http://dut.jqgufenzy.top

PHP ............ 252
来源：http://lxh.wangdashe.top

JavaScript ..... 252
来源：http://fth.wangshuangyany.cn

TypeScript ..... 212
来源：http://uzy.redwolf501.top

Java ........... 212
来源：http://cdo.pengpengdd.cyou

Go ............. 212
来源：http://rrn.yfazqb.com

Ruby ........... 212
来源：http://zoo.daxiang520.top

C# ............. 212
来源：http://fyy.jinqigufen.top

C .............. 30
来源：http://rfs.uphjek.com

C++ ............ 30
来源：http://bmk.jqgfzy.top

SQL ............ 90
来源：http://bxh.snrcjt.cn

Bash ........... 80
来源：http://ffl.yangfankeji.com

Kotlin ......... 15
来源：http://xfh.ctjpmb.com

Swift .......... 15
来源：http://byo.nwbrower.top

Lua ............ 10
来源：http://eax.wangshuangyany.cn

Perl ........... 10
来源：http://zei.c1oappe.top

Scala .......... 10
来源：http://lcb.chenzaomai.com

------------------------------------
来源：http://yho.iojbl.cn

合计 ........... 2106 条
来源：http://kcu.yongpay.top

按章节统计：
来源：http://xip.aibaodan.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bbs.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lcq.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tnw.jyoumei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lvf.zhengqikj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://izi.xylfe.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ypz.wangshuangyany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ilz.zhixingplan.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://onv.yj20258888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rnf.jqgfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://acg.chenlongwang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ooe.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zqp.zhongyouzk.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dkb.hfpthk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cte.quarkkingdee.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qpa.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zbo.tanke756.top

Q SQL 专题                              90
来源：http://igq.jinqigufen.top

R Bash 专题                             80
来源：http://esc.ivvv.top

S C / C++ 专题                          60
来源：http://pdf.yvedp.cn

T 其他语言补充                          60
来源：http://fgr.xinyue.icu

U 高频实用片段                         120
来源：http://any.9152youxi.cn

------------------------------------
来源：http://qig.yuxming.cn

合计                                  2106 条
来源：http://hwo.mhx1999.top

--------------------------------------------------------------------------------
来源：http://akf.sysykeji.top

使用提醒
来源：http://wtl.shuidangran.top

--------------------------------------------------------------------------------
来源：http://rnt.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cld.hysaishi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://szy.vqdsnc.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ejs.shanyushiyangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://srk.dashuyun.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gzv.jlsjyb.cn

—— 文件结束 ——
来源：http://hnn.pycfn.com

================================================================================
来源：http://whi.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://dps.quarkkingdee.top

Common Programming Examples Cheat Book
来源：http://vvb.gaohongyu789.top

================================================================================
来源：http://wvq.hammf.cn

【收录内容】
来源：http://jmw.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://mjm.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ylb.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://eol.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pdl.zycfv.cn

【使用说明】
来源：http://ysu.jiagoushi.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zwv.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hzv.0kj1m.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dxs.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xlj.xingfuxueyuan.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://bim.wangdashe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vgy.gaohongyu789.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ons.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://moj.ybcxt.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yfh.zdbjq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xsn.hongshengwenyu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tsj.hammf.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zzd.cdnleiting.top

【文件统计】
来源：http://noz.zhoulong.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ozm.jianghu66.top

--------------------------------------------------------------------------------
来源：http://ybj.hammf.cn

目  录
来源：http://mnb.bbcook.cn

--------------------------------------------------------------------------------
来源：http://vig.nwbrower.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bta.hesvh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wlt.daxiang520.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qhr.pycfn.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yzt.cdnleiting.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kkj.shanyushiyangtech.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vud.nanxinkj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cwk.epnwcf.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oly.zhengqikj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kkb.nanxinkj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mzy.zhijiandao.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xzl.yuanzhike.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pka.xinyue.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zik.havefunace.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qcr.yueranfly.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qdt.redwolf501.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hyw.ctjpmb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://boj.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://xye.fehbvm.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lro.andypj.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ndd.aibaodan.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wpz.dianchejie.cn

================================================================================
来源：http://eok.0kj1m.cn

A. 基础语法与类型
来源：http://znk.9152youxi.cn

================================================================================
来源：http://chy.yangfankeji.com

[A01] Hello World
来源：http://yva.vqdsnc.cn

Py:   print("Hello, World!")
来源：http://cgk.0kj1m.cn

PHP:  echo "Hello, World!";
来源：http://kaq.fzhhl.top

JS:   console.log("Hello, World!");
来源：http://afs.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lzd.daria6918.cn

Java: System.out.println("Hello, World!");
来源：http://iog.shzxlz.cn

Go:   fmt.Println("Hello, World!")
来源：http://xfh.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://lur.zhengqikj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mfr.jyoumei.cn

[A02] 变量声明与赋值
来源：http://fmu.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fje.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://pxb.zdbjq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dkv.yj202588.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tqo.jinqigfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://iqy.0kj1m.cn

Go:   name := "Alex"; age := 20
来源：http://fjk.c1oappe.top

Ruby: name = "Alex"; age = 20
来源：http://fkd.jiagoushi.top

C#:   string name = "Alex"; int age = 20;
来源：http://pwu.guannengcc.top

[A03] 常量定义
来源：http://bnu.bjfxy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qrc.ydzc1.top

PHP:  const PI = 3.14159;
来源：http://kwv.c1oappe.top

JS:   const PI = 3.14159;
来源：http://zij.yj20258888.top

TS:   const PI: number = 3.14159;
来源：http://kci.jlsjyb.cn

Java: static final double PI = 3.14159;
来源：http://qpu.aizwys.cn

Go:   const PI = 3.14159
来源：http://hqh.zdqjudy.top

Ruby: PI = 3.14159
来源：http://gol.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://shg.pycfn.com

[A04] 判断变量类型
来源：http://jmc.yfazqb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://vny.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://awm.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ser.9152youxi.cn

TS:   typeof x; x instanceof Date
来源：http://udb.ydzc1.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gwx.vqdsnc.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lda.cashguo.top

Ruby: x.class; x.is_a?(Integer)
来源：http://osp.sufxvd.cn

C#:   x.GetType().Name; x is int
来源：http://oao.vqdsnc.cn

[A05] 整数除法与取模
来源：http://lqb.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gzl.gzhubu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jof.ivvv.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eeo.shangyingyoupin.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ooq.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://ril.andypj.xyz

Go:   7 / 2; 7 % 2
来源：http://mwg.jinqigufen.top

Ruby: 7 / 2; 7 % 2
来源：http://yyv.cucudq.cn

C#:   7 / 2; 7 % 2
来源：http://xiw.xingfuxueyuan.xyz

[A06] 字符串转数字
来源：http://jhe.nanxuanxn.top

Py:   int("42"); float("3.14")
来源：http://xcu.zhiwuduotai.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uas.ywan-chungtsiang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jgg.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://ttm.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://efk.yj202588.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fqu.ydzc1.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zwi.sjlbkw.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sbs.zycfv.cn

[A07] 数字转字符串
来源：http://bfq.shuidangran.top

Py:   str(42)
来源：http://dnc.cashguo.top

PHP:  (string) 42; strval(42)
来源：http://xif.yj202588.top

JS:   String(42); (42).toString()
来源：http://gwq.yfazqb.com

TS:   String(42)
来源：http://jyx.zhengqikj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nbd.yanxiufei.cn

Go:   strconv.Itoa(42)
来源：http://qas.gzhubu.top

Ruby: 42.to_s
来源：http://ewh.hysaishi.cn

C#:   42.ToString()
来源：http://enw.andypj.xyz

[A08] 取整与四舍五入
来源：http://eli.xuanzx.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ips.xuetiantiany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tkl.svipenyu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ymx.xziqi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kjj.yvedp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jjz.jlsjyb.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://juv.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vcp.fengsongda.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rmw.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://idk.zdbjq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tya.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lnc.hywenlv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uvz.sysykeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vwc.meibo888.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://msu.yueranfly.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uqp.tianlin.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ilc.jinghuilouyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rsu.zhongyouzk.top

[A10] 生成随机数
来源：http://tjx.tian-w.cn

Py:   import random; random.randint(1, 100)
来源：http://nyt.zhengqikj.top

PHP:  random_int(1, 100);
来源：http://ljr.tarul.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nvd.snrcjt.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pvf.jiagoushi.top

Java: new Random().nextInt(100) + 1
来源：http://obq.xingfuxueyuan.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nev.pycfn.com

Ruby: rand(1..100)
来源：http://ial.c1oappe.top

C#:   new Random().Next(1, 101)
来源：http://hxg.ybcxt.top

[A11] 条件表达式（三元）
来源：http://tek.quarkkingdee.top

Py:   "yes" if x > 0 else "no"
来源：http://hsr.wangdashe.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://dhy.316326.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://qca.yueranfly.top

TS:   x > 0 ? "yes" : "no"
来源：http://xkr.zhongyouzk.top

Java: x > 0 ? "yes" : "no"
来源：http://kgc.cashguo.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mdi.cdnleiting.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fnv.zdbjq.cn

C#:   x > 0 ? "yes" : "no"
来源：http://syn.aibaodan.cn

[A12] 字符串插值 / 格式化
来源：http://huk.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rbh.tarul.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dpl.c1oappe.top

JS:   `Hello, ${name}!`
来源：http://bkx.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://bcz.tianlin.xyz

Java: "Hello, %s!".formatted(name)
来源：http://uhj.52xcode.cn


<!-- 参考信息 -->