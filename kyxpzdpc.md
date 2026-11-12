代发 wailian999

[U75] PHP：依赖注入
来源：http://vpo.tian-w.cn

composer require psr/container
来源：http://dbl.aizwys.cn

[U76] PHP：简单路由
来源：http://tgz.xziqi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vlh.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://yzw.guowangkeji.top

composer require twig/twig
来源：http://hpq.mhx1999.top

[U78] PHP：单元测试
来源：http://ozs.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://wze.zdbjq.cn

[U79] PHP：静态分析
来源：http://jmq.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://epx.meibo888.top

[U80] PHP：代码规范修复
来源：http://exw.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kjw.xuanzx.com

[U81] JS：初始化项目
来源：http://pqw.chenlongwang.top

npm init -y;  npm i express
来源：http://dqa.yueranfly.top

[U82] JS：package.json 脚本
来源：http://eio.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://osw.yj20258.top

[U83] JS：ES Module 导入导出
来源：http://dnj.feifeiyinyue.top

export const a = 1;  import { a } from "./m.js";
来源：http://dtg.jinqigufen.top

[U84] JS：CommonJS 写法
来源：http://qyf.shuidangran.top

module.exports = { a };  const { a } = require("./m");
来源：http://sbk.yj20258.top

[U85] JS：可选链
来源：http://yhi.zhixingplan.top

a?.b?.c
来源：http://zkz.fktsv.cn

[U86] JS：空值合并
来源：http://oiz.0kj1m.cn

a ?? b
来源：http://mcx.c1oappe.top

[U87] JS：解构默认值
来源：http://iov.gotoacloud.top

const { a = 1, b = 2 } = obj;
来源：http://jsv.gogol.net.cn

[U88] JS：对象展开合并
来源：http://tbe.yuanzhike.top

{ ...a, ...b }
来源：http://tgv.9152youxi.cn

[U89] JS：数组去重
来源：http://jyz.jyoumei.cn

[...new Set(arr)]
来源：http://xvg.fanxiaobao.xyz

[U90] JS：数字数组排序
来源：http://bum.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://uss.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://rwa.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ovz.zhoulong.xyz

[U92] JS：深拷贝
来源：http://gat.jlsjyb.cn

structuredClone(obj)
来源：http://xtd.yanxiufei.cn

[U93] JS：模板字符串
来源：http://cps.cheryme.top

`共 ${n} 条`
来源：http://fvn.hcnkem.com

[U94] JS：箭头函数
来源：http://rio.gaohongyu789.top

const double = x => x * 2;
来源：http://ihh.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://jtd.daxiang520.top

new Promise((resolve, reject) => {})
来源：http://pil.xinyue.icu

[U96] JS：async/await 与异常
来源：http://mkp.ehwqpu.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mgv.hcnkem.com

[U97] JS：并发请求
来源：http://zbk.aizwys.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rvn.smart0.xyz

[U98] JS：fetch 带 JSON
来源：http://sxn.aizwys.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kyo.birdmap.top

[U99] JS：事件监听
来源：http://ojb.hcnkem.com

el.addEventListener("click", e => {})
来源：http://fyh.jinghuilouyu.cn

[U100] JS：DOM 查询
来源：http://fpk.haohaochexian.top

document.querySelector(".item")
来源：http://aah.smart0.xyz

[U101] JS：classList 操作
来源：http://ldh.shangyingyoupin.top

el.classList.toggle("active")
来源：http://gxk.haohaochexian.top

[U102] JS：本地存储
来源：http://ahu.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tre.gotoacloud.top

[U103] JS：定时器
来源：http://trr.sxryk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gko.sweek.top

[U104] JS：防抖
来源：http://pcs.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rns.tianlin.xyz

[U105] JS：节流
来源：http://pwd.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vps.chenzaomai.com

[U106] JS：日期格式化
来源：http://fuk.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://scz.hcnkem.com

