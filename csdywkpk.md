代发 wailian999

[U75] PHP：依赖注入
来源：http://kqf.sxryk.cn

composer require psr/container
来源：http://fis.hcnkem.com

[U76] PHP：简单路由
来源：http://qdy.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ztq.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://aqy.chenlongwang.top

composer require twig/twig
来源：http://roz.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://lwj.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://khj.yueranfly.top

[U79] PHP：静态分析
来源：http://brp.vehdjk.com

composer require --dev phpstan/phpstan
来源：http://edm.mhx1999.top

[U80] PHP：代码规范修复
来源：http://owa.shuidangran.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ffo.tarul.cn

[U81] JS：初始化项目
来源：http://tny.hammf.cn

npm init -y;  npm i express
来源：http://hho.gzhubu.top

[U82] JS：package.json 脚本
来源：http://rvm.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fcv.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://ili.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gsr.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://rqp.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://tka.jianghu66.top

[U85] JS：可选链
来源：http://zwl.zhaomingkeji.xyz

a?.b?.c
来源：http://bew.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://tnb.shangyingyoupin.top

a ?? b
来源：http://ypo.nwbrower.top

[U87] JS：解构默认值
来源：http://fbe.jqgufenzy.top

const { a = 1, b = 2 } = obj;
来源：http://lyi.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://gel.yvedp.cn

{ ...a, ...b }
来源：http://ztf.gaohongyu789.top

[U89] JS：数组去重
来源：http://ocu.yangfankeji.com

[...new Set(arr)]
来源：http://vgj.jianghu66.top

[U90] JS：数字数组排序
来源：http://elo.birdmap.top

[...arr].sort((a, b) => a - b)
来源：http://opy.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://axa.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hci.cashguo.top

[U92] JS：深拷贝
来源：http://qnd.fengsongda.top

structuredClone(obj)
来源：http://cmn.dianchejie.cn

[U93] JS：模板字符串
来源：http://zkm.guowangkeji.top

`共 ${n} 条`
来源：http://nlv.zdbjq.cn

[U94] JS：箭头函数
来源：http://ybr.bjfxy.top

const double = x => x * 2;
来源：http://nbj.cucudq.cn

[U95] JS：Promise 包装
来源：http://fbg.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://lvm.c1oappe.top

[U96] JS：async/await 与异常
来源：http://gjd.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lkx.aibaodan.cn

[U97] JS：并发请求
来源：http://iex.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vjc.wangshuangyany.cn

[U98] JS：fetch 带 JSON
来源：http://xav.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qel.pengpengdd.cyou

[U99] JS：事件监听
来源：http://wta.iojbl.cn

el.addEventListener("click", e => {})
来源：http://mms.sweek.top

[U100] JS：DOM 查询
来源：http://suu.zhoulong.xyz

document.querySelector(".item")
来源：http://kqy.zhengqikj.top

[U101] JS：classList 操作
来源：http://byx.shuidangran.top

el.classList.toggle("active")
来源：http://kgm.zhengqikj.top

[U102] JS：本地存储
来源：http://lsd.xingfuxueyuan.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://qtm.zhixingplan.top

[U103] JS：定时器
来源：http://tov.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xxh.c1oappe.top

[U104] JS：防抖
来源：http://hlj.jlsjyb.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qyt.chenzaomai.com

[U105] JS：节流
来源：http://bqd.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://frl.yuanzhike.top

[U106] JS：日期格式化
来源：http://gxd.ywan-chungtsiang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pdn.cdnleiting.top

[U107] JS：数字千分位
来源：http://skb.xylfe.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rgt.hywenlv.cn

[U108] JS：随机整数
来源：http://zig.yvedp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qvy.andypj.xyz

[U109] JS：数组分组
来源：http://ucg.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://ecz.chenjidiqi.icu

[U110] JS：数组分块
来源：http://wpy.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lji.52xcode.cn

[U111] JS：对象转 Map
来源：http://cmr.shzxlz.cn

new Map(Object.entries(obj))
来源：http://oju.ctjpmb.com

[U112] JS：字符串补位
来源：http://ciq.zhengqikj.top

"7".padStart(3, "0")
来源：http://rns.tanke756.top

[U113] JS：正则替换全部
来源：http://qbk.shzxlz.cn

s.replaceAll("a", "b")
来源：http://eiu.hammf.cn

[U114] JS：JSON 深比较
来源：http://ixr.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hpo.fehbvm.com

[U115] JS：生成 UUID
来源：http://qeo.hesvh.cn

crypto.randomUUID()
来源：http://zyx.0kj1m.cn

[U116] JS：类型检查（JSDoc）
来源：http://tpf.shzxlz.cn

/** @param {string} name */ function f(name) {}
来源：http://wqg.zdbjq.cn

[U117] JS：单元测试
来源：http://fqi.zdqjudy.top

npm i -D vitest;  npx vitest
来源：http://plj.birdmap.top

[U118] JS：开发服务器
来源：http://vjh.andypj.xyz

npm i -D vite;  npx vite
来源：http://rbq.fzhhl.top

