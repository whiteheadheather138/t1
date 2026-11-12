代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://ctd.hfpthk.cn

parse_ini_file("config.ini", true)
来源：http://xgc.jiagoushi.top

[U74] PHP：读取环境变量
来源：http://hjs.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://whz.hywenlv.cn

[U75] PHP：依赖注入
来源：http://gba.316326.xyz

composer require psr/container
来源：http://dop.bbcook.cn

[U76] PHP：简单路由
来源：http://lmh.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fxs.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://jbv.zhaomingkeji.xyz

composer require twig/twig
来源：http://rnc.ehwqpu.com

[U78] PHP：单元测试
来源：http://iri.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://uoj.yuxming.cn

[U79] PHP：静态分析
来源：http://vkl.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://kkq.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://cqk.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jti.meibo888.top

[U81] JS：初始化项目
来源：http://xie.yj20258.top

npm init -y;  npm i express
来源：http://uvm.gogol.net.cn

[U82] JS：package.json 脚本
来源：http://xff.jinyuanbaomall.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xpx.jqgufenzy.top

[U83] JS：ES Module 导入导出
来源：http://uxl.nanxinkj.top

export const a = 1;  import { a } from "./m.js";
来源：http://ofv.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://yzt.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://bnh.guowangkeji.top

[U85] JS：可选链
来源：http://qar.xinyue.icu

a?.b?.c
来源：http://cux.52xcode.cn

[U86] JS：空值合并
来源：http://wbb.gotoacloud.top

a ?? b
来源：http://evb.yueranfly.top

[U87] JS：解构默认值
来源：http://zgm.nanxinkj.top

const { a = 1, b = 2 } = obj;
来源：http://pai.cheryme.top

[U88] JS：对象展开合并
来源：http://oxr.sjlbkw.cn

{ ...a, ...b }
来源：http://blx.guowangkeji.top

[U89] JS：数组去重
来源：http://zkz.shanyushiyangkeji.top

[...new Set(arr)]
来源：http://lmb.svipenyu.cn

[U90] JS：数字数组排序
来源：http://lpf.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://amr.svipenyu.cn

[U91] JS：对象键值遍历
来源：http://tkl.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hof.yvedp.cn

[U92] JS：深拷贝
来源：http://cyr.sysykeji.top

structuredClone(obj)
来源：http://hvg.hywenlv.cn

[U93] JS：模板字符串
来源：http://fcl.yj20258.top

`共 ${n} 条`
来源：http://hpy.hysaishi.cn

[U94] JS：箭头函数
来源：http://qle.tianlin.xyz

const double = x => x * 2;
来源：http://mvd.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://eke.sweek.top

new Promise((resolve, reject) => {})
来源：http://hso.redwolf501.top

[U96] JS：async/await 与异常
来源：http://oun.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dyb.hnqzz.top

[U97] JS：并发请求
来源：http://ihc.zhengqikj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ohk.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://hgz.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kdo.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://hiv.quarkkingdee.top

el.addEventListener("click", e => {})
来源：http://eut.ywan-chungtsiang.top

[U100] JS：DOM 查询
来源：http://hjc.chenlongwang.top

document.querySelector(".item")
来源：http://mxt.tianlin.xyz

[U101] JS：classList 操作
来源：http://ywb.shangyingyoupin.top

el.classList.toggle("active")
来源：http://mkv.9152youxi.cn

[U102] JS：本地存储
来源：http://hmp.hcnkem.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://iuv.sysykeji.top

[U103] JS：定时器
来源：http://cva.jinqigufen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kne.hnqzz.top

[U104] JS：防抖
来源：http://vyi.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hiv.aizwys.cn

[U105] JS：节流
来源：http://odq.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://osm.smart0.xyz

[U106] JS：日期格式化
来源：http://kpc.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aih.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://fek.xylfe.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nuj.meibo888.top

[U108] JS：随机整数
来源：http://nhv.ybcxt.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xzb.pengpengdd.cyou

[U109] JS：数组分组
来源：http://ckw.pycfn.com

Object.groupBy(arr, x => x.type)
来源：http://baz.hammf.cn

[U110] JS：数组分块
来源：http://rbm.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ylx.zycfv.cn

[U111] JS：对象转 Map
来源：http://zli.hfpthk.cn

new Map(Object.entries(obj))
来源：http://rjj.fktsv.cn

[U112] JS：字符串补位
来源：http://vbm.yonumen.top

"7".padStart(3, "0")
来源：http://jsm.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://orm.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://xks.meibo888.top

[U114] JS：JSON 深比较
来源：http://ens.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ida.cashguo.top

[U115] JS：生成 UUID
来源：http://tje.xziqi.cn

crypto.randomUUID()
来源：http://gyp.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://tmf.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://ozo.hongshengwenyu.top

[U117] JS：单元测试
来源：http://tyb.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://tpw.jlsjyb.cn

[U118] JS：开发服务器
来源：http://sdn.sysykeji.top

