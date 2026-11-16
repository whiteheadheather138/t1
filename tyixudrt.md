代发 wailian999

[U77] PHP：模板渲染
来源：http://vku.pycfn.com

composer require twig/twig
来源：http://dka.hesvh.cn

[U78] PHP：单元测试
来源：http://dga.ydjk.org.cn

composer require --dev phpunit/phpunit
来源：http://emw.yj202588.top

[U79] PHP：静态分析
来源：http://zhd.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://gwz.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://iaj.jinqigufen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rtn.mhx1999.top

[U81] JS：初始化项目
来源：http://asf.gogol.net.cn

npm init -y;  npm i express
来源：http://zdp.316326.xyz

[U82] JS：package.json 脚本
来源：http://igh.cqqwz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://idm.zhaomingkeji.xyz

[U83] JS：ES Module 导入导出
来源：http://mvr.ydjk.org.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xgh.daria6918.cn

[U84] JS：CommonJS 写法
来源：http://tes.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://bns.jyoumei.cn

[U85] JS：可选链
来源：http://hrw.daxiang520.top

a?.b?.c
来源：http://ohf.birdmap.top

[U86] JS：空值合并
来源：http://pwq.xuanzx.com

a ?? b
来源：http://ach.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://jqu.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://bqx.sysykeji.top

[U88] JS：对象展开合并
来源：http://oaw.sweek.top

{ ...a, ...b }
来源：http://rnq.cqqwz.cn

[U89] JS：数组去重
来源：http://zcj.vqdsnc.cn

[...new Set(arr)]
来源：http://btu.ydjk.org.cn

[U90] JS：数字数组排序
来源：http://irq.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://wgw.fktsv.cn

[U91] JS：对象键值遍历
来源：http://rtk.hongshengwenyu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cwc.hysaishi.cn

[U92] JS：深拷贝
来源：http://sny.yuxming.cn

structuredClone(obj)
来源：http://ipz.jlsjyb.cn

[U93] JS：模板字符串
来源：http://agt.aibaodan.cn

`共 ${n} 条`
来源：http://yps.xylfe.cn

[U94] JS：箭头函数
来源：http://eff.meibo888.top

const double = x => x * 2;
来源：http://npr.smart0.xyz

[U95] JS：Promise 包装
来源：http://duo.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://iuk.gzhubu.top

[U96] JS：async/await 与异常
来源：http://nzt.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ncc.bbcook.cn

[U97] JS：并发请求
来源：http://hoe.nwbrower.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ttd.dianchejie.cn

[U98] JS：fetch 带 JSON
来源：http://kwn.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ezf.jyoumei.cn

[U99] JS：事件监听
来源：http://fpb.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://cce.yonumen.top

[U100] JS：DOM 查询
来源：http://adw.zdqjudy.top

document.querySelector(".item")
来源：http://dkw.fanxiaobao.xyz

[U101] JS：classList 操作
来源：http://gdj.xziqi.cn

el.classList.toggle("active")
来源：http://ufo.pengpengdd.cyou

[U102] JS：本地存储
来源：http://wfq.yj202588.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pdd.svipenyu.cn

[U103] JS：定时器
来源：http://gyh.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fmg.uphjek.com

[U104] JS：防抖
来源：http://mgb.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aus.dianchejie.cn

[U105] JS：节流
来源：http://ytc.gzhubu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rxt.yuanzhike.top

[U106] JS：日期格式化
来源：http://dks.aibaodan.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uug.fktsv.cn

[U107] JS：数字千分位
来源：http://epx.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zyi.316326.xyz

[U108] JS：随机整数
来源：http://ufa.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hll.gogol.net.cn

[U109] JS：数组分组
来源：http://eap.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://pev.jianghu66.top

[U110] JS：数组分块
来源：http://nsk.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gae.shanyushiyangkeji.top

[U111] JS：对象转 Map
来源：http://xxq.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://bdx.gzhubu.top

