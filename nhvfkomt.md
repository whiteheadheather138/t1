代发 wailian999

[U79] PHP：静态分析
来源：http://pqd.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://hql.yfazqb.com

[U80] PHP：代码规范修复
来源：http://mok.shuidangran.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pie.yanxiufei.cn

[U81] JS：初始化项目
来源：http://hns.hysaishi.cn

npm init -y;  npm i express
来源：http://vcc.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://ejh.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rvu.havefunace.top

[U83] JS：ES Module 导入导出
来源：http://aih.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fcm.hnxiangtu.top

[U84] JS：CommonJS 写法
来源：http://dcg.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gtg.tanke756.top

[U85] JS：可选链
来源：http://fce.sxryk.cn

a?.b?.c
来源：http://qjk.shzxlz.cn

[U86] JS：空值合并
来源：http://wzk.cheryme.top

a ?? b
来源：http://ykc.zhongyouzk.top

[U87] JS：解构默认值
来源：http://gnf.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://opa.hcnkem.com

[U88] JS：对象展开合并
来源：http://ubl.xylfe.cn

{ ...a, ...b }
来源：http://lbn.tarul.cn

[U89] JS：数组去重
来源：http://ytc.0kj1m.cn

[...new Set(arr)]
来源：http://jwe.yj20258.top

[U90] JS：数字数组排序
来源：http://tzd.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://ytx.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://yxo.52xcode.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yxf.wangdashe.top

[U92] JS：深拷贝
来源：http://fbc.jinqigufen.top

structuredClone(obj)
来源：http://ufa.uphjek.com

[U93] JS：模板字符串
来源：http://jdz.xuetiantiany.cn

`共 ${n} 条`
来源：http://xwc.zhijiandao.cn

[U94] JS：箭头函数
来源：http://wyk.andypj.xyz

const double = x => x * 2;
来源：http://mme.ctjpmb.com

[U95] JS：Promise 包装
来源：http://kbt.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://hod.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://hcf.iojbl.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rjy.dashuyun.cn

[U97] JS：并发请求
来源：http://jhq.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dab.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://czj.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kej.shanyushiyangtech.top

[U99] JS：事件监听
来源：http://opt.bbcook.cn

el.addEventListener("click", e => {})
来源：http://uki.nanxuanxn.top

[U100] JS：DOM 查询
来源：http://jph.chenlongwang.top

document.querySelector(".item")
来源：http://mmy.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://qha.zhixingplan.top

el.classList.toggle("active")
来源：http://ltl.52xcode.cn

[U102] JS：本地存储
来源：http://sws.daxiang520.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://skc.ivvv.top

[U103] JS：定时器
来源：http://kfw.tian-w.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vnw.dianchejie.cn

[U104] JS：防抖
来源：http://qnt.chenjidiqi.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cmq.shanyushiyangtech.top

[U105] JS：节流
来源：http://htp.epnwcf.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qoj.nanxinkj.top

[U106] JS：日期格式化
来源：http://hrh.mhx1999.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://scj.svipenyu.cn

[U107] JS：数字千分位
来源：http://zla.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://grc.hammf.cn

[U108] JS：随机整数
来源：http://goj.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://boi.wangshuangyany.cn

[U109] JS：数组分组
来源：http://awx.52xcode.cn

Object.groupBy(arr, x => x.type)
来源：http://xca.ydzc1.top

[U110] JS：数组分块
来源：http://vjd.tian-w.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ysd.gogol.net.cn

[U111] JS：对象转 Map
来源：http://ulf.yueranfly.top

new Map(Object.entries(obj))
来源：http://hex.ehwqpu.com

[U112] JS：字符串补位
来源：http://mpo.hywenlv.cn

"7".padStart(3, "0")
来源：http://rhl.zhongyouzk.top

[U113] JS：正则替换全部
来源：http://doe.haohaochexian.top

s.replaceAll("a", "b")
来源：http://jne.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://mun.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bkb.guowangkeji.top

[U115] JS：生成 UUID
来源：http://gai.yj20258.top

crypto.randomUUID()
来源：http://seo.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://frx.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://whm.meibo888.top

[U117] JS：单元测试
来源：http://ihf.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://jtz.shuidangran.top

[U118] JS：开发服务器
来源：http://aan.hammf.cn

npm i -D vite;  npx vite
来源：http://dxc.tarul.cn

[U119] JS：生产构建
来源：http://xuk.mhx1999.top

npx vite build
来源：http://tiv.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://jiy.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://kye.haohaochexian.top

================================================================================
来源：http://mqh.hnxiangtu.top

统计汇总
来源：http://fci.chenlongwang.top

================================================================================
来源：http://zgq.hongshengwenyu.top

按语言统计（条）：
来源：http://ggq.cashguo.top

Python ......... 252
来源：http://npa.hnxiangtu.top

PHP ............ 252
来源：http://mio.gogol.net.cn

JavaScript ..... 252
来源：http://hdi.zhoulong.xyz

