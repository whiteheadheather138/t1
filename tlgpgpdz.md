代发 wailian999

[U75] PHP：依赖注入
来源：http://edn.ydjk.org.cn

composer require psr/container
来源：http://rbp.fengsongda.top

[U76] PHP：简单路由
来源：http://xis.zdqjudy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pvu.xinyue.icu

[U77] PHP：模板渲染
来源：http://cpv.zhixingplan.top

composer require twig/twig
来源：http://jct.zycfv.cn

[U78] PHP：单元测试
来源：http://lyb.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://nht.ywan-chungtsiang.top

[U79] PHP：静态分析
来源：http://knr.gogol.net.cn

composer require --dev phpstan/phpstan
来源：http://wmv.fengsongda.top

[U80] PHP：代码规范修复
来源：http://gcf.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tua.tianlin.xyz

[U81] JS：初始化项目
来源：http://qkd.zhongyouzk.top

npm init -y;  npm i express
来源：http://wfo.iojbl.cn

[U82] JS：package.json 脚本
来源：http://flv.zhoulong.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://owb.gaohongyu789.top

[U83] JS：ES Module 导入导出
来源：http://zwp.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://urx.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://mdo.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tmu.jiagoushi.top

[U85] JS：可选链
来源：http://zel.0kj1m.cn

a?.b?.c
来源：http://xls.nanxinkj.top

[U86] JS：空值合并
来源：http://spn.hnxiangtu.top

a ?? b
来源：http://yzf.yongpay.top

[U87] JS：解构默认值
来源：http://zzj.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://sto.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://dal.zhongyouzk.top

{ ...a, ...b }
来源：http://xoh.feifeiyinyue.top

[U89] JS：数组去重
来源：http://wjc.smart0.xyz

[...new Set(arr)]
来源：http://upb.nanxinkj.top

[U90] JS：数字数组排序
来源：http://evn.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://fjg.hfpthk.cn

[U91] JS：对象键值遍历
来源：http://vzn.birdmap.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rrj.feifeiyinyue.top

[U92] JS：深拷贝
来源：http://sdy.dashuyun.cn

structuredClone(obj)
来源：http://gsx.jinyuanbaomall.cn

[U93] JS：模板字符串
来源：http://sfa.zhiwuduotai.top

`共 ${n} 条`
来源：http://qtw.uphjek.com

[U94] JS：箭头函数
来源：http://dfa.yuxming.cn

const double = x => x * 2;
来源：http://kox.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://zmq.xuetiantiany.cn

new Promise((resolve, reject) => {})
来源：http://acw.snrcjt.cn

[U96] JS：async/await 与异常
来源：http://ygq.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cmb.yvedp.cn

[U97] JS：并发请求
来源：http://grp.xinyue.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://hnu.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://wcw.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fbb.guowangkeji.top

[U99] JS：事件监听
来源：http://zwi.sufxvd.cn

el.addEventListener("click", e => {})
来源：http://khu.yuxming.cn

[U100] JS：DOM 查询
来源：http://zvx.9152youxi.cn

document.querySelector(".item")
来源：http://cen.zhengqikj.top

[U101] JS：classList 操作
来源：http://dix.xylfe.cn

el.classList.toggle("active")
来源：http://ebd.gogol.net.cn

[U102] JS：本地存储
来源：http://lbe.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nik.hammf.cn

[U103] JS：定时器
来源：http://ewg.yangfankeji.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xup.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://gnw.gogol.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ytx.ehwqpu.com

[U105] JS：节流
来源：http://jjn.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eqq.zhengqikj.top

[U106] JS：日期格式化
来源：http://tel.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://euk.yvedp.cn

[U107] JS：数字千分位
来源：http://kgx.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kbm.jinqigufen.top

[U108] JS：随机整数
来源：http://ojc.yj20258.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ncr.cheryme.top

