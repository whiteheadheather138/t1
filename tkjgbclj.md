代发 wailian999

[U77] PHP：模板渲染
来源：http://ajs.cdnleiting.top

composer require twig/twig
来源：http://jyd.gzhubu.top

[U78] PHP：单元测试
来源：http://etr.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://gje.fktsv.cn

[U79] PHP：静态分析
来源：http://mzh.wangshuangyany.cn

composer require --dev phpstan/phpstan
来源：http://jhc.bbcook.cn

[U80] PHP：代码规范修复
来源：http://ywb.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yjw.hcnkem.com

[U81] JS：初始化项目
来源：http://utd.havefunace.top

npm init -y;  npm i express
来源：http://bpk.andypj.xyz

[U82] JS：package.json 脚本
来源：http://als.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kcp.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://rqa.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://epw.c1oappe.top

[U84] JS：CommonJS 写法
来源：http://hym.andypj.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://mhi.sufxvd.cn

[U85] JS：可选链
来源：http://yrb.shuidangran.top

a?.b?.c
来源：http://jzx.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://tgp.yfazqb.com

a ?? b
来源：http://zbu.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://kyz.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://sgd.tian-w.cn

[U88] JS：对象展开合并
来源：http://xfd.wangshuangyany.cn

{ ...a, ...b }
来源：http://nzr.vqdsnc.cn

[U89] JS：数组去重
来源：http://iry.yonumen.top

[...new Set(arr)]
来源：http://sne.yuanzhike.top

[U90] JS：数字数组排序
来源：http://kqn.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://cyz.sysykeji.top

[U91] JS：对象键值遍历
来源：http://wkl.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hcx.nanxuanxn.top

[U92] JS：深拷贝
来源：http://nyl.xylfe.cn

structuredClone(obj)
来源：http://twl.sufxvd.cn

[U93] JS：模板字符串
来源：http://vam.gaohongyu789.top

`共 ${n} 条`
来源：http://sty.kuanghao11.cn

[U94] JS：箭头函数
来源：http://ltp.tian-w.cn

const double = x => x * 2;
来源：http://pzt.xinyue.icu

[U95] JS：Promise 包装
来源：http://zsk.wangdashe.top

new Promise((resolve, reject) => {})
来源：http://qzz.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://ebl.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://grh.aibaodan.cn

[U97] JS：并发请求
来源：http://bgh.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xjm.wangshuangyany.cn

[U98] JS：fetch 带 JSON
来源：http://kvm.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dib.cqqwz.cn

[U99] JS：事件监听
来源：http://hdy.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://qfr.yueranfly.top

[U100] JS：DOM 查询
来源：http://aiz.pengpengdd.cyou

document.querySelector(".item")
来源：http://whd.sysykeji.top

[U101] JS：classList 操作
来源：http://bdl.yueranfly.top

el.classList.toggle("active")
来源：http://jqg.cqqwz.cn

[U102] JS：本地存储
来源：http://ppt.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ojt.shangyingyoupin.top

[U103] JS：定时器
来源：http://qbp.uphjek.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://plq.chenlongwang.top

[U104] JS：防抖
来源：http://hka.gzhubu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bew.xuetiantiany.cn

[U105] JS：节流
来源：http://wwu.zhijiandao.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ioh.yvedp.cn

[U106] JS：日期格式化
来源：http://ber.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rqw.gogol.net.cn

[U107] JS：数字千分位
来源：http://ksm.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kzz.xylfe.cn

[U108] JS：随机整数
来源：http://jos.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hxe.meibo888.top

[U109] JS：数组分组
来源：http://ggp.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://gxf.vehdjk.com

[U110] JS：数组分块
来源：http://myi.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vtn.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://vyq.yuanzhike.top

new Map(Object.entries(obj))
来源：http://fyf.haohaochexian.top

[U112] JS：字符串补位
来源：http://wsh.meibo888.top

"7".padStart(3, "0")
来源：http://nso.jiagoushi.top

[U113] JS：正则替换全部
来源：http://qgl.yj202588.top

s.replaceAll("a", "b")
来源：http://geg.xziqi.cn

[U114] JS：JSON 深比较
来源：http://hoz.epnwcf.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://tdk.jinqigufen.top

[U115] JS：生成 UUID
来源：http://tuk.nwbrower.top

crypto.randomUUID()
来源：http://uec.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://urg.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://tts.sweek.top

[U117] JS：单元测试
来源：http://xbj.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://ooy.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://zxa.birdmap.top

npm i -D vite;  npx vite
来源：http://sxd.yangfankeji.com

[U119] JS：生产构建
来源：http://ftx.guowangkeji.top

npx vite build
来源：http://lsm.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://waj.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://tzf.zhaomingkeji.xyz

================================================================================
来源：http://wdv.yj202588.top

统计汇总
来源：http://ysl.zhaomingkeji.xyz

================================================================================
来源：http://zqg.guannengcc.top

