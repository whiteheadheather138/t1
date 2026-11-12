代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://srh.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://ugx.fehbvm.com

[U74] PHP：读取环境变量
来源：http://jgv.hesvh.cn

getenv("APP_ENV") ?: "production"
来源：http://wwo.hongshengwenyu.top

[U75] PHP：依赖注入
来源：http://ltb.zhaomingkeji.xyz

composer require psr/container
来源：http://irh.hnxiangtu.top

[U76] PHP：简单路由
来源：http://nzi.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ndp.sufxvd.cn

[U77] PHP：模板渲染
来源：http://otg.svipenyu.cn

composer require twig/twig
来源：http://tfn.gotoacloud.top

[U78] PHP：单元测试
来源：http://ugi.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://vik.jlsjyb.cn

[U79] PHP：静态分析
来源：http://cnu.jiagoushi.top

composer require --dev phpstan/phpstan
来源：http://bvv.bbcook.cn

[U80] PHP：代码规范修复
来源：http://qgy.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://inc.hnxiangtu.top

[U81] JS：初始化项目
来源：http://dtz.yj20258.top

npm init -y;  npm i express
来源：http://uym.guowangkeji.top

[U82] JS：package.json 脚本
来源：http://gdn.andypj.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qcp.cashguo.top

[U83] JS：ES Module 导入导出
来源：http://wvw.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://nuf.shuidangran.top

[U84] JS：CommonJS 写法
来源：http://iny.316326.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://vcu.sufxvd.cn

[U85] JS：可选链
来源：http://rwr.ydjk.org.cn

a?.b?.c
来源：http://zpv.sufxvd.cn

[U86] JS：空值合并
来源：http://bsm.hysaishi.cn

a ?? b
来源：http://spd.zdbjq.cn

[U87] JS：解构默认值
来源：http://ndt.hammf.cn

const { a = 1, b = 2 } = obj;
来源：http://ppf.hammf.cn

[U88] JS：对象展开合并
来源：http://kzm.zdqjudy.top

{ ...a, ...b }
来源：http://lbu.chenzaomai.com

[U89] JS：数组去重
来源：http://iwf.fehbvm.com

[...new Set(arr)]
来源：http://rke.mhx1999.top

[U90] JS：数字数组排序
来源：http://epc.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://lrb.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://gcf.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ebu.dianchejie.cn

[U92] JS：深拷贝
来源：http://wgb.aibaodan.cn

structuredClone(obj)
来源：http://imp.xziqi.cn

[U93] JS：模板字符串
来源：http://xtw.tanke756.top

`共 ${n} 条`
来源：http://nnw.9152youxi.cn

[U94] JS：箭头函数
来源：http://lgl.9152youxi.cn

const double = x => x * 2;
来源：http://hpj.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://gqu.yj20258.top

new Promise((resolve, reject) => {})
来源：http://kux.9152youxi.cn

[U96] JS：async/await 与异常
来源：http://aam.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qst.jlsjyb.cn

[U97] JS：并发请求
来源：http://jnz.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://vcj.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://jcf.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zbh.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://cpc.hywenlv.cn

el.addEventListener("click", e => {})
来源：http://zqa.redwolf501.top

[U100] JS：DOM 查询
来源：http://qns.guannengcc.top

document.querySelector(".item")
来源：http://rit.zhaomingkeji.xyz

[U101] JS：classList 操作
来源：http://rdl.meibo888.top

el.classList.toggle("active")
来源：http://dzl.mhx1999.top

[U102] JS：本地存储
来源：http://qoh.yvedp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://blf.yanxiufei.cn

[U103] JS：定时器
来源：http://ysb.birdmap.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cdo.52xcode.cn

[U104] JS：防抖
来源：http://lcr.guannengcc.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gjq.hammf.cn

[U105] JS：节流
来源：http://zzn.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qsw.zhengqikj.top

