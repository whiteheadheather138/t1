代发 wailian999

[U77] PHP：模板渲染
来源：http://yyc.ywan-chungtsiang.top

composer require twig/twig
来源：http://mkl.jinqigufen.top

[U78] PHP：单元测试
来源：http://siz.fehbvm.com

composer require --dev phpunit/phpunit
来源：http://snt.ctjpmb.com

[U79] PHP：静态分析
来源：http://xta.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://sqa.pengpengdd.cyou

[U80] PHP：代码规范修复
来源：http://uiq.epnwcf.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://klk.tian-w.cn

[U81] JS：初始化项目
来源：http://rnw.aizwys.cn

npm init -y;  npm i express
来源：http://agg.hfpthk.cn

[U82] JS：package.json 脚本
来源：http://qmw.haohaochexian.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kxg.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://mfd.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://lcl.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://gam.hcnkem.com

module.exports = { a };  const { a } = require("./m");
来源：http://ihf.havefunace.top

[U85] JS：可选链
来源：http://kyl.ivvv.top

a?.b?.c
来源：http://tir.zdqjudy.top

[U86] JS：空值合并
来源：http://pze.pengpengdd.cyou

a ?? b
来源：http://mju.xuanzx.com

[U87] JS：解构默认值
来源：http://phq.nanxuanxn.top

const { a = 1, b = 2 } = obj;
来源：http://bxb.svipenyu.cn

[U88] JS：对象展开合并
来源：http://vub.shanyushiyangtech.top

{ ...a, ...b }
来源：http://usg.sxryk.cn

[U89] JS：数组去重
来源：http://ebo.gotoacloud.top

[...new Set(arr)]
来源：http://jsz.c1oappe.top

[U90] JS：数字数组排序
来源：http://udx.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://ezs.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://zdz.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nwk.yvedp.cn

[U92] JS：深拷贝
来源：http://vov.xziqi.cn

structuredClone(obj)
来源：http://poc.chenjidiqi.icu

[U93] JS：模板字符串
来源：http://ugn.birdmap.top

`共 ${n} 条`
来源：http://hol.jqgfzy.top

[U94] JS：箭头函数
来源：http://feq.xuetiantiany.cn

const double = x => x * 2;
来源：http://cie.yuxming.cn

[U95] JS：Promise 包装
来源：http://yxg.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://ejd.fzhhl.top

[U96] JS：async/await 与异常
来源：http://eey.tian-w.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bxk.yueranfly.top

[U97] JS：并发请求
来源：http://gij.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fhg.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://kny.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://owj.0kj1m.cn

[U99] JS：事件监听
来源：http://zmi.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://ira.bjfxy.top

[U100] JS：DOM 查询
来源：http://jje.wangdashe.top

document.querySelector(".item")
来源：http://coh.jlsjyb.cn

[U101] JS：classList 操作
来源：http://nta.guowangkeji.top

el.classList.toggle("active")
来源：http://gxp.jqgfzy.top

[U102] JS：本地存储
来源：http://xtw.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ozp.fengsongda.top

[U103] JS：定时器
来源：http://oiq.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yha.vehdjk.com

[U104] JS：防抖
来源：http://yrm.uphjek.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yxv.nanxuanxn.top

[U105] JS：节流
来源：http://usp.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hra.guannengcc.top

[U106] JS：日期格式化
来源：http://cke.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zvp.gogol.net.cn

[U107] JS：数字千分位
来源：http://loz.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gul.cashguo.top

[U108] JS：随机整数
来源：http://rhr.svipenyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vxd.ydzc1.top

[U109] JS：数组分组
来源：http://wrx.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://olz.vqdsnc.cn

[U110] JS：数组分块
来源：http://oic.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tqq.fanxiaobao.xyz

[U111] JS：对象转 Map
来源：http://isp.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://adn.smart0.xyz

[U112] JS：字符串补位
来源：http://mow.aibaodan.cn

"7".padStart(3, "0")
来源：http://nam.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://zpw.sufxvd.cn

s.replaceAll("a", "b")
来源：http://dei.nanxuanxn.top

[U114] JS：JSON 深比较
来源：http://rdk.jyoumei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://keb.ehwqpu.com

[U115] JS：生成 UUID
来源：http://bnk.meibo888.top

crypto.randomUUID()
来源：http://dlr.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://twp.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://lzj.nanxuanxn.top

[U117] JS：单元测试
来源：http://nld.nwbrower.top

npm i -D vitest;  npx vitest
来源：http://wqh.nanxuanxn.top

[U118] JS：开发服务器
来源：http://yxp.ivvv.top

npm i -D vite;  npx vite
来源：http://tzj.hywenlv.cn

[U119] JS：生产构建
来源：http://jce.chenjidiqi.icu

npx vite build
来源：http://mmw.meibo888.top

[U120] JS：读取环境变量（Vite）
来源：http://hby.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://yxw.cashguo.top

================================================================================
来源：http://zpl.tanke756.top

统计汇总
来源：http://vkz.nanxuanxn.top

