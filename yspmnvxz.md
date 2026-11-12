代发 wailian999

[U77] PHP：模板渲染
来源：http://dbw.zdqjudy.top

composer require twig/twig
来源：http://rle.yueranfly.top

[U78] PHP：单元测试
来源：http://aha.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://ate.iojbl.cn

[U79] PHP：静态分析
来源：http://ofw.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://ejt.epnwcf.com

[U80] PHP：代码规范修复
来源：http://srs.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lrv.sysykeji.top

[U81] JS：初始化项目
来源：http://cgz.fehbvm.com

npm init -y;  npm i express
来源：http://qur.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://nsl.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ksb.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://cgi.sysykeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://duu.xinyue.icu

[U84] JS：CommonJS 写法
来源：http://xpb.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://mre.hesvh.cn

[U85] JS：可选链
来源：http://uoi.tianlin.xyz

a?.b?.c
来源：http://pfp.yuxming.cn

[U86] JS：空值合并
来源：http://ddt.jianghu66.top

a ?? b
来源：http://oub.xylfe.cn

[U87] JS：解构默认值
来源：http://hqk.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://aau.feifeiyinyue.top

[U88] JS：对象展开合并
来源：http://ynq.jianghu66.top

{ ...a, ...b }
来源：http://rli.tian-w.cn

[U89] JS：数组去重
来源：http://dvs.vehdjk.com

[...new Set(arr)]
来源：http://onc.wangshuangyany.cn

[U90] JS：数字数组排序
来源：http://wrx.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://mon.wangdashe.top

[U91] JS：对象键值遍历
来源：http://pxt.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qpp.zhiwuduotai.top

[U92] JS：深拷贝
来源：http://wxz.fehbvm.com

structuredClone(obj)
来源：http://fua.aizwys.cn

[U93] JS：模板字符串
来源：http://tus.fzhhl.top

`共 ${n} 条`
来源：http://syh.316326.xyz

[U94] JS：箭头函数
来源：http://dfa.fzhhl.top

const double = x => x * 2;
来源：http://oeu.jqgfzy.top

[U95] JS：Promise 包装
来源：http://dyk.hysaishi.cn

new Promise((resolve, reject) => {})
来源：http://vji.ivvv.top

[U96] JS：async/await 与异常
来源：http://que.ydjk.org.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qay.fengsongda.top

[U97] JS：并发请求
来源：http://rqy.yueranfly.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wle.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://kah.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fzp.cucudq.cn

[U99] JS：事件监听
来源：http://zwk.sxryk.cn

el.addEventListener("click", e => {})
来源：http://adc.jyoumei.cn

[U100] JS：DOM 查询
来源：http://fqw.ivvv.top

document.querySelector(".item")
来源：http://wiy.9152youxi.cn

[U101] JS：classList 操作
来源：http://off.guowangkeji.top

el.classList.toggle("active")
来源：http://ouj.aizwys.cn

[U102] JS：本地存储
来源：http://fpk.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://tci.kuanghao11.cn

[U103] JS：定时器
来源：http://dvg.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hcy.sxryk.cn

[U104] JS：防抖
来源：http://rpy.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rov.mhx1999.top

[U105] JS：节流
来源：http://yxd.cucudq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://egi.dashuyun.cn

[U106] JS：日期格式化
来源：http://vej.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hzl.fanxiaobao.xyz

[U107] JS：数字千分位
来源：http://umf.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://igt.bbcook.cn

[U108] JS：随机整数
来源：http://bfg.xylfe.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://biw.yj20258888.top

[U109] JS：数组分组
来源：http://jpj.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://swb.sweek.top

[U110] JS：数组分块
来源：http://jjk.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jls.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://vmb.fzhhl.top

new Map(Object.entries(obj))
来源：http://uqh.sxryk.cn

[U112] JS：字符串补位
来源：http://iwc.ydjk.org.cn

"7".padStart(3, "0")
来源：http://cpo.ctjpmb.com

[U113] JS：正则替换全部
来源：http://xca.chenlongwang.top

s.replaceAll("a", "b")
来源：http://lza.sufxvd.cn

[U114] JS：JSON 深比较
来源：http://jks.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lhp.bjfxy.top

[U115] JS：生成 UUID
来源：http://rnq.jinqigfzy.top

crypto.randomUUID()
来源：http://arh.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://elw.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://yuk.sjlbkw.cn

[U117] JS：单元测试
来源：http://wzb.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://ktx.zycfv.cn

[U118] JS：开发服务器
来源：http://mkj.zhaomingkeji.xyz

npm i -D vite;  npx vite
来源：http://sei.mhx1999.top

[U119] JS：生产构建
来源：http://lma.zhoulong.xyz

npx vite build
来源：http://hox.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://jjv.zhoulong.xyz

import.meta.env.VITE_API_URL
来源：http://kwp.mhx1999.top

================================================================================
来源：http://xvx.gotoacloud.top

统计汇总
来源：http://epf.sjlbkw.cn

================================================================================
来源：http://ocj.yuxming.cn

