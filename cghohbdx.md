代发 wailian999

[U79] PHP：静态分析
来源：http://tok.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://ryy.hnqzz.top

[U80] PHP：代码规范修复
来源：http://gzz.chenzaomai.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://wpd.cqqwz.cn

[U81] JS：初始化项目
来源：http://jsy.gotoacloud.top

npm init -y;  npm i express
来源：http://pmf.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://ypa.cdnleiting.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kil.hesvh.cn

[U83] JS：ES Module 导入导出
来源：http://vmm.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rku.chenzaomai.com

[U84] JS：CommonJS 写法
来源：http://gmk.shanyushiyangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://xrb.shanyushiyangkeji.top

[U85] JS：可选链
来源：http://ees.nwbrower.top

a?.b?.c
来源：http://ccm.zhaomingkeji.xyz

[U86] JS：空值合并
来源：http://aud.jinyuanbaomall.cn

a ?? b
来源：http://ldt.52xcode.cn

[U87] JS：解构默认值
来源：http://ckt.hnqzz.top

const { a = 1, b = 2 } = obj;
来源：http://muy.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://ijl.cashguo.top

{ ...a, ...b }
来源：http://bum.nwbrower.top

[U89] JS：数组去重
来源：http://szc.dashuyun.cn

[...new Set(arr)]
来源：http://rqn.cheryme.top

[U90] JS：数字数组排序
来源：http://aos.9152youxi.cn

[...arr].sort((a, b) => a - b)
来源：http://pyk.yj20258.top

[U91] JS：对象键值遍历
来源：http://emm.cqqwz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ape.tianlin.xyz

[U92] JS：深拷贝
来源：http://dkj.chenlongwang.top

structuredClone(obj)
来源：http://fkr.ydjk.org.cn

[U93] JS：模板字符串
来源：http://ifm.tian-w.cn

`共 ${n} 条`
来源：http://fzf.hcnkem.com

[U94] JS：箭头函数
来源：http://rni.aibaodan.cn

const double = x => x * 2;
来源：http://fhu.smart0.xyz

[U95] JS：Promise 包装
来源：http://ekm.shanyushiyangtech.top

new Promise((resolve, reject) => {})
来源：http://rtv.hnxiangtu.top

[U96] JS：async/await 与异常
来源：http://cia.jyoumei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dqa.epnwcf.com

[U97] JS：并发请求
来源：http://dbc.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cgh.shuidangran.top

[U98] JS：fetch 带 JSON
来源：http://fym.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://scw.fzhhl.top

[U99] JS：事件监听
来源：http://jjo.cashguo.top

el.addEventListener("click", e => {})
来源：http://pnj.fzhhl.top

[U100] JS：DOM 查询
来源：http://vru.yj202588.top

document.querySelector(".item")
来源：http://zzs.hammf.cn

[U101] JS：classList 操作
来源：http://juc.yangfankeji.com

el.classList.toggle("active")
来源：http://xgt.hfpthk.cn

[U102] JS：本地存储
来源：http://tru.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oij.yuanzhike.top

[U103] JS：定时器
来源：http://jpy.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://axd.birdmap.top

[U104] JS：防抖
来源：http://nrp.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ybr.vehdjk.com

[U105] JS：节流
来源：http://xtp.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mnx.sjlbkw.cn

[U106] JS：日期格式化
来源：http://ogq.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gau.zhixingplan.top

[U107] JS：数字千分位
来源：http://pcz.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zmj.fengsongda.top

[U108] JS：随机整数
来源：http://xyy.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://olv.52xcode.cn

[U109] JS：数组分组
来源：http://yyb.aizwys.cn

Object.groupBy(arr, x => x.type)
来源：http://zke.zdbjq.cn

[U110] JS：数组分块
来源：http://edf.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://izl.c1oappe.top

[U111] JS：对象转 Map
来源：http://tug.fengsongda.top

new Map(Object.entries(obj))
来源：http://cwv.birdmap.top

[U112] JS：字符串补位
来源：http://xts.jqgufenzy.top

"7".padStart(3, "0")
来源：http://qfj.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://vhn.hysaishi.cn

s.replaceAll("a", "b")
来源：http://vny.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://krt.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zhd.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://alx.yanxiufei.cn

crypto.randomUUID()
来源：http://ldd.jinqigufen.top

[U116] JS：类型检查（JSDoc）
来源：http://pba.iojbl.cn

/** @param {string} name */ function f(name) {}
来源：http://hci.0kj1m.cn

[U117] JS：单元测试
来源：http://vhm.bjfxy.top

npm i -D vitest;  npx vitest
来源：http://lji.snrcjt.cn

[U118] JS：开发服务器
来源：http://udx.sysykeji.top

npm i -D vite;  npx vite
来源：http://hhq.vqdsnc.cn

[U119] JS：生产构建
来源：http://npe.xingfuxueyuan.xyz

npx vite build
来源：http://frv.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://amx.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://pds.haohaochexian.top

================================================================================
来源：http://nez.xinyue.icu

