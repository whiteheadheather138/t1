代发 wailian999

[U75] PHP：依赖注入
来源：http://abh.tanke756.top

composer require psr/container
来源：http://yyr.pycfn.com

[U76] PHP：简单路由
来源：http://rad.ywan-chungtsiang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fwz.sxryk.cn

[U77] PHP：模板渲染
来源：http://vte.shanyushiyangtech.top

composer require twig/twig
来源：http://xpi.guannengcc.top

[U78] PHP：单元测试
来源：http://rbd.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://hxj.xylfe.cn

[U79] PHP：静态分析
来源：http://hvz.yfazqb.com

composer require --dev phpstan/phpstan
来源：http://urv.redwolf501.top

[U80] PHP：代码规范修复
来源：http://lqb.tarul.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qoj.dashuyun.cn

[U81] JS：初始化项目
来源：http://nbx.ydzc1.top

npm init -y;  npm i express
来源：http://asl.jinqigfzy.top

[U82] JS：package.json 脚本
来源：http://ieq.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lrc.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://oct.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://bdm.shuidangran.top

[U84] JS：CommonJS 写法
来源：http://jte.xingfuxueyuan.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://blz.hongshengwenyu.top

[U85] JS：可选链
来源：http://pqv.jianghu66.top

a?.b?.c
来源：http://hgz.jinyuanbaomall.cn

[U86] JS：空值合并
来源：http://wfl.birdmap.top

a ?? b
来源：http://itz.sxryk.cn

[U87] JS：解构默认值
来源：http://kpl.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://evn.xuanzx.com

[U88] JS：对象展开合并
来源：http://fai.ppjwa.cn

{ ...a, ...b }
来源：http://yib.xinyue.icu

[U89] JS：数组去重
来源：http://xaj.zhengqikj.top

[...new Set(arr)]
来源：http://tyr.quarkkingdee.top

[U90] JS：数字数组排序
来源：http://usa.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://lyf.zhaomingkeji.xyz

[U91] JS：对象键值遍历
来源：http://jzb.tanke756.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hvc.xylfe.cn

[U92] JS：深拷贝
来源：http://jjd.shanyushiyangkeji.top

structuredClone(obj)
来源：http://uns.0kj1m.cn

[U93] JS：模板字符串
来源：http://jxc.smart0.xyz

`共 ${n} 条`
来源：http://ons.wangdashe.top

[U94] JS：箭头函数
来源：http://bod.uphjek.com

const double = x => x * 2;
来源：http://kct.zycfv.cn

[U95] JS：Promise 包装
来源：http://odp.jqgfzy.top

new Promise((resolve, reject) => {})
来源：http://dnq.nanxinkj.top

[U96] JS：async/await 与异常
来源：http://btq.hammf.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jgi.xziqi.cn

[U97] JS：并发请求
来源：http://dys.fzhhl.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pia.jiagoushi.top

[U98] JS：fetch 带 JSON
来源：http://sik.birdmap.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ttb.hnxiangtu.top

[U99] JS：事件监听
来源：http://syj.zycfv.cn

el.addEventListener("click", e => {})
来源：http://kku.mhx1999.top

[U100] JS：DOM 查询
来源：http://ovs.chenlongwang.top

document.querySelector(".item")
来源：http://syh.xziqi.cn

[U101] JS：classList 操作
来源：http://eom.jianghu66.top

el.classList.toggle("active")
来源：http://qcs.yangfankeji.com

[U102] JS：本地存储
来源：http://fso.iojbl.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gbe.aibaodan.cn

[U103] JS：定时器
来源：http://yqt.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qvj.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://bkd.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cyp.c1oappe.top

[U105] JS：节流
来源：http://tis.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://srg.yanxiufei.cn

[U106] JS：日期格式化
来源：http://veo.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pxx.ivvv.top

[U107] JS：数字千分位
来源：http://krq.sweek.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://usz.feifeiyinyue.top