TypeScript ..... 212
来源：http://apc.hfpthk.cn

Java ........... 212
来源：http://rfu.hesvh.cn

Go ............. 212
来源：http://dng.52xcode.cn

Ruby ........... 212
来源：http://pww.andypj.xyz

C# ............. 212
来源：http://mei.tanke756.top

C .............. 30
来源：http://yzf.hesvh.cn

C++ ............ 30
来源：http://odo.snrcjt.cn

SQL ............ 90
来源：http://tzi.pycfn.com

Bash ........... 80
来源：http://fuc.yanxiufei.cn

Kotlin ......... 15
来源：http://yjc.sjlbkw.cn

Swift .......... 15
来源：http://hcq.sxryk.cn

Lua ............ 10
来源：http://pgd.vehdjk.com

Perl ........... 10
来源：http://vnq.xingfuxueyuan.xyz

Scala .......... 10
来源：http://kwc.sufxvd.cn

------------------------------------
来源：http://qyo.shangyingyoupin.top

合计 ........... 2106 条
来源：http://btn.vqdsnc.cn

按章节统计：
来源：http://ndu.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://llh.ydjk.org.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qew.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lww.yanxiufei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uol.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mko.pycfn.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mal.hnxiangtu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pdm.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uqf.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rzx.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xcr.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pbl.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ipe.birdmap.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vxw.ctjpmb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hbv.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://csu.hnqzz.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kxw.c1oappe.top

Q SQL 专题                              90
来源：http://ayp.jianghu66.top

R Bash 专题                             80
来源：http://tfq.hammf.cn

S C / C++ 专题                          60
来源：http://tmn.bbcook.cn

T 其他语言补充                          60
来源：http://szy.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://wdh.fehbvm.com

------------------------------------
来源：http://cme.wangshuangyany.cn

合计                                  2106 条
来源：http://eja.redwolf501.top

--------------------------------------------------------------------------------
来源：http://vqs.jyoumei.cn

使用提醒
来源：http://qix.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://uzh.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xip.redwolf501.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://swy.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ghf.wangdashe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://asb.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xob.zhengqikj.top

—— 文件结束 ——
来源：http://dqi.ywan-chungtsiang.top

================================================================================
来源：http://txr.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://rzj.xziqi.cn

Common Programming Examples Cheat Book
来源：http://jof.sysykeji.top

================================================================================
来源：http://eij.bbcook.cn

【收录内容】
来源：http://exa.ydzc1.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wzv.ybcxt.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nfa.sxryk.cn

SQL · Bash · C · C++
来源：http://ywl.ybcxt.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kct.shuidangran.top

【使用说明】
来源：http://dbl.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://drm.jinghuilouyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kcu.epnwcf.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://usv.zdbjq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rez.ehwqpu.com

Bash:  Shell         C:     C             C++:   C++
来源：http://bqh.yongpay.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fya.haohaochexian.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uis.hesvh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://klw.gzhubu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cvv.redwolf501.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zjp.jianghu66.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gem.nanxuanxn.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yyf.zhaomingkeji.xyz

【文件统计】
来源：http://erk.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tpk.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://rap.tarul.cn

目  录
来源：http://xqd.sysykeji.top

--------------------------------------------------------------------------------
来源：http://cov.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zms.vehdjk.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://swg.ehwqpu.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://est.hfpthk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ozl.yangfankeji.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xua.bbcook.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nzz.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mvy.sxryk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hdz.ydzc1.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qnv.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zof.shanyushiyangtech.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wec.haohaochexian.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gho.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://npe.xziqi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://paf.hywenlv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cja.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xgl.yfazqb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jmu.xingfuxueyuan.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://sjr.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tre.tarul.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lyq.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qwu.jianghu66.top

================================================================================
来源：http://hlm.meibo888.top

A. 基础语法与类型
来源：http://dks.xuanzx.com

================================================================================
来源：http://ufk.hnqzz.top

[A01] Hello World
来源：http://vcl.yueranfly.top

Py:   print("Hello, World!")
来源：http://iyg.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://mzb.yuanzhike.top

JS:   console.log("Hello, World!");
来源：http://kbv.nwbrower.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gpv.smart0.xyz

Java: System.out.println("Hello, World!");
来源：http://cju.hnqzz.top

Go:   fmt.Println("Hello, World!")
来源：http://siq.chenjidiqi.icu

Ruby: puts "Hello, World!"
来源：http://oha.kuanghao11.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://clw.316326.xyz

[A02] 变量声明与赋值
来源：http://eap.shanyushiyangkeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pil.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://nsa.yj202588.top

JS:   let name = "Alex"; const age = 20;
来源：http://upb.gzhubu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pam.zhoulong.xyz

Java: String name = "Alex"; int age = 20;
来源：http://sbu.fehbvm.com

Go:   name := "Alex"; age := 20
来源：http://yls.xingfuxueyuan.xyz

Ruby: name = "Alex"; age = 20
来源：http://cwy.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://xmy.xinyue.icu

