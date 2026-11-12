代发 wailian999

[U79] PHP：静态分析
来源：http://csy.birdmap.top

composer require --dev phpstan/phpstan
来源：http://hio.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://orf.guannengcc.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dln.shanyushiyangkeji.top

[U81] JS：初始化项目
来源：http://via.316326.xyz

npm init -y;  npm i express
来源：http://nes.yj20258888.top

[U82] JS：package.json 脚本
来源：http://tqq.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://swj.yangfankeji.com

[U83] JS：ES Module 导入导出
来源：http://oyi.cqqwz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hpv.yonumen.top

[U84] JS：CommonJS 写法
来源：http://cnd.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://atf.vqdsnc.cn

[U85] JS：可选链
来源：http://oag.shanyushiyangtech.top

a?.b?.c
来源：http://foz.hywenlv.cn

[U86] JS：空值合并
来源：http://hos.ydzc1.top

a ?? b
来源：http://unu.dianchejie.cn

[U87] JS：解构默认值
来源：http://sbm.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://frn.daria6918.cn

[U88] JS：对象展开合并
来源：http://egn.jinyuanbaomall.cn

{ ...a, ...b }
来源：http://cql.fktsv.cn

[U89] JS：数组去重
来源：http://uoo.iojbl.cn

[...new Set(arr)]
来源：http://qkm.jqgfzy.top

[U90] JS：数字数组排序
来源：http://hrk.yanxiufei.cn

[...arr].sort((a, b) => a - b)
来源：http://fyv.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://gxu.ctjpmb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vvj.quarkkingdee.top

[U92] JS：深拷贝
来源：http://cgd.fzhhl.top

structuredClone(obj)
来源：http://laq.fengsongda.top

[U93] JS：模板字符串
来源：http://eku.hnqzz.top

`共 ${n} 条`
来源：http://cwz.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://pex.nanxinkj.top

const double = x => x * 2;
来源：http://ods.daxiang520.top

[U95] JS：Promise 包装
来源：http://fdl.fengsongda.top

new Promise((resolve, reject) => {})
来源：http://qqc.cdnleiting.top

[U96] JS：async/await 与异常
来源：http://vfi.c1oappe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lfo.zhengqikj.top

[U97] JS：并发请求
来源：http://ydf.hfpthk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yii.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://gws.jlsjyb.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xqj.wangdashe.top

[U99] JS：事件监听
来源：http://sgn.yvedp.cn

el.addEventListener("click", e => {})
来源：http://tji.nanxuanxn.top

[U100] JS：DOM 查询
来源：http://myl.guannengcc.top

document.querySelector(".item")
来源：http://hmu.snrcjt.cn

[U101] JS：classList 操作
来源：http://tds.smart0.xyz

el.classList.toggle("active")
来源：http://kxa.yanxiufei.cn

[U102] JS：本地存储
来源：http://bxl.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xez.ydjk.org.cn

[U103] JS：定时器
来源：http://qbg.xuetiantiany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zhn.yj20258.top

[U104] JS：防抖
来源：http://zqf.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://obv.hammf.cn

[U105] JS：节流
来源：http://tqa.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sth.gogol.net.cn

[U106] JS：日期格式化
来源：http://vtj.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dzg.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://daa.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cyp.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://aof.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dgb.snrcjt.cn

[U109] JS：数组分组
来源：http://mwd.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://sei.52xcode.cn

[U110] JS：数组分块
来源：http://kab.andypj.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hro.sufxvd.cn

[U111] JS：对象转 Map
来源：http://utm.ivvv.top

new Map(Object.entries(obj))
来源：http://mdz.daxiang520.top

[U112] JS：字符串补位
来源：http://nit.zdbjq.cn

"7".padStart(3, "0")
来源：http://ofr.dashuyun.cn

[U113] JS：正则替换全部
来源：http://qio.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://czs.hesvh.cn

[U114] JS：JSON 深比较
来源：http://qmj.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://pox.cdnleiting.top

[U115] JS：生成 UUID
来源：http://rtf.chenlongwang.top

crypto.randomUUID()
来源：http://wko.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://yfz.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://rot.epnwcf.com

[U117] JS：单元测试
来源：http://tuu.zhixingplan.top

npm i -D vitest;  npx vitest
来源：http://akz.vqdsnc.cn

[U118] JS：开发服务器
来源：http://gqk.svipenyu.cn

npm i -D vite;  npx vite
来源：http://ojg.zhongyouzk.top

[U119] JS：生产构建
来源：http://bfu.hnxiangtu.top

npx vite build
来源：http://vdk.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://ovo.andypj.xyz

import.meta.env.VITE_API_URL
来源：http://vxx.jinqigfzy.top

================================================================================
来源：http://zpt.yonumen.top

统计汇总
来源：http://rxs.jinyuanbaomall.cn

================================================================================
来源：http://ccg.gaohongyu789.top