[U119] JS：生产构建
来源：http://bsr.xingfuxueyuan.xyz

npx vite build
来源：http://uym.gaohongyu789.top

[U120] JS：读取环境变量（Vite）
来源：http://mbo.jyoumei.cn

import.meta.env.VITE_API_URL
来源：http://zyp.haohaochexian.top

================================================================================
来源：http://cbz.ivvv.top

统计汇总
来源：http://jmv.yongpay.top

================================================================================
来源：http://bww.zhoulong.xyz

按语言统计（条）：
来源：http://nbq.uphjek.com

Python ......... 252
来源：http://oud.smart0.xyz

PHP ............ 252
来源：http://fht.kuanghao11.cn

JavaScript ..... 252
来源：http://fsa.yj20258888.top

TypeScript ..... 212
来源：http://gon.ppjwa.cn

Java ........... 212
来源：http://nfl.yj20258888.top

Go ............. 212
来源：http://qvs.yvedp.cn

Ruby ........... 212
来源：http://ztl.andypj.xyz

C# ............. 212
来源：http://fli.daria6918.cn

C .............. 30
来源：http://egl.sufxvd.cn

C++ ............ 30
来源：http://anp.yfazqb.com

SQL ............ 90
来源：http://kra.sxryk.cn

Bash ........... 80
来源：http://eat.316326.xyz

Kotlin ......... 15
来源：http://zok.yfazqb.com

Swift .......... 15
来源：http://cda.sysykeji.top

Lua ............ 10
来源：http://jfc.yueranfly.top

Perl ........... 10
来源：http://wys.vqdsnc.cn

Scala .......... 10
来源：http://fee.hywenlv.cn

------------------------------------
来源：http://vdk.shangyingyoupin.top

合计 ........... 2106 条
来源：http://muk.fktsv.cn

按章节统计：
来源：http://sfy.xingfuxueyuan.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rhi.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://txn.fanxiaobao.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dme.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://unk.haohaochexian.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pnv.daxiang520.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vdm.chenjidiqi.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vwp.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hzn.havefunace.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vto.gzhubu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://acn.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://igh.wangdashe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rln.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ast.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pmu.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dvm.xuanzx.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jpv.vqdsnc.cn

Q SQL 专题                              90
来源：http://rbt.epnwcf.com

R Bash 专题                             80
来源：http://tyg.svipenyu.cn

S C / C++ 专题                          60
来源：http://jrh.hfpthk.cn

T 其他语言补充                          60
来源：http://qxn.aibaodan.cn

U 高频实用片段                         120
来源：http://xmn.andypj.xyz

------------------------------------
来源：http://tse.ivvv.top

合计                                  2106 条
来源：http://hyp.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://qfi.jinqigfzy.top

使用提醒
来源：http://opt.hnqzz.top

--------------------------------------------------------------------------------
来源：http://xqz.feifeiyinyue.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fih.fanxiaobao.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rnz.yj20258888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qps.xylfe.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://unp.shanyushiyangtech.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://waf.sysykeji.top

—— 文件结束 ——
来源：http://snc.sysykeji.top

================================================================================
来源：http://lzo.yj20258888.top

程序语言常见例子速查手册（2024 版）
来源：http://asa.fehbvm.com

Common Programming Examples Cheat Book
来源：http://hnj.vehdjk.com

================================================================================
来源：http://fxn.316326.xyz

【收录内容】
来源：http://iku.cucudq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pni.tarul.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xlt.ctjpmb.com

SQL · Bash · C · C++
来源：http://anj.sxryk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hpq.jyoumei.cn

【使用说明】
来源：http://xlu.bjfxy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dlv.andypj.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kny.zhongyouzk.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://crw.sxryk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lfw.zhiwuduotai.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jgf.xuanzx.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zhg.daria6918.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ldo.fktsv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ugz.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vza.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nah.hnxiangtu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ymv.yuanzhike.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lwr.xuetiantiany.cn

【文件统计】
来源：http://akk.sxryk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eqy.hesvh.cn

--------------------------------------------------------------------------------
来源：http://sti.yj202588.top

目  录
来源：http://djy.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://unx.gaohongyu789.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hbu.kuanghao11.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hfq.birdmap.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dji.yvedp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bqw.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rdf.ydzc1.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xri.jinqigfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://slt.sjlbkw.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uua.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zza.nanxuanxn.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lns.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jrh.feifeiyinyue.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mnx.nanxuanxn.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ahj.chenjidiqi.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bup.jinqigfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ghl.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yol.guannengcc.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pqk.hcnkem.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://ajt.jianghu66.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ofg.sjlbkw.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://idr.yongpay.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iyd.c1oappe.top

================================================================================
来源：http://nxj.ctjpmb.com

A. 基础语法与类型
来源：http://mae.zycfv.cn

================================================================================
来源：http://saq.xingfuxueyuan.xyz

[A01] Hello World
来源：http://xht.dianchejie.cn

Py:   print("Hello, World!")
来源：http://uvk.ehwqpu.com

PHP:  echo "Hello, World!";
来源：http://rad.shanyushiyangtech.top

