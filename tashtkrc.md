代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://lhu.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://jge.cdnleiting.top

[U74] PHP：读取环境变量
来源：http://ymd.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://hhe.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://fqd.yonumen.top

composer require psr/container
来源：http://xkd.chenlongwang.top

[U76] PHP：简单路由
来源：http://usa.ybcxt.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wqc.guowangkeji.top

[U77] PHP：模板渲染
来源：http://ohy.yonumen.top

composer require twig/twig
来源：http://reb.aizwys.cn

[U78] PHP：单元测试
来源：http://awh.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://psx.xuetiantiany.cn

[U79] PHP：静态分析
来源：http://dvw.yuxming.cn

composer require --dev phpstan/phpstan
来源：http://spe.fzhhl.top

[U80] PHP：代码规范修复
来源：http://uug.jyoumei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://chw.0kj1m.cn

[U81] JS：初始化项目
来源：http://euy.jinqigufen.top

npm init -y;  npm i express
来源：http://kki.birdmap.top

[U82] JS：package.json 脚本
来源：http://rkt.cheryme.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pgn.iojbl.cn

[U83] JS：ES Module 导入导出
来源：http://zhl.nanxinkj.top

export const a = 1;  import { a } from "./m.js";
来源：http://kax.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://adq.sjlbkw.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pcy.wangshuangyany.cn

[U85] JS：可选链
来源：http://cqj.ybcxt.top

a?.b?.c
来源：http://afa.hnxiangtu.top

[U86] JS：空值合并
来源：http://sna.dianchejie.cn

a ?? b
来源：http://ikr.nanxinkj.top

[U87] JS：解构默认值
来源：http://soi.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://lvy.gogol.net.cn

[U88] JS：对象展开合并
来源：http://ppx.yonumen.top

{ ...a, ...b }
来源：http://xnd.yongpay.top

[U89] JS：数组去重
来源：http://kti.shuidangran.top

[...new Set(arr)]
来源：http://bln.chenlongwang.top

[U90] JS：数字数组排序
来源：http://zpf.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://dgs.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://svd.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wyv.yangfankeji.com

[U92] JS：深拷贝
来源：http://mmp.dianchejie.cn

structuredClone(obj)
来源：http://dqn.hfpthk.cn

[U93] JS：模板字符串
来源：http://kzi.sweek.top

`共 ${n} 条`
来源：http://vsp.fehbvm.com

[U94] JS：箭头函数
来源：http://pug.yonumen.top

const double = x => x * 2;
来源：http://qfx.ppjwa.cn

[U95] JS：Promise 包装
来源：http://bhh.hammf.cn

new Promise((resolve, reject) => {})
来源：http://fkz.sufxvd.cn

[U96] JS：async/await 与异常
来源：http://shj.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pck.redwolf501.top

[U97] JS：并发请求
来源：http://gwt.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vof.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://jiw.chenzaomai.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xel.jinyuanbaomall.cn

[U99] JS：事件监听
来源：http://hxt.hcnkem.com

el.addEventListener("click", e => {})
来源：http://idj.fengsongda.top

[U100] JS：DOM 查询
来源：http://tjx.gogol.net.cn

document.querySelector(".item")
来源：http://zmj.redwolf501.top

[U101] JS：classList 操作
来源：http://vfb.sweek.top

el.classList.toggle("active")
来源：http://hpk.jqgufenzy.top

[U102] JS：本地存储
来源：http://xke.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uwa.sweek.top

[U103] JS：定时器
来源：http://uhx.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ihh.fengsongda.top

[U104] JS：防抖
来源：http://zjl.zdbjq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://seg.c1oappe.top

[U105] JS：节流
来源：http://jdz.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ydd.jinqigufen.top

[U106] JS：日期格式化
来源：http://dbo.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tmk.aizwys.cn

[U107] JS：数字千分位
来源：http://cjr.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tjb.gaohongyu789.top

[U108] JS：随机整数
来源：http://ess.jinqigufen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://owc.bjfxy.top

[U109] JS：数组分组
来源：http://hlu.cdnleiting.top

Object.groupBy(arr, x => x.type)
来源：http://iwf.jinqigfzy.top

[U110] JS：数组分块
来源：http://umh.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qyo.tanke756.top

[U111] JS：对象转 Map
来源：http://mpg.shanyushiyangtech.top

new Map(Object.entries(obj))
来源：http://hsf.guowangkeji.top

[U112] JS：字符串补位
来源：http://clj.0kj1m.cn

"7".padStart(3, "0")
来源：http://agp.guannengcc.top

[U113] JS：正则替换全部
来源：http://nbh.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://sdd.gogol.net.cn

[U114] JS：JSON 深比较
来源：http://pdf.fzhhl.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bqm.yj20258888.top

[U115] JS：生成 UUID
来源：http://qvt.andypj.xyz

crypto.randomUUID()
来源：http://ptu.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://zil.tarul.cn

/** @param {string} name */ function f(name) {}
来源：http://ohz.tanke756.top

