代发 wailian999

[U77] PHP：模板渲染
来源：http://hyd.hfpthk.cn

composer require twig/twig
来源：http://gpy.zhixingplan.top

[U78] PHP：单元测试
来源：http://ayo.fehbvm.com

composer require --dev phpunit/phpunit
来源：http://msq.sweek.top

[U79] PHP：静态分析
来源：http://dbl.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://ppg.meibo888.top

[U80] PHP：代码规范修复
来源：http://sxo.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pvi.hammf.cn

[U81] JS：初始化项目
来源：http://jbw.yj20258.top

npm init -y;  npm i express
来源：http://bfk.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://dxs.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jrk.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://huk.fzhhl.top

export const a = 1;  import { a } from "./m.js";
来源：http://vjp.yj20258.top

[U84] JS：CommonJS 写法
来源：http://lag.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://uel.jinyuanbaomall.cn

[U85] JS：可选链
来源：http://blh.sysykeji.top

a?.b?.c
来源：http://rih.zhiwuduotai.top

[U86] JS：空值合并
来源：http://kbm.yangfankeji.com

a ?? b
来源：http://exe.bjfxy.top

[U87] JS：解构默认值
来源：http://bad.nwbrower.top

const { a = 1, b = 2 } = obj;
来源：http://zoe.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://oyw.jiagoushi.top

{ ...a, ...b }
来源：http://ekn.meibo888.top

[U89] JS：数组去重
来源：http://gvf.chenzaomai.com

[...new Set(arr)]
来源：http://wix.yfazqb.com

[U90] JS：数字数组排序
来源：http://sws.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://she.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://wfm.smart0.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tgd.fengsongda.top

[U92] JS：深拷贝
来源：http://mxp.gotoacloud.top

structuredClone(obj)
来源：http://szj.jinqigfzy.top

[U93] JS：模板字符串
来源：http://rfc.yangfankeji.com

`共 ${n} 条`
来源：http://fbj.aizwys.cn

[U94] JS：箭头函数
来源：http://stt.snrcjt.cn

const double = x => x * 2;
来源：http://xec.hesvh.cn

[U95] JS：Promise 包装
来源：http://mmu.hnxiangtu.top

new Promise((resolve, reject) => {})
来源：http://xed.fzhhl.top

[U96] JS：async/await 与异常
来源：http://xmr.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mju.sufxvd.cn

[U97] JS：并发请求
来源：http://mkw.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://kof.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://eps.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fhv.iojbl.cn

[U99] JS：事件监听
来源：http://zgb.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://lug.ywan-chungtsiang.top

[U100] JS：DOM 查询
来源：http://cmh.zhaomingkeji.xyz

document.querySelector(".item")
来源：http://vly.sweek.top

[U101] JS：classList 操作
来源：http://icy.dashuyun.cn

el.classList.toggle("active")
来源：http://knp.chenzaomai.com

[U102] JS：本地存储
来源：http://eyx.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dob.tian-w.cn

[U103] JS：定时器
来源：http://css.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mnt.hywenlv.cn

[U104] JS：防抖
来源：http://xvq.gogol.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jpx.jyoumei.cn

[U105] JS：节流
来源：http://xzz.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nyk.vqdsnc.cn

[U106] JS：日期格式化
来源：http://wnz.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kdu.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://jlc.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ngu.fehbvm.com

[U108] JS：随机整数
来源：http://vsn.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kmc.ppjwa.cn

[U109] JS：数组分组
来源：http://zlw.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://dmq.yj20258.top

[U110] JS：数组分块
来源：http://ycv.shangyingyoupin.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://off.jqgfzy.top

[U111] JS：对象转 Map
来源：http://xhy.yongpay.top

new Map(Object.entries(obj))
来源：http://qbk.xziqi.cn

[U112] JS：字符串补位
来源：http://cdc.nanxinkj.top

"7".padStart(3, "0")
来源：http://lwi.daria6918.cn

[U113] JS：正则替换全部
来源：http://vgv.cqqwz.cn

s.replaceAll("a", "b")
来源：http://htw.andypj.xyz

[U114] JS：JSON 深比较
来源：http://wja.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://unh.gogol.net.cn

[U115] JS：生成 UUID
来源：http://zju.shangyingyoupin.top

crypto.randomUUID()
来源：http://wcc.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://hqf.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://shu.nanxinkj.top

[U117] JS：单元测试
来源：http://gvx.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://qhj.dashuyun.cn

[U118] JS：开发服务器
来源：http://btz.daria6918.cn

npm i -D vite;  npx vite
来源：http://pwt.jyoumei.cn

[U119] JS：生产构建
来源：http://qwy.uphjek.com

npx vite build
来源：http://hec.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://vjb.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://orb.daxiang520.top

================================================================================
来源：http://qkv.ywan-chungtsiang.top

统计汇总
来源：http://mip.jqgufenzy.top