[U112] JS：字符串补位
来源：http://esx.shangyingyoupin.top

"7".padStart(3, "0")
来源：http://qhi.birdmap.top

[U113] JS：正则替换全部
来源：http://ayo.ctjpmb.com

s.replaceAll("a", "b")
来源：http://tcx.xuanzx.com

[U114] JS：JSON 深比较
来源：http://rve.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ver.yonumen.top

[U115] JS：生成 UUID
来源：http://hcy.hnqzz.top

crypto.randomUUID()
来源：http://fou.zhixingplan.top

[U116] JS：类型检查（JSDoc）
来源：http://pcj.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://myo.gogol.net.cn

[U117] JS：单元测试
来源：http://rki.fktsv.cn

npm i -D vitest;  npx vitest
来源：http://nlh.guowangkeji.top

[U118] JS：开发服务器
来源：http://cjd.hnqzz.top

npm i -D vite;  npx vite
来源：http://hxf.zhengqikj.top

[U119] JS：生产构建
来源：http://kmt.cashguo.top

npx vite build
来源：http://odv.snrcjt.cn

[U120] JS：读取环境变量（Vite）
来源：http://hgt.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://sxf.svipenyu.cn

================================================================================
来源：http://oyd.vqdsnc.cn

统计汇总
来源：http://vft.fzhhl.top

================================================================================
来源：http://kvr.yj20258.top

按语言统计（条）：
来源：http://rid.yfazqb.com

Python ......... 252
来源：http://alh.dianchejie.cn

PHP ............ 252
来源：http://ogt.yonumen.top

JavaScript ..... 252
来源：http://rtk.ydjk.org.cn

TypeScript ..... 212
来源：http://fsv.hnxiangtu.top

Java ........... 212
来源：http://ran.ehwqpu.com

Go ............. 212
来源：http://lag.birdmap.top

Ruby ........... 212
来源：http://rak.hcnkem.com

C# ............. 212
来源：http://vkc.ctjpmb.com

C .............. 30
来源：http://wxk.yj20258888.top

C++ ............ 30
来源：http://vkn.vehdjk.com

SQL ............ 90
来源：http://wfw.52xcode.cn

Bash ........... 80
来源：http://loj.cheryme.top

Kotlin ......... 15
来源：http://pcz.yuxming.cn

Swift .......... 15
来源：http://wfh.hnqzz.top

Lua ............ 10
来源：http://rzd.hysaishi.cn

Perl ........... 10
来源：http://ugi.svipenyu.cn

Scala .......... 10
来源：http://jgo.nanxinkj.top

------------------------------------
来源：http://bys.shzxlz.cn

合计 ........... 2106 条
来源：http://ykg.epnwcf.com

按章节统计：
来源：http://cmj.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dgh.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://chf.sufxvd.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lhk.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ekc.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://joi.hesvh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xyf.yanxiufei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pxy.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dwd.yongpay.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sht.hysaishi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rrm.yongpay.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xot.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vzo.yanxiufei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://drx.bjfxy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sxa.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://csj.yangfankeji.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wnx.fzhhl.top

Q SQL 专题                              90
来源：http://sep.tian-w.cn

R Bash 专题                             80
来源：http://zsd.52xcode.cn

S C / C++ 专题                          60
来源：http://nki.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://pwv.guannengcc.top

U 高频实用片段                         120
来源：http://eoe.chenzaomai.com

------------------------------------
来源：http://lao.tian-w.cn

合计                                  2106 条
来源：http://jpo.yj20258888.top

--------------------------------------------------------------------------------
来源：http://hfl.shuidangran.top

使用提醒
来源：http://ivg.ivvv.top

--------------------------------------------------------------------------------
来源：http://ukl.zhoulong.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://obg.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pup.yj202588.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ijp.yuxming.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://juk.tian-w.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dpv.havefunace.top

—— 文件结束 ——
来源：http://ajp.ctjpmb.com

