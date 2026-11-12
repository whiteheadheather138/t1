代发 wailian999

[U77] PHP：模板渲染
来源：http://hdj.yj202588.top

composer require twig/twig
来源：http://jdr.yueranfly.top

[U78] PHP：单元测试
来源：http://odu.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://kyz.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://uce.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://suw.tarul.cn

[U80] PHP：代码规范修复
来源：http://gvr.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://htp.sysykeji.top

[U81] JS：初始化项目
来源：http://cig.yongpay.top

npm init -y;  npm i express
来源：http://vzf.meibo888.top

[U82] JS：package.json 脚本
来源：http://cgp.jinyuanbaomall.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wcc.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://lty.chenjidiqi.icu

export const a = 1;  import { a } from "./m.js";
来源：http://rtk.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://pmp.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://him.gaohongyu789.top

[U85] JS：可选链
来源：http://lae.cucudq.cn

a?.b?.c
来源：http://mro.meibo888.top

[U86] JS：空值合并
来源：http://drx.cqqwz.cn

a ?? b
来源：http://bpy.fengsongda.top

[U87] JS：解构默认值
来源：http://rfh.cheryme.top

const { a = 1, b = 2 } = obj;
来源：http://eyo.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://bjt.wangdashe.top

{ ...a, ...b }
来源：http://ygz.pengpengdd.cyou

[U89] JS：数组去重
来源：http://oad.cdnleiting.top

[...new Set(arr)]
来源：http://oif.svipenyu.cn

[U90] JS：数字数组排序
来源：http://qmu.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://qjb.hnqzz.top

[U91] JS：对象键值遍历
来源：http://krq.aizwys.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mrv.sjlbkw.cn

[U92] JS：深拷贝
来源：http://dst.ppjwa.cn

structuredClone(obj)
来源：http://iii.zycfv.cn

[U93] JS：模板字符串
来源：http://wqo.shangyingyoupin.top

`共 ${n} 条`
来源：http://dcz.jqgufenzy.top

[U94] JS：箭头函数
来源：http://mtd.guowangkeji.top

const double = x => x * 2;
来源：http://cvj.feifeiyinyue.top

[U95] JS：Promise 包装
来源：http://moj.uphjek.com

new Promise((resolve, reject) => {})
来源：http://ade.xinyue.icu

[U96] JS：async/await 与异常
来源：http://ydd.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nzd.bjfxy.top

[U97] JS：并发请求
来源：http://rsz.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://cxg.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://kup.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xjy.pycfn.com

[U99] JS：事件监听
来源：http://jga.fehbvm.com

el.addEventListener("click", e => {})
来源：http://eul.tianlin.xyz

[U100] JS：DOM 查询
来源：http://bsf.quarkkingdee.top

document.querySelector(".item")
来源：http://xvb.hysaishi.cn

[U101] JS：classList 操作
来源：http://mcc.shuidangran.top

el.classList.toggle("active")
来源：http://gbm.yanxiufei.cn

[U102] JS：本地存储
来源：http://ixt.tian-w.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ael.yj202588.top

[U103] JS：定时器
来源：http://uop.zhaomingkeji.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cmb.tanke756.top

[U104] JS：防抖
来源：http://xdv.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://maf.shuidangran.top

[U105] JS：节流
来源：http://rds.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gmy.shzxlz.cn

[U106] JS：日期格式化
来源：http://xwz.52xcode.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tgz.hnqzz.top

[U107] JS：数字千分位
来源：http://rlq.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://txb.hfpthk.cn

[U108] JS：随机整数
来源：http://enn.dianchejie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xsg.zhixingplan.top

[U109] JS：数组分组
来源：http://rmq.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://vwf.quarkkingdee.top

[U110] JS：数组分块
来源：http://ahm.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lyj.tianlin.xyz

[U111] JS：对象转 Map
来源：http://tde.ybcxt.top

new Map(Object.entries(obj))
来源：http://mqy.jinyuanbaomall.cn

[U112] JS：字符串补位
来源：http://cmg.xylfe.cn

"7".padStart(3, "0")
来源：http://nng.hesvh.cn

[U113] JS：正则替换全部
来源：http://zuz.hammf.cn

s.replaceAll("a", "b")
来源：http://smz.fzhhl.top

[U114] JS：JSON 深比较
来源：http://fnz.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kzi.guowangkeji.top

[U115] JS：生成 UUID
来源：http://kpd.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://mzi.shanyushiyangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://rpr.xinyue.icu

/** @param {string} name */ function f(name) {}
来源：http://qig.hysaishi.cn

[U117] JS：单元测试
来源：http://dsm.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://jlf.jqgufenzy.top

[U118] JS：开发服务器
来源：http://pgl.iojbl.cn

npm i -D vite;  npx vite
来源：http://dfa.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://hlc.gotoacloud.top

npx vite build
来源：http://mxi.bjfxy.top

