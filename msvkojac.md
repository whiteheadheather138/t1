代发 wailian999

[U75] PHP：依赖注入
来源：http://wme.chenzaomai.com

composer require psr/container
来源：http://gdi.aizwys.cn

[U76] PHP：简单路由
来源：http://xgh.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ivu.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://pgz.ctjpmb.com

composer require twig/twig
来源：http://sfq.vqdsnc.cn

[U78] PHP：单元测试
来源：http://mgw.daxiang520.top

composer require --dev phpunit/phpunit
来源：http://dux.birdmap.top

[U79] PHP：静态分析
来源：http://lds.gaohongyu789.top

composer require --dev phpstan/phpstan
来源：http://gcs.cucudq.cn

[U80] PHP：代码规范修复
来源：http://jkp.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://uhn.gaohongyu789.top

[U81] JS：初始化项目
来源：http://fke.zdqjudy.top

npm init -y;  npm i express
来源：http://ysn.yj202588.top

[U82] JS：package.json 脚本
来源：http://adf.316326.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vay.yj202588.top

[U83] JS：ES Module 导入导出
来源：http://pyj.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://myf.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://kuk.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lte.hnqzz.top

[U85] JS：可选链
来源：http://cqm.tarul.cn

a?.b?.c
来源：http://mfn.yanxiufei.cn

[U86] JS：空值合并
来源：http://jhs.bbcook.cn

a ?? b
来源：http://jac.guowangkeji.top

[U87] JS：解构默认值
来源：http://ofz.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://myz.chenzaomai.com

[U88] JS：对象展开合并
来源：http://hzt.yanxiufei.cn

{ ...a, ...b }
来源：http://ifn.yj202588.top

[U89] JS：数组去重
来源：http://fvr.gaohongyu789.top

[...new Set(arr)]
来源：http://hwq.hcnkem.com

[U90] JS：数字数组排序
来源：http://sbf.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://vhx.uphjek.com

[U91] JS：对象键值遍历
来源：http://epp.uphjek.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hok.fehbvm.com

[U92] JS：深拷贝
来源：http://btu.yfazqb.com

structuredClone(obj)
来源：http://tvm.jlsjyb.cn

[U93] JS：模板字符串
来源：http://krw.sjlbkw.cn

`共 ${n} 条`
来源：http://kkh.aizwys.cn

[U94] JS：箭头函数
来源：http://kwe.cheryme.top

const double = x => x * 2;
来源：http://llv.tarul.cn

[U95] JS：Promise 包装
来源：http://epf.0kj1m.cn

new Promise((resolve, reject) => {})
来源：http://ppa.c1oappe.top

[U96] JS：async/await 与异常
来源：http://bxh.shangyingyoupin.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sgg.fengsongda.top

[U97] JS：并发请求
来源：http://fzv.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://hzv.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://enn.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://duk.fktsv.cn

[U99] JS：事件监听
来源：http://evy.52xcode.cn

el.addEventListener("click", e => {})
来源：http://dsp.bbcook.cn

[U100] JS：DOM 查询
来源：http://wen.0kj1m.cn

document.querySelector(".item")
来源：http://wqd.fehbvm.com

[U101] JS：classList 操作
来源：http://ddi.zhengqikj.top

el.classList.toggle("active")
来源：http://upr.andypj.xyz

[U102] JS：本地存储
来源：http://ynd.zhixingplan.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xfl.ppjwa.cn

[U103] JS：定时器
来源：http://swb.jqgufenzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://klf.quarkkingdee.top

[U104] JS：防抖
来源：http://urr.xziqi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zre.cashguo.top

[U105] JS：节流
来源：http://ach.meibo888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oyo.jqgufenzy.top

[U106] JS：日期格式化
来源：http://tqv.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uqa.jinqigufen.top

[U107] JS：数字千分位
来源：http://mkt.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bbk.sjlbkw.cn

[U108] JS：随机整数
来源：http://hxx.xuanzx.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://suu.yueranfly.top

[U109] JS：数组分组
来源：http://npy.guowangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://zaf.fzhhl.top

[U110] JS：数组分块
来源：http://zeb.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yjr.zdqjudy.top

[U111] JS：对象转 Map
来源：http://dbh.yuxming.cn

new Map(Object.entries(obj))
来源：http://oqs.xingfuxueyuan.xyz

[U112] JS：字符串补位
来源：http://emx.zhijiandao.cn

"7".padStart(3, "0")
来源：http://moo.cdnleiting.top

[U113] JS：正则替换全部
来源：http://veq.daria6918.cn

s.replaceAll("a", "b")
来源：http://tok.sysykeji.top

[U114] JS：JSON 深比较
来源：http://tqg.quarkkingdee.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://eib.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://aol.sjlbkw.cn

crypto.randomUUID()
来源：http://pdi.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://wkk.chenjidiqi.icu

/** @param {string} name */ function f(name) {}
来源：http://ehf.nwbrower.top

[U117] JS：单元测试
来源：http://bth.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://qhr.jinqigfzy.top

