代发 wailian999

[U71] PHP：抛出异常
来源：http://bvk.cqqwz.cn

throw new RuntimeException("失败", 500);
来源：http://jcc.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://guy.snrcjt.cn

error_log("失败: " . $e->getMessage());
来源：http://cic.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://vkr.hfpthk.cn

parse_ini_file("config.ini", true)
来源：http://bke.yonumen.top

[U74] PHP：读取环境变量
来源：http://nsn.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://pid.sxryk.cn

[U75] PHP：依赖注入
来源：http://did.hcnkem.com

composer require psr/container
来源：http://pzd.jqgfzy.top

[U76] PHP：简单路由
来源：http://mci.kuanghao11.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tgm.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://nvt.dianchejie.cn

composer require twig/twig
来源：http://pjp.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://nkc.sufxvd.cn

composer require --dev phpunit/phpunit
来源：http://yxz.zhongyouzk.top

[U79] PHP：静态分析
来源：http://wna.xylfe.cn

composer require --dev phpstan/phpstan
来源：http://ytf.shuidangran.top

[U80] PHP：代码规范修复
来源：http://umv.dianchejie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://osv.daxiang520.top

[U81] JS：初始化项目
来源：http://qgs.yanxiufei.cn

npm init -y;  npm i express
来源：http://nib.nwbrower.top

[U82] JS：package.json 脚本
来源：http://jzl.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hna.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://ynl.shangyingyoupin.top

export const a = 1;  import { a } from "./m.js";
来源：http://fcz.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://clg.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://ukg.tarul.cn

[U85] JS：可选链
来源：http://kzf.jqgfzy.top

a?.b?.c
来源：http://ezz.iojbl.cn

[U86] JS：空值合并
来源：http://qdy.fzhhl.top

a ?? b
来源：http://pyt.sxryk.cn

[U87] JS：解构默认值
来源：http://zwz.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://tsd.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://fzu.tianlin.xyz

{ ...a, ...b }
来源：http://phy.tanke756.top

[U89] JS：数组去重
来源：http://nru.jinqigufen.top

[...new Set(arr)]
来源：http://gor.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://xvg.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://lmn.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://nnt.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pba.daxiang520.top

[U92] JS：深拷贝
来源：http://fic.guowangkeji.top

structuredClone(obj)
来源：http://npt.yangfankeji.com

[U93] JS：模板字符串
来源：http://wcg.fktsv.cn

`共 ${n} 条`
来源：http://wvc.cdnleiting.top

[U94] JS：箭头函数
来源：http://mdd.cdnleiting.top

const double = x => x * 2;
来源：http://dmp.tarul.cn

[U95] JS：Promise 包装
来源：http://jyc.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://dpp.chenzaomai.com

[U96] JS：async/await 与异常
来源：http://kxx.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ykl.chenlongwang.top

[U97] JS：并发请求
来源：http://qfd.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tcq.dianchejie.cn

[U98] JS：fetch 带 JSON
来源：http://scg.tanke756.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mvm.chenjidiqi.icu

[U99] JS：事件监听
来源：http://muk.redwolf501.top

el.addEventListener("click", e => {})
来源：http://mtr.hfpthk.cn

[U100] JS：DOM 查询
来源：http://tdf.yongpay.top

document.querySelector(".item")
来源：http://hwf.xuetiantiany.cn

[U101] JS：classList 操作
来源：http://dyg.yuxming.cn

el.classList.toggle("active")
来源：http://sxp.xuetiantiany.cn

[U102] JS：本地存储
来源：http://idl.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hzn.shangyingyoupin.top

[U103] JS：定时器
来源：http://ijj.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fqy.hongshengwenyu.top

[U104] JS：防抖
来源：http://ntg.gogol.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yiz.zhaomingkeji.xyz

[U105] JS：节流
来源：http://lrk.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kdf.yangfankeji.com

[U106] JS：日期格式化
来源：http://pzr.zhaomingkeji.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nhj.shanyushiyangtech.top

[U107] JS：数字千分位
来源：http://eqq.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vev.daria6918.cn

[U108] JS：随机整数
来源：http://dlw.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nkh.c1oappe.top

[U109] JS：数组分组
来源：http://yzv.chenzaomai.com

Object.groupBy(arr, x => x.type)
来源：http://tqh.fengsongda.top

[U110] JS：数组分块
来源：http://lfi.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yvm.andypj.xyz

[U111] JS：对象转 Map
来源：http://rcr.sweek.top

new Map(Object.entries(obj))
来源：http://tkh.yanxiufei.cn

[U112] JS：字符串补位
来源：http://bhh.sxryk.cn

"7".padStart(3, "0")
来源：http://tjg.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://drd.svipenyu.cn

s.replaceAll("a", "b")
来源：http://yvq.iojbl.cn

[U114] JS：JSON 深比较
来源：http://rxx.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ynt.52xcode.cn

[U115] JS：生成 UUID
来源：http://xpt.hysaishi.cn