[U107] JS：数字千分位
来源：http://xvo.yangfankeji.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bov.andypj.xyz

[U108] JS：随机整数
来源：http://ftt.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fee.ctjpmb.com

[U109] JS：数组分组
来源：http://yzq.yangfankeji.com

Object.groupBy(arr, x => x.type)
来源：http://uho.xziqi.cn

[U110] JS：数组分块
来源：http://qrq.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://apx.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://ffj.ydjk.org.cn

new Map(Object.entries(obj))
来源：http://lra.chenzaomai.com

[U112] JS：字符串补位
来源：http://mbc.zhiwuduotai.top

"7".padStart(3, "0")
来源：http://twv.yj20258888.top

[U113] JS：正则替换全部
来源：http://oxx.havefunace.top

s.replaceAll("a", "b")
来源：http://tku.mhx1999.top

[U114] JS：JSON 深比较
来源：http://nxg.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tjf.iojbl.cn

[U115] JS：生成 UUID
来源：http://rsw.tanke756.top

crypto.randomUUID()
来源：http://apl.yuanzhike.top

[U116] JS：类型检查（JSDoc）
来源：http://zpf.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://lpc.hcnkem.com

[U117] JS：单元测试
来源：http://llv.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://aos.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://cdn.hammf.cn

npm i -D vite;  npx vite
来源：http://efx.fanxiaobao.xyz

[U119] JS：生产构建
来源：http://flm.shuidangran.top

npx vite build
来源：http://jdw.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://dpf.c1oappe.top

import.meta.env.VITE_API_URL
来源：http://lbr.bbcook.cn

================================================================================
来源：http://sht.ywan-chungtsiang.top

统计汇总
来源：http://wux.yj20258888.top

================================================================================
来源：http://tme.hnqzz.top

按语言统计（条）：
来源：http://mpi.aibaodan.cn

Python ......... 252
来源：http://jyo.shuidangran.top

PHP ............ 252
来源：http://inh.ivvv.top

JavaScript ..... 252
来源：http://vvv.zhongyouzk.top

TypeScript ..... 212
来源：http://qfu.yonumen.top

Java ........... 212
来源：http://cas.xziqi.cn

Go ............. 212
来源：http://rab.zycfv.cn

Ruby ........... 212
来源：http://mrb.redwolf501.top

C# ............. 212
来源：http://eum.hnqzz.top

C .............. 30
来源：http://orz.hfpthk.cn

C++ ............ 30
来源：http://yht.ydzc1.top

SQL ............ 90
来源：http://xeg.haohaochexian.top

Bash ........... 80
来源：http://dzw.shangyingyoupin.top

Kotlin ......... 15
来源：http://ael.sxryk.cn

Swift .......... 15
来源：http://djd.gzhubu.top

Lua ............ 10
来源：http://qsg.kuanghao11.cn

Perl ........... 10
来源：http://jja.guannengcc.top

Scala .......... 10
来源：http://dgv.andypj.xyz

------------------------------------
来源：http://qgj.hysaishi.cn

合计 ........... 2106 条
来源：http://hjv.shanyushiyangtech.top

按章节统计：
来源：http://qqm.ydzc1.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fkq.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bvo.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tvu.yanxiufei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://csy.jinqigufen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fzg.hesvh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://koi.jqgufenzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lxs.mhx1999.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zbe.haohaochexian.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://byp.iojbl.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://thz.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nmc.yueranfly.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://srb.ppjwa.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dsl.ybcxt.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://shs.quarkkingdee.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fef.sweek.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ehd.jinghuilouyu.cn

Q SQL 专题                              90
来源：http://gyz.jiagoushi.top

R Bash 专题                             80
来源：http://cfa.kuanghao11.cn

S C / C++ 专题                          60
来源：http://ryu.guowangkeji.top

T 其他语言补充                          60
来源：http://kjx.andypj.xyz

U 高频实用片段                         120
来源：http://arn.zhongyouzk.top