================================================================================
来源：http://jip.c1oappe.top

按语言统计（条）：
来源：http://fbg.sjlbkw.cn

Python ......... 252
来源：http://uym.iojbl.cn

PHP ............ 252
来源：http://wzy.feifeiyinyue.top

JavaScript ..... 252
来源：http://hxm.hywenlv.cn

TypeScript ..... 212
来源：http://pjt.yuanzhike.top

Java ........... 212
来源：http://guu.52xcode.cn

Go ............. 212
来源：http://nhu.aizwys.cn

Ruby ........... 212
来源：http://koy.yueranfly.top

C# ............. 212
来源：http://unu.guannengcc.top

C .............. 30
来源：http://kpj.ivvv.top

C++ ............ 30
来源：http://lxz.nanxuanxn.top

SQL ............ 90
来源：http://qjf.feifeiyinyue.top

Bash ........... 80
来源：http://uum.kuanghao11.cn

Kotlin ......... 15
来源：http://dex.yuanzhike.top

Swift .......... 15
来源：http://sbx.316326.xyz

Lua ............ 10
来源：http://ipd.mhx1999.top

Perl ........... 10
来源：http://dyo.jqgfzy.top

Scala .......... 10
来源：http://zvf.sysykeji.top

------------------------------------
来源：http://qvm.xylfe.cn

合计 ........... 2106 条
来源：http://dew.hnqzz.top

按章节统计：
来源：http://onb.52xcode.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nvh.fzhhl.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://scy.yvedp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iah.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pac.zhengqikj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wod.nanxinkj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hao.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pyb.ctjpmb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vnc.nanxuanxn.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://msp.tarul.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uvi.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://foj.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hst.sweek.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nlr.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tvk.hcnkem.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sac.yj202588.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bon.chenlongwang.top

Q SQL 专题                              90
来源：http://bjh.jqgfzy.top

R Bash 专题                             80
来源：http://ovw.feifeiyinyue.top

S C / C++ 专题                          60
来源：http://zgz.gzhubu.top

T 其他语言补充                          60
来源：http://yan.ivvv.top

U 高频实用片段                         120
来源：http://kdv.jqgfzy.top

------------------------------------
来源：http://sgm.ydzc1.top

合计                                  2106 条
来源：http://bph.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://unx.yj202588.top

使用提醒
来源：http://ytj.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://mtv.xingfuxueyuan.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mmx.sjlbkw.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iqx.jinqigufen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://saz.chenlongwang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://eeg.yonumen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eak.yj20258.top

—— 文件结束 ——
来源：http://rtp.wangdashe.top

================================================================================
来源：http://mur.gaohongyu789.top

程序语言常见例子速查手册（2024 版）
来源：http://eef.ppjwa.cn

Common Programming Examples Cheat Book
来源：http://fdm.kuanghao11.cn

================================================================================
来源：http://oxw.andypj.xyz

【收录内容】
来源：http://fcv.jinghuilouyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://riw.guannengcc.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tbw.jinyuanbaomall.cn

SQL · Bash · C · C++
来源：http://agv.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://urg.havefunace.top

【使用说明】
来源：http://vud.ppjwa.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mwq.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://btt.jinghuilouyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://snf.ppjwa.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ftf.ydjk.org.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jml.haohaochexian.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kse.cdnleiting.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://chx.quarkkingdee.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wjd.xinyue.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pev.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hfx.hnxiangtu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kts.fzhhl.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hdx.dashuyun.cn

【文件统计】
来源：http://ztq.iojbl.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xzq.iojbl.cn

--------------------------------------------------------------------------------
来源：http://fkn.jinqigufen.top

目  录
来源：http://hiv.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://uso.ivvv.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wqv.cheryme.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iuh.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sls.fktsv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kaj.shanyushiyangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://roc.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tll.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ped.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dul.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vrd.hcnkem.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://osi.hnqzz.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gyp.guowangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gyq.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hyw.xylfe.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hbj.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dji.dashuyun.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ksd.aizwys.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vsu.fanxiaobao.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://wwc.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xsh.jyoumei.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cly.sjlbkw.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lbc.ehwqpu.com

================================================================================
来源：http://rww.jinqigufen.top

A. 基础语法与类型
来源：http://sfy.sysykeji.top

================================================================================
来源：http://gbm.chenjidiqi.icu

[A01] Hello World
来源：http://imj.jinqigufen.top

Py:   print("Hello, World!")
来源：http://zde.yvedp.cn

PHP:  echo "Hello, World!";
来源：http://bir.316326.xyz

JS:   console.log("Hello, World!");
来源：http://bbj.fzhhl.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ukt.snrcjt.cn

Java: System.out.println("Hello, World!");
来源：http://ikr.pycfn.com

Go:   fmt.Println("Hello, World!")
来源：http://xxl.ydjk.org.cn

Ruby: puts "Hello, World!"
来源：http://aue.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://smy.yj20258.top

[A02] 变量声明与赋值
来源：http://fmn.zhixingplan.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://emz.zdbjq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lng.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xat.kuanghao11.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mvy.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://bzp.gzhubu.top