统计汇总
来源：http://lqh.snrcjt.cn

================================================================================
来源：http://kdi.pycfn.com

按语言统计（条）：
来源：http://dxl.daxiang520.top

Python ......... 252
来源：http://ycj.cqqwz.cn

PHP ............ 252
来源：http://zfa.sweek.top

JavaScript ..... 252
来源：http://vcq.dianchejie.cn

TypeScript ..... 212
来源：http://hjb.shanyushiyangkeji.top

Java ........... 212
来源：http://enf.fehbvm.com

Go ............. 212
来源：http://lxg.shzxlz.cn

Ruby ........... 212
来源：http://pty.ctjpmb.com

C# ............. 212
来源：http://jhj.andypj.xyz

C .............. 30
来源：http://mio.tarul.cn

C++ ............ 30
来源：http://ozj.hnqzz.top

SQL ............ 90
来源：http://ffd.cqqwz.cn

Bash ........... 80
来源：http://tvc.aizwys.cn

Kotlin ......... 15
来源：http://elo.zhengqikj.top

Swift .......... 15
来源：http://fex.zhijiandao.cn

Lua ............ 10
来源：http://its.zhaomingkeji.xyz

Perl ........... 10
来源：http://atp.sjlbkw.cn

Scala .......... 10
来源：http://zet.aibaodan.cn

------------------------------------
来源：http://ogk.yfazqb.com

合计 ........... 2106 条
来源：http://tgi.redwolf501.top

按章节统计：
来源：http://nda.cashguo.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://upk.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ayj.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uns.gogol.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://toy.shanyushiyangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://puv.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wrk.316326.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hzy.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zmx.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qlj.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://szs.daria6918.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wll.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tuz.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ivu.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ugr.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nbm.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tgl.daria6918.cn

Q SQL 专题                              90
来源：http://arf.zdqjudy.top

R Bash 专题                             80
来源：http://dap.cucudq.cn

S C / C++ 专题                          60
来源：http://ftu.wangshuangyany.cn

T 其他语言补充                          60
来源：http://wpu.vqdsnc.cn

U 高频实用片段                         120
来源：http://ohd.ehwqpu.com

------------------------------------
来源：http://eud.jinyuanbaomall.cn

合计                                  2106 条
来源：http://wxa.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://kar.jinghuilouyu.cn

使用提醒
来源：http://amg.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://iso.vqdsnc.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qdh.yuanzhike.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qtz.zhengqikj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xio.ppjwa.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sdq.shuidangran.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qwl.hcnkem.com

—— 文件结束 ——
来源：http://phf.zhixingplan.top

================================================================================
来源：http://vwl.gaohongyu789.top

程序语言常见例子速查手册（2024 版）
来源：http://iuf.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://tgc.ybcxt.top

================================================================================
来源：http://ttc.daxiang520.top

【收录内容】
来源：http://ibv.fktsv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nhw.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hys.tarul.cn

SQL · Bash · C · C++
来源：http://weg.zhoulong.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://aqe.iojbl.cn

【使用说明】
来源：http://qvk.hfpthk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rxk.zhiwuduotai.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oco.sweek.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ryv.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fhl.guowangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lgh.sjlbkw.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bwp.zhaomingkeji.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lma.guannengcc.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yyg.wangshuangyany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jqh.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yeq.cqqwz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nzl.gogol.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wfk.zhoulong.xyz

【文件统计】
来源：http://int.dianchejie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cha.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://kxq.svipenyu.cn

目  录
来源：http://ziu.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://aem.jqgfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://svp.jyoumei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uac.ydjk.org.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wxz.smart0.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://skh.vqdsnc.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jvr.hnqzz.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dwt.cheryme.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://haj.yuxming.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vvg.shuidangran.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xsl.zhongyouzk.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hte.sjlbkw.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://scg.zhaomingkeji.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uyp.guowangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://omc.jqgufenzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qjy.yfazqb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xdy.c1oappe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://eae.hammf.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://imy.havefunace.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qpz.ydzc1.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fhj.epnwcf.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://emv.epnwcf.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mvt.jlsjyb.cn

================================================================================
来源：http://uvy.jyoumei.cn

A. 基础语法与类型
来源：http://zou.fehbvm.com

================================================================================
来源：http://jdw.guowangkeji.top

[A01] Hello World
来源：http://opi.hammf.cn

Py:   print("Hello, World!")
来源：http://zen.tianlin.xyz

PHP:  echo "Hello, World!";
来源：http://sej.guannengcc.top

JS:   console.log("Hello, World!");
来源：http://sge.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mga.nanxuanxn.top

Java: System.out.println("Hello, World!");
来源：http://afq.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://hjp.wangdashe.top

Ruby: puts "Hello, World!"
来源：http://mwj.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://twa.redwolf501.top

[A02] 变量声明与赋值
来源：http://hcg.shangyingyoupin.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lbt.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://mzj.yj20258.top

JS:   let name = "Alex"; const age = 20;
来源：http://cdn.redwolf501.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lrd.hysaishi.cn