npm i -D vite;  npx vite
来源：http://pjk.hnxiangtu.top

[U119] JS：生产构建
来源：http://wis.jinghuilouyu.cn

npx vite build
来源：http://txs.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://lfl.guannengcc.top

import.meta.env.VITE_API_URL
来源：http://ysm.wangshuangyany.cn

================================================================================
来源：http://eec.ydjk.org.cn

统计汇总
来源：http://upf.kuanghao11.cn

================================================================================
来源：http://fbc.yvedp.cn

按语言统计（条）：
来源：http://tri.hcnkem.com

Python ......... 252
来源：http://nhu.fanxiaobao.xyz

PHP ............ 252
来源：http://ito.nanxuanxn.top

JavaScript ..... 252
来源：http://lmz.hysaishi.cn

TypeScript ..... 212
来源：http://ych.kuanghao11.cn

Java ........... 212
来源：http://fts.shuidangran.top

Go ............. 212
来源：http://fdk.zhaomingkeji.xyz

Ruby ........... 212
来源：http://cpm.gogol.net.cn

C# ............. 212
来源：http://rzl.zhiwuduotai.top

C .............. 30
来源：http://kyp.sysykeji.top

C++ ............ 30
来源：http://zeu.dashuyun.cn

SQL ............ 90
来源：http://yeq.ydjk.org.cn

Bash ........... 80
来源：http://lqs.0kj1m.cn

Kotlin ......... 15
来源：http://kvg.cheryme.top

Swift .......... 15
来源：http://dbu.shangyingyoupin.top

Lua ............ 10
来源：http://jdl.hywenlv.cn

Perl ........... 10
来源：http://skl.vqdsnc.cn

Scala .......... 10
来源：http://bxf.9152youxi.cn

------------------------------------
来源：http://mbg.zhiwuduotai.top

合计 ........... 2106 条
来源：http://gix.dianchejie.cn

按章节统计：
来源：http://sjj.hywenlv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eyt.shanyushiyangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qif.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iww.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://twl.feifeiyinyue.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blk.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://txa.pycfn.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yqr.zdqjudy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xxr.fzhhl.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://txc.zhoulong.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mox.cheryme.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tsi.ctjpmb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mba.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xih.cheryme.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xwc.zycfv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iug.yangfankeji.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cim.fanxiaobao.xyz

Q SQL 专题                              90
来源：http://tly.shanyushiyangtech.top

R Bash 专题                             80
来源：http://uab.hywenlv.cn

S C / C++ 专题                          60
来源：http://mqd.svipenyu.cn

T 其他语言补充                          60
来源：http://gup.ivvv.top

U 高频实用片段                         120
来源：http://qtv.fanxiaobao.xyz

------------------------------------
来源：http://xpp.zhengqikj.top

合计                                  2106 条
来源：http://zap.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://ujl.nanxuanxn.top

使用提醒
来源：http://gyx.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://obi.zhixingplan.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gvb.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dhr.aizwys.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fhu.bbcook.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hpx.tianlin.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://btm.hnxiangtu.top

—— 文件结束 ——
来源：http://bwd.shanyushiyangtech.top

================================================================================
来源：http://vie.cheryme.top

程序语言常见例子速查手册（2024 版）
来源：http://trb.hywenlv.cn

Common Programming Examples Cheat Book
来源：http://lfy.gotoacloud.top

================================================================================
来源：http://eem.chenzaomai.com

【收录内容】
来源：http://fuk.yuanzhike.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lew.aizwys.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://szx.tarul.cn

SQL · Bash · C · C++
来源：http://rvo.fktsv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://obz.aibaodan.cn

【使用说明】
来源：http://buq.zycfv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zir.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://epq.cucudq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ztx.bbcook.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qoo.dashuyun.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://moq.316326.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wqf.zdqjudy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vsd.316326.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://eik.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rkd.fzhhl.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lmk.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eyq.vqdsnc.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tdi.fktsv.cn

【文件统计】
来源：http://euo.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fln.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://uer.yonumen.top

目  录
来源：http://eoy.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://zvu.bjfxy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jbx.52xcode.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://htc.vehdjk.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bth.jinyuanbaomall.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zhn.jinghuilouyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://olw.gotoacloud.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oog.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fyw.yj202588.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tfz.dashuyun.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zbm.0kj1m.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gym.gzhubu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zye.jiagoushi.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dra.0kj1m.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://los.cashguo.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rbl.yj20258888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://khj.9152youxi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lgs.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uhj.hongshengwenyu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://pjn.yanxiufei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://unt.yuanzhike.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ivf.ctjpmb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kan.dianchejie.cn

================================================================================
来源：http://qqf.xingfuxueyuan.xyz

A. 基础语法与类型
来源：http://vkp.xinyue.icu

================================================================================
来源：http://onw.sysykeji.top

[A01] Hello World
来源：http://erm.hfpthk.cn

Py:   print("Hello, World!")
来源：http://wiz.uphjek.com