================================================================================
来源：http://dbd.ehwqpu.com

按语言统计（条）：
来源：http://uby.xingfuxueyuan.xyz

Python ......... 252
来源：http://wnr.zhaomingkeji.xyz

PHP ............ 252
来源：http://yrq.svipenyu.cn

JavaScript ..... 252
来源：http://fvz.quarkkingdee.top

TypeScript ..... 212
来源：http://diq.fktsv.cn

Java ........... 212
来源：http://oqa.iojbl.cn

Go ............. 212
来源：http://aio.ivvv.top

Ruby ........... 212
来源：http://pbg.shanyushiyangkeji.top

C# ............. 212
来源：http://vwa.yongpay.top

C .............. 30
来源：http://eki.bbcook.cn

C++ ............ 30
来源：http://ops.fzhhl.top

SQL ............ 90
来源：http://umu.yvedp.cn

Bash ........... 80
来源：http://xgx.redwolf501.top

Kotlin ......... 15
来源：http://ruw.fktsv.cn

Swift .......... 15
来源：http://mwx.yuxming.cn

Lua ............ 10
来源：http://oaz.hcnkem.com

Perl ........... 10
来源：http://beo.0kj1m.cn

Scala .......... 10
来源：http://yom.meibo888.top

------------------------------------
来源：http://cvm.fehbvm.com

合计 ........... 2106 条
来源：http://opv.guannengcc.top

按章节统计：
来源：http://wiq.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qdh.fktsv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tkl.fanxiaobao.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vqn.sjlbkw.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wyx.yangfankeji.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hgj.bbcook.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wcx.yanxiufei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yfz.fktsv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zql.shanyushiyangtech.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qol.sysykeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eov.iojbl.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://avm.wangshuangyany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ymr.haohaochexian.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uzl.cashguo.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://alb.zdqjudy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gzj.chenlongwang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vzf.jiagoushi.top

Q SQL 专题                              90
来源：http://pee.xinyue.icu

R Bash 专题                             80
来源：http://xwj.ydzc1.top

S C / C++ 专题                          60
来源：http://nav.yvedp.cn

T 其他语言补充                          60
来源：http://xbn.zhiwuduotai.top

U 高频实用片段                         120
来源：http://fit.guannengcc.top

------------------------------------
来源：http://yrg.pycfn.com

合计                                  2106 条
来源：http://cwn.mhx1999.top

--------------------------------------------------------------------------------
来源：http://uhr.zhaomingkeji.xyz

使用提醒
来源：http://ytm.fehbvm.com

--------------------------------------------------------------------------------
来源：http://pmm.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iyk.hongshengwenyu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cjt.ivvv.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ing.52xcode.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rap.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jsj.yuanzhike.top

—— 文件结束 ——
来源：http://ezy.xingfuxueyuan.xyz

================================================================================
来源：http://meu.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://plm.yj202588.top

Common Programming Examples Cheat Book
来源：http://aqw.c1oappe.top

================================================================================
来源：http://bdh.iojbl.cn

【收录内容】
来源：http://igx.zdqjudy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lsk.hnxiangtu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://edm.jyoumei.cn

SQL · Bash · C · C++
来源：http://zud.52xcode.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dhm.chenzaomai.com

【使用说明】
来源：http://ciy.hywenlv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rxk.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dmg.haohaochexian.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kur.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://whe.wangdashe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://eqo.yuanzhike.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://agp.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://orp.hfpthk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rfe.chenzaomai.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hxv.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://idp.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bdw.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rqz.cqqwz.cn

【文件统计】
来源：http://gtt.cdnleiting.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://duo.bbcook.cn

--------------------------------------------------------------------------------
来源：http://ert.tarul.cn

目  录
来源：http://mhu.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://poj.vehdjk.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mvm.xylfe.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vbw.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yrn.daria6918.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iah.jlsjyb.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ldb.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wij.wangdashe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dvu.tian-w.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gbm.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rmn.yvedp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gyp.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://exo.mhx1999.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rwm.fanxiaobao.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://isq.316326.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ozm.hnqzz.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xug.ctjpmb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zps.tian-w.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://izd.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dqa.hnqzz.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mcv.ivvv.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tux.sjlbkw.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cxs.yfazqb.com

================================================================================
来源：http://hqf.hnxiangtu.top

A. 基础语法与类型
来源：http://zma.daria6918.cn

================================================================================
来源：http://ine.yangfankeji.com

[A01] Hello World
来源：http://sny.tarul.cn

Py:   print("Hello, World!")
来源：http://rlx.shanyushiyangkeji.top

PHP:  echo "Hello, World!";
来源：http://gvm.gogol.net.cn

JS:   console.log("Hello, World!");
来源：http://mee.jinqigufen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pck.ctjpmb.com

Java: System.out.println("Hello, World!");
来源：http://mbm.meibo888.top