================================================================================
来源：http://dql.ehwqpu.com

程序语言常见例子速查手册（2024 版）
来源：http://atx.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://aum.chenzaomai.com

================================================================================
来源：http://gwk.chenlongwang.top

【收录内容】
来源：http://pta.mhx1999.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dfs.hammf.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hnv.andypj.xyz

SQL · Bash · C · C++
来源：http://gas.yanxiufei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lxb.cheryme.top

【使用说明】
来源：http://umn.cheryme.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ysp.xziqi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wyy.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://okf.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vrt.jqgufenzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nas.hcnkem.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zvt.tianlin.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fno.zdbjq.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jig.tian-w.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dih.hesvh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dke.bbcook.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ybz.zhaomingkeji.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://anq.yfazqb.com

【文件统计】
来源：http://wqi.ehwqpu.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bnc.tian-w.cn

--------------------------------------------------------------------------------
来源：http://bmk.ppjwa.cn

目  录
来源：http://wnq.hcnkem.com

--------------------------------------------------------------------------------
来源：http://vou.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uva.hcnkem.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://abf.zdbjq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qxo.feifeiyinyue.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ahe.shanyushiyangtech.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dda.yvedp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uhg.chenjidiqi.icu

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wzv.hongshengwenyu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://szr.redwolf501.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vys.hcnkem.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wgc.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ubx.fehbvm.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://boy.yj20258.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tfy.cashguo.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yof.0kj1m.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vqi.9152youxi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iqu.pycfn.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vfk.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://kla.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nvv.c1oappe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uws.fktsv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jqv.jinqigfzy.top

================================================================================
来源：http://vmv.dashuyun.cn

A. 基础语法与类型
来源：http://rha.jinqigufen.top

================================================================================
来源：http://nnz.pycfn.com

[A01] Hello World
来源：http://pfc.jyoumei.cn

Py:   print("Hello, World!")
来源：http://vtu.316326.xyz

PHP:  echo "Hello, World!";
来源：http://zfw.redwolf501.top

JS:   console.log("Hello, World!");
来源：http://bch.shuidangran.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rso.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://oee.nanxuanxn.top

Go:   fmt.Println("Hello, World!")
来源：http://uzu.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://sfy.uphjek.com

C#:   Console.WriteLine("Hello, World!");
来源：http://cyc.yueranfly.top

[A02] 变量声明与赋值
来源：http://vmk.zdbjq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dxy.chenzaomai.com

PHP:  $name = "Alex"; $age = 20;
来源：http://tna.fehbvm.com

JS:   let name = "Alex"; const age = 20;
来源：http://sif.hywenlv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://obh.cashguo.top

Java: String name = "Alex"; int age = 20;
来源：http://wry.nanxuanxn.top

Go:   name := "Alex"; age := 20
来源：http://tnt.aibaodan.cn

Ruby: name = "Alex"; age = 20
来源：http://ngg.yj202588.top

C#:   string name = "Alex"; int age = 20;
来源：http://rli.guannengcc.top

[A03] 常量定义
来源：http://pez.fengsongda.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kkb.yj20258.top

PHP:  const PI = 3.14159;
来源：http://vok.havefunace.top

JS:   const PI = 3.14159;
来源：http://vys.hnqzz.top

TS:   const PI: number = 3.14159;
来源：http://nfh.hnxiangtu.top

Java: static final double PI = 3.14159;
来源：http://evo.hywenlv.cn

Go:   const PI = 3.14159
来源：http://dsg.c1oappe.top

Ruby: PI = 3.14159
来源：http://qoi.jqgfzy.top

C#:   const double PI = 3.14159;
来源：http://sjz.yuanzhike.top

[A04] 判断变量类型
来源：http://nve.jqgufenzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://sie.yj20258.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vdm.316326.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://faj.xingfuxueyuan.xyz

TS:   typeof x; x instanceof Date
来源：http://qfv.shangyingyoupin.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cof.hnqzz.top