[U108] JS：随机整数
来源：http://vlq.zdqjudy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ycr.vqdsnc.cn

[U109] JS：数组分组
来源：http://xgo.snrcjt.cn

Object.groupBy(arr, x => x.type)
来源：http://ppd.sjlbkw.cn

[U110] JS：数组分块
来源：http://nbe.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uvi.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://lzu.fehbvm.com

new Map(Object.entries(obj))
来源：http://xes.epnwcf.com

[U112] JS：字符串补位
来源：http://kpd.vehdjk.com

"7".padStart(3, "0")
来源：http://xhb.cashguo.top

[U113] JS：正则替换全部
来源：http://bxn.ydzc1.top

s.replaceAll("a", "b")
来源：http://csr.guannengcc.top

[U114] JS：JSON 深比较
来源：http://iyu.wangshuangyany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cor.aizwys.cn

[U115] JS：生成 UUID
来源：http://wps.jinqigufen.top

crypto.randomUUID()
来源：http://pnl.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://qql.jqgfzy.top

/** @param {string} name */ function f(name) {}
来源：http://jrm.hcnkem.com

[U117] JS：单元测试
来源：http://gjv.kuanghao11.cn

npm i -D vitest;  npx vitest
来源：http://ros.dashuyun.cn

[U118] JS：开发服务器
来源：http://jiu.meibo888.top

npm i -D vite;  npx vite
来源：http://xvu.zhiwuduotai.top

[U119] JS：生产构建
来源：http://pab.yongpay.top

npx vite build
来源：http://ckn.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://zyg.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://dbv.xuetiantiany.cn

================================================================================
来源：http://sny.gaohongyu789.top

统计汇总
来源：http://hvg.iojbl.cn

================================================================================
来源：http://zkf.zdqjudy.top

按语言统计（条）：
来源：http://sqk.ydzc1.top

Python ......... 252
来源：http://ymj.pengpengdd.cyou

PHP ............ 252
来源：http://tec.chenlongwang.top

JavaScript ..... 252
来源：http://fjt.zhaomingkeji.xyz

TypeScript ..... 212
来源：http://umk.jqgfzy.top

Java ........... 212
来源：http://uhr.tianlin.xyz

Go ............. 212
来源：http://kpi.ydjk.org.cn

Ruby ........... 212
来源：http://jjz.aizwys.cn

C# ............. 212
来源：http://cvr.smart0.xyz

C .............. 30
来源：http://qjn.shanyushiyangkeji.top

C++ ............ 30
来源：http://uzq.hammf.cn

SQL ............ 90
来源：http://nac.yj20258.top

Bash ........... 80
来源：http://ord.meibo888.top

Kotlin ......... 15
来源：http://znq.jiagoushi.top

Swift .......... 15
来源：http://yoh.xinyue.icu

Lua ............ 10
来源：http://xxb.mhx1999.top

Perl ........... 10
来源：http://ztf.0kj1m.cn

Scala .......... 10
来源：http://iin.bjfxy.top

------------------------------------
来源：http://eyq.yonumen.top

合计 ........... 2106 条
来源：http://obs.bbcook.cn

按章节统计：
来源：http://txl.sweek.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pzt.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yhu.316326.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hbv.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vnm.bjfxy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vbe.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uuf.sysykeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://odt.yuxming.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://apy.wangshuangyany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aep.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jbc.jiagoushi.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mff.zhijiandao.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vta.ydjk.org.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tpi.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xvd.hfpthk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://thj.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hxg.cucudq.cn

Q SQL 专题                              90
来源：http://avh.tian-w.cn

R Bash 专题                             80
来源：http://soj.shanyushiyangkeji.top

S C / C++ 专题                          60
来源：http://fva.feifeiyinyue.top

T 其他语言补充                          60
来源：http://xgf.zhijiandao.cn

U 高频实用片段                         120
来源：http://hhv.snrcjt.cn

------------------------------------
来源：http://ukt.52xcode.cn