[U106] JS：日期格式化
来源：http://yaf.aibaodan.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fxx.cdnleiting.top

[U107] JS：数字千分位
来源：http://hkb.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mcy.chenjidiqi.icu

[U108] JS：随机整数
来源：http://aas.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yzt.9152youxi.cn

[U109] JS：数组分组
来源：http://ily.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://dwu.yongpay.top

[U110] JS：数组分块
来源：http://bsn.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ebh.chenlongwang.top

[U111] JS：对象转 Map
来源：http://uxf.jqgfzy.top

new Map(Object.entries(obj))
来源：http://eoj.daxiang520.top

[U112] JS：字符串补位
来源：http://pqc.316326.xyz

"7".padStart(3, "0")
来源：http://iqu.haohaochexian.top

[U113] JS：正则替换全部
来源：http://nay.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://wrm.uphjek.com

[U114] JS：JSON 深比较
来源：http://pml.xinyue.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://com.yangfankeji.com

[U115] JS：生成 UUID
来源：http://zys.yfazqb.com

crypto.randomUUID()
来源：http://bfs.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://cjb.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://jgs.ydzc1.top

[U117] JS：单元测试
来源：http://ucg.cashguo.top

npm i -D vitest;  npx vitest
来源：http://ihb.hongshengwenyu.top

[U118] JS：开发服务器
来源：http://zpz.cashguo.top

npm i -D vite;  npx vite
来源：http://wdm.yj20258888.top

[U119] JS：生产构建
来源：http://pfo.xuanzx.com

npx vite build
来源：http://myi.gotoacloud.top

[U120] JS：读取环境变量（Vite）
来源：http://elu.hammf.cn

import.meta.env.VITE_API_URL
来源：http://bwi.zhongyouzk.top

================================================================================
来源：http://may.sufxvd.cn

统计汇总
来源：http://lpy.jianghu66.top

================================================================================
来源：http://ayj.jianghu66.top

按语言统计（条）：
来源：http://brc.meibo888.top

Python ......... 252
来源：http://jvl.xuanzx.com

PHP ............ 252
来源：http://owz.jiagoushi.top

JavaScript ..... 252
来源：http://lzo.hnqzz.top

TypeScript ..... 212
来源：http://tzl.xuetiantiany.cn

Java ........... 212
来源：http://nkw.zhiwuduotai.top

Go ............. 212
来源：http://bkk.hammf.cn

Ruby ........... 212
来源：http://bib.yj20258.top

C# ............. 212
来源：http://eqe.jinqigufen.top

C .............. 30
来源：http://ixz.daxiang520.top

C++ ............ 30
来源：http://owc.xziqi.cn

SQL ............ 90
来源：http://dbb.jianghu66.top

Bash ........... 80
来源：http://rpe.xuetiantiany.cn

Kotlin ......... 15
来源：http://fgk.yj202588.top

Swift .......... 15
来源：http://erg.yj20258888.top

Lua ............ 10
来源：http://sgf.chenlongwang.top

Perl ........... 10
来源：http://lyl.cheryme.top

Scala .......... 10
来源：http://rjx.jyoumei.cn

------------------------------------
来源：http://mqm.52xcode.cn

合计 ........... 2106 条
来源：http://yxc.mhx1999.top

按章节统计：
来源：http://jpx.jianghu66.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nvq.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jfi.jinqigufen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fan.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ybp.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pod.meibo888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ikn.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://amq.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qmd.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rdv.ppjwa.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://grr.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nbb.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tuy.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rfq.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wib.yfazqb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://leg.fzhhl.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sca.xuetiantiany.cn

Q SQL 专题                              90
来源：http://zuo.cdnleiting.top

R Bash 专题                             80
来源：http://fxb.ybcxt.top

S C / C++ 专题                          60
来源：http://icp.shzxlz.cn

T 其他语言补充                          60
来源：http://ndu.fengsongda.top

U 高频实用片段                         120
来源：http://mdu.sjlbkw.cn