按语言统计（条）：
来源：http://rsh.tanke756.top

Python ......... 252
来源：http://yzs.hywenlv.cn

PHP ............ 252
来源：http://rtl.cheryme.top

JavaScript ..... 252
来源：http://mre.hysaishi.cn

TypeScript ..... 212
来源：http://hka.feifeiyinyue.top

Java ........... 212
来源：http://qyh.jianghu66.top

Go ............. 212
来源：http://fvt.wangshuangyany.cn

Ruby ........... 212
来源：http://qcg.hnxiangtu.top

C# ............. 212
来源：http://xct.smart0.xyz

C .............. 30
来源：http://rzf.dianchejie.cn

C++ ............ 30
来源：http://mqk.jinqigfzy.top

SQL ............ 90
来源：http://efx.guannengcc.top

Bash ........... 80
来源：http://abj.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://mbo.xylfe.cn

Swift .......... 15
来源：http://xiy.vqdsnc.cn

Lua ............ 10
来源：http://xbw.daria6918.cn

Perl ........... 10
来源：http://ihe.zhongyouzk.top

Scala .......... 10
来源：http://uef.jqgufenzy.top

------------------------------------
来源：http://vqm.316326.xyz

合计 ........... 2106 条
来源：http://upm.pycfn.com

按章节统计：
来源：http://hdx.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nwy.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xvz.hammf.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tep.shanyushiyangtech.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sko.fzhhl.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ajb.9152youxi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rfl.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tqo.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gjj.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gil.zhijiandao.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ezx.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://erf.cheryme.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://spf.zdqjudy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qfh.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fql.uphjek.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ojj.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qsw.ybcxt.top

Q SQL 专题                              90
来源：http://mtk.chenzaomai.com

R Bash 专题                             80
来源：http://bzp.sjlbkw.cn

S C / C++ 专题                          60
来源：http://sse.fzhhl.top

T 其他语言补充                          60
来源：http://kap.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://coe.xylfe.cn

------------------------------------
来源：http://mzq.aizwys.cn

合计                                  2106 条
来源：http://bvf.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://aov.hfpthk.cn

使用提醒
来源：http://omm.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://ktl.fzhhl.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qny.cucudq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fim.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://snl.jiagoushi.top

在旧版本上使用前请先确认语法支持情况。
来源：http://odp.shanyushiyangtech.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zde.aizwys.cn

—— 文件结束 ——
来源：http://pzh.aibaodan.cn

================================================================================
来源：http://vzp.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://sgm.sufxvd.cn

Common Programming Examples Cheat Book
来源：http://dsy.cdnleiting.top

================================================================================
来源：http://tsv.xuanzx.com

【收录内容】
来源：http://cve.feifeiyinyue.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zfx.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kzx.tian-w.cn

SQL · Bash · C · C++
来源：http://dxj.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qxj.sjlbkw.cn

【使用说明】
来源：http://ijz.redwolf501.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baa.shzxlz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kew.ppjwa.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rdc.jinghuilouyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://izm.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://yyj.hysaishi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://egz.gogol.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wpr.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ifu.havefunace.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xob.dianchejie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nfo.meibo888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://odc.yuanzhike.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vjw.ywan-chungtsiang.top

【文件统计】
来源：http://gwi.hysaishi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vxo.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://dyk.guannengcc.top

目  录
来源：http://gmg.fzhhl.top

--------------------------------------------------------------------------------
来源：http://two.52xcode.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tgi.svipenyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rvk.cqqwz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sit.pengpengdd.cyou

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cml.hammf.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pqk.uphjek.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gus.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hub.andypj.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ral.xinyue.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://opo.yangfankeji.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sdg.pengpengdd.cyou

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gsy.hongshengwenyu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://avt.hammf.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sfd.zdbjq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ddt.vqdsnc.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ggb.gotoacloud.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nsj.daria6918.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mdw.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://ada.redwolf501.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gta.zdqjudy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mkm.hywenlv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://waq.svipenyu.cn

================================================================================
来源：http://lcr.chenzaomai.com

A. 基础语法与类型
来源：http://cth.zhijiandao.cn

================================================================================
来源：http://skr.zdbjq.cn

[A01] Hello World
来源：http://ktv.zhoulong.xyz

Py:   print("Hello, World!")
来源：http://kpq.redwolf501.top

PHP:  echo "Hello, World!";
来源：http://lof.dianchejie.cn

JS:   console.log("Hello, World!");
来源：http://ojx.hfpthk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wwp.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://zzc.pycfn.com

Go:   fmt.Println("Hello, World!")
来源：http://lma.nanxinkj.top

Ruby: puts "Hello, World!"
来源：http://wps.fengsongda.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kzv.yonumen.top

[A02] 变量声明与赋值
来源：http://iuu.zdqjudy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yve.daria6918.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yxf.yanxiufei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mfj.fzhhl.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://whf.cashguo.top

Java: String name = "Alex"; int age = 20;
来源：http://ewk.cdnleiting.top

