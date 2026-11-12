代发 wailian999

[U79] PHP：静态分析
来源：http://wnc.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://chx.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://nla.zhaomingkeji.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://tov.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://qft.daxiang520.top

npm init -y;  npm i express
来源：http://qie.epnwcf.com

[U82] JS：package.json 脚本
来源：http://lhy.xuetiantiany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ccn.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://wls.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qrb.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://dec.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://xck.fengsongda.top

[U85] JS：可选链
来源：http://fpu.jianghu66.top

a?.b?.c
来源：http://sla.yongpay.top

[U86] JS：空值合并
来源：http://dqe.yvedp.cn

a ?? b
来源：http://aub.9152youxi.cn

[U87] JS：解构默认值
来源：http://alq.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://fdz.yj202588.top

[U88] JS：对象展开合并
来源：http://dtf.jinqigufen.top

{ ...a, ...b }
来源：http://acn.ehwqpu.com

[U89] JS：数组去重
来源：http://rjb.pycfn.com

[...new Set(arr)]
来源：http://pra.9152youxi.cn

[U90] JS：数字数组排序
来源：http://bvh.bbcook.cn

[...arr].sort((a, b) => a - b)
来源：http://ovr.kuanghao11.cn

[U91] JS：对象键值遍历
来源：http://nnm.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bky.gotoacloud.top

[U92] JS：深拷贝
来源：http://bsu.zhoulong.xyz

structuredClone(obj)
来源：http://rde.xylfe.cn

[U93] JS：模板字符串
来源：http://jjt.hcnkem.com

`共 ${n} 条`
来源：http://mii.fzhhl.top

[U94] JS：箭头函数
来源：http://gew.shangyingyoupin.top

const double = x => x * 2;
来源：http://mrw.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://bdl.smart0.xyz

new Promise((resolve, reject) => {})
来源：http://rpa.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://mke.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lzy.xinyue.icu

[U97] JS：并发请求
来源：http://zgl.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hfv.gzhubu.top

[U98] JS：fetch 带 JSON
来源：http://zcz.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://chd.yj202588.top

[U99] JS：事件监听
来源：http://rcu.yongpay.top

el.addEventListener("click", e => {})
来源：http://whp.sweek.top

[U100] JS：DOM 查询
来源：http://jkq.hammf.cn

document.querySelector(".item")
来源：http://bon.iojbl.cn

[U101] JS：classList 操作
来源：http://qzd.yuxming.cn

el.classList.toggle("active")
来源：http://kvc.daxiang520.top

[U102] JS：本地存储
来源：http://wwv.daxiang520.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://eqf.hfpthk.cn

[U103] JS：定时器
来源：http://wdu.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://exw.fzhhl.top

[U104] JS：防抖
来源：http://ntp.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ixv.hongshengwenyu.top

[U105] JS：节流
来源：http://zcn.epnwcf.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vhd.tianlin.xyz

[U106] JS：日期格式化
来源：http://sjd.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cbt.ppjwa.cn

[U107] JS：数字千分位
来源：http://pmd.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://elo.xinyue.icu

[U108] JS：随机整数
来源：http://tgp.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uoc.zhixingplan.top

[U109] JS：数组分组
来源：http://gfs.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://szp.wangdashe.top

[U110] JS：数组分块
来源：http://zol.hnxiangtu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vsz.jianghu66.top

[U111] JS：对象转 Map
来源：http://ymg.hnqzz.top

new Map(Object.entries(obj))
来源：http://cbw.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://xjj.jianghu66.top

"7".padStart(3, "0")
来源：http://iun.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://moc.jlsjyb.cn

s.replaceAll("a", "b")
来源：http://fbi.shanyushiyangkeji.top

[U114] JS：JSON 深比较
来源：http://xhg.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yci.dianchejie.cn

[U115] JS：生成 UUID
来源：http://jiy.mhx1999.top

crypto.randomUUID()
来源：http://njl.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://haj.sysykeji.top

/** @param {string} name */ function f(name) {}
来源：http://vik.tian-w.cn

[U117] JS：单元测试
来源：http://jnm.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://qni.daxiang520.top

[U118] JS：开发服务器
来源：http://moe.daxiang520.top

npm i -D vite;  npx vite
来源：http://yzi.havefunace.top

[U119] JS：生产构建
来源：http://uhg.feifeiyinyue.top

npx vite build
来源：http://xia.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://rjn.yj20258888.top

import.meta.env.VITE_API_URL
来源：http://qmz.xinyue.icu

================================================================================
来源：http://qff.fktsv.cn

统计汇总
来源：http://qqo.hammf.cn

================================================================================
来源：http://pak.hnqzz.top

按语言统计（条）：
来源：http://sox.hfpthk.cn

Python ......... 252
来源：http://ieo.c1oappe.top

PHP ............ 252
来源：http://awj.tanke756.top

JavaScript ..... 252
来源：http://pnw.vehdjk.com

TypeScript ..... 212
来源：http://leq.kuanghao11.cn

Java ........... 212
来源：http://vgo.zycfv.cn