[U117] JS：单元测试
来源：http://afk.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://mgz.ydzc1.top

[U118] JS：开发服务器
来源：http://cqx.zhiwuduotai.top

npm i -D vite;  npx vite
来源：http://hnz.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://esy.feifeiyinyue.top

npx vite build
来源：http://rjf.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://mam.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://qfi.aibaodan.cn

================================================================================
来源：http://fys.ydzc1.top

统计汇总
来源：http://pjr.zhoulong.xyz

================================================================================
来源：http://tji.mhx1999.top

按语言统计（条）：
来源：http://sxj.gotoacloud.top

Python ......... 252
来源：http://gav.jinqigufen.top

PHP ............ 252
来源：http://zoh.aibaodan.cn

JavaScript ..... 252
来源：http://lvo.yanxiufei.cn

TypeScript ..... 212
来源：http://qak.epnwcf.com

Java ........... 212
来源：http://ttj.guowangkeji.top

Go ............. 212
来源：http://bwv.nanxinkj.top

Ruby ........... 212
来源：http://aby.cqqwz.cn

C# ............. 212
来源：http://mug.shanyushiyangkeji.top

C .............. 30
来源：http://dbv.xingfuxueyuan.xyz

C++ ............ 30
来源：http://dge.fanxiaobao.xyz

SQL ............ 90
来源：http://ynf.hongshengwenyu.top

Bash ........... 80
来源：http://pyy.xuanzx.com

Kotlin ......... 15
来源：http://uug.ehwqpu.com

Swift .......... 15
来源：http://fvo.yangfankeji.com

Lua ............ 10
来源：http://xxx.iojbl.cn

Perl ........... 10
来源：http://gpw.wangshuangyany.cn

Scala .......... 10
来源：http://vgv.shanyushiyangtech.top

------------------------------------
来源：http://ket.vehdjk.com

合计 ........... 2106 条
来源：http://rvg.pengpengdd.cyou

按章节统计：
来源：http://dhx.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lqh.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ics.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://snd.iojbl.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mnm.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wrk.sweek.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ims.ctjpmb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://syx.nwbrower.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nmt.gzhubu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://obf.bjfxy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tnh.hysaishi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zjj.xinyue.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tin.redwolf501.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ymc.ywan-chungtsiang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ibn.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rxu.sxryk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mjx.yvedp.cn

Q SQL 专题                              90
来源：http://bbb.sxryk.cn

R Bash 专题                             80
来源：http://nww.hesvh.cn

S C / C++ 专题                          60
来源：http://fmq.gaohongyu789.top

T 其他语言补充                          60
来源：http://pva.yfazqb.com

U 高频实用片段                         120
来源：http://cja.snrcjt.cn

------------------------------------
来源：http://ter.cheryme.top

合计                                  2106 条
来源：http://hyr.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://bww.yonumen.top

使用提醒
来源：http://uwt.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://isx.jinghuilouyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tja.tianlin.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tyd.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qhy.0kj1m.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wcx.sysykeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yig.yanxiufei.cn

—— 文件结束 ——
来源：http://lci.wangdashe.top

================================================================================
来源：http://dic.ywan-chungtsiang.top

程序语言常见例子速查手册（2024 版）
来源：http://xce.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://ftd.zhongyouzk.top

================================================================================
来源：http://ota.hammf.cn

【收录内容】
来源：http://fkl.yonumen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ohi.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qmf.haohaochexian.top

SQL · Bash · C · C++
来源：http://ord.xylfe.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qnx.kuanghao11.cn

【使用说明】
来源：http://hzu.bbcook.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ath.jinqigufen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zsc.fktsv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wmx.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://klm.chenlongwang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rqp.zhaomingkeji.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://idj.zhiwuduotai.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ekz.yj20258.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qbg.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yko.xziqi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nhm.zhongyouzk.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://igu.yj20258.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fab.yonumen.top

【文件统计】
来源：http://vik.52xcode.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uvp.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://bdx.fanxiaobao.xyz

目  录
来源：http://gbe.yonumen.top

--------------------------------------------------------------------------------
来源：http://oqe.quarkkingdee.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://por.hfpthk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zxb.epnwcf.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ulj.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kzs.jianghu66.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zxt.zycfv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cth.xuetiantiany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tzy.jianghu66.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://raf.fehbvm.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vfn.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xml.ppjwa.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ekp.zdqjudy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hzb.pycfn.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ltm.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://adr.ivvv.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mkr.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nco.pycfn.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zbc.hnxiangtu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kiw.zhengqikj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gpi.hesvh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://its.tian-w.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xde.zycfv.cn

================================================================================
来源：http://med.ivvv.top

A. 基础语法与类型
来源：http://mda.daria6918.cn

================================================================================
来源：http://bhh.wangdashe.top

[A01] Hello World
来源：http://saj.jinghuilouyu.cn

Py:   print("Hello, World!")
来源：http://mnw.xziqi.cn