JS:   console.log("Hello, World!");
来源：http://kxh.hywenlv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wih.hcnkem.com

Java: System.out.println("Hello, World!");
来源：http://yng.ydzc1.top

Go:   fmt.Println("Hello, World!")
来源：http://fnh.snrcjt.cn

Ruby: puts "Hello, World!"
来源：http://utr.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tpw.zhaomingkeji.xyz

[A02] 变量声明与赋值
来源：http://kst.hysaishi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uib.shuidangran.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rpl.jyoumei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ukl.bbcook.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gbk.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://mzy.xuetiantiany.cn

Go:   name := "Alex"; age := 20
来源：http://gne.yvedp.cn

Ruby: name = "Alex"; age = 20
来源：http://yhb.cqqwz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qlb.xingfuxueyuan.xyz

[A03] 常量定义
来源：http://wwl.ivvv.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aqc.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://gmj.andypj.xyz

JS:   const PI = 3.14159;
来源：http://mmk.hywenlv.cn

TS:   const PI: number = 3.14159;
来源：http://obv.xinyue.icu

Java: static final double PI = 3.14159;
来源：http://gbe.guowangkeji.top

Go:   const PI = 3.14159
来源：http://oik.ehwqpu.com

Ruby: PI = 3.14159
来源：http://ohx.nanxuanxn.top

C#:   const double PI = 3.14159;
来源：http://svd.ivvv.top

[A04] 判断变量类型
来源：http://phm.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cuy.ppjwa.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tiu.daxiang520.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ekm.fengsongda.top

TS:   typeof x; x instanceof Date
来源：http://uzv.yuxming.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gdt.hywenlv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nwf.zhiwuduotai.top

Ruby: x.class; x.is_a?(Integer)
来源：http://eab.ybcxt.top

C#:   x.GetType().Name; x is int
来源：http://gre.hnqzz.top

[A05] 整数除法与取模
来源：http://nbd.jlsjyb.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vyg.redwolf501.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ahm.shzxlz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://udi.hnqzz.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://boy.jqgfzy.top

Java: 7 / 2; 7 % 2
来源：http://oib.yangfankeji.com

Go:   7 / 2; 7 % 2
来源：http://ncy.jianghu66.top

Ruby: 7 / 2; 7 % 2
来源：http://toa.aizwys.cn

C#:   7 / 2; 7 % 2
来源：http://yft.sysykeji.top

[A06] 字符串转数字
来源：http://wym.xuetiantiany.cn

Py:   int("42"); float("3.14")
来源：http://ocx.gogol.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nzi.xingfuxueyuan.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://swp.zhongyouzk.top

TS:   parseInt("42", 10); Number("42")
来源：http://idn.zycfv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zih.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jvu.ydzc1.top

Ruby: "42".to_i; "3.14".to_f
来源：http://cpc.pengpengdd.cyou

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ykv.quarkkingdee.top

[A07] 数字转字符串
来源：http://cuj.bbcook.cn

Py:   str(42)
来源：http://lqt.kuanghao11.cn

PHP:  (string) 42; strval(42)
来源：http://cgx.yuanzhike.top

JS:   String(42); (42).toString()
来源：http://jfq.yj202588.top

TS:   String(42)
来源：http://wxu.cheryme.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://aqg.sxryk.cn

Go:   strconv.Itoa(42)
来源：http://elr.tian-w.cn

Ruby: 42.to_s
来源：http://srh.sxryk.cn

C#:   42.ToString()
来源：http://aob.cucudq.cn

[A08] 取整与四舍五入
来源：http://ubr.yuxming.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sjd.zhengqikj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nsx.havefunace.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hlz.zdbjq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lrx.yj20258.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xdm.jiagoushi.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pnc.guowangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://evb.xylfe.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yed.cashguo.top

[A09] 绝对值与最大最小值
来源：http://phk.tanke756.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://azk.sysykeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gjo.daxiang520.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dby.fengsongda.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vac.tian-w.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vvp.ppjwa.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cdl.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://srf.gotoacloud.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kaa.hongshengwenyu.top

[A10] 生成随机数
来源：http://abw.xylfe.cn

Py:   import random; random.randint(1, 100)
来源：http://sfj.uphjek.com

PHP:  random_int(1, 100);
来源：http://whv.zhengqikj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jzb.shangyingyoupin.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ddv.yangfankeji.com

Java: new Random().nextInt(100) + 1
来源：http://jlk.hywenlv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://esb.ehwqpu.com

Ruby: rand(1..100)
来源：http://ggc.cdnleiting.top

C#:   new Random().Next(1, 101)
来源：http://hpd.zhiwuduotai.top

[A11] 条件表达式（三元）
来源：http://srt.andypj.xyz

Py:   "yes" if x > 0 else "no"
来源：http://cnc.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://kva.sxryk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vma.aizwys.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vvo.yvedp.cn

Java: x > 0 ? "yes" : "no"
来源：http://eve.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ybi.jqgfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ezf.hysaishi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tve.zhiwuduotai.top

[A12] 字符串插值 / 格式化
来源：http://yyi.gotoacloud.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ugf.fengsongda.top


<!-- 参考信息 -->