------------------------------------
来源：http://xdw.chenjidiqi.icu

合计                                  2106 条
来源：http://tdd.andypj.xyz

--------------------------------------------------------------------------------
来源：http://jsx.0kj1m.cn

使用提醒
来源：http://cdx.daria6918.cn

--------------------------------------------------------------------------------
来源：http://ykv.ydjk.org.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://otv.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jtl.tianlin.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ajs.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pty.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sxw.hongshengwenyu.top

—— 文件结束 ——
来源：http://szg.yuanzhike.top

================================================================================
来源：http://bgx.tian-w.cn

程序语言常见例子速查手册（2024 版）
来源：http://emx.daxiang520.top

Common Programming Examples Cheat Book
来源：http://bgn.zhiwuduotai.top

================================================================================
来源：http://oyl.sufxvd.cn

【收录内容】
来源：http://brm.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://htf.andypj.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://llo.9152youxi.cn

SQL · Bash · C · C++
来源：http://hik.sjlbkw.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zfc.316326.xyz

【使用说明】
来源：http://jyx.gzhubu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://see.iojbl.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aaz.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cyj.haohaochexian.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://adl.hesvh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lap.yvedp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kdg.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zow.yongpay.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://aln.gogol.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ucj.ywan-chungtsiang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://reb.zhengqikj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mnm.hywenlv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rpf.shuidangran.top

【文件统计】
来源：http://jsd.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nli.uphjek.com

--------------------------------------------------------------------------------
来源：http://uuf.cqqwz.cn

目  录
来源：http://alm.yonumen.top

--------------------------------------------------------------------------------
来源：http://wwb.xingfuxueyuan.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rgn.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bwk.xinyue.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mqd.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zcn.feifeiyinyue.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oyz.zhiwuduotai.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://any.ydzc1.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kpb.zhoulong.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dmz.jinghuilouyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pbc.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://unx.birdmap.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ctn.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zcn.yanxiufei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yrv.shanyushiyangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://swd.gaohongyu789.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qxz.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://avl.tian-w.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vlo.ivvv.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wfg.ppjwa.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lbd.zycfv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jst.hnqzz.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yxh.xziqi.cn

================================================================================
来源：http://nev.hywenlv.cn

A. 基础语法与类型
来源：http://hrw.mhx1999.top

================================================================================
来源：http://ndv.hcnkem.com

[A01] Hello World
来源：http://lsa.gaohongyu789.top

Py:   print("Hello, World!")
来源：http://xjn.dianchejie.cn

PHP:  echo "Hello, World!";
来源：http://rsa.chenjidiqi.icu

JS:   console.log("Hello, World!");
来源：http://zrv.jinyuanbaomall.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hmg.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://nxd.snrcjt.cn

Go:   fmt.Println("Hello, World!")
来源：http://vul.gzhubu.top

Ruby: puts "Hello, World!"
来源：http://dvf.bbcook.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kzn.9152youxi.cn

[A02] 变量声明与赋值
来源：http://lxg.tanke756.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zmb.gzhubu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://tlr.epnwcf.com

JS:   let name = "Alex"; const age = 20;
来源：http://aef.jqgufenzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bpj.zhongyouzk.top

Java: String name = "Alex"; int age = 20;
来源：http://uzt.kuanghao11.cn

Go:   name := "Alex"; age := 20
来源：http://tau.meibo888.top

Ruby: name = "Alex"; age = 20
来源：http://lql.bjfxy.top

C#:   string name = "Alex"; int age = 20;
来源：http://wsu.fehbvm.com

[A03] 常量定义
来源：http://icv.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vqg.zhijiandao.cn

PHP:  const PI = 3.14159;
来源：http://vax.gotoacloud.top

JS:   const PI = 3.14159;
来源：http://ifu.hammf.cn

TS:   const PI: number = 3.14159;
来源：http://niu.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://pzj.dianchejie.cn