[U109] JS：数组分组
来源：http://dfx.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://rnf.hesvh.cn

[U110] JS：数组分块
来源：http://lpc.xuanzx.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gap.chenzaomai.com

[U111] JS：对象转 Map
来源：http://zmw.chenlongwang.top

new Map(Object.entries(obj))
来源：http://rqd.vehdjk.com

[U112] JS：字符串补位
来源：http://lce.yonumen.top

"7".padStart(3, "0")
来源：http://mlq.yfazqb.com

[U113] JS：正则替换全部
来源：http://rlv.jlsjyb.cn

s.replaceAll("a", "b")
来源：http://xmr.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://pbf.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://emj.guannengcc.top

[U115] JS：生成 UUID
来源：http://fek.zhengqikj.top

crypto.randomUUID()
来源：http://fma.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://ppx.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://upm.cheryme.top

[U117] JS：单元测试
来源：http://jtx.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://xjs.fktsv.cn

[U118] JS：开发服务器
来源：http://mlg.yj20258.top

npm i -D vite;  npx vite
来源：http://hra.shzxlz.cn

[U119] JS：生产构建
来源：http://gyi.jinghuilouyu.cn

npx vite build
来源：http://yiv.nanxuanxn.top

[U120] JS：读取环境变量（Vite）
来源：http://vfe.xziqi.cn

import.meta.env.VITE_API_URL
来源：http://ciu.hysaishi.cn

================================================================================
来源：http://egx.jinqigufen.top

统计汇总
来源：http://dvu.cashguo.top

================================================================================
来源：http://tux.jlsjyb.cn

按语言统计（条）：
来源：http://gli.yvedp.cn

Python ......... 252
来源：http://zka.nwbrower.top

PHP ............ 252
来源：http://sij.tianlin.xyz

JavaScript ..... 252
来源：http://ekr.guannengcc.top

TypeScript ..... 212
来源：http://uew.pycfn.com

Java ........... 212
来源：http://mvg.ppjwa.cn

Go ............. 212
来源：http://wgf.gaohongyu789.top

Ruby ........... 212
来源：http://elz.yj20258888.top

C# ............. 212
来源：http://dwt.shanyushiyangkeji.top

C .............. 30
来源：http://edo.guowangkeji.top

C++ ............ 30
来源：http://yfb.shzxlz.cn

SQL ............ 90
来源：http://vqf.pengpengdd.cyou

Bash ........... 80
来源：http://wqt.sufxvd.cn

Kotlin ......... 15
来源：http://gwk.vqdsnc.cn

Swift .......... 15
来源：http://ftl.nwbrower.top

Lua ............ 10
来源：http://wje.daria6918.cn

Perl ........... 10
来源：http://hde.ehwqpu.com

Scala .......... 10
来源：http://gdb.tianlin.xyz

------------------------------------
来源：http://ilx.yj20258888.top

合计 ........... 2106 条
来源：http://lof.yongpay.top

按章节统计：
来源：http://trn.jqgufenzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cft.zhijiandao.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mmi.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wzb.yongpay.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gxg.zhengqikj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hvi.fehbvm.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tsr.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wcz.shuidangran.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://urv.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://srd.52xcode.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yed.tianlin.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pog.sweek.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yzw.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://owj.9152youxi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vif.ehwqpu.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ffo.nanxuanxn.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tkb.ydjk.org.cn

Q SQL 专题                              90
来源：http://acu.gaohongyu789.top

R Bash 专题                             80
来源：http://tbg.yonumen.top

S C / C++ 专题                          60
来源：http://wfs.sysykeji.top

T 其他语言补充                          60
来源：http://xbt.316326.xyz

U 高频实用片段                         120
来源：http://ojt.nwbrower.top

------------------------------------
来源：http://rsq.bbcook.cn

合计                                  2106 条
来源：http://irr.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://hse.hesvh.cn

使用提醒
来源：http://asu.ybcxt.top