Go ............. 212
来源：http://cgm.jinqigufen.top

Ruby ........... 212
来源：http://rji.sxryk.cn

C# ............. 212
来源：http://zir.ydzc1.top

C .............. 30
来源：http://nwz.zhaomingkeji.xyz

C++ ............ 30
来源：http://vvx.aibaodan.cn

SQL ............ 90
来源：http://npx.yangfankeji.com

Bash ........... 80
来源：http://gvb.ydjk.org.cn

Kotlin ......... 15
来源：http://zqq.havefunace.top

Swift .......... 15
来源：http://cbu.ehwqpu.com

Lua ............ 10
来源：http://qum.mhx1999.top

Perl ........... 10
来源：http://bci.chenjidiqi.icu

Scala .......... 10
来源：http://abz.hammf.cn

------------------------------------
来源：http://hnm.ywan-chungtsiang.top

合计 ........... 2106 条
来源：http://jst.sysykeji.top

按章节统计：
来源：http://cek.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xkj.jinqigufen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lib.tian-w.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iqr.ctjpmb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fgs.cdnleiting.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eas.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zcc.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yiu.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tls.havefunace.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dbq.havefunace.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://agk.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kvz.cheryme.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://azt.zhixingplan.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://liw.gaohongyu789.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lhi.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vyc.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qob.cheryme.top

Q SQL 专题                              90
来源：http://eur.ehwqpu.com

R Bash 专题                             80
来源：http://ufv.cucudq.cn

S C / C++ 专题                          60
来源：http://nnt.zhongyouzk.top

T 其他语言补充                          60
来源：http://fzr.zhixingplan.top

U 高频实用片段                         120
来源：http://gml.bbcook.cn

------------------------------------
来源：http://ruu.dashuyun.cn

合计                                  2106 条
来源：http://iiz.fzhhl.top

--------------------------------------------------------------------------------
来源：http://oqz.xziqi.cn

使用提醒
来源：http://fmt.yongpay.top

--------------------------------------------------------------------------------
来源：http://atj.zhoulong.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tjk.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nwq.cqqwz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qgw.iojbl.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pak.svipenyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fur.chenlongwang.top

—— 文件结束 ——
来源：http://ibx.jinghuilouyu.cn

================================================================================
来源：http://akm.shangyingyoupin.top

程序语言常见例子速查手册（2024 版）
来源：http://fqz.yongpay.top

Common Programming Examples Cheat Book
来源：http://yiv.zycfv.cn

================================================================================
来源：http://awy.tarul.cn

【收录内容】
来源：http://gkh.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://hmo.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qep.jinqigfzy.top

SQL · Bash · C · C++
来源：http://qwz.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mva.fanxiaobao.xyz

【使用说明】
来源：http://qrp.9152youxi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kin.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vga.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://owd.xingfuxueyuan.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://unt.9152youxi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qrs.birdmap.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://reu.bbcook.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pwp.yongpay.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://swo.hnqzz.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mcp.yanxiufei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zwf.uphjek.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://coz.yuanzhike.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://boz.xuetiantiany.cn

【文件统计】
来源：http://jts.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jac.ydzc1.top

--------------------------------------------------------------------------------
来源：http://dob.zycfv.cn

目  录
来源：http://xof.tian-w.cn

--------------------------------------------------------------------------------
来源：http://kny.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ymj.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gaw.yueranfly.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zzv.fengsongda.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rix.chenjidiqi.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hgb.redwolf501.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ixa.cheryme.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ltc.yongpay.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ekb.ydjk.org.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ysn.birdmap.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://doj.shanyushiyangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ewf.cashguo.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hjp.haohaochexian.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lbf.xuanzx.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zdi.yj202588.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kpd.iojbl.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xvy.quarkkingdee.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fwi.jqgufenzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kco.zdqjudy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cee.epnwcf.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vxb.daria6918.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cne.ctjpmb.com

================================================================================
来源：http://iad.shanyushiyangtech.top

A. 基础语法与类型
来源：http://umc.hammf.cn

================================================================================
来源：http://bsf.jianghu66.top

[A01] Hello World
来源：http://woq.xingfuxueyuan.xyz

Py:   print("Hello, World!")
来源：http://ujq.ctjpmb.com

PHP:  echo "Hello, World!";
来源：http://gca.fzhhl.top

JS:   console.log("Hello, World!");
来源：http://uhv.chenjidiqi.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dls.pycfn.com

Java: System.out.println("Hello, World!");
来源：http://kdq.ybcxt.top

Go:   fmt.Println("Hello, World!")
来源：http://gxx.xinyue.icu

Ruby: puts "Hello, World!"
来源：http://row.hammf.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://obx.hammf.cn

[A02] 变量声明与赋值
来源：http://uab.52xcode.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vit.jinqigufen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ibi.shuidangran.top

JS:   let name = "Alex"; const age = 20;
来源：http://ksn.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yce.sweek.top

Java: String name = "Alex"; int age = 20;
来源：http://wse.zdbjq.cn

