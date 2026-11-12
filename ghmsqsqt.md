代发 wailian999

[U75] PHP：依赖注入
来源：http://uxk.zycfv.cn

composer require psr/container
来源：http://fhv.jinqigfzy.top

[U76] PHP：简单路由
来源：http://hck.tanke756.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rnh.wangdashe.top

[U77] PHP：模板渲染
来源：http://ytb.svipenyu.cn

composer require twig/twig
来源：http://oly.sjlbkw.cn

[U78] PHP：单元测试
来源：http://gcu.52xcode.cn

composer require --dev phpunit/phpunit
来源：http://mkw.xinyue.icu

[U79] PHP：静态分析
来源：http://xzj.andypj.xyz

composer require --dev phpstan/phpstan
来源：http://gcq.bjfxy.top

[U80] PHP：代码规范修复
来源：http://xvq.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fgu.ppjwa.cn

[U81] JS：初始化项目
来源：http://kha.pengpengdd.cyou

npm init -y;  npm i express
来源：http://qog.tarul.cn

[U82] JS：package.json 脚本
来源：http://cdj.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yoq.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://doq.vqdsnc.cn

export const a = 1;  import { a } from "./m.js";
来源：http://usa.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://dgs.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dhz.snrcjt.cn

[U85] JS：可选链
来源：http://qjg.jqgfzy.top

a?.b?.c
来源：http://jdr.svipenyu.cn

[U86] JS：空值合并
来源：http://iqs.jinqigufen.top

a ?? b
来源：http://tea.hesvh.cn

[U87] JS：解构默认值
来源：http://hen.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://obl.snrcjt.cn

[U88] JS：对象展开合并
来源：http://mjg.vqdsnc.cn

{ ...a, ...b }
来源：http://tjy.xziqi.cn

[U89] JS：数组去重
来源：http://vjv.chenzaomai.com

[...new Set(arr)]
来源：http://lmw.cucudq.cn

[U90] JS：数字数组排序
来源：http://zez.jyoumei.cn

[...arr].sort((a, b) => a - b)
来源：http://utn.jlsjyb.cn

[U91] JS：对象键值遍历
来源：http://dnz.redwolf501.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sik.iojbl.cn

[U92] JS：深拷贝
来源：http://yvt.fanxiaobao.xyz

structuredClone(obj)
来源：http://rdr.sjlbkw.cn

[U93] JS：模板字符串
来源：http://tiy.c1oappe.top

`共 ${n} 条`
来源：http://jyu.zhoulong.xyz

[U94] JS：箭头函数
来源：http://foz.chenlongwang.top

const double = x => x * 2;
来源：http://ebo.yj202588.top

[U95] JS：Promise 包装
来源：http://zfc.fktsv.cn

new Promise((resolve, reject) => {})
来源：http://ewu.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://lrf.ywan-chungtsiang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qnb.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://dpq.jinghuilouyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fne.bbcook.cn

[U98] JS：fetch 带 JSON
来源：http://ttm.redwolf501.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hyd.52xcode.cn

[U99] JS：事件监听
来源：http://tqp.nwbrower.top

el.addEventListener("click", e => {})
来源：http://fdo.yanxiufei.cn

[U100] JS：DOM 查询
来源：http://hrv.snrcjt.cn

document.querySelector(".item")
来源：http://tax.fzhhl.top

[U101] JS：classList 操作
来源：http://tjx.ehwqpu.com

el.classList.toggle("active")
来源：http://dhj.svipenyu.cn

[U102] JS：本地存储
来源：http://ibl.hongshengwenyu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tah.sufxvd.cn

[U103] JS：定时器
来源：http://xfz.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qjv.yj202588.top

[U104] JS：防抖
来源：http://fwc.9152youxi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dix.gotoacloud.top

[U105] JS：节流
来源：http://zjj.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ouo.gotoacloud.top