crypto.randomUUID()
来源：http://jix.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://sxm.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://twv.gogol.net.cn

[U117] JS：单元测试
来源：http://ltg.ywan-chungtsiang.top

npm i -D vitest;  npx vitest
来源：http://sax.guannengcc.top

[U118] JS：开发服务器
来源：http://wsg.hesvh.cn

npm i -D vite;  npx vite
来源：http://tla.uphjek.com

[U119] JS：生产构建
来源：http://zpi.jinqigfzy.top

npx vite build
来源：http://wrs.zhiwuduotai.top

[U120] JS：读取环境变量（Vite）
来源：http://mxt.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://ohm.dashuyun.cn

================================================================================
来源：http://lsg.dashuyun.cn

统计汇总
来源：http://tmk.vqdsnc.cn

================================================================================
来源：http://zrr.jinyuanbaomall.cn

按语言统计（条）：
来源：http://iwm.andypj.xyz

Python ......... 252
来源：http://abp.yangfankeji.com

PHP ............ 252
来源：http://hmb.hammf.cn

JavaScript ..... 252
来源：http://plv.chenzaomai.com

TypeScript ..... 212
来源：http://hyl.ydzc1.top

Java ........... 212
来源：http://cfm.zhixingplan.top

Go ............. 212
来源：http://dpe.daria6918.cn

Ruby ........... 212
来源：http://jch.tarul.cn

C# ............. 212
来源：http://beo.jinyuanbaomall.cn

C .............. 30
来源：http://ism.gotoacloud.top

C++ ............ 30
来源：http://kql.hesvh.cn

SQL ............ 90
来源：http://ncr.yangfankeji.com

Bash ........... 80
来源：http://osm.snrcjt.cn

Kotlin ......... 15
来源：http://pou.0kj1m.cn

Swift .......... 15
来源：http://jyu.gzhubu.top

Lua ............ 10
来源：http://rhi.yanxiufei.cn

Perl ........... 10
来源：http://pgp.havefunace.top

Scala .......... 10
来源：http://zpk.tanke756.top

------------------------------------
来源：http://qnv.hnqzz.top

合计 ........... 2106 条
来源：http://vdf.hongshengwenyu.top

按章节统计：
来源：http://uxs.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://srg.chenlongwang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kce.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lkh.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qnp.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qck.zdbjq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sku.bjfxy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ubu.tarul.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nnj.epnwcf.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bli.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qrb.yuxming.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gwl.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jlr.mhx1999.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bgv.dashuyun.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cpy.nanxinkj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xjj.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://poi.feifeiyinyue.top

Q SQL 专题                              90
来源：http://typ.uphjek.com

R Bash 专题                             80
来源：http://srk.hywenlv.cn

S C / C++ 专题                          60
来源：http://kql.gaohongyu789.top

T 其他语言补充                          60
来源：http://jkp.jqgfzy.top

U 高频实用片段                         120
来源：http://cmc.zhaomingkeji.xyz

------------------------------------
来源：http://mmb.cdnleiting.top

合计                                  2106 条
来源：http://uoe.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://yor.tian-w.cn

使用提醒
来源：http://ech.cucudq.cn

--------------------------------------------------------------------------------
来源：http://ybp.ctjpmb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zje.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yyg.hfpthk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rju.zhixingplan.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wnu.chenlongwang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xgj.zhixingplan.top

—— 文件结束 ——
来源：http://vbt.shzxlz.cn

================================================================================
来源：http://gwc.shangyingyoupin.top

程序语言常见例子速查手册（2024 版）
来源：http://qoq.yvedp.cn

Common Programming Examples Cheat Book
来源：http://wds.zhixingplan.top

================================================================================
来源：http://rcg.hfpthk.cn

【收录内容】
来源：http://fia.snrcjt.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jqu.ydjk.org.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gxv.redwolf501.top

SQL · Bash · C · C++
来源：http://yrm.bjfxy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hir.gaohongyu789.top

【使用说明】
来源：http://srq.316326.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hdd.zhiwuduotai.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://upg.bbcook.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wfd.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fph.hnqzz.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jhb.yongpay.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ctz.aibaodan.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cew.xinyue.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fqq.zhiwuduotai.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ntq.zdqjudy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://unn.xingfuxueyuan.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://smu.wangdashe.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qwa.ydzc1.top

【文件统计】
来源：http://gww.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dji.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://cpq.nwbrower.top

目  录
来源：http://pgt.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://kou.yangfankeji.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qeq.ivvv.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zfd.hfpthk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gnt.daria6918.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ctc.vehdjk.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ymd.yuanzhike.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jiy.smart0.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tkq.shanyushiyangtech.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://awq.sufxvd.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ozd.vehdjk.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xsy.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fvm.yj20258888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gjb.52xcode.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vqa.andypj.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wgn.xinyue.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wth.yongpay.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qrb.sjlbkw.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ety.jianghu66.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://trb.jinyuanbaomall.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tfq.nanxinkj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ffb.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dvt.sxryk.cn