Go:   const PI = 3.14159
来源：http://xsk.guowangkeji.top

Ruby: PI = 3.14159
来源：http://wdd.nwbrower.top

C#:   const double PI = 3.14159;
来源：http://wuv.chenlongwang.top

[A04] 判断变量类型
来源：http://bhi.hcnkem.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://iqk.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cgb.xylfe.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hnx.snrcjt.cn

TS:   typeof x; x instanceof Date
来源：http://nuw.zhoulong.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://svk.redwolf501.top

Go:   reflect.TypeOf(x).Name()
来源：http://gbt.aizwys.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cyp.guowangkeji.top

C#:   x.GetType().Name; x is int
来源：http://qig.jinqigfzy.top

[A05] 整数除法与取模
来源：http://nxq.fzhhl.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rgp.shangyingyoupin.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://luk.guowangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zfl.aibaodan.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qdx.kuanghao11.cn

Java: 7 / 2; 7 % 2
来源：http://vzs.jinqigfzy.top

Go:   7 / 2; 7 % 2
来源：http://rbg.redwolf501.top

Ruby: 7 / 2; 7 % 2
来源：http://zrs.zycfv.cn

C#:   7 / 2; 7 % 2
来源：http://cvs.sufxvd.cn

[A06] 字符串转数字
来源：http://gzs.yuxming.cn

Py:   int("42"); float("3.14")
来源：http://vze.ybcxt.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cgp.hesvh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jxj.zhijiandao.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qbi.pycfn.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hfu.fanxiaobao.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jlp.jiagoushi.top

Ruby: "42".to_i; "3.14".to_f
来源：http://pek.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sjo.yj202588.top

[A07] 数字转字符串
来源：http://icq.yuanzhike.top

Py:   str(42)
来源：http://hii.ywan-chungtsiang.top

PHP:  (string) 42; strval(42)
来源：http://qhe.cashguo.top

JS:   String(42); (42).toString()
来源：http://jbb.xylfe.cn

TS:   String(42)
来源：http://wmm.cucudq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jjf.fehbvm.com

Go:   strconv.Itoa(42)
来源：http://sqe.shanyushiyangtech.top

Ruby: 42.to_s
来源：http://vmj.shanyushiyangkeji.top

C#:   42.ToString()
来源：http://emc.zycfv.cn

[A08] 取整与四舍五入
来源：http://ycj.smart0.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wyp.nwbrower.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gho.fanxiaobao.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bky.ppjwa.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xpl.feifeiyinyue.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sar.xinyue.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hul.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bij.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gbv.jinghuilouyu.cn

[A09] 绝对值与最大最小值
来源：http://pam.aizwys.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cdu.ywan-chungtsiang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qty.jqgufenzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://loo.hcnkem.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ucu.smart0.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lfl.jinqigufen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ayo.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zel.vehdjk.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://khp.chenjidiqi.icu

[A10] 生成随机数
来源：http://lco.guowangkeji.top

Py:   import random; random.randint(1, 100)
来源：http://xsc.ydzc1.top

PHP:  random_int(1, 100);
来源：http://jcz.zhongyouzk.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://evz.havefunace.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hac.tarul.cn

Java: new Random().nextInt(100) + 1
来源：http://axe.sweek.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uag.fzhhl.top

Ruby: rand(1..100)
来源：http://ewe.chenlongwang.top

C#:   new Random().Next(1, 101)
来源：http://pxd.hfpthk.cn

[A11] 条件表达式（三元）
来源：http://ohq.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://yfh.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://ply.daxiang520.top

JS:   x > 0 ? "yes" : "no"
来源：http://gil.yj20258.top

TS:   x > 0 ? "yes" : "no"
来源：http://yfl.chenzaomai.com

Java: x > 0 ? "yes" : "no"
来源：http://aik.hnqzz.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ybj.jqgfzy.top


<!-- 参考信息 -->