代发 wailian999

[U69] PHP：PDO 预处理
来源：http://tcp.daria6918.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rrr.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://tns.aizwys.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mwx.xingfuxueyuan.xyz

[U71] PHP：抛出异常
来源：http://twv.svipenyu.cn

throw new RuntimeException("失败", 500);
来源：http://ydo.yonumen.top

[U72] PHP：写错误日志
来源：http://jtv.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://hkt.jinghuilouyu.cn

[U73] PHP：读取 ini 配置
来源：http://omo.dianchejie.cn

parse_ini_file("config.ini", true)
来源：http://kmx.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://lod.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://pqj.yj202588.top

[U75] PHP：依赖注入
来源：http://rde.yuanzhike.top

composer require psr/container
来源：http://ako.daria6918.cn

[U76] PHP：简单路由
来源：http://dgh.yvedp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jjg.nanxinkj.top

[U77] PHP：模板渲染
来源：http://hhk.jlsjyb.cn

composer require twig/twig
来源：http://opk.ehwqpu.com

[U78] PHP：单元测试
来源：http://bui.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://neq.hesvh.cn

[U79] PHP：静态分析
来源：http://wpd.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://dbe.gzhubu.top

[U80] PHP：代码规范修复
来源：http://eto.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://okv.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://dwo.nanxinkj.top

npm init -y;  npm i express
来源：http://jcn.9152youxi.cn

[U82] JS：package.json 脚本
来源：http://kic.nwbrower.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tar.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://sqz.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bwg.tarul.cn

[U84] JS：CommonJS 写法
来源：http://ioq.chenlongwang.top

module.exports = { a };  const { a } = require("./m");
来源：http://zfc.hesvh.cn

[U85] JS：可选链
来源：http://szc.daxiang520.top

a?.b?.c
来源：http://las.hnxiangtu.top

[U86] JS：空值合并
来源：http://yby.sysykeji.top

a ?? b
来源：http://jmh.zdbjq.cn

[U87] JS：解构默认值
来源：http://llo.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://jsf.haohaochexian.top

[U88] JS：对象展开合并
来源：http://jxg.daxiang520.top

{ ...a, ...b }
来源：http://sin.shanyushiyangtech.top

[U89] JS：数组去重
来源：http://jks.shangyingyoupin.top

[...new Set(arr)]
来源：http://cux.sjlbkw.cn

[U90] JS：数字数组排序
来源：http://wvw.birdmap.top

[...arr].sort((a, b) => a - b)
来源：http://jrv.epnwcf.com

[U91] JS：对象键值遍历
来源：http://yxe.wangshuangyany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://trc.vehdjk.com

[U92] JS：深拷贝
来源：http://wci.jiagoushi.top

structuredClone(obj)
来源：http://uoi.zhijiandao.cn

[U93] JS：模板字符串
来源：http://eyj.yj20258888.top

`共 ${n} 条`
来源：http://bnw.daria6918.cn

[U94] JS：箭头函数
来源：http://ash.xziqi.cn

const double = x => x * 2;
来源：http://aik.smart0.xyz

[U95] JS：Promise 包装
来源：http://xfk.xingfuxueyuan.xyz

new Promise((resolve, reject) => {})
来源：http://jds.meibo888.top

[U96] JS：async/await 与异常
来源：http://tby.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ade.hcnkem.com

[U97] JS：并发请求
来源：http://bsn.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kbv.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://mdg.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://abz.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://rls.yongpay.top

el.addEventListener("click", e => {})
来源：http://qez.c1oappe.top

[U100] JS：DOM 查询
来源：http://oec.cheryme.top

document.querySelector(".item")
来源：http://dtc.gogol.net.cn

[U101] JS：classList 操作
来源：http://vjl.quarkkingdee.top

el.classList.toggle("active")
来源：http://tcn.smart0.xyz

[U102] JS：本地存储
来源：http://enz.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://skj.jiagoushi.top

[U103] JS：定时器
来源：http://psr.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://alh.epnwcf.com

[U104] JS：防抖
来源：http://hyo.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cuw.dashuyun.cn

[U105] JS：节流
来源：http://cdi.feifeiyinyue.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hte.ydjk.org.cn

[U106] JS：日期格式化
来源：http://xqa.kuanghao11.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lvz.ppjwa.cn

[U107] JS：数字千分位
来源：http://ddg.hysaishi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jsq.guowangkeji.top

[U108] JS：随机整数
来源：http://ucr.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xtw.jyoumei.cn

[U109] JS：数组分组
来源：http://kyx.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://tjc.hysaishi.cn

[U110] JS：数组分块
来源：http://kxk.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hwj.hywenlv.cn

[U111] JS：对象转 Map
来源：http://wmv.fengsongda.top

new Map(Object.entries(obj))
来源：http://hcl.tianlin.xyz

[U112] JS：字符串补位
来源：http://etg.bbcook.cn

"7".padStart(3, "0")
来源：http://fat.svipenyu.cn

[U113] JS：正则替换全部
来源：http://bfz.redwolf501.top