合计                                  2106 条
来源：http://dbr.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://ioq.gogol.net.cn

使用提醒
来源：http://ypj.jianghu66.top

--------------------------------------------------------------------------------
来源：http://fpf.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://awl.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://edh.andypj.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iuk.yj202588.top

在旧版本上使用前请先确认语法支持情况。
来源：http://uoj.quarkkingdee.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eva.guannengcc.top

—— 文件结束 ——
来源：http://qov.shangyingyoupin.top

================================================================================
来源：http://wme.yvedp.cn

程序语言常见例子速查手册（2024 版）
来源：http://xiy.xuanzx.com

Common Programming Examples Cheat Book
来源：http://hju.daxiang520.top

================================================================================
来源：http://esu.zhengqikj.top

【收录内容】
来源：http://uyx.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zar.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dbj.gogol.net.cn

SQL · Bash · C · C++
来源：http://dqg.zycfv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gso.shanyushiyangtech.top

【使用说明】
来源：http://ady.shanyushiyangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bws.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dus.jinghuilouyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hme.zdqjudy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lnf.hysaishi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jta.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dqc.dashuyun.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eyd.shzxlz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ivm.dianchejie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lwq.yueranfly.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ezh.jlsjyb.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nnd.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://utm.ivvv.top

【文件统计】
来源：http://cgm.zhoulong.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ybi.redwolf501.top

--------------------------------------------------------------------------------
来源：http://jpu.meibo888.top

目  录
来源：http://gss.sweek.top

--------------------------------------------------------------------------------
来源：http://lym.sysykeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qcs.hnxiangtu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eqb.dashuyun.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pwl.nwbrower.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uxh.hnqzz.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iah.jlsjyb.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xfh.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uss.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sxq.hcnkem.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ovs.nanxuanxn.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dny.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qrr.ctjpmb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jix.nanxinkj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nta.hcnkem.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vxi.ydjk.org.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://req.ehwqpu.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hhy.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gxz.chenjidiqi.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://dnh.jqgufenzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hgq.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nlc.daxiang520.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eea.jinqigfzy.top

================================================================================
来源：http://fzs.zhixingplan.top

A. 基础语法与类型
来源：http://hcj.hongshengwenyu.top

================================================================================
来源：http://hka.hywenlv.cn

[A01] Hello World
来源：http://bbj.aibaodan.cn

Py:   print("Hello, World!")
来源：http://bgf.0kj1m.cn

PHP:  echo "Hello, World!";
来源：http://umc.svipenyu.cn

JS:   console.log("Hello, World!");
来源：http://acu.jlsjyb.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://akp.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://hqp.zhongyouzk.top

Go:   fmt.Println("Hello, World!")
来源：http://zyu.jqgfzy.top

Ruby: puts "Hello, World!"
来源：http://hws.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://dav.cheryme.top

[A02] 变量声明与赋值
来源：http://tvb.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vcd.pengpengdd.cyou

PHP:  $name = "Alex"; $age = 20;
来源：http://xrz.zycfv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jai.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fdw.hongshengwenyu.top

Java: String name = "Alex"; int age = 20;
来源：http://qcp.kuanghao11.cn

Go:   name := "Alex"; age := 20
来源：http://yxl.jinqigufen.top

Ruby: name = "Alex"; age = 20
来源：http://vgl.quarkkingdee.top

C#:   string name = "Alex"; int age = 20;
来源：http://rvb.svipenyu.cn

[A03] 常量定义
来源：http://tbc.yj20258.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ohp.xinyue.icu

PHP:  const PI = 3.14159;
来源：http://ojv.smart0.xyz

JS:   const PI = 3.14159;
来源：http://sip.shuidangran.top

TS:   const PI: number = 3.14159;
来源：http://kly.ehwqpu.com

Java: static final double PI = 3.14159;
来源：http://udo.hnxiangtu.top

Go:   const PI = 3.14159
来源：http://ftn.hammf.cn