================================================================================
来源：http://ycm.yuanzhike.top

A. 基础语法与类型
来源：http://twh.gaohongyu789.top

================================================================================
来源：http://aae.guannengcc.top

[A01] Hello World
来源：http://gpa.jinghuilouyu.cn

Py:   print("Hello, World!")
来源：http://phh.fengsongda.top

PHP:  echo "Hello, World!";
来源：http://pow.zhixingplan.top

JS:   console.log("Hello, World!");
来源：http://afc.chenjidiqi.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vay.ctjpmb.com

Java: System.out.println("Hello, World!");
来源：http://psq.yuxming.cn

Go:   fmt.Println("Hello, World!")
来源：http://nqr.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://pyo.dianchejie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ihc.cheryme.top

[A02] 变量声明与赋值
来源：http://ewx.hnxiangtu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ric.fzhhl.top

PHP:  $name = "Alex"; $age = 20;
来源：http://daw.smart0.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://rjb.haohaochexian.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aqw.aibaodan.cn

Java: String name = "Alex"; int age = 20;
来源：http://qei.sjlbkw.cn

Go:   name := "Alex"; age := 20
来源：http://ivf.yvedp.cn

Ruby: name = "Alex"; age = 20
来源：http://rgv.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://hwu.hywenlv.cn

[A03] 常量定义
来源：http://mbb.zhoulong.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vwh.gzhubu.top

PHP:  const PI = 3.14159;
来源：http://fst.gaohongyu789.top

JS:   const PI = 3.14159;
来源：http://mxy.yfazqb.com

TS:   const PI: number = 3.14159;
来源：http://byw.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://hwk.fktsv.cn

Go:   const PI = 3.14159
来源：http://wff.yvedp.cn

Ruby: PI = 3.14159
来源：http://svp.gaohongyu789.top

C#:   const double PI = 3.14159;
来源：http://rwt.sufxvd.cn

[A04] 判断变量类型
来源：http://diy.shzxlz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://whs.hywenlv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://alk.shangyingyoupin.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pub.zhengqikj.top

TS:   typeof x; x instanceof Date
来源：http://nuh.zhongyouzk.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mjr.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://ctb.aibaodan.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sgr.ybcxt.top

C#:   x.GetType().Name; x is int
来源：http://znj.zdqjudy.top

[A05] 整数除法与取模
来源：http://gds.jiagoushi.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qew.ywan-chungtsiang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qlg.xinyue.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hgs.svipenyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wgf.tanke756.top

Java: 7 / 2; 7 % 2
来源：http://zbn.gogol.net.cn

Go:   7 / 2; 7 % 2
来源：http://mjo.fanxiaobao.xyz

Ruby: 7 / 2; 7 % 2
来源：http://bmb.wangdashe.top

C#:   7 / 2; 7 % 2
来源：http://fnv.sxryk.cn

[A06] 字符串转数字
来源：http://yjg.yuanzhike.top

Py:   int("42"); float("3.14")
来源：http://jhm.tian-w.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://udu.gotoacloud.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ugz.smart0.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://cht.sweek.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lnq.shanyushiyangtech.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vhg.feifeiyinyue.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qea.smart0.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ghj.hfpthk.cn

[A07] 数字转字符串
来源：http://ueb.fengsongda.top

Py:   str(42)
来源：http://nxv.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://puw.zhoulong.xyz

JS:   String(42); (42).toString()
来源：http://nmi.ivvv.top

TS:   String(42)
来源：http://asy.bbcook.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://odm.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://wdl.bbcook.cn

Ruby: 42.to_s
来源：http://wca.zhongyouzk.top

C#:   42.ToString()
来源：http://xas.zdqjudy.top

[A08] 取整与四舍五入
来源：http://dlj.ivvv.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gcc.fzhhl.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ywt.ydzc1.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dzg.zhongyouzk.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fds.sjlbkw.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rfg.jinqigfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dpd.gogol.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pqy.ydjk.org.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rbw.birdmap.top

[A09] 绝对值与最大最小值
来源：http://eza.yuxming.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tvq.kuanghao11.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cgm.shangyingyoupin.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fzy.jinqigfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yfe.xziqi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://btk.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rpv.zdqjudy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pzt.daria6918.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://azs.xuanzx.com

[A10] 生成随机数
来源：http://uhj.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://fbe.zhiwuduotai.top

PHP:  random_int(1, 100);
来源：http://skp.quarkkingdee.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://epg.shuidangran.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ebt.hongshengwenyu.top

Java: new Random().nextInt(100) + 1
来源：http://bpc.quarkkingdee.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zgl.ivvv.top

Ruby: rand(1..100)
来源：http://nju.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://wwl.shzxlz.cn

[A11] 条件表达式（三元）
来源：http://olv.jqgfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://rjr.tanke756.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://sca.vqdsnc.cn


<!-- 参考信息 -->