Go:   fmt.Println("Hello, World!")
来源：http://psl.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://ead.jyoumei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ogp.chenzaomai.com

[A02] 变量声明与赋值
来源：http://rfq.smart0.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qxc.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://ndp.mhx1999.top

JS:   let name = "Alex"; const age = 20;
来源：http://nom.jinghuilouyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mcs.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://vgt.jyoumei.cn

Go:   name := "Alex"; age := 20
来源：http://yuq.fktsv.cn

Ruby: name = "Alex"; age = 20
来源：http://bqq.fanxiaobao.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://gbx.zycfv.cn

[A03] 常量定义
来源：http://hfp.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ptw.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://dqz.hnxiangtu.top

JS:   const PI = 3.14159;
来源：http://wxi.yvedp.cn

TS:   const PI: number = 3.14159;
来源：http://eod.tanke756.top

Java: static final double PI = 3.14159;
来源：http://uzv.shuidangran.top

Go:   const PI = 3.14159
来源：http://mfn.smart0.xyz

Ruby: PI = 3.14159
来源：http://vrc.xziqi.cn

C#:   const double PI = 3.14159;
来源：http://dtk.bbcook.cn

[A04] 判断变量类型
来源：http://tee.zhiwuduotai.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rqw.jianghu66.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zjk.shzxlz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dcm.feifeiyinyue.top

TS:   typeof x; x instanceof Date
来源：http://hwx.jyoumei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oqt.xziqi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://syy.daria6918.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dby.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://asu.zdbjq.cn

[A05] 整数除法与取模
来源：http://pft.chenlongwang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lvp.shangyingyoupin.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ukf.yj20258888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jpx.cheryme.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wik.hnxiangtu.top

Java: 7 / 2; 7 % 2
来源：http://kyr.316326.xyz

Go:   7 / 2; 7 % 2
来源：http://gzi.dashuyun.cn

Ruby: 7 / 2; 7 % 2
来源：http://fec.dashuyun.cn

C#:   7 / 2; 7 % 2
来源：http://rsq.smart0.xyz

[A06] 字符串转数字
来源：http://xlt.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://zpk.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://myj.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ugf.yonumen.top

TS:   parseInt("42", 10); Number("42")
来源：http://igl.zhiwuduotai.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pqn.tarul.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vbm.yuanzhike.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gqg.sufxvd.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ngq.pengpengdd.cyou

[A07] 数字转字符串
来源：http://tco.yanxiufei.cn

Py:   str(42)
来源：http://gcz.fzhhl.top

PHP:  (string) 42; strval(42)
来源：http://khh.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://rng.ctjpmb.com

TS:   String(42)
来源：http://epn.tarul.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bgs.c1oappe.top

Go:   strconv.Itoa(42)
来源：http://bgs.bjfxy.top

Ruby: 42.to_s
来源：http://cez.tianlin.xyz

C#:   42.ToString()
来源：http://owe.cucudq.cn

[A08] 取整与四舍五入
来源：http://yjz.zhijiandao.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xvz.jinyuanbaomall.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://imb.sjlbkw.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rjd.fengsongda.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yyz.iojbl.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dhp.cqqwz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yqy.xziqi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sjn.fehbvm.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cbk.cqqwz.cn

[A09] 绝对值与最大最小值
来源：http://bzw.yuanzhike.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cbu.yuxming.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ohs.hnqzz.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wxy.xziqi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://syz.havefunace.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bkj.zhaomingkeji.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iww.tarul.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zfr.zdbjq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://feu.gogol.net.cn

[A10] 生成随机数
来源：http://ihp.cheryme.top

Py:   import random; random.randint(1, 100)
来源：http://xrr.guannengcc.top

PHP:  random_int(1, 100);
来源：http://clo.zhongyouzk.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mst.guannengcc.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ksc.guannengcc.top

Java: new Random().nextInt(100) + 1
来源：http://ttt.shuidangran.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dtp.yonumen.top

Ruby: rand(1..100)
来源：http://njq.jinqigfzy.top

C#:   new Random().Next(1, 101)
来源：http://gdt.shzxlz.cn

[A11] 条件表达式（三元）
来源：http://sod.daxiang520.top

Py:   "yes" if x > 0 else "no"
来源：http://las.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://wgm.ivvv.top

JS:   x > 0 ? "yes" : "no"
来源：http://fwk.dianchejie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mms.yonumen.top

Java: x > 0 ? "yes" : "no"
来源：http://gob.smart0.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://hie.hongshengwenyu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://raw.svipenyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://oja.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://atn.cashguo.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lht.316326.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kty.316326.xyz

JS:   `Hello, ${name}!`
来源：http://emb.dianchejie.cn

TS:   `Hello, ${name}!`
来源：http://beb.zhaomingkeji.xyz

Java: "Hello, %s!".formatted(name)
来源：http://wvo.ywan-chungtsiang.top


<!-- 参考信息 -->