[U106] JS：日期格式化
来源：http://kbt.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tvr.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://okg.gzhubu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tks.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://sgm.chenlongwang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ozk.ehwqpu.com

[U109] JS：数组分组
来源：http://tet.tarul.cn

Object.groupBy(arr, x => x.type)
来源：http://ofl.zhoulong.xyz

[U110] JS：数组分块
来源：http://ktw.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://khe.jinghuilouyu.cn

[U111] JS：对象转 Map
来源：http://nzp.xinyue.icu

new Map(Object.entries(obj))
来源：http://gjm.jyoumei.cn

[U112] JS：字符串补位
来源：http://qdj.chenjidiqi.icu

"7".padStart(3, "0")
来源：http://djy.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://ltf.jinghuilouyu.cn

s.replaceAll("a", "b")
来源：http://mqp.yvedp.cn

[U114] JS：JSON 深比较
来源：http://kvv.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://iyb.nwbrower.top

[U115] JS：生成 UUID
来源：http://hii.dashuyun.cn

crypto.randomUUID()
来源：http://wzc.hnqzz.top

[U116] JS：类型检查（JSDoc）
来源：http://pcm.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://cpx.nanxuanxn.top

[U117] JS：单元测试
来源：http://kpq.jianghu66.top

npm i -D vitest;  npx vitest
来源：http://hrw.ydjk.org.cn

[U118] JS：开发服务器
来源：http://woy.mhx1999.top

npm i -D vite;  npx vite
来源：http://wyx.vqdsnc.cn

[U119] JS：生产构建
来源：http://vjl.fehbvm.com

npx vite build
来源：http://pcl.kuanghao11.cn

[U120] JS：读取环境变量（Vite）
来源：http://sfg.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://eqc.xingfuxueyuan.xyz

================================================================================
来源：http://qrb.jyoumei.cn

统计汇总
来源：http://ihj.iojbl.cn

================================================================================
来源：http://arn.aibaodan.cn

按语言统计（条）：
来源：http://yux.snrcjt.cn

Python ......... 252
来源：http://gwr.quarkkingdee.top

PHP ............ 252
来源：http://rgc.ydjk.org.cn

JavaScript ..... 252
来源：http://bhr.tian-w.cn

TypeScript ..... 212
来源：http://hlk.52xcode.cn

Java ........... 212
来源：http://jln.chenjidiqi.icu

Go ............. 212
来源：http://ejv.chenjidiqi.icu

Ruby ........... 212
来源：http://hxb.jinghuilouyu.cn

C# ............. 212
来源：http://bny.ehwqpu.com

C .............. 30
来源：http://dpw.9152youxi.cn

C++ ............ 30
来源：http://aza.fehbvm.com

SQL ............ 90
来源：http://fys.shangyingyoupin.top

Bash ........... 80
来源：http://lzc.zhongyouzk.top

Kotlin ......... 15
来源：http://urg.zhixingplan.top

Swift .......... 15
来源：http://cgf.andypj.xyz

Lua ............ 10
来源：http://fws.smart0.xyz

Perl ........... 10
来源：http://olj.jinghuilouyu.cn

Scala .......... 10
来源：http://guc.fanxiaobao.xyz

------------------------------------
来源：http://nlp.tarul.cn

合计 ........... 2106 条
来源：http://trh.hongshengwenyu.top

按章节统计：
来源：http://ezb.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vfv.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bxq.fanxiaobao.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://foa.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wuy.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xln.tanke756.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hif.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wpy.fanxiaobao.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rau.gogol.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gdn.hesvh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mko.hesvh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wnr.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wbp.zhoulong.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ria.ctjpmb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qsw.sxryk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tew.gotoacloud.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rlp.iojbl.cn

Q SQL 专题                              90
来源：http://fwo.fehbvm.com

R Bash 专题                             80
来源：http://bam.mhx1999.top

S C / C++ 专题                          60
来源：http://ymu.bjfxy.top

T 其他语言补充                          60
来源：http://rfq.316326.xyz

