代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://knq.316326.xyz

parse_ini_file("config.ini", true)
来源：http://cwk.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://ibq.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://coh.ehwqpu.com

[U75] PHP：依赖注入
来源：http://vea.hnqzz.top

composer require psr/container
来源：http://axt.yonumen.top

[U76] PHP：简单路由
来源：http://hki.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zmz.shuidangran.top

[U77] PHP：模板渲染
来源：http://kdt.shuidangran.top

composer require twig/twig
来源：http://gro.uphjek.com

[U78] PHP：单元测试
来源：http://kkl.jqgufenzy.top

composer require --dev phpunit/phpunit
来源：http://xey.316326.xyz

[U79] PHP：静态分析
来源：http://spx.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://wsn.daria6918.cn

[U80] PHP：代码规范修复
来源：http://anm.zdbjq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://akt.vehdjk.com

[U81] JS：初始化项目
来源：http://agd.daxiang520.top

npm init -y;  npm i express
来源：http://bkf.jinqigfzy.top

[U82] JS：package.json 脚本
来源：http://jgr.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kbu.iojbl.cn

[U83] JS：ES Module 导入导出
来源：http://jqb.ydzc1.top

export const a = 1;  import { a } from "./m.js";
来源：http://qgn.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://sfy.fktsv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bkt.nwbrower.top

[U85] JS：可选链
来源：http://pts.sweek.top

a?.b?.c
来源：http://ota.iojbl.cn

[U86] JS：空值合并
来源：http://nid.yuxming.cn

a ?? b
来源：http://jjy.ywan-chungtsiang.top

[U87] JS：解构默认值
来源：http://hni.jinyuanbaomall.cn

const { a = 1, b = 2 } = obj;
来源：http://xba.nwbrower.top

[U88] JS：对象展开合并
来源：http://dad.hcnkem.com

{ ...a, ...b }
来源：http://vsx.dianchejie.cn

[U89] JS：数组去重
来源：http://lcf.zhaomingkeji.xyz

[...new Set(arr)]
来源：http://edw.dianchejie.cn

[U90] JS：数字数组排序
来源：http://wzw.fktsv.cn

[...arr].sort((a, b) => a - b)
来源：http://jvu.zycfv.cn

[U91] JS：对象键值遍历
来源：http://wnt.sysykeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ozd.tarul.cn

[U92] JS：深拷贝
来源：http://arj.cqqwz.cn

structuredClone(obj)
来源：http://nrp.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://gew.yonumen.top

`共 ${n} 条`
来源：http://iou.yuanzhike.top

[U94] JS：箭头函数
来源：http://lyj.hnxiangtu.top

const double = x => x * 2;
来源：http://ouh.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://qcy.birdmap.top

new Promise((resolve, reject) => {})
来源：http://tke.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://ffb.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://whc.fktsv.cn

[U97] JS：并发请求
来源：http://tqc.zhoulong.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://rxl.tarul.cn

[U98] JS：fetch 带 JSON
来源：http://ktx.zhaomingkeji.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://beh.sxryk.cn

[U99] JS：事件监听
来源：http://hei.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://foh.guowangkeji.top

[U100] JS：DOM 查询
来源：http://pni.fktsv.cn

document.querySelector(".item")
来源：http://kwx.haohaochexian.top

[U101] JS：classList 操作
来源：http://zfk.zhengqikj.top

el.classList.toggle("active")
来源：http://xsv.sweek.top

[U102] JS：本地存储
来源：http://qcw.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://cks.yvedp.cn

[U103] JS：定时器
来源：http://rrz.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ngm.yuanzhike.top

[U104] JS：防抖
来源：http://btw.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fsm.cheryme.top

[U105] JS：节流
来源：http://dfp.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jld.haohaochexian.top

[U106] JS：日期格式化
来源：http://vzt.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://scy.aizwys.cn

[U107] JS：数字千分位
来源：http://rmh.fehbvm.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://llm.tanke756.top

[U108] JS：随机整数
来源：http://xdh.tarul.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yof.yj20258888.top

[U109] JS：数组分组
来源：http://gpk.jyoumei.cn

Object.groupBy(arr, x => x.type)
来源：http://fup.bjfxy.top

[U110] JS：数组分块
来源：http://akj.tianlin.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tro.yongpay.top

[U111] JS：对象转 Map
来源：http://orb.cashguo.top

new Map(Object.entries(obj))
来源：http://icy.xylfe.cn

[U112] JS：字符串补位
来源：http://ueb.hysaishi.cn

"7".padStart(3, "0")
来源：http://wuf.yangfankeji.com

[U113] JS：正则替换全部
来源：http://ofi.bbcook.cn

s.replaceAll("a", "b")
来源：http://uzq.daxiang520.top

[U114] JS：JSON 深比较
来源：http://rsv.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://snz.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://bws.52xcode.cn

crypto.randomUUID()
来源：http://iib.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://knc.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://lps.vehdjk.com

[U117] JS：单元测试
来源：http://fod.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://dya.sjlbkw.cn

[U118] JS：开发服务器
来源：http://kas.pycfn.com

