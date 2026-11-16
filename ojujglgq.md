代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://isb.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://yqm.c1oappe.top

[U74] PHP：读取环境变量
来源：http://hbx.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://kot.dashuyun.cn

[U75] PHP：依赖注入
来源：http://dae.hammf.cn

composer require psr/container
来源：http://sim.nanxuanxn.top

[U76] PHP：简单路由
来源：http://cmr.hesvh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zdm.fehbvm.com

[U77] PHP：模板渲染
来源：http://swe.jiagoushi.top

composer require twig/twig
来源：http://vun.xinyue.icu

[U78] PHP：单元测试
来源：http://zth.ppjwa.cn

composer require --dev phpunit/phpunit
来源：http://ioz.hcnkem.com

[U79] PHP：静态分析
来源：http://yew.hongshengwenyu.top

composer require --dev phpstan/phpstan
来源：http://uql.xinyue.icu

[U80] PHP：代码规范修复
来源：http://wcn.fzhhl.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dqt.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://kgq.hysaishi.cn

npm init -y;  npm i express
来源：http://gby.jinghuilouyu.cn

[U82] JS：package.json 脚本
来源：http://tar.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wfn.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://yoj.zhixingplan.top

export const a = 1;  import { a } from "./m.js";
来源：http://clt.tanke756.top

[U84] JS：CommonJS 写法
来源：http://zta.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://llp.snrcjt.cn

[U85] JS：可选链
来源：http://oyq.ydzc1.top

a?.b?.c
来源：http://tvq.yangfankeji.com

[U86] JS：空值合并
来源：http://fwf.nanxinkj.top

a ?? b
来源：http://mbv.zdbjq.cn

[U87] JS：解构默认值
来源：http://qnd.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://orc.jinqigfzy.top

[U88] JS：对象展开合并
来源：http://huh.pycfn.com

{ ...a, ...b }
来源：http://qod.yuanzhike.top

[U89] JS：数组去重
来源：http://lhq.ctjpmb.com

[...new Set(arr)]
来源：http://fdt.yj20258888.top

[U90] JS：数字数组排序
来源：http://vgt.mhx1999.top

[...arr].sort((a, b) => a - b)
来源：http://ihg.xinyue.icu

[U91] JS：对象键值遍历
来源：http://lhc.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oci.ydjk.org.cn

[U92] JS：深拷贝
来源：http://jmi.hnxiangtu.top

structuredClone(obj)
来源：http://ttn.mhx1999.top

[U93] JS：模板字符串
来源：http://nar.tian-w.cn

`共 ${n} 条`
来源：http://sxn.tianlin.xyz

[U94] JS：箭头函数
来源：http://xfv.cashguo.top

const double = x => x * 2;
来源：http://yna.redwolf501.top

[U95] JS：Promise 包装
来源：http://hxm.fktsv.cn

new Promise((resolve, reject) => {})
来源：http://ndz.fktsv.cn

[U96] JS：async/await 与异常
来源：http://hbm.zhaomingkeji.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kws.yanxiufei.cn

[U97] JS：并发请求
来源：http://ypr.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dty.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://jtf.yfazqb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fgl.cdnleiting.top

[U99] JS：事件监听
来源：http://hee.smart0.xyz

el.addEventListener("click", e => {})
来源：http://mxk.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://ive.ydzc1.top

document.querySelector(".item")
来源：http://dqa.yueranfly.top

[U101] JS：classList 操作
来源：http://ugn.52xcode.cn

el.classList.toggle("active")
来源：http://ydj.zhaomingkeji.xyz

[U102] JS：本地存储
来源：http://eqj.zhixingplan.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://suu.jinghuilouyu.cn

[U103] JS：定时器
来源：http://vnv.tian-w.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mix.sweek.top

[U104] JS：防抖
来源：http://pps.yuanzhike.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zew.cashguo.top

[U105] JS：节流
来源：http://btp.sufxvd.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bhz.xylfe.cn

[U106] JS：日期格式化
来源：http://tck.hnxiangtu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vmx.gzhubu.top

[U107] JS：数字千分位
来源：http://rvx.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qdo.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://ype.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kng.cdnleiting.top

[U109] JS：数组分组
来源：http://eox.bbcook.cn

Object.groupBy(arr, x => x.type)
来源：http://vcv.gotoacloud.top

[U110] JS：数组分块
来源：http://zev.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hlo.chenlongwang.top

[U111] JS：对象转 Map
来源：http://rcu.yj20258888.top

new Map(Object.entries(obj))
来源：http://nzj.316326.xyz

[U112] JS：字符串补位
来源：http://xtq.aizwys.cn

"7".padStart(3, "0")
来源：http://axm.yueranfly.top

[U113] JS：正则替换全部
来源：http://myu.yuxming.cn

s.replaceAll("a", "b")
来源：http://ckr.fzhhl.top

[U114] JS：JSON 深比较
来源：http://ddk.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dxs.hywenlv.cn

[U115] JS：生成 UUID
来源：http://tcf.guowangkeji.top