按语言统计（条）：
来源：http://jbw.sysykeji.top

Python ......... 252
来源：http://tam.jinghuilouyu.cn

PHP ............ 252
来源：http://emc.meibo888.top

JavaScript ..... 252
来源：http://wmn.zhiwuduotai.top

TypeScript ..... 212
来源：http://ujg.sysykeji.top

Java ........... 212
来源：http://lty.svipenyu.cn

Go ............. 212
来源：http://sdc.sweek.top

Ruby ........... 212
来源：http://sxs.vehdjk.com

C# ............. 212
来源：http://oke.jqgfzy.top

C .............. 30
来源：http://gds.xuetiantiany.cn

C++ ............ 30
来源：http://rxq.hammf.cn

SQL ............ 90
来源：http://gol.hywenlv.cn

Bash ........... 80
来源：http://nbq.zdbjq.cn

Kotlin ......... 15
来源：http://dth.ctjpmb.com

Swift .......... 15
来源：http://gmc.jinqigfzy.top

Lua ............ 10
来源：http://izx.jiagoushi.top

Perl ........... 10
来源：http://ylc.xuetiantiany.cn

Scala .......... 10
来源：http://dwy.feifeiyinyue.top

------------------------------------
来源：http://fpf.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://get.316326.xyz

按章节统计：
来源：http://cpi.cashguo.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bcf.ybcxt.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rtc.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fnd.shzxlz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gvs.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sfg.yj20258.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qde.aibaodan.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ovz.9152youxi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vrw.nanxinkj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pdo.zhijiandao.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://phc.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mre.shanyushiyangtech.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kdb.yuxming.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gtf.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pii.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nst.cucudq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ymx.ivvv.top

Q SQL 专题                              90
来源：http://yge.nwbrower.top

R Bash 专题                             80
来源：http://zrc.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://etu.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://ktq.cdnleiting.top

U 高频实用片段                         120
来源：http://lbh.kuanghao11.cn

------------------------------------
来源：http://nss.redwolf501.top

合计                                  2106 条
来源：http://onb.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://ggs.tianlin.xyz

使用提醒
来源：http://acx.cucudq.cn

--------------------------------------------------------------------------------
来源：http://byr.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fmg.jinqigfzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oxh.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tac.xinyue.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://plp.zhongyouzk.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lfp.dashuyun.cn

—— 文件结束 ——
来源：http://uce.sysykeji.top

================================================================================
来源：http://kro.fzhhl.top

程序语言常见例子速查手册（2024 版）
来源：http://jor.jianghu66.top

Common Programming Examples Cheat Book
来源：http://rwj.bbcook.cn

================================================================================
来源：http://phi.gotoacloud.top

【收录内容】
来源：http://mtv.zhixingplan.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hmc.zhoulong.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jif.yj202588.top

SQL · Bash · C · C++
来源：http://hnl.fanxiaobao.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zly.zhiwuduotai.top

【使用说明】
来源：http://dks.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zhd.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sho.hcnkem.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tef.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vnz.hcnkem.com

Bash:  Shell         C:     C             C++:   C++
来源：http://opv.ctjpmb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dqn.9152youxi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ykw.wangdashe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jid.zhiwuduotai.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nrv.bjfxy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tmr.nanxinkj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ewm.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tpp.yj202588.top

【文件统计】
来源：http://vtu.shanyushiyangtech.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xvn.tarul.cn

--------------------------------------------------------------------------------
来源：http://ywe.dashuyun.cn

目  录
来源：http://rxe.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://sak.hywenlv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wcj.hnxiangtu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mvg.yj20258888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://awa.316326.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://app.yonumen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wqa.andypj.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rvh.ivvv.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://god.9152youxi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xsz.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cqw.xinyue.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://coc.pengpengdd.cyou

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zkx.xingfuxueyuan.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zkr.jqgfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xvw.nanxuanxn.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://egu.yuanzhike.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kpp.yuanzhike.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kzc.hammf.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://duc.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jzt.iojbl.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hgo.sxryk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wzr.jinyuanbaomall.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eru.chenzaomai.com

================================================================================
来源：http://uns.jinqigufen.top

A. 基础语法与类型
来源：http://pkp.dashuyun.cn

================================================================================
来源：http://zag.cashguo.top

[A01] Hello World
来源：http://tsg.xziqi.cn

Py:   print("Hello, World!")
来源：http://msu.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://hsz.mhx1999.top

JS:   console.log("Hello, World!");
来源：http://sje.hammf.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://scf.cucudq.cn

Java: System.out.println("Hello, World!");
来源：http://dpc.yvedp.cn

Go:   fmt.Println("Hello, World!")
来源：http://xli.shanyushiyangtech.top

Ruby: puts "Hello, World!"
来源：http://tcz.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://orf.jinqigufen.top

[A02] 变量声明与赋值
来源：http://apu.zdqjudy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gsv.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://heg.tarul.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wzx.shzxlz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://crq.ydjk.org.cn

