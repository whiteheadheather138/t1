代发 wailian999

[U71] PHP：抛出异常
来源：http://atr.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://stf.hcnkem.com

[U72] PHP：写错误日志
来源：http://jwi.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://kuu.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://mqg.pengpengdd.cyou

parse_ini_file("config.ini", true)
来源：http://zbf.jyoumei.cn

[U74] PHP：读取环境变量
来源：http://ead.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://jfg.aibaodan.cn

[U75] PHP：依赖注入
来源：http://ohe.chenjidiqi.icu

composer require psr/container
来源：http://rlt.nanxinkj.top

[U76] PHP：简单路由
来源：http://rxu.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jdb.jinqigufen.top

[U77] PHP：模板渲染
来源：http://sxf.aizwys.cn

composer require twig/twig
来源：http://ujd.vqdsnc.cn

[U78] PHP：单元测试
来源：http://iki.fehbvm.com

composer require --dev phpunit/phpunit
来源：http://bgj.ybcxt.top

[U79] PHP：静态分析
来源：http://eiz.fzhhl.top

composer require --dev phpstan/phpstan
来源：http://gcv.9152youxi.cn

[U80] PHP：代码规范修复
来源：http://zhl.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hjx.yj20258.top

[U81] JS：初始化项目
来源：http://jtt.aibaodan.cn

npm init -y;  npm i express
来源：http://awc.redwolf501.top

[U82] JS：package.json 脚本
来源：http://wkl.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nuq.sxryk.cn

[U83] JS：ES Module 导入导出
来源：http://udy.xuetiantiany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zed.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://gty.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://fwq.havefunace.top

[U85] JS：可选链
来源：http://zgp.chenlongwang.top

a?.b?.c
来源：http://rrg.cashguo.top

[U86] JS：空值合并
来源：http://uxt.haohaochexian.top

a ?? b
来源：http://kwi.nwbrower.top

[U87] JS：解构默认值
来源：http://hop.mhx1999.top

const { a = 1, b = 2 } = obj;
来源：http://dzo.yuanzhike.top

[U88] JS：对象展开合并
来源：http://lfj.shzxlz.cn

{ ...a, ...b }
来源：http://mka.ivvv.top

[U89] JS：数组去重
来源：http://mem.guannengcc.top

[...new Set(arr)]
来源：http://vmg.wangdashe.top

[U90] JS：数字数组排序
来源：http://xui.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://gyn.gotoacloud.top

[U91] JS：对象键值遍历
来源：http://uhu.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wji.yj20258.top

[U92] JS：深拷贝
来源：http://xwa.xuetiantiany.cn

structuredClone(obj)
来源：http://cur.havefunace.top

[U93] JS：模板字符串
来源：http://mkt.c1oappe.top

`共 ${n} 条`
来源：http://ogy.jinqigfzy.top

[U94] JS：箭头函数
来源：http://fks.sysykeji.top

const double = x => x * 2;
来源：http://qne.aizwys.cn

[U95] JS：Promise 包装
来源：http://irq.ybcxt.top

new Promise((resolve, reject) => {})
来源：http://rth.guannengcc.top

[U96] JS：async/await 与异常
来源：http://qop.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uvf.hnqzz.top

[U97] JS：并发请求
来源：http://sjo.epnwcf.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://deu.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://ytb.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gdg.haohaochexian.top

[U99] JS：事件监听
来源：http://fpk.daria6918.cn

el.addEventListener("click", e => {})
来源：http://osw.52xcode.cn

[U100] JS：DOM 查询
来源：http://nyk.jqgufenzy.top

document.querySelector(".item")
来源：http://zcs.zycfv.cn

[U101] JS：classList 操作
来源：http://enz.0kj1m.cn

el.classList.toggle("active")
来源：http://nhu.chenjidiqi.icu

[U102] JS：本地存储
来源：http://chh.shzxlz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vex.cashguo.top

[U103] JS：定时器
来源：http://zpu.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tsj.zhijiandao.cn

[U104] JS：防抖
来源：http://jft.tarul.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mxc.yuanzhike.top

[U105] JS：节流
来源：http://xpv.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iii.shuidangran.top

[U106] JS：日期格式化
来源：http://vae.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vqy.aibaodan.cn

[U107] JS：数字千分位
来源：http://hbd.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mkx.yuxming.cn

[U108] JS：随机整数
来源：http://rrz.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cbs.snrcjt.cn

[U109] JS：数组分组
来源：http://zcq.gaohongyu789.top

Object.groupBy(arr, x => x.type)
来源：http://wni.birdmap.top

[U110] JS：数组分块
来源：http://qqy.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vrq.zycfv.cn

[U111] JS：对象转 Map
来源：http://iqj.ywan-chungtsiang.top

new Map(Object.entries(obj))
来源：http://xqq.sufxvd.cn

[U112] JS：字符串补位
来源：http://rtl.jqgfzy.top

"7".padStart(3, "0")
来源：http://hhk.cdnleiting.top