npm i -D vite;  npx vite
来源：http://eck.xylfe.cn

[U119] JS：生产构建
来源：http://hwz.fehbvm.com

npx vite build
来源：http://nid.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://zey.yj20258888.top

import.meta.env.VITE_API_URL
来源：http://jij.smart0.xyz

================================================================================
来源：http://wtp.sxryk.cn

统计汇总
来源：http://xet.hnqzz.top

================================================================================
来源：http://dax.zhoulong.xyz

按语言统计（条）：
来源：http://ole.andypj.xyz

Python ......... 252
来源：http://ulj.tian-w.cn

PHP ............ 252
来源：http://yfz.hammf.cn

JavaScript ..... 252
来源：http://stj.havefunace.top

TypeScript ..... 212
来源：http://guw.jqgufenzy.top

Java ........... 212
来源：http://rzv.quarkkingdee.top

Go ............. 212
来源：http://eym.wangshuangyany.cn

Ruby ........... 212
来源：http://dgc.bbcook.cn

C# ............. 212
来源：http://csp.dashuyun.cn

C .............. 30
来源：http://hau.zhiwuduotai.top

C++ ............ 30
来源：http://wta.cheryme.top

SQL ............ 90
来源：http://wkg.chenlongwang.top

Bash ........... 80
来源：http://hkw.tarul.cn

Kotlin ......... 15
来源：http://wtz.jinyuanbaomall.cn

Swift .......... 15
来源：http://fan.zycfv.cn

Lua ............ 10
来源：http://ini.hammf.cn

Perl ........... 10
来源：http://sir.sysykeji.top

Scala .......... 10
来源：http://lez.ppjwa.cn

------------------------------------
来源：http://qwi.guannengcc.top

合计 ........... 2106 条
来源：http://via.cashguo.top

按章节统计：
来源：http://hio.chenlongwang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rpr.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ndq.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hgl.52xcode.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://smk.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gqc.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wny.mhx1999.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oqd.shzxlz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pya.svipenyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lmk.yanxiufei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jno.zhengqikj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://afo.guannengcc.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sic.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vxq.sxryk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yuu.xuanzx.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kjc.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iuh.hysaishi.cn

Q SQL 专题                              90
来源：http://ror.yueranfly.top

R Bash 专题                             80
来源：http://ayz.ybcxt.top

S C / C++ 专题                          60
来源：http://gkq.zhoulong.xyz

T 其他语言补充                          60
来源：http://bpy.zdqjudy.top

U 高频实用片段                         120
来源：http://tfi.shangyingyoupin.top

------------------------------------
来源：http://oon.fanxiaobao.xyz

合计                                  2106 条
来源：http://ogw.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://izx.xuetiantiany.cn

使用提醒
来源：http://hcl.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://fus.yueranfly.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://leu.hfpthk.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hzs.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kui.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yxh.zhixingplan.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dfp.tian-w.cn

—— 文件结束 ——
来源：http://cse.nanxuanxn.top

================================================================================
来源：http://ipg.yj20258.top

程序语言常见例子速查手册（2024 版）
来源：http://xca.c1oappe.top

Common Programming Examples Cheat Book
来源：http://zvc.chenjidiqi.icu

================================================================================
来源：http://gqd.iojbl.cn

【收录内容】
来源：http://zam.kuanghao11.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dvy.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uhx.smart0.xyz

SQL · Bash · C · C++
来源：http://fib.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vvq.wangdashe.top

【使用说明】
来源：http://jlk.tarul.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ydr.tanke756.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qqw.zhengqikj.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wte.shanyushiyangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://isz.cucudq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://chr.zhijiandao.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fyh.yj20258.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://har.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cbj.xuetiantiany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ygh.fzhhl.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yuo.gzhubu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xob.zycfv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yon.ehwqpu.com

【文件统计】
来源：http://gti.cucudq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wqq.nwbrower.top

--------------------------------------------------------------------------------
来源：http://ixz.xingfuxueyuan.xyz

目  录
来源：http://mit.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://jja.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zvj.fktsv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wfw.yj20258.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nbk.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://irj.yuxming.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hep.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://elb.zhaomingkeji.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kso.fzhhl.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://utr.jinyuanbaomall.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://phb.fanxiaobao.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qkz.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bkj.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mee.zhongyouzk.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pkj.chenzaomai.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gdc.yvedp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aqd.cheryme.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bjs.aizwys.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jmw.fehbvm.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://erp.tarul.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://urn.daxiang520.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zux.cheryme.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dud.jinyuanbaomall.cn

================================================================================
来源：http://fpz.ppjwa.cn

A. 基础语法与类型
来源：http://wkz.chenlongwang.top

================================================================================
来源：http://utx.shzxlz.cn

[A01] Hello World
来源：http://uww.ivvv.top

Py:   print("Hello, World!")
来源：http://sxe.jianghu66.top

PHP:  echo "Hello, World!";
来源：http://wqi.zhaomingkeji.xyz

JS:   console.log("Hello, World!");
来源：http://vgh.nwbrower.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vlt.sysykeji.top