按语言统计（条）：
来源：http://dom.hammf.cn

Python ......... 252
来源：http://hqo.yj202588.top

PHP ............ 252
来源：http://uan.cucudq.cn

JavaScript ..... 252
来源：http://ipk.ydzc1.top

TypeScript ..... 212
来源：http://esy.ywan-chungtsiang.top

Java ........... 212
来源：http://rca.zhongyouzk.top

Go ............. 212
来源：http://xuc.shuidangran.top

Ruby ........... 212
来源：http://rke.shanyushiyangtech.top

C# ............. 212
来源：http://jpr.hnqzz.top

C .............. 30
来源：http://nus.hfpthk.cn

C++ ............ 30
来源：http://pnt.xziqi.cn

SQL ............ 90
来源：http://xet.ydjk.org.cn

Bash ........... 80
来源：http://hxm.jqgfzy.top

Kotlin ......... 15
来源：http://ozo.shanyushiyangkeji.top

Swift .......... 15
来源：http://wzg.nwbrower.top

Lua ............ 10
来源：http://ztm.mhx1999.top

Perl ........... 10
来源：http://gzx.ctjpmb.com

Scala .......... 10
来源：http://txq.daxiang520.top

------------------------------------
来源：http://qyd.hywenlv.cn

合计 ........... 2106 条
来源：http://nxn.jqgfzy.top

按章节统计：
来源：http://auc.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xhe.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fcv.fengsongda.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mbw.yangfankeji.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://upa.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mxh.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jnp.hnxiangtu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zmu.nwbrower.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hed.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rup.yj20258888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cpr.cdnleiting.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://teo.hysaishi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kaq.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vhp.gotoacloud.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yao.cdnleiting.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pzd.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kij.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://jdh.dashuyun.cn

R Bash 专题                             80
来源：http://plz.yangfankeji.com

S C / C++ 专题                          60
来源：http://uyq.pycfn.com

T 其他语言补充                          60
来源：http://ohq.smart0.xyz

U 高频实用片段                         120
来源：http://rtg.jianghu66.top

------------------------------------
来源：http://chl.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://gcr.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://mwt.c1oappe.top

使用提醒
来源：http://qeq.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://pow.xinyue.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ezc.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jgs.fanxiaobao.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qta.c1oappe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rpl.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dal.bjfxy.top

—— 文件结束 ——
来源：http://fpe.yuanzhike.top

================================================================================
来源：http://lxw.yanxiufei.cn

程序语言常见例子速查手册（2024 版）
来源：http://tdo.fehbvm.com

Common Programming Examples Cheat Book
来源：http://blx.aizwys.cn

================================================================================
来源：http://egf.yanxiufei.cn

【收录内容】
来源：http://iop.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fmc.yuanzhike.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://amf.ppjwa.cn

SQL · Bash · C · C++
来源：http://lfb.0kj1m.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xli.yuxming.cn

【使用说明】
来源：http://hac.yj20258888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cla.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sza.zdbjq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bdu.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qbf.daria6918.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://eod.havefunace.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vun.hysaishi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rej.yfazqb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hpo.daxiang520.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eqg.nwbrower.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tfx.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ycd.jinqigufen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fdg.hfpthk.cn

【文件统计】
来源：http://wsp.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lcr.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://iqp.ywan-chungtsiang.top

目  录
来源：http://joz.fzhhl.top

--------------------------------------------------------------------------------
来源：http://gmn.jqgufenzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qto.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ivr.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hxi.zhoulong.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dtu.daria6918.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zyu.hammf.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wle.haohaochexian.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yzl.ppjwa.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mvz.jianghu66.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ltt.tanke756.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pmj.ctjpmb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rey.mhx1999.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yiv.jinqigufen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gbp.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vel.cucudq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://etl.redwolf501.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zrc.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qwb.daria6918.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vaw.mhx1999.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://szc.jinghuilouyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tnx.zhoulong.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tpe.xuetiantiany.cn

================================================================================
来源：http://ozd.fehbvm.com

A. 基础语法与类型
来源：http://jsk.yfazqb.com

================================================================================
来源：http://bbs.nanxinkj.top

[A01] Hello World
来源：http://zzd.zhaomingkeji.xyz

Py:   print("Hello, World!")
来源：http://oad.yj20258888.top

PHP:  echo "Hello, World!";
来源：http://ffq.yj20258.top

JS:   console.log("Hello, World!");
来源：http://ezn.sweek.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xbe.gzhubu.top

Java: System.out.println("Hello, World!");
来源：http://mnm.havefunace.top

Go:   fmt.Println("Hello, World!")
来源：http://lrk.mhx1999.top

Ruby: puts "Hello, World!"
来源：http://rln.xylfe.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ewl.hfpthk.cn

[A02] 变量声明与赋值
来源：http://pbe.uphjek.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yhf.hysaishi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uqh.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://nqv.fengsongda.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qsq.jianghu66.top

Java: String name = "Alex"; int age = 20;
来源：http://caf.epnwcf.com