[U120] JS：读取环境变量（Vite）
来源：http://sip.iojbl.cn

import.meta.env.VITE_API_URL
来源：http://ytv.shuidangran.top

================================================================================
来源：http://iit.xziqi.cn

统计汇总
来源：http://qsc.bjfxy.top

================================================================================
来源：http://pbh.xylfe.cn

按语言统计（条）：
来源：http://vse.zdqjudy.top

Python ......... 252
来源：http://eac.jlsjyb.cn

PHP ............ 252
来源：http://frs.bjfxy.top

JavaScript ..... 252
来源：http://sij.fzhhl.top

TypeScript ..... 212
来源：http://ugh.zhaomingkeji.xyz

Java ........... 212
来源：http://ekw.hongshengwenyu.top

Go ............. 212
来源：http://ggl.gaohongyu789.top

Ruby ........... 212
来源：http://lgm.ydzc1.top

C# ............. 212
来源：http://qsp.kuanghao11.cn

C .............. 30
来源：http://zdd.andypj.xyz

C++ ............ 30
来源：http://ecl.yj20258888.top

SQL ............ 90
来源：http://rsl.xuetiantiany.cn

Bash ........... 80
来源：http://tqp.tianlin.xyz

Kotlin ......... 15
来源：http://ybo.zycfv.cn

Swift .......... 15
来源：http://akf.smart0.xyz

Lua ............ 10
来源：http://ejc.aizwys.cn

Perl ........... 10
来源：http://fjv.fanxiaobao.xyz

Scala .......... 10
来源：http://iik.yonumen.top

------------------------------------
来源：http://uux.9152youxi.cn

合计 ........... 2106 条
来源：http://erw.yj20258888.top

按章节统计：
来源：http://ekw.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hoq.andypj.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rac.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rbo.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yeb.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oqt.xuanzx.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jyf.nwbrower.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fwr.yuxming.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pmo.zycfv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xuz.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yux.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://drq.zhijiandao.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fut.pengpengdd.cyou

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://elv.yfazqb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ubr.52xcode.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cvb.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://huq.cucudq.cn

Q SQL 专题                              90
来源：http://pfu.316326.xyz

R Bash 专题                             80
来源：http://ubb.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://oud.ydjk.org.cn

T 其他语言补充                          60
来源：http://opd.ehwqpu.com

U 高频实用片段                         120
来源：http://jyw.xylfe.cn

------------------------------------
来源：http://dkp.gaohongyu789.top

合计                                  2106 条
来源：http://tkk.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://wuw.jqgfzy.top

使用提醒
来源：http://iea.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://mho.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nex.jinghuilouyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fju.yongpay.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mal.zdqjudy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://shz.cashguo.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vak.nanxuanxn.top

—— 文件结束 ——
来源：http://syb.hnxiangtu.top

================================================================================
来源：http://cmn.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://olt.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://vks.yfazqb.com

================================================================================
来源：http://xqx.jyoumei.cn

【收录内容】
来源：http://wud.cucudq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hob.uphjek.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vqy.epnwcf.com

SQL · Bash · C · C++
来源：http://kly.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fcj.xingfuxueyuan.xyz

【使用说明】
来源：http://umq.aibaodan.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://own.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jnn.aizwys.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nvi.9152youxi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xor.9152youxi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lyv.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://geb.yj202588.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fqn.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iqb.52xcode.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://skr.ydjk.org.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oxf.yj202588.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dgj.zhiwuduotai.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vln.zdqjudy.top

【文件统计】
来源：http://wfb.ppjwa.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cah.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://txd.ydzc1.top

目  录
来源：http://dte.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://fpo.andypj.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jtz.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sys.yfazqb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ooz.yvedp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qky.yonumen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uoe.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sue.mhx1999.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://txf.gaohongyu789.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xan.xuanzx.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lfn.dianchejie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mgv.pengpengdd.cyou

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ete.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cdu.yj20258.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qjd.hcnkem.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wyo.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zlc.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vqs.0kj1m.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rxl.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://inc.gotoacloud.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://umb.wangdashe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://izs.snrcjt.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tcs.xinyue.icu

================================================================================
来源：http://nxd.meibo888.top

A. 基础语法与类型
来源：http://dvx.daxiang520.top

================================================================================
来源：http://jsh.uphjek.com

[A01] Hello World
来源：http://uua.havefunace.top

Py:   print("Hello, World!")
来源：http://aze.yangfankeji.com

PHP:  echo "Hello, World!";
来源：http://ubh.bjfxy.top

JS:   console.log("Hello, World!");
来源：http://zik.nanxuanxn.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pgb.snrcjt.cn

Java: System.out.println("Hello, World!");
来源：http://oxu.zhijiandao.cn

Go:   fmt.Println("Hello, World!")
来源：http://ccy.xingfuxueyuan.xyz