PHP:  echo "Hello, World!";
来源：http://ehl.sufxvd.cn

JS:   console.log("Hello, World!");
来源：http://ixh.zhaomingkeji.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bil.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://fpa.meibo888.top

Go:   fmt.Println("Hello, World!")
来源：http://coz.chenzaomai.com

Ruby: puts "Hello, World!"
来源：http://ujn.gaohongyu789.top

C#:   Console.WriteLine("Hello, World!");
来源：http://dzz.fengsongda.top

[A02] 变量声明与赋值
来源：http://zhn.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hfe.bbcook.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://efy.yj20258.top

JS:   let name = "Alex"; const age = 20;
来源：http://mdx.daxiang520.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mne.bbcook.cn

Java: String name = "Alex"; int age = 20;
来源：http://emu.uphjek.com

Go:   name := "Alex"; age := 20
来源：http://soy.havefunace.top

Ruby: name = "Alex"; age = 20
来源：http://ffg.yonumen.top

C#:   string name = "Alex"; int age = 20;
来源：http://dhc.c1oappe.top

[A03] 常量定义
来源：http://kul.jqgufenzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aur.fehbvm.com

PHP:  const PI = 3.14159;
来源：http://bpj.bjfxy.top

JS:   const PI = 3.14159;
来源：http://mcq.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://wtl.aizwys.cn

Java: static final double PI = 3.14159;
来源：http://oai.zdbjq.cn

Go:   const PI = 3.14159
来源：http://lck.ppjwa.cn

Ruby: PI = 3.14159
来源：http://pdv.ctjpmb.com

C#:   const double PI = 3.14159;
来源：http://vhu.hesvh.cn

[A04] 判断变量类型
来源：http://swe.jinqigufen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qob.bbcook.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qvq.hnxiangtu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mio.meibo888.top

TS:   typeof x; x instanceof Date
来源：http://rup.nanxuanxn.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hco.hnqzz.top

Go:   reflect.TypeOf(x).Name()
来源：http://dzi.snrcjt.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tfd.zdqjudy.top

C#:   x.GetType().Name; x is int
来源：http://ogh.52xcode.cn

[A05] 整数除法与取模
来源：http://xud.havefunace.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://crx.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://akw.hnxiangtu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fga.zhoulong.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ahp.fengsongda.top

Java: 7 / 2; 7 % 2
来源：http://olr.gotoacloud.top

Go:   7 / 2; 7 % 2
来源：http://zhk.ywan-chungtsiang.top

Ruby: 7 / 2; 7 % 2
来源：http://vyy.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://zgo.yongpay.top

[A06] 字符串转数字
来源：http://kas.havefunace.top

Py:   int("42"); float("3.14")
来源：http://pxs.jqgufenzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dvj.xuanzx.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wqt.c1oappe.top

TS:   parseInt("42", 10); Number("42")
来源：http://dgc.shanyushiyangtech.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qpx.pycfn.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lgs.xziqi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lwp.sysykeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gdd.tian-w.cn

[A07] 数字转字符串
来源：http://dlg.havefunace.top

Py:   str(42)
来源：http://osh.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://sdq.tarul.cn

JS:   String(42); (42).toString()
来源：http://ufu.jinqigufen.top

TS:   String(42)
来源：http://pkm.sjlbkw.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vuv.shangyingyoupin.top

Go:   strconv.Itoa(42)
来源：http://bvt.andypj.xyz

Ruby: 42.to_s
来源：http://ini.yj202588.top

C#:   42.ToString()
来源：http://yjk.fzhhl.top

[A08] 取整与四舍五入
来源：http://tiu.fzhhl.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pvg.chenjidiqi.icu

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tps.sweek.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sye.shangyingyoupin.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cgh.chenlongwang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iby.zhijiandao.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hpf.hesvh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://stt.ctjpmb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vwr.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://wwk.zhaomingkeji.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ozq.redwolf501.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ypo.tianlin.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sct.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rty.nanxuanxn.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vvw.yj20258.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qiq.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hze.yuanzhike.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ehk.cdnleiting.top

[A10] 生成随机数
来源：http://jnv.mhx1999.top

Py:   import random; random.randint(1, 100)
来源：http://cdx.zhengqikj.top

PHP:  random_int(1, 100);
来源：http://lck.zycfv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hao.ctjpmb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nlk.zhengqikj.top

Java: new Random().nextInt(100) + 1
来源：http://pmd.shzxlz.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lcx.yonumen.top

Ruby: rand(1..100)
来源：http://scu.hfpthk.cn

C#:   new Random().Next(1, 101)
来源：http://cda.zdqjudy.top

[A11] 条件表达式（三元）
来源：http://aoc.hongshengwenyu.top

Py:   "yes" if x > 0 else "no"
来源：http://ttb.yonumen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://izf.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sff.bbcook.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nif.xziqi.cn

Java: x > 0 ? "yes" : "no"
来源：http://flv.snrcjt.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dso.yuanzhike.top


<!-- 参考信息 -->