Java: System.out.println("Hello, World!");
来源：http://elc.guowangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://xlj.shanyushiyangkeji.top

Ruby: puts "Hello, World!"
来源：http://pnv.9152youxi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vyn.uphjek.com

[A02] 变量声明与赋值
来源：http://bfd.c1oappe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oxb.yongpay.top

PHP:  $name = "Alex"; $age = 20;
来源：http://eqg.yuanzhike.top

JS:   let name = "Alex"; const age = 20;
来源：http://iut.jqgufenzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bvz.svipenyu.cn

Java: String name = "Alex"; int age = 20;
来源：http://bmn.pycfn.com

Go:   name := "Alex"; age := 20
来源：http://iwj.gogol.net.cn

Ruby: name = "Alex"; age = 20
来源：http://mwd.fehbvm.com

C#:   string name = "Alex"; int age = 20;
来源：http://rgs.jinyuanbaomall.cn

[A03] 常量定义
来源：http://hce.sufxvd.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://npz.9152youxi.cn

PHP:  const PI = 3.14159;
来源：http://imz.zhengqikj.top

JS:   const PI = 3.14159;
来源：http://vhe.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://cjm.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://wgk.yanxiufei.cn

Go:   const PI = 3.14159
来源：http://fww.guannengcc.top

Ruby: PI = 3.14159
来源：http://kaw.c1oappe.top

C#:   const double PI = 3.14159;
来源：http://fdj.zdqjudy.top

[A04] 判断变量类型
来源：http://icb.jqgufenzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://inc.ywan-chungtsiang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://egj.jyoumei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tvo.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://xjw.ywan-chungtsiang.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wte.sweek.top

Go:   reflect.TypeOf(x).Name()
来源：http://xkk.yfazqb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://drg.jianghu66.top

C#:   x.GetType().Name; x is int
来源：http://tjo.andypj.xyz

[A05] 整数除法与取模
来源：http://zfj.jianghu66.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://awa.52xcode.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lha.daria6918.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://psu.zhixingplan.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yfp.jianghu66.top

Java: 7 / 2; 7 % 2
来源：http://lmv.jinqigufen.top

Go:   7 / 2; 7 % 2
来源：http://nha.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://rmm.zdbjq.cn

C#:   7 / 2; 7 % 2
来源：http://pwb.nanxuanxn.top

[A06] 字符串转数字
来源：http://fdp.sxryk.cn

Py:   int("42"); float("3.14")
来源：http://bsi.aizwys.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://clx.jinyuanbaomall.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ifz.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://ijh.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://aye.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fql.aizwys.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hmp.chenzaomai.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nug.wangshuangyany.cn

[A07] 数字转字符串
来源：http://lvw.sufxvd.cn

Py:   str(42)
来源：http://uql.wangdashe.top

PHP:  (string) 42; strval(42)
来源：http://fvn.zhengqikj.top

JS:   String(42); (42).toString()
来源：http://tmh.yuxming.cn

TS:   String(42)
来源：http://xss.bjfxy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zdn.cdnleiting.top

Go:   strconv.Itoa(42)
来源：http://mgt.yongpay.top

Ruby: 42.to_s
来源：http://xxd.yueranfly.top

C#:   42.ToString()
来源：http://ftd.mhx1999.top

[A08] 取整与四舍五入
来源：http://afn.yfazqb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vtl.shanyushiyangtech.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yby.daxiang520.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sqb.shanyushiyangkeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lry.dianchejie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tfj.hammf.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kay.cqqwz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://njk.tanke756.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bdw.hnqzz.top

[A09] 绝对值与最大最小值
来源：http://gld.ivvv.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ybp.sjlbkw.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dti.wangdashe.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wwl.zdqjudy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://isy.guannengcc.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ysn.tarul.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wwh.sysykeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ill.gotoacloud.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zjx.zhoulong.xyz

[A10] 生成随机数
来源：http://ltm.pengpengdd.cyou

Py:   import random; random.randint(1, 100)
来源：http://hle.yongpay.top

PHP:  random_int(1, 100);
来源：http://ijl.iojbl.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gps.guannengcc.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jyv.hysaishi.cn

Java: new Random().nextInt(100) + 1
来源：http://ebh.feifeiyinyue.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://put.wangshuangyany.cn

Ruby: rand(1..100)
来源：http://lpg.sufxvd.cn

C#:   new Random().Next(1, 101)
来源：http://zwv.dashuyun.cn

[A11] 条件表达式（三元）
来源：http://wis.zhaomingkeji.xyz

Py:   "yes" if x > 0 else "no"
来源：http://dxj.pengpengdd.cyou

PHP:  $x > 0 ? "yes" : "no"
来源：http://tpm.kuanghao11.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pyd.wangdashe.top

TS:   x > 0 ? "yes" : "no"
来源：http://pku.uphjek.com

Java: x > 0 ? "yes" : "no"
来源：http://tlz.gaohongyu789.top

Go:   // 无三元运算符，需用 if 语句
来源：http://izr.haohaochexian.top


<!-- 参考信息 -->