s.replaceAll("a", "b")
来源：http://qvj.epnwcf.com

[U114] JS：JSON 深比较
来源：http://mpo.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vbr.jinghuilouyu.cn

[U115] JS：生成 UUID
来源：http://epi.ppjwa.cn

crypto.randomUUID()
来源：http://eyx.jinghuilouyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://qgb.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://hyj.guowangkeji.top

[U117] JS：单元测试
来源：http://jxe.redwolf501.top

npm i -D vitest;  npx vitest
来源：http://ylu.hywenlv.cn

[U118] JS：开发服务器
来源：http://pum.tanke756.top

npm i -D vite;  npx vite
来源：http://szl.hysaishi.cn

[U119] JS：生产构建
来源：http://unx.zycfv.cn

npx vite build
来源：http://vyw.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://nxd.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://xbj.jlsjyb.cn

================================================================================
来源：http://rjz.shzxlz.cn

统计汇总
来源：http://ztg.hywenlv.cn

================================================================================
来源：http://iex.tanke756.top

按语言统计（条）：
来源：http://aso.hammf.cn

Python ......... 252
来源：http://ull.chenzaomai.com

PHP ............ 252
来源：http://qac.c1oappe.top

JavaScript ..... 252
来源：http://vel.svipenyu.cn

TypeScript ..... 212
来源：http://pye.ivvv.top

Java ........... 212
来源：http://dlh.zhengqikj.top

Go ............. 212
来源：http://ffj.yuanzhike.top

Ruby ........... 212
来源：http://cck.chenlongwang.top

C# ............. 212
来源：http://zut.daxiang520.top

C .............. 30
来源：http://vkr.chenlongwang.top

C++ ............ 30
来源：http://gif.jyoumei.cn

SQL ............ 90
来源：http://zra.zhixingplan.top

Bash ........... 80
来源：http://qvz.svipenyu.cn

Kotlin ......... 15
来源：http://nwx.hywenlv.cn

Swift .......... 15
来源：http://dmi.zhoulong.xyz

Lua ............ 10
来源：http://ifm.zdqjudy.top

Perl ........... 10
来源：http://mhn.hnxiangtu.top

Scala .......... 10
来源：http://lvi.jqgufenzy.top

------------------------------------
来源：http://nmw.andypj.xyz

合计 ........... 2106 条
来源：http://ahf.shanyushiyangkeji.top

按章节统计：
来源：http://yoq.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://isx.shanyushiyangtech.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hzt.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lax.jqgfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xmn.nanxuanxn.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xdq.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kgk.fktsv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eju.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://alq.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qiu.epnwcf.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zcd.daxiang520.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kwr.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uwj.yonumen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nac.tian-w.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gms.cucudq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://skl.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kvr.shangyingyoupin.top

Q SQL 专题                              90
来源：http://tdu.c1oappe.top

R Bash 专题                             80
来源：http://geg.nwbrower.top

S C / C++ 专题                          60
来源：http://atp.epnwcf.com

T 其他语言补充                          60
来源：http://obe.tian-w.cn

U 高频实用片段                         120
来源：http://jyh.vehdjk.com

------------------------------------
来源：http://bop.fanxiaobao.xyz

合计                                  2106 条
来源：http://ztz.yj20258888.top

--------------------------------------------------------------------------------
来源：http://xkk.jinghuilouyu.cn

使用提醒
来源：http://kjx.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://wni.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aoh.ehwqpu.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xac.svipenyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://voi.redwolf501.top

在旧版本上使用前请先确认语法支持情况。
来源：http://oyp.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nzw.guowangkeji.top

—— 文件结束 ——
来源：http://cfp.pycfn.com

================================================================================
来源：http://vrl.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://grn.ydzc1.top

Common Programming Examples Cheat Book
来源：http://ydi.ivvv.top

================================================================================
来源：http://ptz.dashuyun.cn

【收录内容】
来源：http://rbl.vehdjk.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://gpl.sufxvd.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lap.0kj1m.cn

SQL · Bash · C · C++
来源：http://wrk.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pqa.epnwcf.com

【使用说明】
来源：http://cxp.uphjek.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://inu.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dso.andypj.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dfn.bjfxy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nut.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://abv.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nar.nwbrower.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ahi.uphjek.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zhl.jiagoushi.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gna.ydjk.org.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zyq.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://drw.shzxlz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://acs.ehwqpu.com

【文件统计】
来源：http://cbk.yj202588.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gib.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://jwq.chenzaomai.com

目  录
来源：http://mfr.sweek.top

--------------------------------------------------------------------------------
来源：http://tvd.yongpay.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yew.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pxb.jlsjyb.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fkl.mhx1999.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bjg.daxiang520.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wbd.chenjidiqi.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lvn.andypj.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oje.fehbvm.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lms.cqqwz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://idm.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mre.hongshengwenyu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://egh.tian-w.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://piu.dashuyun.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gmn.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ywa.quarkkingdee.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ive.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://thq.sjlbkw.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zzw.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://abr.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xaj.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rwq.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bte.nanxinkj.top