Go:   name := "Alex"; age := 20
来源：http://ett.hywenlv.cn

Ruby: name = "Alex"; age = 20
来源：http://vus.shanyushiyangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://tic.ehwqpu.com

[A03] 常量定义
来源：http://tie.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wqq.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://qco.shuidangran.top

JS:   const PI = 3.14159;
来源：http://ezp.zdbjq.cn

TS:   const PI: number = 3.14159;
来源：http://hrh.xuetiantiany.cn

Java: static final double PI = 3.14159;
来源：http://nub.hnxiangtu.top

Go:   const PI = 3.14159
来源：http://jqc.cucudq.cn

Ruby: PI = 3.14159
来源：http://dti.cucudq.cn

C#:   const double PI = 3.14159;
来源：http://obc.tianlin.xyz

[A04] 判断变量类型
来源：http://oon.fengsongda.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jwm.jyoumei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://guz.xuetiantiany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lji.cucudq.cn

TS:   typeof x; x instanceof Date
来源：http://gfo.sjlbkw.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ouj.shangyingyoupin.top

Go:   reflect.TypeOf(x).Name()
来源：http://imd.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sbe.kuanghao11.cn

C#:   x.GetType().Name; x is int
来源：http://ytr.xuanzx.com

[A05] 整数除法与取模
来源：http://lbc.ywan-chungtsiang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wck.chenlongwang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tco.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kvh.hcnkem.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gug.ivvv.top

Java: 7 / 2; 7 % 2
来源：http://rzq.fanxiaobao.xyz

Go:   7 / 2; 7 % 2
来源：http://lzb.epnwcf.com

Ruby: 7 / 2; 7 % 2
来源：http://bbg.zhengqikj.top

C#:   7 / 2; 7 % 2
来源：http://ggo.uphjek.com

[A06] 字符串转数字
来源：http://bjv.epnwcf.com

Py:   int("42"); float("3.14")
来源：http://jbj.meibo888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ana.ctjpmb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qbv.iojbl.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nus.havefunace.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jaw.xuanzx.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cjj.mhx1999.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dkx.52xcode.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yin.havefunace.top

[A07] 数字转字符串
来源：http://xyf.shzxlz.cn

Py:   str(42)
来源：http://elx.shzxlz.cn

PHP:  (string) 42; strval(42)
来源：http://qrh.fktsv.cn

JS:   String(42); (42).toString()
来源：http://oap.yueranfly.top

TS:   String(42)
来源：http://kkp.yvedp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://swu.zhongyouzk.top

Go:   strconv.Itoa(42)
来源：http://gjt.jyoumei.cn

Ruby: 42.to_s
来源：http://snn.cucudq.cn

C#:   42.ToString()
来源：http://rzq.guannengcc.top

[A08] 取整与四舍五入
来源：http://oay.redwolf501.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nfq.zycfv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vvj.xingfuxueyuan.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ler.jlsjyb.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lcj.hywenlv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qqr.dashuyun.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kjb.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ots.guannengcc.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ugd.yj20258888.top

[A09] 绝对值与最大最小值
来源：http://mto.meibo888.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qfk.dianchejie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ipx.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://noz.aibaodan.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zfl.daxiang520.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dla.zhengqikj.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fjb.zdbjq.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ket.fengsongda.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kxn.wangshuangyany.cn

[A10] 生成随机数
来源：http://wwr.hfpthk.cn

Py:   import random; random.randint(1, 100)
来源：http://kgh.epnwcf.com

PHP:  random_int(1, 100);
来源：http://pkk.sjlbkw.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://leb.sysykeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uun.zhongyouzk.top

Java: new Random().nextInt(100) + 1
来源：http://ivk.nwbrower.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qgj.hfpthk.cn

Ruby: rand(1..100)
来源：http://emd.shzxlz.cn

C#:   new Random().Next(1, 101)
来源：http://flh.yj20258.top

[A11] 条件表达式（三元）
来源：http://nqv.316326.xyz

Py:   "yes" if x > 0 else "no"
来源：http://qpk.shanyushiyangtech.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://igb.ctjpmb.com

JS:   x > 0 ? "yes" : "no"
来源：http://qhi.jiagoushi.top

TS:   x > 0 ? "yes" : "no"
来源：http://bbb.cqqwz.cn

Java: x > 0 ? "yes" : "no"
来源：http://xge.chenlongwang.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tyb.xuetiantiany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://toq.dianchejie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qbx.shanyushiyangkeji.top

[A12] 字符串插值 / 格式化
来源：http://ttu.nanxinkj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tmz.ppjwa.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iqp.hywenlv.cn

JS:   `Hello, ${name}!`
来源：http://aof.ydzc1.top

TS:   `Hello, ${name}!`
来源：http://cpk.tian-w.cn

Java: "Hello, %s!".formatted(name)
来源：http://fkc.wangshuangyany.cn


<!-- 参考信息 -->