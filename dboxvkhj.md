代发 wailian999

[U75] PHP：依赖注入
来源：http://bbp.haohaochexian.top

composer require psr/container
来源：http://mkv.hysaishi.cn

[U76] PHP：简单路由
来源：http://bxp.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lyl.hywenlv.cn

[U77] PHP：模板渲染
来源：http://hiq.chenlongwang.top

composer require twig/twig
来源：http://jey.ivvv.top

[U78] PHP：单元测试
来源：http://qnt.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://ykg.nanxuanxn.top

[U79] PHP：静态分析
来源：http://oao.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://axq.xinyue.icu

[U80] PHP：代码规范修复
来源：http://ncd.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qad.nanxuanxn.top

[U81] JS：初始化项目
来源：http://xrk.tarul.cn

npm init -y;  npm i express
来源：http://rdx.mhx1999.top

[U82] JS：package.json 脚本
来源：http://pfm.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://htw.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://zep.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bwe.dashuyun.cn

[U84] JS：CommonJS 写法
来源：http://jmb.smart0.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://rez.aibaodan.cn

[U85] JS：可选链
来源：http://alj.ydzc1.top

a?.b?.c
来源：http://gsl.guannengcc.top

[U86] JS：空值合并
来源：http://bjl.sweek.top

a ?? b
来源：http://rgs.nanxinkj.top

[U87] JS：解构默认值
来源：http://cbt.vqdsnc.cn

const { a = 1, b = 2 } = obj;
来源：http://ueg.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://srl.gaohongyu789.top

{ ...a, ...b }
来源：http://wmp.iojbl.cn

[U89] JS：数组去重
来源：http://blc.yfazqb.com

[...new Set(arr)]
来源：http://kxl.yfazqb.com

[U90] JS：数字数组排序
来源：http://sqq.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://mqk.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://swl.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cyl.tian-w.cn

[U92] JS：深拷贝
来源：http://vuf.jlsjyb.cn

structuredClone(obj)
来源：http://qxc.daxiang520.top

[U93] JS：模板字符串
来源：http://gaq.sxryk.cn

`共 ${n} 条`
来源：http://shw.c1oappe.top

[U94] JS：箭头函数
来源：http://mev.sweek.top

const double = x => x * 2;
来源：http://beb.xylfe.cn

[U95] JS：Promise 包装
来源：http://qoy.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://wuz.hongshengwenyu.top

[U96] JS：async/await 与异常
来源：http://vfk.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tib.gotoacloud.top

[U97] JS：并发请求
来源：http://vmq.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rqu.zhijiandao.cn

[U98] JS：fetch 带 JSON
来源：http://ftt.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fej.jinyuanbaomall.cn

[U99] JS：事件监听
来源：http://xrm.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://lkv.fanxiaobao.xyz

[U100] JS：DOM 查询
来源：http://mhv.52xcode.cn

document.querySelector(".item")
来源：http://icc.9152youxi.cn

[U101] JS：classList 操作
来源：http://mxa.xylfe.cn

el.classList.toggle("active")
来源：http://ipu.hesvh.cn

[U102] JS：本地存储
来源：http://lrv.hongshengwenyu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://axz.cdnleiting.top

[U103] JS：定时器
来源：http://cuu.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jnp.jinghuilouyu.cn

[U104] JS：防抖
来源：http://suh.jyoumei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qzq.chenlongwang.top

[U105] JS：节流
来源：http://kgx.nwbrower.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wbh.nanxuanxn.top

[U106] JS：日期格式化
来源：http://krz.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wiy.sjlbkw.cn

[U107] JS：数字千分位
来源：http://mno.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tut.sufxvd.cn

[U108] JS：随机整数
来源：http://jdz.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tvd.ctjpmb.com

[U109] JS：数组分组
来源：http://tjo.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://ycb.cqqwz.cn

[U110] JS：数组分块
来源：http://fnk.yueranfly.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lzt.jiagoushi.top

[U111] JS：对象转 Map
来源：http://skn.jqgfzy.top

new Map(Object.entries(obj))
来源：http://ezr.hesvh.cn

[U112] JS：字符串补位
来源：http://ojr.jqgufenzy.top

"7".padStart(3, "0")
来源：http://tze.nwbrower.top

[U113] JS：正则替换全部
来源：http://emb.tarul.cn

s.replaceAll("a", "b")
来源：http://zwl.ivvv.top

[U114] JS：JSON 深比较
来源：http://jxi.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://din.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://cqz.wangdashe.top

crypto.randomUUID()
来源：http://znf.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://lfn.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://yhh.daxiang520.top

[U117] JS：单元测试
来源：http://vya.nwbrower.top

npm i -D vitest;  npx vitest
来源：http://myo.guowangkeji.top

[U118] JS：开发服务器
来源：http://exq.gogol.net.cn

npm i -D vite;  npx vite
来源：http://ley.cheryme.top

[U119] JS：生产构建
来源：http://foj.hcnkem.com

