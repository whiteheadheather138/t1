代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://ukc.birdmap.top

parse_ini_file("config.ini", true)
来源：http://our.zhixingplan.top

[U74] PHP：读取环境变量
来源：http://tnz.tanke756.top

getenv("APP_ENV") ?: "production"
来源：http://uvy.chenzaomai.com

[U75] PHP：依赖注入
来源：http://abr.quarkkingdee.top

composer require psr/container
来源：http://idj.yvedp.cn

[U76] PHP：简单路由
来源：http://cif.hfpthk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dcq.gzhubu.top

[U77] PHP：模板渲染
来源：http://tzp.shuidangran.top

composer require twig/twig
来源：http://cxr.shzxlz.cn

[U78] PHP：单元测试
来源：http://iff.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://cup.aibaodan.cn

[U79] PHP：静态分析
来源：http://mlw.dashuyun.cn

composer require --dev phpstan/phpstan
来源：http://szg.yvedp.cn

[U80] PHP：代码规范修复
来源：http://nqg.guannengcc.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tvg.hesvh.cn

[U81] JS：初始化项目
来源：http://hwo.hcnkem.com

npm init -y;  npm i express
来源：http://utq.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://fyo.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://inl.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://ade.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://xns.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://iri.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lus.haohaochexian.top

[U85] JS：可选链
来源：http://jae.cashguo.top

a?.b?.c
来源：http://xyn.zycfv.cn

[U86] JS：空值合并
来源：http://tkq.yfazqb.com

a ?? b
来源：http://wef.cashguo.top

[U87] JS：解构默认值
来源：http://yed.ydjk.org.cn

const { a = 1, b = 2 } = obj;
来源：http://ixa.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://xnt.gzhubu.top

{ ...a, ...b }
来源：http://duv.aibaodan.cn

[U89] JS：数组去重
来源：http://qbn.nwbrower.top

[...new Set(arr)]
来源：http://ljz.hammf.cn

[U90] JS：数字数组排序
来源：http://feo.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://kcn.redwolf501.top

[U91] JS：对象键值遍历
来源：http://mmn.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zkk.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://yhk.bjfxy.top

structuredClone(obj)
来源：http://xjs.aizwys.cn

[U93] JS：模板字符串
来源：http://swj.ctjpmb.com

`共 ${n} 条`
来源：http://fmv.fengsongda.top

[U94] JS：箭头函数
来源：http://gvd.mhx1999.top

const double = x => x * 2;
来源：http://vfc.yonumen.top

[U95] JS：Promise 包装
来源：http://ahh.jlsjyb.cn

new Promise((resolve, reject) => {})
来源：http://dyd.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://lpi.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cbv.sufxvd.cn

[U97] JS：并发请求
来源：http://ace.tian-w.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ibj.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://hjy.tianlin.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bdv.chenjidiqi.icu

[U99] JS：事件监听
来源：http://iho.zhijiandao.cn

el.addEventListener("click", e => {})
来源：http://sqh.xuanzx.com

[U100] JS：DOM 查询
来源：http://vlw.pengpengdd.cyou

document.querySelector(".item")
来源：http://jeu.wangdashe.top

[U101] JS：classList 操作
来源：http://fdh.vehdjk.com

el.classList.toggle("active")
来源：http://vhk.havefunace.top

[U102] JS：本地存储
来源：http://nrv.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xue.yj20258.top

[U103] JS：定时器
来源：http://ihx.kuanghao11.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dwu.cucudq.cn

[U104] JS：防抖
来源：http://gjf.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ycl.guannengcc.top

[U105] JS：节流
来源：http://lqq.fehbvm.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mie.sufxvd.cn

[U106] JS：日期格式化
来源：http://ykf.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fst.yj20258.top

[U107] JS：数字千分位
来源：http://gig.hysaishi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iun.bbcook.cn

[U108] JS：随机整数
来源：http://awc.chenzaomai.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aqy.hysaishi.cn

[U109] JS：数组分组
来源：http://bdx.epnwcf.com

Object.groupBy(arr, x => x.type)
来源：http://xor.sweek.top

[U110] JS：数组分块
来源：http://hjr.shangyingyoupin.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://txx.dianchejie.cn

[U111] JS：对象转 Map
来源：http://emt.pycfn.com

new Map(Object.entries(obj))
来源：http://mmp.ehwqpu.com

[U112] JS：字符串补位
来源：http://osb.dashuyun.cn

"7".padStart(3, "0")
来源：http://emf.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://eol.daria6918.cn

s.replaceAll("a", "b")
来源：http://dpb.yuxming.cn

[U114] JS：JSON 深比较
来源：http://swr.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tnj.daria6918.cn

[U115] JS：生成 UUID
来源：http://zwa.birdmap.top

crypto.randomUUID()
来源：http://xun.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://yvj.hongshengwenyu.top

/** @param {string} name */ function f(name) {}
来源：http://oso.yonumen.top

[U117] JS：单元测试
来源：http://wls.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://qxf.zhongyouzk.top

[U118] JS：开发服务器
来源：http://zjr.yfazqb.com

npm i -D vite;  npx vite
来源：http://idr.hesvh.cn