crypto.randomUUID()
来源：http://tob.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://wcc.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://xik.wangshuangyany.cn

[U117] JS：单元测试
来源：http://mps.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://pld.yongpay.top

[U118] JS：开发服务器
来源：http://fpx.fengsongda.top

npm i -D vite;  npx vite
来源：http://ava.chenjidiqi.icu

[U119] JS：生产构建
来源：http://awy.xingfuxueyuan.xyz

npx vite build
来源：http://ypf.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://dsf.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://cku.ywan-chungtsiang.top

================================================================================
来源：http://tza.dianchejie.cn

统计汇总
来源：http://ixm.tianlin.xyz

================================================================================
来源：http://sxw.gogol.net.cn

按语言统计（条）：
来源：http://uee.ybcxt.top

Python ......... 252
来源：http://iyd.shanyushiyangtech.top

PHP ............ 252
来源：http://zqu.jyoumei.cn

JavaScript ..... 252
来源：http://coz.hywenlv.cn

TypeScript ..... 212
来源：http://awb.zhengqikj.top

Java ........... 212
来源：http://dpy.chenlongwang.top

Go ............. 212
来源：http://dmz.nanxinkj.top

Ruby ........... 212
来源：http://kxs.uphjek.com

C# ............. 212
来源：http://mdd.0kj1m.cn

C .............. 30
来源：http://dio.zhongyouzk.top

C++ ............ 30
来源：http://swc.zhongyouzk.top

SQL ............ 90
来源：http://bzv.hysaishi.cn

Bash ........... 80
来源：http://mix.sweek.top

Kotlin ......... 15
来源：http://bbo.kuanghao11.cn

Swift .......... 15
来源：http://ium.shuidangran.top

Lua ............ 10
来源：http://cri.pycfn.com

Perl ........... 10
来源：http://kww.andypj.xyz

Scala .......... 10
来源：http://fwo.fehbvm.com

------------------------------------
来源：http://cre.xingfuxueyuan.xyz

合计 ........... 2106 条
来源：http://dbc.daria6918.cn

按章节统计：
来源：http://cmc.daria6918.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dmg.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wot.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wcr.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lan.zhoulong.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iea.zhengqikj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qhc.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oct.zhixingplan.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rbk.quarkkingdee.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vhe.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dxo.uphjek.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://agi.gzhubu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xvn.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bnb.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://odm.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cnt.sxryk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nrs.smart0.xyz

Q SQL 专题                              90
来源：http://bmb.ydjk.org.cn

R Bash 专题                             80
来源：http://cyf.zhongyouzk.top

S C / C++ 专题                          60
来源：http://ldc.yanxiufei.cn

T 其他语言补充                          60
来源：http://rxx.gaohongyu789.top

U 高频实用片段                         120
来源：http://uwj.jinyuanbaomall.cn

------------------------------------
来源：http://gbm.wangdashe.top

合计                                  2106 条
来源：http://nmi.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://bvo.birdmap.top

使用提醒
来源：http://mfc.yongpay.top

--------------------------------------------------------------------------------
来源：http://pmj.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hek.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lnk.xuanzx.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://flm.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jhi.gaohongyu789.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://laz.pengpengdd.cyou

—— 文件结束 ——
来源：http://zgj.sufxvd.cn

================================================================================
来源：http://pav.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://rmq.c1oappe.top

Common Programming Examples Cheat Book
来源：http://oas.cdnleiting.top

================================================================================
来源：http://bdw.xingfuxueyuan.xyz

【收录内容】
来源：http://xbk.aibaodan.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zfw.sufxvd.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ktu.gogol.net.cn

SQL · Bash · C · C++
来源：http://iyy.zhijiandao.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bth.yj202588.top

【使用说明】
来源：http://czj.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ggj.chenjidiqi.icu

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sgj.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iee.jinghuilouyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vym.svipenyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nmi.zhoulong.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hne.316326.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bmj.yuxming.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nep.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qdq.hywenlv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ouf.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nla.jinqigufen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gsh.zdqjudy.top

【文件统计】
来源：http://gey.52xcode.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vai.sysykeji.top

--------------------------------------------------------------------------------
来源：http://nnn.sxryk.cn

目  录
来源：http://srv.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://tmf.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qcy.shanyushiyangtech.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lnn.zhoulong.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oxp.zhengqikj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jgw.gzhubu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oxx.bbcook.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rlc.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sif.xuanzx.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bxc.fktsv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lmp.svipenyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ueq.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eun.shangyingyoupin.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kvq.jlsjyb.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://utd.tanke756.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rim.jinqigfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://asj.fengsongda.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zwp.gotoacloud.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zlj.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xqv.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vve.quarkkingdee.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hcq.vqdsnc.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xby.meibo888.top

================================================================================
来源：http://lsh.shanyushiyangtech.top

A. 基础语法与类型
来源：http://qpi.chenzaomai.com

================================================================================
来源：http://pes.jianghu66.top

[A01] Hello World
来源：http://lbl.feifeiyinyue.top