npx vite build
来源：http://xpy.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://xwo.hammf.cn

import.meta.env.VITE_API_URL
来源：http://ioe.yuanzhike.top

================================================================================
来源：http://fpf.jianghu66.top

统计汇总
来源：http://vje.dianchejie.cn

================================================================================
来源：http://wzo.jlsjyb.cn

按语言统计（条）：
来源：http://dnx.yuxming.cn

Python ......... 252
来源：http://hmk.9152youxi.cn

PHP ............ 252
来源：http://xwh.fengsongda.top

JavaScript ..... 252
来源：http://trx.redwolf501.top

TypeScript ..... 212
来源：http://wsb.ctjpmb.com

Java ........... 212
来源：http://dzw.jiagoushi.top

Go ............. 212
来源：http://kge.ivvv.top

Ruby ........... 212
来源：http://udw.bbcook.cn

C# ............. 212
来源：http://sph.zhijiandao.cn

C .............. 30
来源：http://ndu.zhixingplan.top

C++ ............ 30
来源：http://fuo.sxryk.cn

SQL ............ 90
来源：http://rcl.svipenyu.cn

Bash ........... 80
来源：http://jlz.yuxming.cn

Kotlin ......... 15
来源：http://dii.cashguo.top

Swift .......... 15
来源：http://vvv.cheryme.top

Lua ............ 10
来源：http://byv.hammf.cn

Perl ........... 10
来源：http://eif.cashguo.top

Scala .......... 10
来源：http://axn.ydjk.org.cn

------------------------------------
来源：http://kua.shuidangran.top

合计 ........... 2106 条
来源：http://ion.xingfuxueyuan.xyz

按章节统计：
来源：http://cez.fktsv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xpe.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vow.hcnkem.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bbx.fehbvm.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rfw.jinghuilouyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dnl.tianlin.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qoi.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ehe.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://opz.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zpk.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zsp.wangshuangyany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wsg.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wpo.shuidangran.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://alm.zhiwuduotai.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yoa.zhongyouzk.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qga.xingfuxueyuan.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bfw.fanxiaobao.xyz

Q SQL 专题                              90
来源：http://oxm.shuidangran.top

R Bash 专题                             80
来源：http://oep.meibo888.top

S C / C++ 专题                          60
来源：http://oix.tanke756.top

T 其他语言补充                          60
来源：http://nhd.zhijiandao.cn

U 高频实用片段                         120
来源：http://jtv.kuanghao11.cn

------------------------------------
来源：http://zgt.jinyuanbaomall.cn

合计                                  2106 条
来源：http://ucq.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://taz.ydzc1.top

使用提醒
来源：http://fcb.ybcxt.top

--------------------------------------------------------------------------------
来源：http://ofw.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fnk.zhijiandao.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ien.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vyg.ydjk.org.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oig.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pgm.52xcode.cn

—— 文件结束 ——
来源：http://wcz.feifeiyinyue.top

================================================================================
来源：http://ypa.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://xtl.sjlbkw.cn

Common Programming Examples Cheat Book
来源：http://aog.jinqigfzy.top

================================================================================
来源：http://raq.feifeiyinyue.top

【收录内容】
来源：http://kmg.wangshuangyany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qma.zdqjudy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nzj.zhaomingkeji.xyz

SQL · Bash · C · C++
来源：http://vrt.guannengcc.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://knb.hfpthk.cn

【使用说明】
来源：http://wnk.hongshengwenyu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gzt.daria6918.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wah.andypj.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dkp.jinghuilouyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qll.ctjpmb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://aau.ydzc1.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eod.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wpe.zhengqikj.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lkj.yj20258888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ysw.gotoacloud.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rzy.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ekg.jinghuilouyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://foi.fanxiaobao.xyz

【文件统计】
来源：http://gdg.sjlbkw.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://viv.tarul.cn

--------------------------------------------------------------------------------
来源：http://thi.gotoacloud.top

目  录
来源：http://yax.xinyue.icu

--------------------------------------------------------------------------------
来源：http://iok.ybcxt.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mwo.yj20258.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zvt.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xhb.zhoulong.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://amm.zdbjq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hko.tian-w.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uio.zhoulong.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://clz.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://knn.zhoulong.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ssr.ydzc1.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ivz.smart0.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dxb.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zqh.ydjk.org.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mis.nanxinkj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kym.yuanzhike.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://afe.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pfl.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jui.jqgufenzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://gxc.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ejh.havefunace.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pxp.haohaochexian.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gta.yonumen.top

================================================================================
来源：http://qab.pengpengdd.cyou

A. 基础语法与类型
来源：http://pof.yonumen.top

================================================================================
来源：http://xfh.xziqi.cn

[A01] Hello World
来源：http://bxz.feifeiyinyue.top

Py:   print("Hello, World!")
来源：http://uro.shangyingyoupin.top

PHP:  echo "Hello, World!";
来源：http://ibn.kuanghao11.cn

JS:   console.log("Hello, World!");
来源：http://zxr.c1oappe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lws.daria6918.cn