[U113] JS：正则替换全部
来源：http://xve.yj20258888.top

s.replaceAll("a", "b")
来源：http://ikd.uphjek.com

[U114] JS：JSON 深比较
来源：http://pxe.shzxlz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qrw.ppjwa.cn

[U115] JS：生成 UUID
来源：http://xjz.ydzc1.top

crypto.randomUUID()
来源：http://igr.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://aze.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://ydy.jiagoushi.top

[U117] JS：单元测试
来源：http://kkq.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://dtq.yangfankeji.com

[U118] JS：开发服务器
来源：http://hlg.zycfv.cn

npm i -D vite;  npx vite
来源：http://sen.jianghu66.top

[U119] JS：生产构建
来源：http://tis.guowangkeji.top

npx vite build
来源：http://jhw.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://hou.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://zwf.jinqigufen.top

================================================================================
来源：http://jzp.52xcode.cn

统计汇总
来源：http://wdq.yj20258888.top

================================================================================
来源：http://vqd.ywan-chungtsiang.top

按语言统计（条）：
来源：http://haq.feifeiyinyue.top

Python ......... 252
来源：http://sye.zycfv.cn

PHP ............ 252
来源：http://prv.tian-w.cn

JavaScript ..... 252
来源：http://xsd.yangfankeji.com

TypeScript ..... 212
来源：http://hny.316326.xyz

Java ........... 212
来源：http://tsq.hywenlv.cn

Go ............. 212
来源：http://nue.smart0.xyz

Ruby ........... 212
来源：http://wns.yonumen.top

C# ............. 212
来源：http://urd.haohaochexian.top

C .............. 30
来源：http://cvj.havefunace.top

C++ ............ 30
来源：http://lle.zhengqikj.top

SQL ............ 90
来源：http://vot.jinghuilouyu.cn

Bash ........... 80
来源：http://jtx.svipenyu.cn

Kotlin ......... 15
来源：http://vei.wangshuangyany.cn

Swift .......... 15
来源：http://doa.hammf.cn

Lua ............ 10
来源：http://mva.epnwcf.com

Perl ........... 10
来源：http://rig.hammf.cn

Scala .......... 10
来源：http://tkf.redwolf501.top

------------------------------------
来源：http://sgy.ybcxt.top

合计 ........... 2106 条
来源：http://omk.hfpthk.cn

按章节统计：
来源：http://kyt.zhengqikj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jiu.xuanzx.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nzo.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jjs.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ttn.zdqjudy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uha.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baq.cucudq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://otk.ydzc1.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tad.tianlin.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://exd.smart0.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ofw.shanyushiyangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hlp.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pvg.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nkp.316326.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sli.dashuyun.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hss.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rys.cashguo.top

Q SQL 专题                              90
来源：http://pfd.yangfankeji.com

R Bash 专题                             80
来源：http://eno.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://ljd.chenlongwang.top

T 其他语言补充                          60
来源：http://pvu.hnxiangtu.top

U 高频实用片段                         120
来源：http://pxy.yangfankeji.com

------------------------------------
来源：http://wud.aibaodan.cn

合计                                  2106 条
来源：http://lvv.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://ehq.pycfn.com

使用提醒
来源：http://nut.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://cxt.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ijx.chenjidiqi.icu

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zcc.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ors.meibo888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://whu.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rbv.yongpay.top

—— 文件结束 ——
来源：http://dde.jiagoushi.top

================================================================================
来源：http://vlo.yueranfly.top

程序语言常见例子速查手册（2024 版）
来源：http://eyu.zycfv.cn

Common Programming Examples Cheat Book
来源：http://zxt.nanxuanxn.top

================================================================================
来源：http://ppm.cucudq.cn

【收录内容】
来源：http://akh.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://irl.hcnkem.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nkb.yongpay.top

SQL · Bash · C · C++
来源：http://ieh.cashguo.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oau.redwolf501.top

【使用说明】
来源：http://qsh.ybcxt.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://myr.chenzaomai.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://apy.shangyingyoupin.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tkk.kuanghao11.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dwu.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://onk.aibaodan.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iey.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jyr.ybcxt.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xbo.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ups.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://adg.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vro.shzxlz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qcl.shzxlz.cn

【文件统计】
来源：http://jzd.9152youxi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ixb.tanke756.top

--------------------------------------------------------------------------------
来源：http://maq.jinyuanbaomall.cn

目  录
来源：http://mjk.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://ipp.sufxvd.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pkf.c1oappe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zsu.jiagoushi.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gih.hnxiangtu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eph.gzhubu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jee.zhengqikj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gcz.sweek.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gzl.shanyushiyangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gjh.ehwqpu.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jgg.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mkn.sysykeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eez.yj20258.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bvj.jyoumei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qec.gogol.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vzc.cqqwz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jid.feifeiyinyue.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://eca.shangyingyoupin.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jcs.sufxvd.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lkb.zdbjq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dbv.yj20258.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://esh.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lby.zhijiandao.cn

================================================================================
来源：http://kpv.vehdjk.com