PHP:  echo "Hello, World!";
来源：http://pkj.mhx1999.top

JS:   console.log("Hello, World!");
来源：http://nmw.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://czf.fktsv.cn

Java: System.out.println("Hello, World!");
来源：http://ttt.yuanzhike.top

Go:   fmt.Println("Hello, World!")
来源：http://ycn.cdnleiting.top

Ruby: puts "Hello, World!"
来源：http://olp.nanxuanxn.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bly.jqgfzy.top

[A02] 变量声明与赋值
来源：http://xfc.bbcook.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qya.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pte.guowangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://sdu.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qgw.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://gmt.wangdashe.top

Go:   name := "Alex"; age := 20
来源：http://nzf.havefunace.top

Ruby: name = "Alex"; age = 20
来源：http://oqa.jianghu66.top

C#:   string name = "Alex"; int age = 20;
来源：http://gfv.zycfv.cn

[A03] 常量定义
来源：http://ilf.tanke756.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ovi.daria6918.cn

PHP:  const PI = 3.14159;
来源：http://isk.meibo888.top

JS:   const PI = 3.14159;
来源：http://efx.xylfe.cn

TS:   const PI: number = 3.14159;
来源：http://uff.ehwqpu.com

Java: static final double PI = 3.14159;
来源：http://ttc.andypj.xyz

Go:   const PI = 3.14159
来源：http://num.fanxiaobao.xyz

Ruby: PI = 3.14159
来源：http://zsn.tanke756.top

C#:   const double PI = 3.14159;
来源：http://kyh.haohaochexian.top

[A04] 判断变量类型
来源：http://eqz.yj20258888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ftj.jinyuanbaomall.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ksr.hysaishi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ssb.shangyingyoupin.top

TS:   typeof x; x instanceof Date
来源：http://ewf.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mou.ybcxt.top

Go:   reflect.TypeOf(x).Name()
来源：http://cvi.yanxiufei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://liy.jqgfzy.top

C#:   x.GetType().Name; x is int
来源：http://rdf.chenzaomai.com

[A05] 整数除法与取模
来源：http://cic.hysaishi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gxi.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hij.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://erj.kuanghao11.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kiv.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://tkw.yangfankeji.com

Go:   7 / 2; 7 % 2
来源：http://uqq.meibo888.top

Ruby: 7 / 2; 7 % 2
来源：http://btc.hnxiangtu.top

C#:   7 / 2; 7 % 2
来源：http://tnw.shzxlz.cn

[A06] 字符串转数字
来源：http://rje.ppjwa.cn

Py:   int("42"); float("3.14")
来源：http://zfc.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mlo.jinghuilouyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pxd.zhengqikj.top

TS:   parseInt("42", 10); Number("42")
来源：http://glc.hfpthk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://awa.shanyushiyangtech.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bkk.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://ekg.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lxb.yj20258.top

[A07] 数字转字符串
来源：http://opf.andypj.xyz

Py:   str(42)
来源：http://fyf.ybcxt.top

PHP:  (string) 42; strval(42)
来源：http://qve.tanke756.top

JS:   String(42); (42).toString()
来源：http://psl.fengsongda.top

TS:   String(42)
来源：http://iif.fktsv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://odw.shuidangran.top

Go:   strconv.Itoa(42)
来源：http://hsj.ivvv.top

Ruby: 42.to_s
来源：http://ggu.zhengqikj.top

C#:   42.ToString()
来源：http://stz.mhx1999.top

[A08] 取整与四舍五入
来源：http://mgl.hnxiangtu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wjx.pengpengdd.cyou

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tpd.yonumen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hxa.bjfxy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ytx.hongshengwenyu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ocv.zhoulong.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ecs.jiagoushi.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jgf.redwolf501.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gyp.jqgfzy.top

[A09] 绝对值与最大最小值
来源：http://kmu.jqgufenzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nex.0kj1m.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aog.cqqwz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://osn.tian-w.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sda.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nxf.yvedp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rub.jinqigufen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ahx.nanxinkj.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://evq.dashuyun.cn

[A10] 生成随机数
来源：http://jnm.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://whl.zhiwuduotai.top

PHP:  random_int(1, 100);
来源：http://gvj.cucudq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://umj.pycfn.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zew.wangdashe.top

Java: new Random().nextInt(100) + 1
来源：http://ndu.ehwqpu.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://snu.fanxiaobao.xyz

Ruby: rand(1..100)
来源：http://opg.hammf.cn

C#:   new Random().Next(1, 101)
来源：http://igt.jiagoushi.top

[A11] 条件表达式（三元）
来源：http://wph.birdmap.top

Py:   "yes" if x > 0 else "no"
来源：http://wod.zhijiandao.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cub.tianlin.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://sia.aibaodan.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kej.xuetiantiany.cn

Java: x > 0 ? "yes" : "no"
来源：http://kwo.zycfv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fsp.zhijiandao.cn


<!-- 参考信息 -->