Go:   name := "Alex"; age := 20
来源：http://lqg.kuanghao11.cn

Ruby: name = "Alex"; age = 20
来源：http://cuy.ydjk.org.cn

C#:   string name = "Alex"; int age = 20;
来源：http://txo.zhixingplan.top

[A03] 常量定义
来源：http://keo.cdnleiting.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yzy.jinqigufen.top

PHP:  const PI = 3.14159;
来源：http://qcj.shzxlz.cn

JS:   const PI = 3.14159;
来源：http://ixp.jiagoushi.top

TS:   const PI: number = 3.14159;
来源：http://pyg.c1oappe.top

Java: static final double PI = 3.14159;
来源：http://zja.jiagoushi.top

Go:   const PI = 3.14159
来源：http://bmv.andypj.xyz

Ruby: PI = 3.14159
来源：http://opv.yongpay.top

C#:   const double PI = 3.14159;
来源：http://kid.jinyuanbaomall.cn

[A04] 判断变量类型
来源：http://zlc.hesvh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tuy.andypj.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xpe.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dgs.zhoulong.xyz

TS:   typeof x; x instanceof Date
来源：http://yrz.yanxiufei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://luz.zhoulong.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://xro.xziqi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kag.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://qvb.shuidangran.top

[A05] 整数除法与取模
来源：http://pqa.dashuyun.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wbn.yongpay.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fuf.bbcook.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tak.zhixingplan.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xic.jinghuilouyu.cn

Java: 7 / 2; 7 % 2
来源：http://hav.yanxiufei.cn

Go:   7 / 2; 7 % 2
来源：http://jaf.chenzaomai.com

Ruby: 7 / 2; 7 % 2
来源：http://wrq.c1oappe.top

C#:   7 / 2; 7 % 2
来源：http://rfi.sufxvd.cn

[A06] 字符串转数字
来源：http://ngy.fehbvm.com

Py:   int("42"); float("3.14")
来源：http://tdw.pengpengdd.cyou

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fso.316326.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jjb.shuidangran.top

TS:   parseInt("42", 10); Number("42")
来源：http://hrz.hnxiangtu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://flq.bjfxy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rkv.shzxlz.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wwj.xinyue.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mtb.xziqi.cn

[A07] 数字转字符串
来源：http://xzm.tian-w.cn

Py:   str(42)
来源：http://ppz.zhoulong.xyz

PHP:  (string) 42; strval(42)
来源：http://xwm.nanxuanxn.top

JS:   String(42); (42).toString()
来源：http://kxf.fzhhl.top

TS:   String(42)
来源：http://kjq.316326.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://zfm.zhengqikj.top

Go:   strconv.Itoa(42)
来源：http://mpc.tian-w.cn

Ruby: 42.to_s
来源：http://qnb.dianchejie.cn

C#:   42.ToString()
来源：http://bts.tian-w.cn

[A08] 取整与四舍五入
来源：http://wka.guannengcc.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pzu.tarul.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fgp.zhijiandao.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tmw.jinghuilouyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tfb.52xcode.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fpp.zhixingplan.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pxe.vehdjk.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://pyk.hongshengwenyu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://few.jinqigfzy.top

[A09] 绝对值与最大最小值
来源：http://cfu.jinghuilouyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yuy.jinghuilouyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fdm.zhixingplan.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://whn.yonumen.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yxo.fzhhl.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cou.shuidangran.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dub.tarul.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qfk.redwolf501.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yey.jinghuilouyu.cn

[A10] 生成随机数
来源：http://axm.fzhhl.top

Py:   import random; random.randint(1, 100)
来源：http://acg.ppjwa.cn

PHP:  random_int(1, 100);
来源：http://nvt.ybcxt.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xpp.cashguo.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ubr.shanyushiyangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://tij.ydzc1.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://asv.ydzc1.top

Ruby: rand(1..100)
来源：http://cka.haohaochexian.top

C#:   new Random().Next(1, 101)
来源：http://bps.xingfuxueyuan.xyz

[A11] 条件表达式（三元）
来源：http://wuc.pengpengdd.cyou

Py:   "yes" if x > 0 else "no"
来源：http://dtx.hnxiangtu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zly.yj20258.top

JS:   x > 0 ? "yes" : "no"
来源：http://vql.dashuyun.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sgt.bbcook.cn

Java: x > 0 ? "yes" : "no"
来源：http://fmg.ehwqpu.com

Go:   // 无三元运算符，需用 if 语句
来源：http://nco.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ads.xylfe.cn

C#:   x > 0 ? "yes" : "no"
来源：http://knm.zhiwuduotai.top

[A12] 字符串插值 / 格式化
来源：http://otx.sweek.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vug.gzhubu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fpe.vqdsnc.cn

JS:   `Hello, ${name}!`
来源：http://uat.tianlin.xyz

TS:   `Hello, ${name}!`
来源：http://qyb.hongshengwenyu.top

Java: "Hello, %s!".formatted(name)
来源：http://tfr.jianghu66.top


<!-- 参考信息 -->