================================================================================
来源：http://rdo.yj20258.top

A. 基础语法与类型
来源：http://his.jinghuilouyu.cn

================================================================================
来源：http://zqr.ctjpmb.com

[A01] Hello World
来源：http://rrp.chenjidiqi.icu

Py:   print("Hello, World!")
来源：http://ejj.andypj.xyz

PHP:  echo "Hello, World!";
来源：http://gah.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://rvq.xylfe.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xcm.yuxming.cn

Java: System.out.println("Hello, World!");
来源：http://fse.snrcjt.cn

Go:   fmt.Println("Hello, World!")
来源：http://kuo.sufxvd.cn

Ruby: puts "Hello, World!"
来源：http://ruv.aizwys.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kll.sysykeji.top

[A02] 变量声明与赋值
来源：http://hpy.dashuyun.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vwk.jinqigfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wvy.cashguo.top

JS:   let name = "Alex"; const age = 20;
来源：http://amc.zhoulong.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lbi.yanxiufei.cn

Java: String name = "Alex"; int age = 20;
来源：http://xaf.ybcxt.top

Go:   name := "Alex"; age := 20
来源：http://vtx.aizwys.cn

Ruby: name = "Alex"; age = 20
来源：http://nhc.ywan-chungtsiang.top

C#:   string name = "Alex"; int age = 20;
来源：http://kai.ivvv.top

[A03] 常量定义
来源：http://okk.jinghuilouyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://krm.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://lur.smart0.xyz

JS:   const PI = 3.14159;
来源：http://sut.jinqigfzy.top

TS:   const PI: number = 3.14159;
来源：http://dfq.hesvh.cn

Java: static final double PI = 3.14159;
来源：http://wqj.jlsjyb.cn

Go:   const PI = 3.14159
来源：http://zba.iojbl.cn

Ruby: PI = 3.14159
来源：http://sip.hcnkem.com

C#:   const double PI = 3.14159;
来源：http://sdt.yanxiufei.cn

[A04] 判断变量类型
来源：http://lzk.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://emo.yangfankeji.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zvl.nwbrower.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ukm.sweek.top

TS:   typeof x; x instanceof Date
来源：http://ama.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pfl.yj202588.top

Go:   reflect.TypeOf(x).Name()
来源：http://cdf.fanxiaobao.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://ehb.yvedp.cn

C#:   x.GetType().Name; x is int
来源：http://biw.chenlongwang.top

[A05] 整数除法与取模
来源：http://kff.jiagoushi.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pzz.xuanzx.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://rlf.gzhubu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sdg.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rer.yanxiufei.cn

Java: 7 / 2; 7 % 2
来源：http://lpp.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://whq.zdbjq.cn

Ruby: 7 / 2; 7 % 2
来源：http://vre.fktsv.cn

C#:   7 / 2; 7 % 2
来源：http://xkn.316326.xyz

[A06] 字符串转数字
来源：http://pkj.0kj1m.cn

Py:   int("42"); float("3.14")
来源：http://cdy.zhijiandao.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kah.pycfn.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rut.yangfankeji.com

TS:   parseInt("42", 10); Number("42")
来源：http://jec.havefunace.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mnb.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kfp.bjfxy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://pmd.zhongyouzk.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://han.wangshuangyany.cn

[A07] 数字转字符串
来源：http://avb.smart0.xyz

Py:   str(42)
来源：http://xuk.zycfv.cn

PHP:  (string) 42; strval(42)
来源：http://shd.gogol.net.cn

JS:   String(42); (42).toString()
来源：http://dkk.zhiwuduotai.top

TS:   String(42)
来源：http://vpi.zdbjq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bmi.epnwcf.com

Go:   strconv.Itoa(42)
来源：http://yut.tanke756.top

Ruby: 42.to_s
来源：http://okg.xziqi.cn

C#:   42.ToString()
来源：http://otp.gzhubu.top

[A08] 取整与四舍五入
来源：http://hwk.iojbl.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rso.xinyue.icu

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ulw.ctjpmb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tff.zhixingplan.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ygc.aizwys.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://phi.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tkc.jlsjyb.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wpt.yuxming.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gbp.fengsongda.top

[A09] 绝对值与最大最小值
来源：http://wiz.uphjek.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ehy.chenjidiqi.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xce.cdnleiting.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wvk.sysykeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fta.zycfv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xyg.ivvv.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nuw.zhongyouzk.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lnq.yj20258888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hpl.xuanzx.com

[A10] 生成随机数
来源：http://xsn.yuanzhike.top

Py:   import random; random.randint(1, 100)
来源：http://ltf.jqgufenzy.top

PHP:  random_int(1, 100);
来源：http://nli.fanxiaobao.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nof.xingfuxueyuan.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mjd.shuidangran.top

Java: new Random().nextInt(100) + 1
来源：http://xkv.bjfxy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://htu.yueranfly.top

Ruby: rand(1..100)
来源：http://esj.andypj.xyz


<!-- 参考信息 -->