A. 基础语法与类型
来源：http://nte.shanyushiyangkeji.top

================================================================================
来源：http://hpl.tanke756.top

[A01] Hello World
来源：http://vyc.jqgufenzy.top

Py:   print("Hello, World!")
来源：http://zcy.fzhhl.top

PHP:  echo "Hello, World!";
来源：http://wwc.nwbrower.top

JS:   console.log("Hello, World!");
来源：http://shy.yvedp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ypc.tian-w.cn

Java: System.out.println("Hello, World!");
来源：http://uuq.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://unm.cheryme.top

Ruby: puts "Hello, World!"
来源：http://xrr.yj20258888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hou.birdmap.top

[A02] 变量声明与赋值
来源：http://run.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fmp.gotoacloud.top

PHP:  $name = "Alex"; $age = 20;
来源：http://upa.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://lyb.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kxy.ppjwa.cn

Java: String name = "Alex"; int age = 20;
来源：http://uzo.bbcook.cn

Go:   name := "Alex"; age := 20
来源：http://rqb.ctjpmb.com

Ruby: name = "Alex"; age = 20
来源：http://ixv.svipenyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nho.316326.xyz

[A03] 常量定义
来源：http://bgr.dianchejie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://shp.hysaishi.cn

PHP:  const PI = 3.14159;
来源：http://duj.redwolf501.top

JS:   const PI = 3.14159;
来源：http://kxb.sweek.top

TS:   const PI: number = 3.14159;
来源：http://qed.yj202588.top

Java: static final double PI = 3.14159;
来源：http://dri.xuanzx.com

Go:   const PI = 3.14159
来源：http://cav.ydzc1.top

Ruby: PI = 3.14159
来源：http://ijo.havefunace.top

C#:   const double PI = 3.14159;
来源：http://njs.feifeiyinyue.top

[A04] 判断变量类型
来源：http://nmi.sysykeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://sjw.fktsv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mrk.shzxlz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dlb.sxryk.cn

TS:   typeof x; x instanceof Date
来源：http://jxg.chenzaomai.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qwu.jlsjyb.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oij.iojbl.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ufl.yangfankeji.com

C#:   x.GetType().Name; x is int
来源：http://klq.0kj1m.cn

[A05] 整数除法与取模
来源：http://mnf.dashuyun.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bml.epnwcf.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://sly.yfazqb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kqr.0kj1m.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://aqi.shanyushiyangkeji.top

Java: 7 / 2; 7 % 2
来源：http://ddi.yongpay.top

Go:   7 / 2; 7 % 2
来源：http://wxy.epnwcf.com

Ruby: 7 / 2; 7 % 2
来源：http://sjd.sweek.top

C#:   7 / 2; 7 % 2
来源：http://xre.kuanghao11.cn

[A06] 字符串转数字
来源：http://uez.yj20258.top

Py:   int("42"); float("3.14")
来源：http://mes.vehdjk.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hhg.zhiwuduotai.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fif.daria6918.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nmo.yanxiufei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vuu.zhiwuduotai.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wxc.yj202588.top

Ruby: "42".to_i; "3.14".to_f
来源：http://grj.cdnleiting.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wez.hnxiangtu.top

[A07] 数字转字符串
来源：http://pjl.yj20258.top

Py:   str(42)
来源：http://wha.birdmap.top

PHP:  (string) 42; strval(42)
来源：http://kva.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://yfb.yongpay.top

TS:   String(42)
来源：http://dkh.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wqq.xylfe.cn

Go:   strconv.Itoa(42)
来源：http://som.shangyingyoupin.top

Ruby: 42.to_s
来源：http://fcu.hfpthk.cn

C#:   42.ToString()
来源：http://lwa.dashuyun.cn

[A08] 取整与四舍五入
来源：http://ynw.shanyushiyangkeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://iai.nwbrower.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rus.yuanzhike.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dhl.sjlbkw.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pzo.sjlbkw.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wfh.zhengqikj.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cak.c1oappe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://tfv.shzxlz.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kqv.ywan-chungtsiang.top

[A09] 绝对值与最大最小值
来源：http://tet.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cry.yj20258888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rde.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oau.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tle.daria6918.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jdm.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fun.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dja.zhijiandao.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ibj.0kj1m.cn

[A10] 生成随机数
来源：http://muu.tanke756.top

Py:   import random; random.randint(1, 100)
来源：http://zmk.yuanzhike.top

PHP:  random_int(1, 100);
来源：http://kpv.gogol.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sth.zhiwuduotai.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://obu.yvedp.cn

Java: new Random().nextInt(100) + 1
来源：http://rdp.iojbl.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kzp.zhiwuduotai.top

Ruby: rand(1..100)
来源：http://iph.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://qts.uphjek.com

[A11] 条件表达式（三元）
来源：http://lwf.zdbjq.cn

Py:   "yes" if x > 0 else "no"
来源：http://kdu.hnxiangtu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mct.chenzaomai.com


<!-- 参考信息 -->