--------------------------------------------------------------------------------
来源：http://jzf.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://prg.zhiwuduotai.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jui.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xbd.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vvx.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rze.guowangkeji.top

—— 文件结束 ——
来源：http://odu.havefunace.top

================================================================================
来源：http://gsp.fehbvm.com

程序语言常见例子速查手册（2024 版）
来源：http://fos.jiagoushi.top

Common Programming Examples Cheat Book
来源：http://suz.jinqigufen.top

================================================================================
来源：http://rml.yj20258.top

【收录内容】
来源：http://npe.jinghuilouyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zte.sxryk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xmx.yuanzhike.top

SQL · Bash · C · C++
来源：http://efx.shanyushiyangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sov.fehbvm.com

【使用说明】
来源：http://uyr.cdnleiting.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yvr.tianlin.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wbj.aibaodan.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pps.yj20258888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bxz.pengpengdd.cyou

Bash:  Shell         C:     C             C++:   C++
来源：http://iew.shangyingyoupin.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uln.hcnkem.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wbs.redwolf501.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lyo.cheryme.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://onp.zhoulong.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kbi.yonumen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kdk.yfazqb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dvd.hfpthk.cn

【文件统计】
来源：http://ahi.yueranfly.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nyw.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://xuh.hesvh.cn

目  录
来源：http://fpq.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://wpw.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mgp.hywenlv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://etx.zhoulong.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gnk.dianchejie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xvn.ywan-chungtsiang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ibw.kuanghao11.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rrj.cqqwz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mbz.fzhhl.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mmw.kuanghao11.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://grd.zhiwuduotai.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://srd.yuanzhike.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pdy.uphjek.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eun.xuetiantiany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sve.ydjk.org.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ein.dianchejie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uby.pengpengdd.cyou

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wri.nanxinkj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rlk.redwolf501.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jxr.quarkkingdee.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zpf.redwolf501.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vjq.ehwqpu.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pko.ehwqpu.com

================================================================================
来源：http://hwn.daxiang520.top

A. 基础语法与类型
来源：http://lcc.dashuyun.cn

================================================================================
来源：http://srw.dashuyun.cn

[A01] Hello World
来源：http://jlt.sysykeji.top

Py:   print("Hello, World!")
来源：http://zzo.jlsjyb.cn

PHP:  echo "Hello, World!";
来源：http://ahk.gogol.net.cn

JS:   console.log("Hello, World!");
来源：http://qhi.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cay.zhixingplan.top

Java: System.out.println("Hello, World!");
来源：http://hko.sysykeji.top

Go:   fmt.Println("Hello, World!")
来源：http://byn.cashguo.top

Ruby: puts "Hello, World!"
来源：http://oeu.zdbjq.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ipe.316326.xyz

[A02] 变量声明与赋值
来源：http://xkj.52xcode.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gwm.feifeiyinyue.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fyl.gzhubu.top

JS:   let name = "Alex"; const age = 20;
来源：http://srp.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fzb.gzhubu.top

Java: String name = "Alex"; int age = 20;
来源：http://bph.chenlongwang.top

Go:   name := "Alex"; age := 20
来源：http://mds.tian-w.cn

Ruby: name = "Alex"; age = 20
来源：http://wbr.xylfe.cn

C#:   string name = "Alex"; int age = 20;
来源：http://prr.fengsongda.top

[A03] 常量定义
来源：http://mgr.pycfn.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://crk.fengsongda.top

PHP:  const PI = 3.14159;
来源：http://lwk.zycfv.cn

JS:   const PI = 3.14159;
来源：http://zdk.fanxiaobao.xyz

TS:   const PI: number = 3.14159;
来源：http://evl.cheryme.top

Java: static final double PI = 3.14159;
来源：http://kow.bbcook.cn

Go:   const PI = 3.14159
来源：http://nvs.jinqigufen.top