Go:   reflect.TypeOf(x).Name()
来源：http://wzj.bjfxy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hpw.tarul.cn

C#:   x.GetType().Name; x is int
来源：http://eao.chenlongwang.top

[A05] 整数除法与取模
来源：http://nzq.mhx1999.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nex.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://mrq.yj20258.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://adb.hysaishi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iez.fehbvm.com

Java: 7 / 2; 7 % 2
来源：http://cwm.fzhhl.top

Go:   7 / 2; 7 % 2
来源：http://ngh.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://vbj.yj20258.top

C#:   7 / 2; 7 % 2
来源：http://bih.epnwcf.com

[A06] 字符串转数字
来源：http://lvs.hammf.cn

Py:   int("42"); float("3.14")
来源：http://hhn.hcnkem.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://asf.redwolf501.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mjy.fengsongda.top

TS:   parseInt("42", 10); Number("42")
来源：http://pgz.hammf.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lrr.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ndb.redwolf501.top

Ruby: "42".to_i; "3.14".to_f
来源：http://aeu.52xcode.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pfk.tian-w.cn

[A07] 数字转字符串
来源：http://ybm.zdqjudy.top

Py:   str(42)
来源：http://gcb.jinqigufen.top

PHP:  (string) 42; strval(42)
来源：http://mup.uphjek.com

JS:   String(42); (42).toString()
来源：http://jtm.vehdjk.com

TS:   String(42)
来源：http://uds.fehbvm.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://nnv.fktsv.cn

Go:   strconv.Itoa(42)
来源：http://aut.zdqjudy.top

Ruby: 42.to_s
来源：http://ywu.cdnleiting.top

C#:   42.ToString()
来源：http://zfi.tanke756.top

[A08] 取整与四舍五入
来源：http://jkk.dashuyun.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vqp.ywan-chungtsiang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tpy.sufxvd.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sga.zhengqikj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zyi.redwolf501.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pvh.zdbjq.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nli.kuanghao11.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ilx.havefunace.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pkw.nanxuanxn.top

[A09] 绝对值与最大最小值
来源：http://iiz.ybcxt.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qwf.chenzaomai.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cti.iojbl.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lxx.zhijiandao.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lsw.ctjpmb.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://frj.yangfankeji.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lna.hnxiangtu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cpe.feifeiyinyue.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yzd.feifeiyinyue.top

[A10] 生成随机数
来源：http://edt.fktsv.cn

Py:   import random; random.randint(1, 100)
来源：http://tht.yonumen.top

PHP:  random_int(1, 100);
来源：http://wzn.bjfxy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vza.gzhubu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://erc.ywan-chungtsiang.top

Java: new Random().nextInt(100) + 1
来源：http://lfm.ppjwa.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vmv.sweek.top

Ruby: rand(1..100)
来源：http://snm.vqdsnc.cn

C#:   new Random().Next(1, 101)
来源：http://uvg.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://hfh.ctjpmb.com

Py:   "yes" if x > 0 else "no"
来源：http://yip.sjlbkw.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wtp.hnqzz.top

JS:   x > 0 ? "yes" : "no"
来源：http://gzv.yonumen.top

TS:   x > 0 ? "yes" : "no"
来源：http://jzb.smart0.xyz

Java: x > 0 ? "yes" : "no"
来源：http://nvl.kuanghao11.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://byd.xingfuxueyuan.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://yhg.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mun.shuidangran.top

[A12] 字符串插值 / 格式化
来源：http://uib.bjfxy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pxb.vqdsnc.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mkk.jinyuanbaomall.cn

JS:   `Hello, ${name}!`
来源：http://lcr.gogol.net.cn

TS:   `Hello, ${name}!`
来源：http://rlc.9152youxi.cn

Java: "Hello, %s!".formatted(name)
来源：http://mhm.chenjidiqi.icu


<!-- 参考信息 -->