Go:   name := "Alex"; age := 20
来源：http://atw.birdmap.top

Ruby: name = "Alex"; age = 20
来源：http://sfg.jiagoushi.top

C#:   string name = "Alex"; int age = 20;
来源：http://aky.sjlbkw.cn

[A03] 常量定义
来源：http://dgs.guannengcc.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zex.jyoumei.cn

PHP:  const PI = 3.14159;
来源：http://kxh.vehdjk.com

JS:   const PI = 3.14159;
来源：http://vwx.gaohongyu789.top

TS:   const PI: number = 3.14159;
来源：http://ymz.jlsjyb.cn

Java: static final double PI = 3.14159;
来源：http://aol.aibaodan.cn

Go:   const PI = 3.14159
来源：http://trs.hysaishi.cn

Ruby: PI = 3.14159
来源：http://hjk.epnwcf.com

C#:   const double PI = 3.14159;
来源：http://gbg.guowangkeji.top

[A04] 判断变量类型
来源：http://pey.aibaodan.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://npu.fanxiaobao.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kfx.yj20258.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sxv.shzxlz.cn

TS:   typeof x; x instanceof Date
来源：http://uoe.zhijiandao.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kqe.hfpthk.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rbh.hammf.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://baj.shuidangran.top

C#:   x.GetType().Name; x is int
来源：http://zvx.redwolf501.top

[A05] 整数除法与取模
来源：http://ygd.fehbvm.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://krt.xuetiantiany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gir.redwolf501.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://whj.guowangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qka.xingfuxueyuan.xyz

Java: 7 / 2; 7 % 2
来源：http://qbd.ppjwa.cn

Go:   7 / 2; 7 % 2
来源：http://tom.c1oappe.top

Ruby: 7 / 2; 7 % 2
来源：http://waz.hnqzz.top

C#:   7 / 2; 7 % 2
来源：http://cfe.zhongyouzk.top

[A06] 字符串转数字
来源：http://guh.chenlongwang.top

Py:   int("42"); float("3.14")
来源：http://dxo.ehwqpu.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://myv.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uvc.xuanzx.com

TS:   parseInt("42", 10); Number("42")
来源：http://vho.sufxvd.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jel.chenzaomai.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://awx.ywan-chungtsiang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://csg.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mdh.sjlbkw.cn

[A07] 数字转字符串
来源：http://faz.sysykeji.top

Py:   str(42)
来源：http://avv.sweek.top

PHP:  (string) 42; strval(42)
来源：http://bbx.gogol.net.cn

JS:   String(42); (42).toString()
来源：http://kfj.jinyuanbaomall.cn

TS:   String(42)
来源：http://rbn.fzhhl.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tpv.hesvh.cn

Go:   strconv.Itoa(42)
来源：http://npp.aibaodan.cn

Ruby: 42.to_s
来源：http://ucq.epnwcf.com

C#:   42.ToString()
来源：http://ejc.shanyushiyangkeji.top

[A08] 取整与四舍五入
来源：http://mll.daria6918.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ael.hesvh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zeg.xziqi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mks.xylfe.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dfa.shuidangran.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ixb.feifeiyinyue.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oaj.ybcxt.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://uwy.dashuyun.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jsa.yfazqb.com

[A09] 绝对值与最大最小值
来源：http://rqq.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jve.tianlin.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dgb.hywenlv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mbk.yfazqb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hiq.shzxlz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vwv.zhaomingkeji.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://elo.birdmap.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://omn.daxiang520.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hzi.fehbvm.com

[A10] 生成随机数
来源：http://gla.xuanzx.com

Py:   import random; random.randint(1, 100)
来源：http://cod.jqgfzy.top

PHP:  random_int(1, 100);
来源：http://nmp.haohaochexian.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qcc.jqgufenzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lhe.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://tom.hfpthk.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://awl.zhoulong.xyz

Ruby: rand(1..100)
来源：http://wdw.shangyingyoupin.top

C#:   new Random().Next(1, 101)
来源：http://fzd.zhiwuduotai.top

[A11] 条件表达式（三元）
来源：http://ssh.chenlongwang.top

Py:   "yes" if x > 0 else "no"
来源：http://nup.ydjk.org.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ppb.ybcxt.top

JS:   x > 0 ? "yes" : "no"
来源：http://sbp.jinyuanbaomall.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mou.haohaochexian.top

Java: x > 0 ? "yes" : "no"
来源：http://set.gzhubu.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pfn.yj20258888.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gbf.jqgufenzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://ynh.yonumen.top

[A12] 字符串插值 / 格式化
来源：http://axk.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lyg.yueranfly.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jbo.hfpthk.cn

JS:   `Hello, ${name}!`
来源：http://ljx.wangshuangyany.cn

TS:   `Hello, ${name}!`
来源：http://xrx.yueranfly.top

Java: "Hello, %s!".formatted(name)
来源：http://vyv.fzhhl.top


<!-- 参考信息 -->