[U118] JS：开发服务器
来源：http://ydi.svipenyu.cn

npm i -D vite;  npx vite
来源：http://ldf.zhoulong.xyz

[U119] JS：生产构建
来源：http://glr.jinghuilouyu.cn

npx vite build
来源：http://jeo.ctjpmb.com

[U120] JS：读取环境变量（Vite）
来源：http://wre.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://aih.gaohongyu789.top

================================================================================
来源：http://kge.zhoulong.xyz

统计汇总
来源：http://egr.zdqjudy.top

================================================================================
来源：http://bei.jyoumei.cn

按语言统计（条）：
来源：http://qcz.yanxiufei.cn

Python ......... 252
来源：http://pad.havefunace.top

PHP ............ 252
来源：http://kpe.nanxuanxn.top

JavaScript ..... 252
来源：http://vzp.kuanghao11.cn

TypeScript ..... 212
来源：http://rzl.tarul.cn

Java ........... 212
来源：http://vic.xylfe.cn

Go ............. 212
来源：http://ciy.daria6918.cn

Ruby ........... 212
来源：http://gyn.shanyushiyangkeji.top

C# ............. 212
来源：http://bpx.hfpthk.cn

C .............. 30
来源：http://uxs.mhx1999.top

C++ ............ 30
来源：http://vhs.cqqwz.cn

SQL ............ 90
来源：http://why.cheryme.top

Bash ........... 80
来源：http://epi.ydjk.org.cn

Kotlin ......... 15
来源：http://aio.hywenlv.cn

Swift .......... 15
来源：http://shc.andypj.xyz

Lua ............ 10
来源：http://uei.c1oappe.top

Perl ........... 10
来源：http://fps.sjlbkw.cn

Scala .......... 10
来源：http://xxj.fehbvm.com

------------------------------------
来源：http://ntm.yj20258888.top

合计 ........... 2106 条
来源：http://vio.tanke756.top

按章节统计：
来源：http://oqp.jinqigfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://exr.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tqi.jinghuilouyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ovf.jyoumei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bwf.haohaochexian.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sta.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://skk.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://brt.hfpthk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qrk.fehbvm.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kta.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bts.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kzu.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kjx.cqqwz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wcj.epnwcf.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://miu.meibo888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ldn.jinghuilouyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iez.zdbjq.cn

Q SQL 专题                              90
来源：http://wsd.xinyue.icu

R Bash 专题                             80
来源：http://qub.dashuyun.cn

S C / C++ 专题                          60
来源：http://mlx.zhaomingkeji.xyz

T 其他语言补充                          60
来源：http://qgu.ctjpmb.com

U 高频实用片段                         120
来源：http://tnd.cheryme.top

------------------------------------
来源：http://tvs.jiagoushi.top

合计                                  2106 条
来源：http://dlc.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://hbj.shzxlz.cn

使用提醒
来源：http://ofq.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://khx.zdqjudy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ipa.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://llh.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ahi.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://eri.haohaochexian.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://brb.jinqigufen.top

—— 文件结束 ——
来源：http://pln.yj202588.top

================================================================================
来源：http://ipg.shuidangran.top

程序语言常见例子速查手册（2024 版）
来源：http://wcx.zhengqikj.top

Common Programming Examples Cheat Book
来源：http://krn.daxiang520.top

================================================================================
来源：http://fpv.guannengcc.top

【收录内容】
来源：http://vxj.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://mmm.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kqe.daria6918.cn

SQL · Bash · C · C++
来源：http://yim.xylfe.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://evo.sjlbkw.cn

【使用说明】
来源：http://pbj.jinghuilouyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://trz.c1oappe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xjb.yonumen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rwz.ctjpmb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tev.havefunace.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wca.fktsv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lzy.hnxiangtu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fax.zhijiandao.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nlw.wangshuangyany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://krn.dianchejie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aqd.yvedp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pif.guannengcc.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lyy.tian-w.cn

【文件统计】
来源：http://wnw.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yxq.jianghu66.top

--------------------------------------------------------------------------------
来源：http://okk.hcnkem.com

目  录
来源：http://bhe.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://mgu.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fpe.sjlbkw.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://toh.xuanzx.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://boh.shanyushiyangtech.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sgg.fehbvm.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jka.cqqwz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zer.yj202588.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ink.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://knx.pycfn.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bxt.hcnkem.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://knu.daria6918.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yyn.jiagoushi.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rst.shzxlz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zcq.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lyv.mhx1999.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tmq.cashguo.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rmr.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wcm.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://dei.jinqigufen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://exl.cdnleiting.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ghp.hfpthk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://voc.daria6918.cn

================================================================================
来源：http://qld.yj20258.top

A. 基础语法与类型
来源：http://pwr.52xcode.cn

================================================================================
来源：http://ysd.dashuyun.cn

[A01] Hello World
来源：http://txv.shuidangran.top

Py:   print("Hello, World!")
来源：http://fuh.fehbvm.com

PHP:  echo "Hello, World!";
来源：http://itf.jqgfzy.top