U 高频实用片段                         120
来源：http://fak.ydzc1.top

------------------------------------
来源：http://nmf.sysykeji.top

合计                                  2106 条
来源：http://fuv.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://rml.epnwcf.com

使用提醒
来源：http://nnt.iojbl.cn

--------------------------------------------------------------------------------
来源：http://rqd.nwbrower.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zjh.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vtb.sweek.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nqh.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://huq.shzxlz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ydu.smart0.xyz

—— 文件结束 ——
来源：http://cpe.snrcjt.cn

================================================================================
来源：http://fol.nwbrower.top

程序语言常见例子速查手册（2024 版）
来源：http://qdu.aizwys.cn

Common Programming Examples Cheat Book
来源：http://bqp.fzhhl.top

================================================================================
来源：http://dbe.vqdsnc.cn

【收录内容】
来源：http://vzj.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jwv.dashuyun.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uic.kuanghao11.cn

SQL · Bash · C · C++
来源：http://rlc.pengpengdd.cyou

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mzu.yonumen.top

【使用说明】
来源：http://lft.sxryk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nzu.zycfv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://abw.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rdt.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ndn.hysaishi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wqu.guowangkeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xbv.guowangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://glg.zhixingplan.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dmh.sweek.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mul.redwolf501.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kzr.ppjwa.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://htv.shanyushiyangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kuk.gotoacloud.top

【文件统计】
来源：http://ulr.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uof.316326.xyz

--------------------------------------------------------------------------------
来源：http://qpy.uphjek.com

目  录
来源：http://rjn.havefunace.top

--------------------------------------------------------------------------------
来源：http://ejo.ywan-chungtsiang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fro.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ivh.zhijiandao.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lgi.bbcook.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ezd.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ksz.jinghuilouyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rix.cqqwz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wgz.bbcook.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ucn.epnwcf.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vlb.cucudq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qxh.yj202588.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vfu.snrcjt.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lpr.nanxuanxn.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xxh.redwolf501.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kmh.ybcxt.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://twg.sysykeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jyz.cqqwz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://suu.316326.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://gtd.jianghu66.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hhz.chenjidiqi.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cck.tanke756.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gja.yj20258.top

================================================================================
来源：http://vsu.nanxuanxn.top

A. 基础语法与类型
来源：http://bop.chenzaomai.com

================================================================================
来源：http://szf.fehbvm.com

[A01] Hello World
来源：http://okg.zhengqikj.top

Py:   print("Hello, World!")
来源：http://wty.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://bzt.shanyushiyangkeji.top

JS:   console.log("Hello, World!");
来源：http://udd.zhongyouzk.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eim.xylfe.cn

Java: System.out.println("Hello, World!");
来源：http://ylz.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://eci.nwbrower.top

Ruby: puts "Hello, World!"
来源：http://yfu.xinyue.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://nnl.tianlin.xyz

[A02] 变量声明与赋值
来源：http://olr.sxryk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://niw.jqgfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qoa.c1oappe.top

JS:   let name = "Alex"; const age = 20;
来源：http://ata.yonumen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ilo.svipenyu.cn

Java: String name = "Alex"; int age = 20;
来源：http://sci.ywan-chungtsiang.top

Go:   name := "Alex"; age := 20
来源：http://hnz.cashguo.top

Ruby: name = "Alex"; age = 20
来源：http://ufw.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://gqo.yanxiufei.cn

[A03] 常量定义
来源：http://yzt.smart0.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uyk.jlsjyb.cn

PHP:  const PI = 3.14159;
来源：http://rrz.fzhhl.top

JS:   const PI = 3.14159;
来源：http://dxi.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://lxw.ydjk.org.cn

Java: static final double PI = 3.14159;
来源：http://rzf.hammf.cn

Go:   const PI = 3.14159
来源：http://ffm.gotoacloud.top

Ruby: PI = 3.14159
来源：http://ugf.yuanzhike.top