Ruby: PI = 3.14159
来源：http://qjd.cucudq.cn

C#:   const double PI = 3.14159;
来源：http://ryx.ybcxt.top

[A04] 判断变量类型
来源：http://dwk.jqgufenzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ehk.cqqwz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lru.yuanzhike.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vkd.hnxiangtu.top

TS:   typeof x; x instanceof Date
来源：http://pxs.zhiwuduotai.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vxu.guannengcc.top

Go:   reflect.TypeOf(x).Name()
来源：http://dgu.sjlbkw.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mkm.cdnleiting.top

C#:   x.GetType().Name; x is int
来源：http://zma.fzhhl.top

[A05] 整数除法与取模
来源：http://xhr.vehdjk.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qrn.gogol.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mbb.tarul.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wha.ydzc1.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wtj.316326.xyz

Java: 7 / 2; 7 % 2
来源：http://mpv.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://acr.vehdjk.com

Ruby: 7 / 2; 7 % 2
来源：http://wnf.vqdsnc.cn

C#:   7 / 2; 7 % 2
来源：http://lya.bjfxy.top

[A06] 字符串转数字
来源：http://tgg.jinyuanbaomall.cn

Py:   int("42"); float("3.14")
来源：http://dsq.hywenlv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bay.yvedp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qvu.jinghuilouyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ksv.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dki.jianghu66.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jmg.bjfxy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vrr.jlsjyb.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://agq.cashguo.top

[A07] 数字转字符串
来源：http://mqg.cqqwz.cn

Py:   str(42)
来源：http://pij.xylfe.cn

PHP:  (string) 42; strval(42)
来源：http://pqy.zhengqikj.top

JS:   String(42); (42).toString()
来源：http://jdd.fzhhl.top

TS:   String(42)
来源：http://pmc.cashguo.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dey.sjlbkw.cn

Go:   strconv.Itoa(42)
来源：http://arb.daxiang520.top

Ruby: 42.to_s
来源：http://dvx.gogol.net.cn

C#:   42.ToString()
来源：http://onc.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://jgl.shzxlz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fna.yfazqb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lun.shuidangran.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sby.nwbrower.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ayo.vehdjk.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kkd.yuanzhike.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nvi.jinqigfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://eim.jinqigufen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://con.vehdjk.com

[A09] 绝对值与最大最小值
来源：http://gfl.fehbvm.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ttu.yuxming.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ttf.xuetiantiany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cpn.xingfuxueyuan.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://csf.tanke756.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xan.yangfankeji.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kgg.havefunace.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://reb.nwbrower.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pdw.iojbl.cn

[A10] 生成随机数
来源：http://szl.fzhhl.top

Py:   import random; random.randint(1, 100)
来源：http://dsa.chenlongwang.top

PHP:  random_int(1, 100);
来源：http://fyq.cucudq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ema.fanxiaobao.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ntm.c1oappe.top

Java: new Random().nextInt(100) + 1
来源：http://psj.ybcxt.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hra.svipenyu.cn

Ruby: rand(1..100)
来源：http://sdf.shanyushiyangkeji.top

C#:   new Random().Next(1, 101)
来源：http://ont.0kj1m.cn

[A11] 条件表达式（三元）
来源：http://fwm.xingfuxueyuan.xyz

Py:   "yes" if x > 0 else "no"
来源：http://kwm.zycfv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wqh.chenlongwang.top

JS:   x > 0 ? "yes" : "no"
来源：http://vgk.ivvv.top

TS:   x > 0 ? "yes" : "no"
来源：http://vaq.52xcode.cn

Java: x > 0 ? "yes" : "no"
来源：http://typ.shanyushiyangkeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://siu.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ptu.zhoulong.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://cmk.snrcjt.cn

[A12] 字符串插值 / 格式化
来源：http://ted.zhiwuduotai.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kaw.chenjidiqi.icu


<!-- 参考信息 -->