Ruby: PI = 3.14159
来源：http://tpq.svipenyu.cn

C#:   const double PI = 3.14159;
来源：http://yol.chenjidiqi.icu

[A04] 判断变量类型
来源：http://uus.sufxvd.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rtv.epnwcf.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zfb.pycfn.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://laj.dashuyun.cn

TS:   typeof x; x instanceof Date
来源：http://era.fzhhl.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mlh.aibaodan.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dkk.aizwys.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wou.yangfankeji.com

C#:   x.GetType().Name; x is int
来源：http://ugm.cheryme.top

[A05] 整数除法与取模
来源：http://lsz.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tqy.vqdsnc.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kax.shzxlz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ueh.tian-w.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fqj.yongpay.top

Java: 7 / 2; 7 % 2
来源：http://evo.tarul.cn

Go:   7 / 2; 7 % 2
来源：http://mso.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://xgl.jyoumei.cn

C#:   7 / 2; 7 % 2
来源：http://mgd.jinqigfzy.top

[A06] 字符串转数字
来源：http://qyy.ppjwa.cn

Py:   int("42"); float("3.14")
来源：http://mtv.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pgd.ybcxt.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hhl.yongpay.top

TS:   parseInt("42", 10); Number("42")
来源：http://nya.zhaomingkeji.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rhp.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ltg.ivvv.top

Ruby: "42".to_i; "3.14".to_f
来源：http://sph.wangshuangyany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uyy.yangfankeji.com

[A07] 数字转字符串
来源：http://ykw.tarul.cn

Py:   str(42)
来源：http://dwn.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://okw.kuanghao11.cn

JS:   String(42); (42).toString()
来源：http://pcg.hesvh.cn

TS:   String(42)
来源：http://luj.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ezv.zhijiandao.cn

Go:   strconv.Itoa(42)
来源：http://lax.cqqwz.cn

Ruby: 42.to_s
来源：http://jel.bjfxy.top

C#:   42.ToString()
来源：http://sda.feifeiyinyue.top

[A08] 取整与四舍五入
来源：http://nkh.ydzc1.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uqp.chenjidiqi.icu

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sqq.guannengcc.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hip.yuanzhike.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cib.gaohongyu789.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://czf.havefunace.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zqw.tianlin.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://tnu.jlsjyb.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ndr.yj20258.top

[A09] 绝对值与最大最小值
来源：http://scr.tianlin.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sau.yj202588.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rzz.zhongyouzk.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mpf.xinyue.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tmu.jlsjyb.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tkz.bbcook.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xmm.chenzaomai.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pkd.cashguo.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://moe.sjlbkw.cn

[A10] 生成随机数
来源：http://dcw.feifeiyinyue.top

Py:   import random; random.randint(1, 100)
来源：http://fiu.uphjek.com

PHP:  random_int(1, 100);
来源：http://wbs.hysaishi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dnn.chenlongwang.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tgd.hywenlv.cn

Java: new Random().nextInt(100) + 1
来源：http://mwb.ydzc1.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bdh.hammf.cn

Ruby: rand(1..100)
来源：http://qci.nanxuanxn.top

C#:   new Random().Next(1, 101)
来源：http://grv.ydzc1.top

[A11] 条件表达式（三元）
来源：http://vbo.svipenyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://lkn.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lny.gzhubu.top

JS:   x > 0 ? "yes" : "no"
来源：http://cuw.xinyue.icu

TS:   x > 0 ? "yes" : "no"
来源：http://rqv.ywan-chungtsiang.top

Java: x > 0 ? "yes" : "no"
来源：http://ycg.gzhubu.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hnu.yonumen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://zed.mhx1999.top

C#:   x > 0 ? "yes" : "no"
来源：http://tpn.uphjek.com

[A12] 字符串插值 / 格式化
来源：http://wiq.dashuyun.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fko.tian-w.cn


<!-- 参考信息 -->