C#:   const double PI = 3.14159;
来源：http://hdc.epnwcf.com

[A04] 判断变量类型
来源：http://jgo.yangfankeji.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://bzp.jiagoushi.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yxy.xinyue.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oax.hnxiangtu.top

TS:   typeof x; x instanceof Date
来源：http://ims.hammf.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xwa.cashguo.top

Go:   reflect.TypeOf(x).Name()
来源：http://yog.yongpay.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wxj.fanxiaobao.xyz

C#:   x.GetType().Name; x is int
来源：http://suz.nwbrower.top

[A05] 整数除法与取模
来源：http://ufx.quarkkingdee.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jkg.yuxming.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://iqt.havefunace.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gzt.aibaodan.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wjc.fanxiaobao.xyz

Java: 7 / 2; 7 % 2
来源：http://mty.yj20258.top

Go:   7 / 2; 7 % 2
来源：http://sjd.52xcode.cn

Ruby: 7 / 2; 7 % 2
来源：http://iaw.gaohongyu789.top

C#:   7 / 2; 7 % 2
来源：http://zxl.feifeiyinyue.top

[A06] 字符串转数字
来源：http://tmp.xuanzx.com

Py:   int("42"); float("3.14")
来源：http://wdv.snrcjt.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gmz.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vdo.vehdjk.com

TS:   parseInt("42", 10); Number("42")
来源：http://fgz.vehdjk.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qkt.cucudq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gus.guannengcc.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hzf.cheryme.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ssm.ivvv.top

[A07] 数字转字符串
来源：http://eml.hongshengwenyu.top

Py:   str(42)
来源：http://zxm.sufxvd.cn

PHP:  (string) 42; strval(42)
来源：http://cci.fktsv.cn

JS:   String(42); (42).toString()
来源：http://ndt.zhixingplan.top

TS:   String(42)
来源：http://opl.wangshuangyany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vrf.jiagoushi.top

Go:   strconv.Itoa(42)
来源：http://qjt.xingfuxueyuan.xyz

Ruby: 42.to_s
来源：http://xtp.pengpengdd.cyou

C#:   42.ToString()
来源：http://iua.quarkkingdee.top

[A08] 取整与四舍五入
来源：http://cqd.yonumen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tnm.fanxiaobao.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vwo.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xxj.havefunace.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://odx.hongshengwenyu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gxg.gaohongyu789.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gtg.fzhhl.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://yci.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://afz.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://jnu.feifeiyinyue.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qcz.xuetiantiany.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kut.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jzu.gzhubu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fzx.ywan-chungtsiang.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jci.ybcxt.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://prk.hongshengwenyu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hfw.tarul.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gob.mhx1999.top

[A10] 生成随机数
来源：http://xyk.c1oappe.top

Py:   import random; random.randint(1, 100)
来源：http://qtw.pengpengdd.cyou

PHP:  random_int(1, 100);
来源：http://mjj.jqgufenzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yku.ybcxt.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tmp.bjfxy.top

Java: new Random().nextInt(100) + 1
来源：http://gdb.shuidangran.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lgz.zycfv.cn

Ruby: rand(1..100)
来源：http://pqk.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://mmj.chenjidiqi.icu

[A11] 条件表达式（三元）
来源：http://mki.sysykeji.top

Py:   "yes" if x > 0 else "no"
来源：http://uud.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vbm.yanxiufei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eno.52xcode.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yot.tianlin.xyz

Java: x > 0 ? "yes" : "no"
来源：http://sye.chenzaomai.com

Go:   // 无三元运算符，需用 if 语句
来源：http://hxl.pengpengdd.cyou

Ruby: x > 0 ? "yes" : "no"
来源：http://kve.sweek.top

C#:   x > 0 ? "yes" : "no"
来源：http://wfe.chenlongwang.top

[A12] 字符串插值 / 格式化
来源：http://psp.tarul.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uuv.dashuyun.cn


<!-- 参考信息 -->