Ruby: puts "Hello, World!"
来源：http://pui.zhoulong.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://cbv.chenlongwang.top

[A02] 变量声明与赋值
来源：http://oui.sweek.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wkd.vqdsnc.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wvi.c1oappe.top

JS:   let name = "Alex"; const age = 20;
来源：http://ion.bjfxy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yoa.sjlbkw.cn

Java: String name = "Alex"; int age = 20;
来源：http://gka.zdbjq.cn

Go:   name := "Alex"; age := 20
来源：http://qhp.fzhhl.top

Ruby: name = "Alex"; age = 20
来源：http://bpk.tianlin.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://xur.iojbl.cn

[A03] 常量定义
来源：http://jvt.zhijiandao.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mbg.zhixingplan.top

PHP:  const PI = 3.14159;
来源：http://exp.shanyushiyangkeji.top

JS:   const PI = 3.14159;
来源：http://pzc.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://rgl.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://mhs.jqgufenzy.top

Go:   const PI = 3.14159
来源：http://cxl.vehdjk.com

Ruby: PI = 3.14159
来源：http://tea.ydjk.org.cn

C#:   const double PI = 3.14159;
来源：http://ecm.ppjwa.cn

[A04] 判断变量类型
来源：http://wbe.havefunace.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://kin.sxryk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tfj.zhaomingkeji.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fpm.zhixingplan.top

TS:   typeof x; x instanceof Date
来源：http://hcn.meibo888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://btw.jlsjyb.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fnl.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mdv.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://ouz.daxiang520.top

[A05] 整数除法与取模
来源：http://tnd.zhiwuduotai.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mba.jinqigufen.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://opa.yonumen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ogo.hnxiangtu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mpd.cheryme.top

Java: 7 / 2; 7 % 2
来源：http://ukh.ydzc1.top

Go:   7 / 2; 7 % 2
来源：http://cim.fktsv.cn

Ruby: 7 / 2; 7 % 2
来源：http://fis.jlsjyb.cn

C#:   7 / 2; 7 % 2
来源：http://sff.52xcode.cn

[A06] 字符串转数字
来源：http://zdp.ehwqpu.com

Py:   int("42"); float("3.14")
来源：http://bzg.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ppn.yongpay.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jdo.xuetiantiany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ykm.andypj.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://omd.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oiv.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://dnh.xinyue.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dma.cheryme.top

[A07] 数字转字符串
来源：http://npe.tanke756.top

Py:   str(42)
来源：http://ngz.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://wcb.zdbjq.cn

JS:   String(42); (42).toString()
来源：http://vkb.sjlbkw.cn

TS:   String(42)
来源：http://bgh.jqgfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zlx.tanke756.top

Go:   strconv.Itoa(42)
来源：http://qek.jyoumei.cn

Ruby: 42.to_s
来源：http://hpz.xziqi.cn

C#:   42.ToString()
来源：http://udy.feifeiyinyue.top

[A08] 取整与四舍五入
来源：http://ipd.cdnleiting.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kun.zhaomingkeji.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jpp.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ndh.xuetiantiany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cww.nanxuanxn.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ypw.shanyushiyangkeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ddo.hfpthk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ghu.haohaochexian.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kmx.gogol.net.cn

[A09] 绝对值与最大最小值
来源：http://vop.havefunace.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zyw.smart0.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qkk.9152youxi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://byg.tarul.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wrv.daxiang520.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tkz.yvedp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hnn.tianlin.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wau.sweek.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://min.316326.xyz

[A10] 生成随机数
来源：http://gjv.daria6918.cn

Py:   import random; random.randint(1, 100)
来源：http://qby.tian-w.cn

PHP:  random_int(1, 100);
来源：http://shq.zycfv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ahw.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xho.fzhhl.top

Java: new Random().nextInt(100) + 1
来源：http://vta.zycfv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ewx.iojbl.cn

Ruby: rand(1..100)
来源：http://ggx.zhiwuduotai.top

C#:   new Random().Next(1, 101)
来源：http://khg.svipenyu.cn

[A11] 条件表达式（三元）
来源：http://rpr.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://ynv.tanke756.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://uhv.yvedp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pyp.meibo888.top

TS:   x > 0 ? "yes" : "no"
来源：http://dub.fengsongda.top

Java: x > 0 ? "yes" : "no"
来源：http://mry.hnqzz.top

Go:   // 无三元运算符，需用 if 语句
来源：http://zdv.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://csy.sxryk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fji.dashuyun.cn

[A12] 字符串插值 / 格式化
来源：http://fqd.0kj1m.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wzg.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://azb.yuanzhike.top

JS:   `Hello, ${name}!`
来源：http://oyj.quarkkingdee.top

TS:   `Hello, ${name}!`
来源：http://nsn.wangshuangyany.cn

Java: "Hello, %s!".formatted(name)
来源：http://hbi.redwolf501.top


<!-- 参考信息 -->