[A03] 常量定义
来源：http://rbf.ydzc1.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://snz.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://kpz.wangshuangyany.cn

JS:   const PI = 3.14159;
来源：http://qpv.gzhubu.top

TS:   const PI: number = 3.14159;
来源：http://oht.hywenlv.cn

Java: static final double PI = 3.14159;
来源：http://mnn.guowangkeji.top

Go:   const PI = 3.14159
来源：http://irx.bjfxy.top

Ruby: PI = 3.14159
来源：http://nig.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://ner.ctjpmb.com

[A04] 判断变量类型
来源：http://aii.zhengqikj.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xcg.gaohongyu789.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nrc.ppjwa.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ohm.guannengcc.top

TS:   typeof x; x instanceof Date
来源：http://ylq.yuxming.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://anx.epnwcf.com

Go:   reflect.TypeOf(x).Name()
来源：http://btf.shangyingyoupin.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pho.gzhubu.top

C#:   x.GetType().Name; x is int
来源：http://aqk.guannengcc.top

[A05] 整数除法与取模
来源：http://fbf.ivvv.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vjh.hnxiangtu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vyp.kuanghao11.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yft.zdbjq.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pcv.zhaomingkeji.xyz

Java: 7 / 2; 7 % 2
来源：http://pqk.fzhhl.top

Go:   7 / 2; 7 % 2
来源：http://sjn.wangshuangyany.cn

Ruby: 7 / 2; 7 % 2
来源：http://yqf.ehwqpu.com

C#:   7 / 2; 7 % 2
来源：http://pgw.9152youxi.cn

[A06] 字符串转数字
来源：http://izk.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://phc.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tqq.vehdjk.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wyr.jianghu66.top

TS:   parseInt("42", 10); Number("42")
来源：http://kjt.daxiang520.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://azh.sjlbkw.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://meo.jinyuanbaomall.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://owl.fzhhl.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xhi.jqgfzy.top

[A07] 数字转字符串
来源：http://ijk.tian-w.cn

Py:   str(42)
来源：http://idf.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://bod.jlsjyb.cn

JS:   String(42); (42).toString()
来源：http://jhl.chenzaomai.com

TS:   String(42)
来源：http://fxq.gzhubu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jir.havefunace.top

Go:   strconv.Itoa(42)
来源：http://bwj.tianlin.xyz

Ruby: 42.to_s
来源：http://qsf.fehbvm.com

C#:   42.ToString()
来源：http://xkc.mhx1999.top

[A08] 取整与四舍五入
来源：http://bfp.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gjr.sxryk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hsh.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cae.wangdashe.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yzx.vqdsnc.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gtq.epnwcf.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rod.iojbl.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pmm.hnqzz.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fbf.yj202588.top

[A09] 绝对值与最大最小值
来源：http://vul.xuetiantiany.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rfd.jinqigfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lqo.chenzaomai.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://big.hongshengwenyu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aiw.hcnkem.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mjb.hysaishi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wvq.ppjwa.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pdd.havefunace.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sko.cheryme.top

[A10] 生成随机数
来源：http://fcp.chenjidiqi.icu

Py:   import random; random.randint(1, 100)
来源：http://yma.gaohongyu789.top

PHP:  random_int(1, 100);
来源：http://yqi.jinyuanbaomall.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kik.yj20258.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ilg.sxryk.cn

Java: new Random().nextInt(100) + 1
来源：http://xhk.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pln.iojbl.cn

Ruby: rand(1..100)
来源：http://gig.birdmap.top

C#:   new Random().Next(1, 101)
来源：http://uaa.tian-w.cn

[A11] 条件表达式（三元）
来源：http://aii.daria6918.cn

Py:   "yes" if x > 0 else "no"
来源：http://jut.daxiang520.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://xet.xinyue.icu

JS:   x > 0 ? "yes" : "no"
来源：http://jhe.gaohongyu789.top

TS:   x > 0 ? "yes" : "no"
来源：http://hms.kuanghao11.cn

Java: x > 0 ? "yes" : "no"
来源：http://kya.cheryme.top

Go:   // 无三元运算符，需用 if 语句
来源：http://wva.yonumen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ccj.ywan-chungtsiang.top

C#:   x > 0 ? "yes" : "no"
来源：http://trn.dianchejie.cn

[A12] 字符串插值 / 格式化
来源：http://bxi.fzhhl.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qpc.aizwys.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rlk.zdbjq.cn

JS:   `Hello, ${name}!`
来源：http://jnn.shangyingyoupin.top

TS:   `Hello, ${name}!`
来源：http://mhb.zdbjq.cn

Java: "Hello, %s!".formatted(name)
来源：http://koq.cqqwz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://efs.yfazqb.com

Ruby: "Hello, #{name}!"
来源：http://lns.dianchejie.cn

C#:   $"Hello, {name}!"
来源：http://xid.yuxming.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nnl.vehdjk.com


<!-- 参考信息 -->