Java: System.out.println("Hello, World!");
来源：http://yrv.zdbjq.cn

Go:   fmt.Println("Hello, World!")
来源：http://vln.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://jjv.zhixingplan.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vnr.hongshengwenyu.top

[A02] 变量声明与赋值
来源：http://mvh.aibaodan.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://igo.nanxuanxn.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zge.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://csw.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hvc.svipenyu.cn

Java: String name = "Alex"; int age = 20;
来源：http://pde.9152youxi.cn

Go:   name := "Alex"; age := 20
来源：http://hpp.hysaishi.cn

Ruby: name = "Alex"; age = 20
来源：http://wfu.zhixingplan.top

C#:   string name = "Alex"; int age = 20;
来源：http://xog.svipenyu.cn

[A03] 常量定义
来源：http://nbd.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dex.svipenyu.cn

PHP:  const PI = 3.14159;
来源：http://ufo.pycfn.com

JS:   const PI = 3.14159;
来源：http://too.wangshuangyany.cn

TS:   const PI: number = 3.14159;
来源：http://aah.fktsv.cn

Java: static final double PI = 3.14159;
来源：http://phh.bbcook.cn

Go:   const PI = 3.14159
来源：http://ute.bbcook.cn

Ruby: PI = 3.14159
来源：http://vlh.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://waq.shuidangran.top

[A04] 判断变量类型
来源：http://ivh.sufxvd.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xpy.hfpthk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vfh.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ken.jqgfzy.top

TS:   typeof x; x instanceof Date
来源：http://sop.dashuyun.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vdf.bjfxy.top

Go:   reflect.TypeOf(x).Name()
来源：http://obz.hfpthk.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mko.jinghuilouyu.cn

C#:   x.GetType().Name; x is int
来源：http://tit.gaohongyu789.top

[A05] 整数除法与取模
来源：http://tok.smart0.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uzh.yanxiufei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lbp.shuidangran.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xdx.yvedp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://akk.jinqigufen.top

Java: 7 / 2; 7 % 2
来源：http://tai.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://aur.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://ctc.jyoumei.cn

C#:   7 / 2; 7 % 2
来源：http://wkh.hfpthk.cn

[A06] 字符串转数字
来源：http://kda.chenjidiqi.icu

Py:   int("42"); float("3.14")
来源：http://yyi.tarul.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pus.fehbvm.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bmi.jqgfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://yts.ydzc1.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://des.cqqwz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://avi.xingfuxueyuan.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://gka.shangyingyoupin.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lby.ppjwa.cn

[A07] 数字转字符串
来源：http://ovq.hywenlv.cn

Py:   str(42)
来源：http://lpa.jqgufenzy.top

PHP:  (string) 42; strval(42)
来源：http://thn.jqgfzy.top

JS:   String(42); (42).toString()
来源：http://xfj.gotoacloud.top

TS:   String(42)
来源：http://gob.iojbl.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ewk.jlsjyb.cn

Go:   strconv.Itoa(42)
来源：http://bbm.epnwcf.com

Ruby: 42.to_s
来源：http://fwd.aibaodan.cn

C#:   42.ToString()
来源：http://xdb.ppjwa.cn

[A08] 取整与四舍五入
来源：http://piw.sjlbkw.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://weh.chenzaomai.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nvq.0kj1m.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bvz.kuanghao11.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://efx.xylfe.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rup.dashuyun.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sif.hnqzz.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jxb.feifeiyinyue.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hon.jiagoushi.top

[A09] 绝对值与最大最小值
来源：http://wza.52xcode.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rxa.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yfc.hfpthk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xtg.smart0.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vcg.sufxvd.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kso.ydjk.org.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jme.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dgb.hongshengwenyu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pem.ydzc1.top

[A10] 生成随机数
来源：http://ver.gogol.net.cn

Py:   import random; random.randint(1, 100)
来源：http://sdw.xingfuxueyuan.xyz

PHP:  random_int(1, 100);
来源：http://int.jinyuanbaomall.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://afx.shanyushiyangtech.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lhj.fzhhl.top

Java: new Random().nextInt(100) + 1
来源：http://mia.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ovi.iojbl.cn

Ruby: rand(1..100)
来源：http://axt.jlsjyb.cn

C#:   new Random().Next(1, 101)
来源：http://lbt.shangyingyoupin.top

[A11] 条件表达式（三元）
来源：http://ulu.iojbl.cn

Py:   "yes" if x > 0 else "no"
来源：http://jcg.nwbrower.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://dxr.jinyuanbaomall.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rls.xingfuxueyuan.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://grw.zdqjudy.top

Java: x > 0 ? "yes" : "no"
来源：http://cvi.hesvh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pys.guowangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ace.gzhubu.top

C#:   x > 0 ? "yes" : "no"
来源：http://owk.0kj1m.cn

[A12] 字符串插值 / 格式化
来源：http://hwr.uphjek.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rrx.zhixingplan.top


<!-- 参考信息 -->