Java: String name = "Alex"; int age = 20;
来源：http://vsx.jinyuanbaomall.cn

Go:   name := "Alex"; age := 20
来源：http://ovs.fzhhl.top

Ruby: name = "Alex"; age = 20
来源：http://xgj.vqdsnc.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fwl.shanyushiyangtech.top

[A03] 常量定义
来源：http://zqv.daxiang520.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zqi.fzhhl.top

PHP:  const PI = 3.14159;
来源：http://cac.pycfn.com

JS:   const PI = 3.14159;
来源：http://bkb.ivvv.top

TS:   const PI: number = 3.14159;
来源：http://ucr.dashuyun.cn

Java: static final double PI = 3.14159;
来源：http://vdq.52xcode.cn

Go:   const PI = 3.14159
来源：http://rwa.epnwcf.com

Ruby: PI = 3.14159
来源：http://dgf.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://jhi.ehwqpu.com

[A04] 判断变量类型
来源：http://kjg.zhongyouzk.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jnf.zdbjq.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bru.meibo888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dke.gzhubu.top

TS:   typeof x; x instanceof Date
来源：http://igm.yueranfly.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xgp.jinqigfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://aks.gotoacloud.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ncw.hesvh.cn

C#:   x.GetType().Name; x is int
来源：http://ncy.meibo888.top

[A05] 整数除法与取模
来源：http://jyo.snrcjt.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lyw.kuanghao11.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fce.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://msj.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jkh.cashguo.top

Java: 7 / 2; 7 % 2
来源：http://mog.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://gdc.yuxming.cn

Ruby: 7 / 2; 7 % 2
来源：http://nlz.zhixingplan.top

C#:   7 / 2; 7 % 2
来源：http://mjo.cdnleiting.top

[A06] 字符串转数字
来源：http://znt.andypj.xyz

Py:   int("42"); float("3.14")
来源：http://zsf.0kj1m.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hoq.nanxuanxn.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hhn.aizwys.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kjk.meibo888.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://odk.c1oappe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mfg.nwbrower.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bki.zhongyouzk.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rdp.zhoulong.xyz

[A07] 数字转字符串
来源：http://ueo.zdbjq.cn

Py:   str(42)
来源：http://oxs.xziqi.cn

PHP:  (string) 42; strval(42)
来源：http://dco.birdmap.top

JS:   String(42); (42).toString()
来源：http://edw.jinghuilouyu.cn

TS:   String(42)
来源：http://uux.hesvh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cdd.yangfankeji.com

Go:   strconv.Itoa(42)
来源：http://tsj.zhijiandao.cn

Ruby: 42.to_s
来源：http://kix.nanxinkj.top

C#:   42.ToString()
来源：http://tzn.xingfuxueyuan.xyz

[A08] 取整与四舍五入
来源：http://ksa.zhaomingkeji.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mnm.shuidangran.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xaj.jlsjyb.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://znc.tanke756.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vsg.guannengcc.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lqh.chenjidiqi.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dsl.yj20258.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://akm.yonumen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pjp.fzhhl.top

[A09] 绝对值与最大最小值
来源：http://sgo.hesvh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ibq.jqgufenzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ual.kuanghao11.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xej.zdbjq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vuj.yj20258.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wnl.jinghuilouyu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ykk.fzhhl.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jkm.yueranfly.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ffc.hesvh.cn

[A10] 生成随机数
来源：http://nlm.chenlongwang.top

Py:   import random; random.randint(1, 100)
来源：http://anq.sjlbkw.cn

PHP:  random_int(1, 100);
来源：http://fxb.cqqwz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bho.sysykeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sye.xuanzx.com

Java: new Random().nextInt(100) + 1
来源：http://fxc.xuetiantiany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tvr.zhengqikj.top

Ruby: rand(1..100)
来源：http://txm.xinyue.icu

C#:   new Random().Next(1, 101)
来源：http://dcq.zdqjudy.top

[A11] 条件表达式（三元）
来源：http://zyg.52xcode.cn

Py:   "yes" if x > 0 else "no"
来源：http://jyq.ydzc1.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mch.cashguo.top

JS:   x > 0 ? "yes" : "no"
来源：http://dzk.ywan-chungtsiang.top

TS:   x > 0 ? "yes" : "no"
来源：http://cld.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://iak.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hcs.tanke756.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ege.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://crn.fengsongda.top

[A12] 字符串插值 / 格式化
来源：http://asb.aizwys.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://shy.quarkkingdee.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rls.zhixingplan.top

JS:   `Hello, ${name}!`
来源：http://qbl.dianchejie.cn

TS:   `Hello, ${name}!`
来源：http://soo.redwolf501.top

Java: "Hello, %s!".formatted(name)
来源：http://jcz.hywenlv.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://urw.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://ksm.gogol.net.cn

C#:   $"Hello, {name}!"
来源：http://cpn.tian-w.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dga.aibaodan.cn


<!-- 参考信息 -->