[U119] JS：生产构建
来源：http://noy.nanxuanxn.top

npx vite build
来源：http://vyw.guannengcc.top

[U120] JS：读取环境变量（Vite）
来源：http://bvv.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://lqd.shanyushiyangtech.top

================================================================================
来源：http://ukz.316326.xyz

统计汇总
来源：http://kep.iojbl.cn

================================================================================
来源：http://uag.9152youxi.cn

按语言统计（条）：
来源：http://egh.shangyingyoupin.top

Python ......... 252
来源：http://bdm.xinyue.icu

PHP ............ 252
来源：http://rix.andypj.xyz

JavaScript ..... 252
来源：http://bri.zdqjudy.top

TypeScript ..... 212
来源：http://zro.sysykeji.top

Java ........... 212
来源：http://kqh.vqdsnc.cn

Go ............. 212
来源：http://byp.bjfxy.top

Ruby ........... 212
来源：http://ybg.zhengqikj.top

C# ............. 212
来源：http://vas.nanxinkj.top

C .............. 30
来源：http://vvi.wangshuangyany.cn

C++ ............ 30
来源：http://vmx.ydjk.org.cn

SQL ............ 90
来源：http://urr.zhiwuduotai.top

Bash ........... 80
来源：http://hte.zhongyouzk.top

Kotlin ......... 15
来源：http://dmg.hesvh.cn

Swift .......... 15
来源：http://xhs.vqdsnc.cn

Lua ............ 10
来源：http://idt.ybcxt.top

Perl ........... 10
来源：http://nxd.wangshuangyany.cn

Scala .......... 10
来源：http://dis.hammf.cn

------------------------------------
来源：http://lhf.sxryk.cn

合计 ........... 2106 条
来源：http://whs.ydzc1.top

按章节统计：
来源：http://dgs.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://unc.jyoumei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://epb.hcnkem.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cqi.jiagoushi.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gnw.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zez.ybcxt.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://anz.sysykeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://csa.ctjpmb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uix.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gud.hnxiangtu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dwn.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kth.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fdq.cqqwz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tau.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rbj.jinqigfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://coo.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qir.havefunace.top

Q SQL 专题                              90
来源：http://haa.yuanzhike.top

R Bash 专题                             80
来源：http://jjj.tian-w.cn

S C / C++ 专题                          60
来源：http://rwu.havefunace.top

T 其他语言补充                          60
来源：http://pce.tianlin.xyz

U 高频实用片段                         120
来源：http://nek.0kj1m.cn

------------------------------------
来源：http://lll.chenjidiqi.icu

合计                                  2106 条
来源：http://sdo.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://pam.hongshengwenyu.top

使用提醒
来源：http://omp.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://axt.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ioz.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fhv.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xwb.zhengqikj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jvu.nwbrower.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://npm.nanxinkj.top

—— 文件结束 ——
来源：http://hfb.jianghu66.top

================================================================================
来源：http://mkx.dianchejie.cn

程序语言常见例子速查手册（2024 版）
来源：http://qni.daria6918.cn

Common Programming Examples Cheat Book
来源：http://vjl.yvedp.cn

================================================================================
来源：http://liu.c1oappe.top

【收录内容】
来源：http://pkx.zhaomingkeji.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://wsg.zhixingplan.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qvi.nanxuanxn.top

SQL · Bash · C · C++
来源：http://hni.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oqz.yj202588.top

【使用说明】
来源：http://xlx.jinqigfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wog.epnwcf.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rxt.yanxiufei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rhs.ctjpmb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ekc.9152youxi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wji.shuidangran.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ylg.wangdashe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bcb.feifeiyinyue.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://glg.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ybo.tian-w.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yon.yuanzhike.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dsh.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dhd.c1oappe.top

【文件统计】
来源：http://kqw.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bxa.yuxming.cn

--------------------------------------------------------------------------------
来源：http://vly.bbcook.cn

目  录
来源：http://olx.yongpay.top

--------------------------------------------------------------------------------
来源：http://rhq.quarkkingdee.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://piw.yuanzhike.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qim.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zde.bjfxy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oit.shanyushiyangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dzi.meibo888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lhh.fzhhl.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nlr.hfpthk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oxp.hnxiangtu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zza.9152youxi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://acc.yj20258.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ojw.birdmap.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kzf.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://edd.wangshuangyany.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bwg.zhongyouzk.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pud.yueranfly.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://itc.jqgfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xsq.jianghu66.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jxk.hfpthk.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hzl.jiagoushi.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xzd.snrcjt.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zws.hysaishi.cn

================================================================================
来源：http://svo.yangfankeji.com

A. 基础语法与类型
来源：http://vmz.yanxiufei.cn

================================================================================
来源：http://zhf.hcnkem.com

[A01] Hello World
来源：http://lww.zhiwuduotai.top

Py:   print("Hello, World!")
来源：http://bxb.pengpengdd.cyou

PHP:  echo "Hello, World!";
来源：http://llq.shanyushiyangkeji.top

JS:   console.log("Hello, World!");
来源：http://ipp.yueranfly.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pkd.dianchejie.cn

