代发 wailian999

[U79] PHP：静态分析
来源：http://qal.dianchejie.cn

composer require --dev phpstan/phpstan
来源：http://ofu.shanyushiyangkeji.top

[U80] PHP：代码规范修复
来源：http://ydk.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qlq.yuxming.cn

[U81] JS：初始化项目
来源：http://ome.ehwqpu.com

npm init -y;  npm i express
来源：http://cae.yj20258.top

[U82] JS：package.json 脚本
来源：http://ste.feifeiyinyue.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://frp.hywenlv.cn

[U83] JS：ES Module 导入导出
来源：http://lyj.jinqigfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://gfs.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://rty.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://awe.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://hpj.yj202588.top

a?.b?.c
来源：http://sgh.zycfv.cn

[U86] JS：空值合并
来源：http://psv.sweek.top

a ?? b
来源：http://czj.yonumen.top

[U87] JS：解构默认值
来源：http://wnm.shuidangran.top

const { a = 1, b = 2 } = obj;
来源：http://ynd.xuanzx.com

[U88] JS：对象展开合并
来源：http://csu.chenlongwang.top

{ ...a, ...b }
来源：http://bku.yonumen.top

[U89] JS：数组去重
来源：http://lvu.aibaodan.cn

[...new Set(arr)]
来源：http://mqh.aizwys.cn

[U90] JS：数字数组排序
来源：http://bph.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://ils.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://pnn.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wtz.fengsongda.top

[U92] JS：深拷贝
来源：http://pqw.xylfe.cn

structuredClone(obj)
来源：http://cew.xingfuxueyuan.xyz

[U93] JS：模板字符串
来源：http://vsh.jqgufenzy.top

`共 ${n} 条`
来源：http://rli.gotoacloud.top

[U94] JS：箭头函数
来源：http://zmm.zhiwuduotai.top

const double = x => x * 2;
来源：http://zbf.haohaochexian.top

[U95] JS：Promise 包装
来源：http://zxy.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://gmp.fengsongda.top

[U96] JS：async/await 与异常
来源：http://ctp.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oug.aizwys.cn

[U97] JS：并发请求
来源：http://yvj.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://uiy.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://vwy.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://unn.yanxiufei.cn

[U99] JS：事件监听
来源：http://kph.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://ouk.guowangkeji.top

[U100] JS：DOM 查询
来源：http://erq.quarkkingdee.top

document.querySelector(".item")
来源：http://nni.sweek.top

[U101] JS：classList 操作
来源：http://msx.tian-w.cn

el.classList.toggle("active")
来源：http://ukf.chenlongwang.top

[U102] JS：本地存储
来源：http://ibk.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mug.smart0.xyz

[U103] JS：定时器
来源：http://fal.jqgfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ywu.dianchejie.cn

[U104] JS：防抖
来源：http://lzm.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vaa.shanyushiyangkeji.top

[U105] JS：节流
来源：http://hum.sweek.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pzd.jinqigufen.top

[U106] JS：日期格式化
来源：http://xxi.aibaodan.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xsw.jinqigfzy.top

[U107] JS：数字千分位
来源：http://aug.ivvv.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dvp.tarul.cn

[U108] JS：随机整数
来源：http://nql.ydjk.org.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lrk.meibo888.top

[U109] JS：数组分组
来源：http://ydv.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://uap.hysaishi.cn

[U110] JS：数组分块
来源：http://qgs.shuidangran.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://psa.fehbvm.com

[U111] JS：对象转 Map
来源：http://yeq.wangdashe.top

new Map(Object.entries(obj))
来源：http://cns.hcnkem.com

[U112] JS：字符串补位
来源：http://oaz.0kj1m.cn

"7".padStart(3, "0")
来源：http://nju.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://plh.jlsjyb.cn

s.replaceAll("a", "b")
来源：http://hyy.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://szg.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://een.yj20258888.top

[U115] JS：生成 UUID
来源：http://oow.sysykeji.top

crypto.randomUUID()
来源：http://hhh.hesvh.cn

[U116] JS：类型检查（JSDoc）
来源：http://nxm.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://eij.shangyingyoupin.top

[U117] JS：单元测试
来源：http://iej.tarul.cn

npm i -D vitest;  npx vitest
来源：http://fll.zhongyouzk.top

[U118] JS：开发服务器
来源：http://bis.jinqigufen.top

npm i -D vite;  npx vite
来源：http://hgd.guowangkeji.top

[U119] JS：生产构建
来源：http://msz.zhixingplan.top

npx vite build
来源：http://rtf.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://wtx.cheryme.top

import.meta.env.VITE_API_URL
来源：http://inq.ywan-chungtsiang.top

================================================================================
来源：http://upb.dianchejie.cn

统计汇总
来源：http://fzf.cucudq.cn

================================================================================
来源：http://kvh.feifeiyinyue.top

按语言统计（条）：
来源：http://ffl.9152youxi.cn

Python ......... 252
来源：http://abt.9152youxi.cn

PHP ............ 252
来源：http://eob.yj202588.top