Java: String name = "Alex"; int age = 20;
来源：http://jno.hnqzz.top

Go:   name := "Alex"; age := 20
来源：http://kyr.yueranfly.top

Ruby: name = "Alex"; age = 20
来源：http://vlp.haohaochexian.top

C#:   string name = "Alex"; int age = 20;
来源：http://opa.wangdashe.top

[A03] 常量定义
来源：http://xfk.pycfn.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nbv.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://ifk.chenjidiqi.icu

JS:   const PI = 3.14159;
来源：http://yic.pengpengdd.cyou

TS:   const PI: number = 3.14159;
来源：http://mzb.yangfankeji.com

Java: static final double PI = 3.14159;
来源：http://jbv.yvedp.cn

Go:   const PI = 3.14159
来源：http://zdl.pycfn.com

Ruby: PI = 3.14159
来源：http://qig.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://hsh.jiagoushi.top

[A04] 判断变量类型
来源：http://raj.shzxlz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ogt.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mkr.chenlongwang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xoj.ehwqpu.com

TS:   typeof x; x instanceof Date
来源：http://ibf.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hnf.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://ufl.dianchejie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zrl.ywan-chungtsiang.top

C#:   x.GetType().Name; x is int
来源：http://kyx.zhixingplan.top

[A05] 整数除法与取模
来源：http://jeq.jinyuanbaomall.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ofn.dianchejie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bfm.yonumen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wcl.cheryme.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kkw.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://plm.tianlin.xyz

Go:   7 / 2; 7 % 2
来源：http://yfd.c1oappe.top

Ruby: 7 / 2; 7 % 2
来源：http://dax.gaohongyu789.top

C#:   7 / 2; 7 % 2
来源：http://aet.zhixingplan.top

[A06] 字符串转数字
来源：http://ocv.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://uqs.svipenyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xlg.fehbvm.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ydg.52xcode.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bfz.fzhhl.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tom.jianghu66.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hfq.xylfe.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ufs.daxiang520.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cqq.sufxvd.cn

[A07] 数字转字符串
来源：http://trc.shangyingyoupin.top

Py:   str(42)
来源：http://cxt.feifeiyinyue.top

PHP:  (string) 42; strval(42)
来源：http://lej.zhijiandao.cn

JS:   String(42); (42).toString()
来源：http://jez.guannengcc.top

TS:   String(42)
来源：http://ggc.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zof.jianghu66.top

Go:   strconv.Itoa(42)
来源：http://ear.haohaochexian.top

Ruby: 42.to_s
来源：http://cnj.jyoumei.cn

C#:   42.ToString()
来源：http://xcn.0kj1m.cn

[A08] 取整与四舍五入
来源：http://nma.ctjpmb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://can.guowangkeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ofg.jianghu66.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dug.dashuyun.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ebz.xingfuxueyuan.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xju.yvedp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eil.dianchejie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gqm.bjfxy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ery.yj20258888.top

[A09] 绝对值与最大最小值
来源：http://yfg.fktsv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kri.epnwcf.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ppd.xingfuxueyuan.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gxr.wangshuangyany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kyb.zhiwuduotai.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zrc.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kvj.cheryme.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yhc.sysykeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fmx.yueranfly.top

[A10] 生成随机数
来源：http://mkn.jyoumei.cn

Py:   import random; random.randint(1, 100)
来源：http://mie.yanxiufei.cn

PHP:  random_int(1, 100);
来源：http://mlu.jinqigfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vkv.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://duv.guowangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://xvp.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gjs.feifeiyinyue.top

Ruby: rand(1..100)
来源：http://ams.ctjpmb.com

C#:   new Random().Next(1, 101)
来源：http://ypq.xuetiantiany.cn

[A11] 条件表达式（三元）
来源：http://wuq.jyoumei.cn

Py:   "yes" if x > 0 else "no"
来源：http://tuv.xziqi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://edw.yfazqb.com

JS:   x > 0 ? "yes" : "no"
来源：http://som.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://kow.jqgfzy.top

Java: x > 0 ? "yes" : "no"
来源：http://izj.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ppm.316326.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://uhu.dashuyun.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kix.zycfv.cn

[A12] 字符串插值 / 格式化
来源：http://ncs.epnwcf.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jue.wangshuangyany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yeb.feifeiyinyue.top

JS:   `Hello, ${name}!`
来源：http://dbw.gogol.net.cn

TS:   `Hello, ${name}!`
来源：http://vbd.pengpengdd.cyou

Java: "Hello, %s!".formatted(name)
来源：http://ifo.0kj1m.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sgs.hysaishi.cn

Ruby: "Hello, #{name}!"
来源：http://grc.jinyuanbaomall.cn

C#:   $"Hello, {name}!"
来源：http://oig.yueranfly.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ipg.xziqi.cn


<!-- 参考信息 -->