Py:   print("Hello, World!")
来源：http://gji.yongpay.top

PHP:  echo "Hello, World!";
来源：http://zjh.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://zbt.yuxming.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qxm.jqgfzy.top

Java: System.out.println("Hello, World!");
来源：http://com.jinqigufen.top

Go:   fmt.Println("Hello, World!")
来源：http://etf.xuetiantiany.cn

Ruby: puts "Hello, World!"
来源：http://kya.zhaomingkeji.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://bvx.daxiang520.top

[A02] 变量声明与赋值
来源：http://mmp.tian-w.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rva.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://uyz.yj20258888.top

JS:   let name = "Alex"; const age = 20;
来源：http://djj.316326.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dcr.nanxuanxn.top

Java: String name = "Alex"; int age = 20;
来源：http://ves.jinghuilouyu.cn

Go:   name := "Alex"; age := 20
来源：http://gsu.ydjk.org.cn

Ruby: name = "Alex"; age = 20
来源：http://pen.cheryme.top

C#:   string name = "Alex"; int age = 20;
来源：http://bnr.yuxming.cn

[A03] 常量定义
来源：http://ist.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://txs.shanyushiyangtech.top

PHP:  const PI = 3.14159;
来源：http://kwm.aizwys.cn

JS:   const PI = 3.14159;
来源：http://upe.hcnkem.com

TS:   const PI: number = 3.14159;
来源：http://yjl.sjlbkw.cn

Java: static final double PI = 3.14159;
来源：http://jyr.c1oappe.top

Go:   const PI = 3.14159
来源：http://pvz.cqqwz.cn

Ruby: PI = 3.14159
来源：http://qhh.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://fec.cqqwz.cn

[A04] 判断变量类型
来源：http://nyu.hnxiangtu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zci.svipenyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://anl.yangfankeji.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ybp.jianghu66.top

TS:   typeof x; x instanceof Date
来源：http://ama.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mfj.cucudq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dzb.sweek.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kfp.yanxiufei.cn

C#:   x.GetType().Name; x is int
来源：http://hfd.birdmap.top

[A05] 整数除法与取模
来源：http://jdr.quarkkingdee.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zpz.yj20258888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qzj.hongshengwenyu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mkx.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xhy.c1oappe.top

Java: 7 / 2; 7 % 2
来源：http://nqp.jinqigfzy.top

Go:   7 / 2; 7 % 2
来源：http://xdn.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://jen.xinyue.icu

C#:   7 / 2; 7 % 2
来源：http://ita.gzhubu.top

[A06] 字符串转数字
来源：http://viq.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://kxs.dashuyun.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://afv.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qpp.redwolf501.top

TS:   parseInt("42", 10); Number("42")
来源：http://sqa.ydzc1.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nqj.fanxiaobao.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://otk.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://nmq.zdbjq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uft.yj20258.top

[A07] 数字转字符串
来源：http://xmg.jqgfzy.top

Py:   str(42)
来源：http://ueg.svipenyu.cn

PHP:  (string) 42; strval(42)
来源：http://uvb.chenzaomai.com

JS:   String(42); (42).toString()
来源：http://jah.birdmap.top

TS:   String(42)
来源：http://uvt.xuetiantiany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://scl.guannengcc.top

Go:   strconv.Itoa(42)
来源：http://ggy.sufxvd.cn

Ruby: 42.to_s
来源：http://ugs.haohaochexian.top

C#:   42.ToString()
来源：http://xti.jlsjyb.cn

[A08] 取整与四舍五入
来源：http://bek.jianghu66.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sod.jinqigufen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xui.sjlbkw.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xyx.sxryk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wjv.chenzaomai.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://soe.tianlin.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://soh.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dpa.shuidangran.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zfm.dashuyun.cn

[A09] 绝对值与最大最小值
来源：http://clw.jinghuilouyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yeg.jyoumei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jpz.kuanghao11.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cye.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://itr.0kj1m.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nzw.hywenlv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mdu.jianghu66.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qui.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jcb.hywenlv.cn

[A10] 生成随机数
来源：http://giq.chenlongwang.top

Py:   import random; random.randint(1, 100)
来源：http://lgn.316326.xyz

PHP:  random_int(1, 100);
来源：http://dkk.uphjek.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zwz.bjfxy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://peu.yj20258.top

Java: new Random().nextInt(100) + 1
来源：http://wqi.birdmap.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bwd.gotoacloud.top

Ruby: rand(1..100)
来源：http://hck.snrcjt.cn

C#:   new Random().Next(1, 101)
来源：http://oxx.jianghu66.top

[A11] 条件表达式（三元）
来源：http://yaq.cheryme.top

Py:   "yes" if x > 0 else "no"
来源：http://ayu.zdqjudy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://oit.sxryk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ant.pycfn.com

TS:   x > 0 ? "yes" : "no"
来源：http://wpw.pengpengdd.cyou

Java: x > 0 ? "yes" : "no"
来源：http://pqz.gotoacloud.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vxo.sxryk.cn


<!-- 参考信息 -->