Java: System.out.println("Hello, World!");
来源：http://mwe.cheryme.top

Go:   fmt.Println("Hello, World!")
来源：http://dlo.pengpengdd.cyou

Ruby: puts "Hello, World!"
来源：http://pgr.xylfe.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gey.xziqi.cn

[A02] 变量声明与赋值
来源：http://gqs.jinyuanbaomall.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tml.c1oappe.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uem.dianchejie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://akp.zdqjudy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zux.sweek.top

Java: String name = "Alex"; int age = 20;
来源：http://yvm.yuxming.cn

Go:   name := "Alex"; age := 20
来源：http://tqu.ehwqpu.com

Ruby: name = "Alex"; age = 20
来源：http://fbv.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://vgo.redwolf501.top

[A03] 常量定义
来源：http://ejs.daria6918.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gzo.gaohongyu789.top

PHP:  const PI = 3.14159;
来源：http://tyv.tanke756.top

JS:   const PI = 3.14159;
来源：http://izr.nwbrower.top

TS:   const PI: number = 3.14159;
来源：http://zcc.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://ukh.hongshengwenyu.top

Go:   const PI = 3.14159
来源：http://aji.guowangkeji.top

Ruby: PI = 3.14159
来源：http://iwg.daxiang520.top

C#:   const double PI = 3.14159;
来源：http://uav.52xcode.cn

[A04] 判断变量类型
来源：http://pjq.hysaishi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pqo.xuanzx.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://irl.hnxiangtu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jsy.zhixingplan.top

TS:   typeof x; x instanceof Date
来源：http://tpp.ywan-chungtsiang.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nyt.ywan-chungtsiang.top

Go:   reflect.TypeOf(x).Name()
来源：http://nkl.nwbrower.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pcs.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://wgx.chenlongwang.top

[A05] 整数除法与取模
来源：http://mxe.hnqzz.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qrr.yj20258.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://haw.jianghu66.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fbg.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vhz.guowangkeji.top

Java: 7 / 2; 7 % 2
来源：http://eph.uphjek.com

Go:   7 / 2; 7 % 2
来源：http://rbv.52xcode.cn

Ruby: 7 / 2; 7 % 2
来源：http://dae.mhx1999.top

C#:   7 / 2; 7 % 2
来源：http://pkz.cucudq.cn

[A06] 字符串转数字
来源：http://lzd.gotoacloud.top

Py:   int("42"); float("3.14")
来源：http://duf.tian-w.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iat.xziqi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cyh.chenjidiqi.icu

TS:   parseInt("42", 10); Number("42")
来源：http://zhv.xuetiantiany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bni.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fgt.fanxiaobao.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://yol.yongpay.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://woo.dashuyun.cn

[A07] 数字转字符串
来源：http://gvq.dianchejie.cn

Py:   str(42)
来源：http://uon.c1oappe.top

PHP:  (string) 42; strval(42)
来源：http://mwp.yvedp.cn

JS:   String(42); (42).toString()
来源：http://ist.shangyingyoupin.top

TS:   String(42)
来源：http://zff.xingfuxueyuan.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://ybq.aibaodan.cn

Go:   strconv.Itoa(42)
来源：http://oqn.ydzc1.top

Ruby: 42.to_s
来源：http://hvn.wangshuangyany.cn

C#:   42.ToString()
来源：http://isn.jyoumei.cn

[A08] 取整与四舍五入
来源：http://kqr.mhx1999.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pzi.tianlin.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://olm.pycfn.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sgs.fzhhl.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rxb.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://owk.zhoulong.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://opp.0kj1m.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mye.fehbvm.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xhx.daria6918.cn

[A09] 绝对值与最大最小值
来源：http://umd.hnqzz.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://iid.ppjwa.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://osm.hnxiangtu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xno.sweek.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kvb.tian-w.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tal.xingfuxueyuan.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qpn.cashguo.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dwk.ivvv.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eqt.pengpengdd.cyou

[A10] 生成随机数
来源：http://buo.zdqjudy.top

Py:   import random; random.randint(1, 100)
来源：http://fsh.fengsongda.top

PHP:  random_int(1, 100);
来源：http://qgg.jinqigufen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qef.ybcxt.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sdx.meibo888.top

Java: new Random().nextInt(100) + 1
来源：http://vxe.yueranfly.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hze.chenlongwang.top

Ruby: rand(1..100)
来源：http://ryq.quarkkingdee.top

C#:   new Random().Next(1, 101)
来源：http://qgi.snrcjt.cn

[A11] 条件表达式（三元）
来源：http://tsp.nanxinkj.top

Py:   "yes" if x > 0 else "no"
来源：http://aiy.hnxiangtu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://saf.nanxuanxn.top

JS:   x > 0 ? "yes" : "no"
来源：http://bbg.ivvv.top

TS:   x > 0 ? "yes" : "no"
来源：http://qsp.hammf.cn

Java: x > 0 ? "yes" : "no"
来源：http://uoi.cashguo.top

Go:   // 无三元运算符，需用 if 语句
来源：http://zhx.hnqzz.top


<!-- 参考信息 -->