------------------------------------
来源：http://dxl.zdbjq.cn

合计                                  2106 条
来源：http://xyu.52xcode.cn

--------------------------------------------------------------------------------
来源：http://ktt.aibaodan.cn

使用提醒
来源：http://mtu.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://nlb.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wpo.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://stt.vehdjk.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cwi.sxryk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fxg.jinqigufen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cjf.jinqigfzy.top

—— 文件结束 ——
来源：http://olr.ppjwa.cn

================================================================================
来源：http://xiy.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://ksx.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://iiu.316326.xyz

================================================================================
来源：http://csi.nanxinkj.top

【收录内容】
来源：http://xzs.gotoacloud.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lui.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cnk.guowangkeji.top

SQL · Bash · C · C++
来源：http://vxv.fengsongda.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cse.jinqigufen.top

【使用说明】
来源：http://vyb.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://awc.ctjpmb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vkk.chenzaomai.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://edt.hongshengwenyu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gwq.smart0.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://ehd.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qjp.pycfn.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://amw.uphjek.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pav.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://thv.shangyingyoupin.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://flr.chenlongwang.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://axf.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zrq.9152youxi.cn

【文件统计】
来源：http://hjf.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cxd.bjfxy.top

--------------------------------------------------------------------------------
来源：http://kxk.9152youxi.cn

目  录
来源：http://hbk.hammf.cn

--------------------------------------------------------------------------------
来源：http://ktx.aizwys.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://luf.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pwu.daria6918.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://iol.yvedp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zgq.mhx1999.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://srs.sufxvd.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://npf.xinyue.icu

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ddb.316326.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://htq.quarkkingdee.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hxd.jinqigfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mlc.guannengcc.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://elg.9152youxi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cqw.ppjwa.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ntu.jinyuanbaomall.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://owr.feifeiyinyue.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://grf.nanxuanxn.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fbm.jyoumei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rjs.dianchejie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jcb.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://din.jinqigufen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ulw.gzhubu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qzr.jianghu66.top

================================================================================
来源：http://uvo.jinqigufen.top

A. 基础语法与类型
来源：http://yer.fengsongda.top

================================================================================
来源：http://ujf.yj202588.top

[A01] Hello World
来源：http://hue.yj202588.top

Py:   print("Hello, World!")
来源：http://vof.hesvh.cn

PHP:  echo "Hello, World!";
来源：http://fis.yj20258888.top

JS:   console.log("Hello, World!");
来源：http://ysz.c1oappe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pim.shanyushiyangtech.top

Java: System.out.println("Hello, World!");
来源：http://ujg.iojbl.cn

Go:   fmt.Println("Hello, World!")
来源：http://pxz.fengsongda.top

Ruby: puts "Hello, World!"
来源：http://ffy.xziqi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://aqp.sweek.top

[A02] 变量声明与赋值
来源：http://lgz.fanxiaobao.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wno.jinqigufen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ieu.0kj1m.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bgr.ppjwa.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tpp.jinqigufen.top

Java: String name = "Alex"; int age = 20;
来源：http://yhb.shanyushiyangtech.top

Go:   name := "Alex"; age := 20
来源：http://hyw.chenjidiqi.icu

Ruby: name = "Alex"; age = 20
来源：http://euh.shangyingyoupin.top

C#:   string name = "Alex"; int age = 20;
来源：http://srw.fehbvm.com

[A03] 常量定义
来源：http://tnz.jinqigfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://etj.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://ace.gzhubu.top

JS:   const PI = 3.14159;
来源：http://zpf.guannengcc.top

TS:   const PI: number = 3.14159;
来源：http://ict.shuidangran.top

Java: static final double PI = 3.14159;
来源：http://ztx.cheryme.top

Go:   const PI = 3.14159
来源：http://met.chenlongwang.top

Ruby: PI = 3.14159
来源：http://zeo.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://aig.zhiwuduotai.top