Go:   name := "Alex"; age := 20
来源：http://zrh.ctjpmb.com

Ruby: name = "Alex"; age = 20
来源：http://elz.jiagoushi.top

C#:   string name = "Alex"; int age = 20;
来源：http://rlx.yanxiufei.cn

[A03] 常量定义
来源：http://eza.xuetiantiany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dor.havefunace.top

PHP:  const PI = 3.14159;
来源：http://qup.pycfn.com

JS:   const PI = 3.14159;
来源：http://ndg.zhiwuduotai.top

TS:   const PI: number = 3.14159;
来源：http://rlz.hnxiangtu.top

Java: static final double PI = 3.14159;
来源：http://nao.haohaochexian.top

Go:   const PI = 3.14159
来源：http://mpb.vqdsnc.cn

Ruby: PI = 3.14159
来源：http://mlc.sjlbkw.cn

C#:   const double PI = 3.14159;
来源：http://ujt.vehdjk.com

[A04] 判断变量类型
来源：http://gks.gotoacloud.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zth.cqqwz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dbh.zhengqikj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kle.feifeiyinyue.top

TS:   typeof x; x instanceof Date
来源：http://wxu.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wul.fanxiaobao.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://oor.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yxw.vehdjk.com

C#:   x.GetType().Name; x is int
来源：http://zfw.birdmap.top

[A05] 整数除法与取模
来源：http://nzb.zhongyouzk.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://osw.yangfankeji.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://qkb.pengpengdd.cyou

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://umx.chenlongwang.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rzf.hywenlv.cn

Java: 7 / 2; 7 % 2
来源：http://oit.jlsjyb.cn

Go:   7 / 2; 7 % 2
来源：http://gqs.jyoumei.cn

Ruby: 7 / 2; 7 % 2
来源：http://auj.yvedp.cn

C#:   7 / 2; 7 % 2
来源：http://fmf.cheryme.top

[A06] 字符串转数字
来源：http://kmu.sjlbkw.cn

Py:   int("42"); float("3.14")
来源：http://zkg.svipenyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://saf.havefunace.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iyx.pycfn.com

TS:   parseInt("42", 10); Number("42")
来源：http://mqz.yj20258888.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pqi.yvedp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iqr.jqgufenzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://cqk.xuetiantiany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gyd.hammf.cn

[A07] 数字转字符串
来源：http://gep.haohaochexian.top

Py:   str(42)
来源：http://oxw.fehbvm.com

PHP:  (string) 42; strval(42)
来源：http://nyq.yj20258.top

JS:   String(42); (42).toString()
来源：http://wae.hnxiangtu.top

TS:   String(42)
来源：http://acd.zhiwuduotai.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nje.jlsjyb.cn

Go:   strconv.Itoa(42)
来源：http://flu.fzhhl.top

Ruby: 42.to_s
来源：http://zjy.jlsjyb.cn

C#:   42.ToString()
来源：http://bob.guannengcc.top

[A08] 取整与四舍五入
来源：http://cxq.zhijiandao.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dyy.gaohongyu789.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mov.meibo888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hbg.zhijiandao.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sfr.daxiang520.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://djf.gaohongyu789.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zgu.c1oappe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gkt.gaohongyu789.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rjh.ybcxt.top

[A09] 绝对值与最大最小值
来源：http://xdi.yanxiufei.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fzh.hysaishi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ksy.jinghuilouyu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://aln.jqgufenzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gbf.sysykeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lsu.cdnleiting.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mku.cucudq.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jno.jinqigufen.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kwp.ydzc1.top

[A10] 生成随机数
来源：http://lpe.svipenyu.cn

Py:   import random; random.randint(1, 100)
来源：http://aao.tanke756.top

PHP:  random_int(1, 100);
来源：http://pzk.jinyuanbaomall.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vpl.sweek.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qek.shzxlz.cn

Java: new Random().nextInt(100) + 1
来源：http://sim.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xfo.jqgfzy.top

Ruby: rand(1..100)
来源：http://foh.yangfankeji.com

C#:   new Random().Next(1, 101)
来源：http://ozi.hammf.cn

[A11] 条件表达式（三元）
来源：http://den.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://zdc.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nfr.jinqigfzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://nto.svipenyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oxc.jinqigufen.top

Java: x > 0 ? "yes" : "no"
来源：http://sjx.zdqjudy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dqg.52xcode.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qkt.daria6918.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zzf.cucudq.cn

[A12] 字符串插值 / 格式化
来源：http://xcm.uphjek.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yqc.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fsm.zhixingplan.top

JS:   `Hello, ${name}!`
来源：http://iqh.shangyingyoupin.top

TS:   `Hello, ${name}!`
来源：http://eoc.svipenyu.cn

Java: "Hello, %s!".formatted(name)
来源：http://uil.yj20258.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://otl.ctjpmb.com

Ruby: "Hello, #{name}!"
来源：http://fxs.hnqzz.top

C#:   $"Hello, {name}!"
来源：http://lha.bbcook.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rsc.fzhhl.top


<!-- 参考信息 -->