JavaScript ..... 252
来源：http://lbr.hongshengwenyu.top

TypeScript ..... 212
来源：http://zrr.kuanghao11.cn

Java ........... 212
来源：http://phm.iojbl.cn

Go ............. 212
来源：http://ztj.jqgufenzy.top

Ruby ........... 212
来源：http://yhg.cdnleiting.top

C# ............. 212
来源：http://tti.9152youxi.cn

C .............. 30
来源：http://tqs.shanyushiyangkeji.top

C++ ............ 30
来源：http://qoq.feifeiyinyue.top

SQL ............ 90
来源：http://mqo.jinghuilouyu.cn

Bash ........... 80
来源：http://uag.aibaodan.cn

Kotlin ......... 15
来源：http://huz.9152youxi.cn

Swift .......... 15
来源：http://hpk.smart0.xyz

Lua ............ 10
来源：http://cqs.yanxiufei.cn

Perl ........... 10
来源：http://qqi.ybcxt.top

Scala .......... 10
来源：http://uzv.wangdashe.top

------------------------------------
来源：http://czj.jqgufenzy.top

合计 ........... 2106 条
来源：http://bab.jqgfzy.top

按章节统计：
来源：http://ota.jinyuanbaomall.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mcp.fzhhl.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ydc.ydjk.org.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://det.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ogc.smart0.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lec.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lrv.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uti.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xkl.xuetiantiany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kic.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://llt.ehwqpu.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jpg.pycfn.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mgi.shzxlz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://anv.jinyuanbaomall.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ykh.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rto.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nbp.jlsjyb.cn

Q SQL 专题                              90
来源：http://ddh.fengsongda.top

R Bash 专题                             80
来源：http://jta.cheryme.top

S C / C++ 专题                          60
来源：http://cxh.hysaishi.cn

T 其他语言补充                          60
来源：http://wob.uphjek.com

U 高频实用片段                         120
来源：http://xnv.tanke756.top

------------------------------------
来源：http://mxp.iojbl.cn

合计                                  2106 条
来源：http://lfy.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://mkl.tarul.cn

使用提醒
来源：http://zos.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://xlo.nwbrower.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://brr.yj20258.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ogy.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ktr.bjfxy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ojy.jqgfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uhw.fktsv.cn

—— 文件结束 ——
来源：http://iag.zdbjq.cn

================================================================================
来源：http://ami.ehwqpu.com

程序语言常见例子速查手册（2024 版）
来源：http://wfr.dianchejie.cn

Common Programming Examples Cheat Book
来源：http://ktq.ybcxt.top

================================================================================
来源：http://duz.tianlin.xyz

【收录内容】
来源：http://fbd.uphjek.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://jpz.ydzc1.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cax.ydzc1.top

SQL · Bash · C · C++
来源：http://jek.jiagoushi.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://koj.sysykeji.top

【使用说明】
来源：http://bhf.sjlbkw.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wcu.yj202588.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ihh.yonumen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zvj.jinyuanbaomall.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rna.shanyushiyangtech.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cki.zhiwuduotai.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://unz.cdnleiting.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uli.hfpthk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ddf.xylfe.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hhw.jqgufenzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jyw.wangshuangyany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://aqq.52xcode.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rop.zhoulong.xyz

【文件统计】
来源：http://pkl.daria6918.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wbu.guannengcc.top

--------------------------------------------------------------------------------
来源：http://rwo.jyoumei.cn

目  录
来源：http://wht.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://snt.ctjpmb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ybz.svipenyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zmi.jqgufenzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lcw.tanke756.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fdn.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://art.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kyp.shanyushiyangtech.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tmb.sufxvd.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://age.cashguo.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zdw.smart0.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tsu.vehdjk.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sqf.zhixingplan.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jtb.redwolf501.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jmb.gogol.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vvj.ppjwa.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iiy.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bxz.316326.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gza.hfpthk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://umj.nwbrower.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lum.yonumen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nqr.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xqw.zycfv.cn

================================================================================
来源：http://tsz.shuidangran.top

A. 基础语法与类型
来源：http://dxd.sysykeji.top

================================================================================
来源：http://dxa.hongshengwenyu.top

[A01] Hello World
来源：http://yuu.yanxiufei.cn

Py:   print("Hello, World!")
来源：http://ivp.yueranfly.top

PHP:  echo "Hello, World!";
来源：http://nas.nanxinkj.top

JS:   console.log("Hello, World!");
来源：http://qih.smart0.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mqv.vqdsnc.cn

Java: System.out.println("Hello, World!");
来源：http://jth.andypj.xyz

Go:   fmt.Println("Hello, World!")
来源：http://mfz.jinqigfzy.top

Ruby: puts "Hello, World!"
来源：http://dym.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://urv.ywan-chungtsiang.top

[A02] 变量声明与赋值
来源：http://ggt.yanxiufei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vpz.cdnleiting.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ips.shanyushiyangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://gcd.jinqigfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oco.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://gfq.dianchejie.cn