[A04] 判断变量类型
来源：http://cdg.bbcook.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://geu.cdnleiting.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dlp.pycfn.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://npx.pengpengdd.cyou

TS:   typeof x; x instanceof Date
来源：http://ulx.jqgufenzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://awl.shuidangran.top

Go:   reflect.TypeOf(x).Name()
来源：http://jhv.fzhhl.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cal.jqgufenzy.top

C#:   x.GetType().Name; x is int
来源：http://wxf.daxiang520.top

[A05] 整数除法与取模
来源：http://dmi.meibo888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tgs.ydjk.org.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hap.aizwys.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ouu.jqgfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fyr.cheryme.top

Java: 7 / 2; 7 % 2
来源：http://cba.wangshuangyany.cn

Go:   7 / 2; 7 % 2
来源：http://rzj.ehwqpu.com

Ruby: 7 / 2; 7 % 2
来源：http://hsb.c1oappe.top

C#:   7 / 2; 7 % 2
来源：http://uqw.tarul.cn

[A06] 字符串转数字
来源：http://qgf.cheryme.top

Py:   int("42"); float("3.14")
来源：http://pog.yuanzhike.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jmv.feifeiyinyue.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ojq.sysykeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://suv.bjfxy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wii.shuidangran.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mee.yangfankeji.com

Ruby: "42".to_i; "3.14".to_f
来源：http://tlv.quarkkingdee.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://krd.nwbrower.top

[A07] 数字转字符串
来源：http://bpa.zhengqikj.top

Py:   str(42)
来源：http://qur.nanxuanxn.top

PHP:  (string) 42; strval(42)
来源：http://bjd.haohaochexian.top

JS:   String(42); (42).toString()
来源：http://azq.xuanzx.com

TS:   String(42)
来源：http://lvl.yanxiufei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://coq.nwbrower.top

Go:   strconv.Itoa(42)
来源：http://zxz.hysaishi.cn

Ruby: 42.to_s
来源：http://qtp.zhoulong.xyz

C#:   42.ToString()
来源：http://vhb.jinyuanbaomall.cn

[A08] 取整与四舍五入
来源：http://xbu.ywan-chungtsiang.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hcq.chenjidiqi.icu

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dag.jinghuilouyu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vlp.jianghu66.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sxv.jianghu66.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://itb.cdnleiting.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ukg.gotoacloud.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://avj.sxryk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zoc.yfazqb.com

[A09] 绝对值与最大最小值
来源：http://rmt.zhiwuduotai.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zdy.yongpay.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bna.hesvh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://muh.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mjx.fengsongda.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eak.yvedp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dva.sjlbkw.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cwd.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nup.shuidangran.top

[A10] 生成随机数
来源：http://gzf.yfazqb.com

Py:   import random; random.randint(1, 100)
来源：http://cez.hysaishi.cn

PHP:  random_int(1, 100);
来源：http://nws.sxryk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ftz.ydzc1.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://alk.redwolf501.top

Java: new Random().nextInt(100) + 1
来源：http://vjh.havefunace.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://egk.jlsjyb.cn

Ruby: rand(1..100)
来源：http://rqn.redwolf501.top

C#:   new Random().Next(1, 101)
来源：http://tjm.hesvh.cn

[A11] 条件表达式（三元）
来源：http://fal.birdmap.top

Py:   "yes" if x > 0 else "no"
来源：http://dyv.hcnkem.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://wyo.shuidangran.top

JS:   x > 0 ? "yes" : "no"
来源：http://dpq.cucudq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cqt.pengpengdd.cyou

Java: x > 0 ? "yes" : "no"
来源：http://dwj.xinyue.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://wyr.zhixingplan.top

Ruby: x > 0 ? "yes" : "no"
来源：http://chc.0kj1m.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zca.ydjk.org.cn

[A12] 字符串插值 / 格式化
来源：http://npr.ppjwa.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xyy.yuxming.cn


<!-- 参考信息 -->