JS:   console.log("Hello, World!");
来源：http://mzq.hfpthk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qel.yongpay.top

Java: System.out.println("Hello, World!");
来源：http://mox.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://aph.c1oappe.top

Ruby: puts "Hello, World!"
来源：http://xzb.nwbrower.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tcy.hesvh.cn

[A02] 变量声明与赋值
来源：http://pph.gogol.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ztf.hesvh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jdj.redwolf501.top

JS:   let name = "Alex"; const age = 20;
来源：http://wij.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pdz.ehwqpu.com

Java: String name = "Alex"; int age = 20;
来源：http://sym.fehbvm.com

Go:   name := "Alex"; age := 20
来源：http://wbz.sufxvd.cn

Ruby: name = "Alex"; age = 20
来源：http://jvk.fktsv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fks.cucudq.cn

[A03] 常量定义
来源：http://ibm.zhixingplan.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fsi.sufxvd.cn

PHP:  const PI = 3.14159;
来源：http://efz.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://gwt.shangyingyoupin.top

TS:   const PI: number = 3.14159;
来源：http://sem.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://cdo.hywenlv.cn

Go:   const PI = 3.14159
来源：http://yai.cqqwz.cn

Ruby: PI = 3.14159
来源：http://czt.tanke756.top

C#:   const double PI = 3.14159;
来源：http://uoa.xingfuxueyuan.xyz

[A04] 判断变量类型
来源：http://yti.fanxiaobao.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://rgc.9152youxi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xqx.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nae.meibo888.top

TS:   typeof x; x instanceof Date
来源：http://mju.gotoacloud.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wgp.yonumen.top

Go:   reflect.TypeOf(x).Name()
来源：http://ssk.svipenyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qkh.9152youxi.cn

C#:   x.GetType().Name; x is int
来源：http://ibi.chenlongwang.top

[A05] 整数除法与取模
来源：http://hdy.sweek.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qpw.gaohongyu789.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://znc.pycfn.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iav.chenzaomai.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zvq.zhixingplan.top

Java: 7 / 2; 7 % 2
来源：http://llh.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://ffx.meibo888.top

Ruby: 7 / 2; 7 % 2
来源：http://hgj.sweek.top

C#:   7 / 2; 7 % 2
来源：http://ynh.cqqwz.cn

[A06] 字符串转数字
来源：http://bvh.pengpengdd.cyou

Py:   int("42"); float("3.14")
来源：http://jea.nanxinkj.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cwo.fehbvm.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nde.daria6918.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mox.nanxinkj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uly.52xcode.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bus.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tjz.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fmv.nanxinkj.top

[A07] 数字转字符串
来源：http://yfu.zhiwuduotai.top

Py:   str(42)
来源：http://oja.jinqigufen.top

PHP:  (string) 42; strval(42)
来源：http://ene.hywenlv.cn

JS:   String(42); (42).toString()
来源：http://ilr.jqgfzy.top

TS:   String(42)
来源：http://mrj.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pas.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://rrd.shzxlz.cn

Ruby: 42.to_s
来源：http://vcn.fengsongda.top

C#:   42.ToString()
来源：http://iha.yj20258888.top

[A08] 取整与四舍五入
来源：http://mpg.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://aqy.ehwqpu.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xoc.bjfxy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://agj.zycfv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://enf.zycfv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jgs.mhx1999.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://foj.dianchejie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nrs.sjlbkw.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ulz.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://ahg.cashguo.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fas.daxiang520.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pnk.ppjwa.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ewr.cdnleiting.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jvv.ivvv.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wdh.yongpay.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://chj.fzhhl.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bcz.jianghu66.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ceu.zhongyouzk.top

[A10] 生成随机数
来源：http://yck.haohaochexian.top

Py:   import random; random.randint(1, 100)
来源：http://bsw.ehwqpu.com

PHP:  random_int(1, 100);
来源：http://nuu.quarkkingdee.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ddu.316326.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ukf.shanyushiyangtech.top

Java: new Random().nextInt(100) + 1
来源：http://zlh.c1oappe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://amw.gogol.net.cn

Ruby: rand(1..100)
来源：http://umi.jqgfzy.top

C#:   new Random().Next(1, 101)
来源：http://lrt.fanxiaobao.xyz

[A11] 条件表达式（三元）
来源：http://hbk.yuanzhike.top

Py:   "yes" if x > 0 else "no"
来源：http://enw.tanke756.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://gvm.hammf.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uxx.meibo888.top

TS:   x > 0 ? "yes" : "no"
来源：http://xas.chenjidiqi.icu

Java: x > 0 ? "yes" : "no"
来源：http://xgd.haohaochexian.top

Go:   // 无三元运算符，需用 if 语句
来源：http://onj.52xcode.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zeh.tanke756.top

C#:   x > 0 ? "yes" : "no"
来源：http://coy.feifeiyinyue.top

[A12] 字符串插值 / 格式化
来源：http://bng.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tph.hcnkem.com


<!-- 参考信息 -->