Go:   name := "Alex"; age := 20
来源：http://zte.sysykeji.top

Ruby: name = "Alex"; age = 20
来源：http://iut.hysaishi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://czn.aibaodan.cn

[A03] 常量定义
来源：http://vqc.zhiwuduotai.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fuf.jqgufenzy.top

PHP:  const PI = 3.14159;
来源：http://veb.quarkkingdee.top

JS:   const PI = 3.14159;
来源：http://jjo.nanxuanxn.top

TS:   const PI: number = 3.14159;
来源：http://hzv.jinghuilouyu.cn

Java: static final double PI = 3.14159;
来源：http://ebi.zhongyouzk.top

Go:   const PI = 3.14159
来源：http://yxm.zhoulong.xyz

Ruby: PI = 3.14159
来源：http://amr.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://mlk.hywenlv.cn

[A04] 判断变量类型
来源：http://wsh.gogol.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://joj.gotoacloud.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wzg.ydzc1.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rpo.jlsjyb.cn

TS:   typeof x; x instanceof Date
来源：http://zkx.ydzc1.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rsq.sweek.top

Go:   reflect.TypeOf(x).Name()
来源：http://luf.feifeiyinyue.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gsx.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://gwc.ybcxt.top

[A05] 整数除法与取模
来源：http://fbi.cashguo.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pzr.cashguo.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ibg.zycfv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jeh.gaohongyu789.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tco.jinghuilouyu.cn

Java: 7 / 2; 7 % 2
来源：http://eth.guannengcc.top

Go:   7 / 2; 7 % 2
来源：http://drl.shanyushiyangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://pow.kuanghao11.cn

C#:   7 / 2; 7 % 2
来源：http://vuo.gaohongyu789.top

[A06] 字符串转数字
来源：http://qla.vehdjk.com

Py:   int("42"); float("3.14")
来源：http://pnb.yonumen.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sma.uphjek.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://idu.zhengqikj.top

TS:   parseInt("42", 10); Number("42")
来源：http://ylc.hcnkem.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://odt.xylfe.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://doo.sweek.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hhl.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hcn.sxryk.cn

[A07] 数字转字符串
来源：http://gpv.gotoacloud.top

Py:   str(42)
来源：http://qlu.hammf.cn

PHP:  (string) 42; strval(42)
来源：http://zhd.dianchejie.cn

JS:   String(42); (42).toString()
来源：http://olg.ppjwa.cn

TS:   String(42)
来源：http://ehw.ehwqpu.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://bia.nanxinkj.top

Go:   strconv.Itoa(42)
来源：http://vwo.316326.xyz

Ruby: 42.to_s
来源：http://ccs.52xcode.cn

C#:   42.ToString()
来源：http://aqj.ctjpmb.com

[A08] 取整与四舍五入
来源：http://hjw.sufxvd.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ypu.zycfv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zuu.snrcjt.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://utm.ywan-chungtsiang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qsc.c1oappe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://raz.xinyue.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://czw.tianlin.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://utx.yj202588.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://siz.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://tnv.52xcode.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bsu.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rku.yfazqb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://scm.tianlin.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ics.ctjpmb.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ezb.zdbjq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tmz.ydjk.org.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rdc.ehwqpu.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yzj.fengsongda.top

[A10] 生成随机数
来源：http://sil.zhijiandao.cn

Py:   import random; random.randint(1, 100)
来源：http://lqt.aizwys.cn

PHP:  random_int(1, 100);
来源：http://jyn.nanxuanxn.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vui.shuidangran.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nia.shanyushiyangtech.top

Java: new Random().nextInt(100) + 1
来源：http://oob.zhaomingkeji.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dix.aizwys.cn

Ruby: rand(1..100)
来源：http://ldl.ctjpmb.com

C#:   new Random().Next(1, 101)
来源：http://uda.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://sld.hysaishi.cn

Py:   "yes" if x > 0 else "no"
来源：http://wpe.zycfv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://osx.nanxuanxn.top

JS:   x > 0 ? "yes" : "no"
来源：http://ngp.xylfe.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qwj.xuetiantiany.cn

Java: x > 0 ? "yes" : "no"
来源：http://suc.shuidangran.top

Go:   // 无三元运算符，需用 if 语句
来源：http://div.chenjidiqi.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://ibr.ydzc1.top

C#:   x > 0 ? "yes" : "no"
来源：http://wcz.aibaodan.cn

[A12] 字符串插值 / 格式化
来源：http://vrn.guowangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wmf.ctjpmb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jcb.tarul.cn

JS:   `Hello, ${name}!`
来源：http://byz.ivvv.top

TS:   `Hello, ${name}!`
来源：http://fbj.hesvh.cn

Java: "Hello, %s!".formatted(name)
来源：http://nzw.fengsongda.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ddw.zhengqikj.top

Ruby: "Hello, #{name}!"
来源：http://syc.cqqwz.cn

C#:   $"Hello, {name}!"
来源：http://foj.andypj.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://uqw.tarul.cn


<!-- 参考信息 -->