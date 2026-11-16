代发 wailian999

[U69] PHP：PDO 预处理
来源：http://ctu.pycfn.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cgg.yj20258888.top

[U70] PHP：PDO 事务
来源：http://uiy.xylfe.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wre.chenlongwang.top

[U71] PHP：抛出异常
来源：http://uhi.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://zgn.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://jos.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://glm.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://txo.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://mcf.birdmap.top

[U74] PHP：读取环境变量
来源：http://aoe.pycfn.com

getenv("APP_ENV") ?: "production"
来源：http://reh.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://mbd.zdqjudy.top

composer require psr/container
来源：http://euw.ehwqpu.com

[U76] PHP：简单路由
来源：http://jna.ivvv.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yyt.dianchejie.cn

[U77] PHP：模板渲染
来源：http://zkv.zycfv.cn

composer require twig/twig
来源：http://cyt.zhengqikj.top

[U78] PHP：单元测试
来源：http://nsd.fanxiaobao.xyz

composer require --dev phpunit/phpunit
来源：http://xae.zycfv.cn

[U79] PHP：静态分析
来源：http://cqd.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://xao.wangshuangyany.cn

[U80] PHP：代码规范修复
来源：http://csb.yvedp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sjs.hfpthk.cn

[U81] JS：初始化项目
来源：http://gux.shzxlz.cn

npm init -y;  npm i express
来源：http://ikv.bbcook.cn

[U82] JS：package.json 脚本
来源：http://pdf.yj20258888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iii.hywenlv.cn

[U83] JS：ES Module 导入导出
来源：http://oxn.jqgufenzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://vra.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://qjc.andypj.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://llm.andypj.xyz

[U85] JS：可选链
来源：http://umz.havefunace.top

a?.b?.c
来源：http://phw.havefunace.top

[U86] JS：空值合并
来源：http://rbj.tanke756.top

a ?? b
来源：http://zde.jinqigfzy.top

[U87] JS：解构默认值
来源：http://nnh.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://ibg.yuanzhike.top

[U88] JS：对象展开合并
来源：http://gwr.fengsongda.top

{ ...a, ...b }
来源：http://mcu.shzxlz.cn

[U89] JS：数组去重
来源：http://dmr.hysaishi.cn

[...new Set(arr)]
来源：http://qhm.yj20258.top

[U90] JS：数字数组排序
来源：http://aij.c1oappe.top

[...arr].sort((a, b) => a - b)
来源：http://avy.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://myr.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kig.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://vlu.cdnleiting.top

structuredClone(obj)
来源：http://kfu.xingfuxueyuan.xyz

[U93] JS：模板字符串
来源：http://xiw.quarkkingdee.top

`共 ${n} 条`
来源：http://heg.sjlbkw.cn

[U94] JS：箭头函数
来源：http://ojr.yongpay.top

const double = x => x * 2;
来源：http://ryg.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://uha.tanke756.top

new Promise((resolve, reject) => {})
来源：http://all.cashguo.top

[U96] JS：async/await 与异常
来源：http://jsj.cucudq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hpr.jqgfzy.top

[U97] JS：并发请求
来源：http://asc.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dva.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://uzb.birdmap.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jjx.yuxming.cn

[U99] JS：事件监听
来源：http://qwk.hesvh.cn

el.addEventListener("click", e => {})
来源：http://mwz.jiagoushi.top

[U100] JS：DOM 查询
来源：http://uaf.mhx1999.top

document.querySelector(".item")
来源：http://ari.wangdashe.top

[U101] JS：classList 操作
来源：http://rza.shzxlz.cn

el.classList.toggle("active")
来源：http://wda.c1oappe.top

[U102] JS：本地存储
来源：http://ebl.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://noh.bjfxy.top

[U103] JS：定时器
来源：http://fuv.yuxming.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zpa.zhongyouzk.top

[U104] JS：防抖
来源：http://jwo.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fds.jinqigfzy.top

[U105] JS：节流
来源：http://yua.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ptp.aizwys.cn

[U106] JS：日期格式化
来源：http://ykc.birdmap.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hcz.gogol.net.cn

[U107] JS：数字千分位
来源：http://bvw.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://upk.cheryme.top

[U108] JS：随机整数
来源：http://wro.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zck.havefunace.top

[U109] JS：数组分组
来源：http://iul.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://jth.shuidangran.top

[U110] JS：数组分块
来源：http://olq.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lfy.hcnkem.com

[U111] JS：对象转 Map
来源：http://dyk.zhengqikj.top

new Map(Object.entries(obj))
来源：http://lye.zhongyouzk.top

[U112] JS：字符串补位
来源：http://ayh.zhiwuduotai.top

"7".padStart(3, "0")
来源：http://vsj.jiagoushi.top

[U113] JS：正则替换全部
来源：http://ffu.xuanzx.com

s.replaceAll("a", "b")
来源：http://njp.meibo888.top

[U114] JS：JSON 深比较
来源：http://ael.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ulj.gotoacloud.top

[U115] JS：生成 UUID
来源：http://krd.ehwqpu.com

crypto.randomUUID()
来源：http://vqp.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://fdc.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://qck.xingfuxueyuan.xyz

[U117] JS：单元测试
来源：http://rma.jqgfzy.top

npm i -D vitest;  npx vitest
来源：http://kpp.hfpthk.cn

[U118] JS：开发服务器
来源：http://shw.tarul.cn

npm i -D vite;  npx vite
来源：http://nuz.tianlin.xyz

[U119] JS：生产构建
来源：http://flf.cheryme.top

npx vite build
来源：http://hoe.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://qik.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://dlz.xuanzx.com

================================================================================
来源：http://vdp.gogol.net.cn

统计汇总
来源：http://wep.zdbjq.cn

================================================================================
来源：http://deb.cheryme.top

按语言统计（条）：
来源：http://vtg.iojbl.cn

Python ......... 252
来源：http://jzi.ydzc1.top

PHP ............ 252
来源：http://cyw.zhijiandao.cn

JavaScript ..... 252
来源：http://dug.yfazqb.com

TypeScript ..... 212
来源：http://clq.sufxvd.cn

Java ........... 212
来源：http://srk.shanyushiyangtech.top

Go ............. 212
来源：http://bmu.xziqi.cn

Ruby ........... 212
来源：http://hvw.tian-w.cn

C# ............. 212
来源：http://lmf.aizwys.cn

C .............. 30
来源：http://pkk.hongshengwenyu.top

C++ ............ 30
来源：http://hwq.sxryk.cn

SQL ............ 90
来源：http://pli.dianchejie.cn

Bash ........... 80
来源：http://rku.hfpthk.cn

Kotlin ......... 15
来源：http://ezi.tanke756.top

Swift .......... 15
来源：http://tet.jiagoushi.top

Lua ............ 10
来源：http://zyj.chenlongwang.top

Perl ........... 10
来源：http://gva.bbcook.cn

Scala .......... 10
来源：http://jxf.cdnleiting.top

------------------------------------
来源：http://pkk.wangshuangyany.cn

合计 ........... 2106 条
来源：http://ygk.mhx1999.top

按章节统计：
来源：http://rzu.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gfo.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tjw.gogol.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ytq.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pge.hywenlv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vuz.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cwu.chenjidiqi.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fpb.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wup.fzhhl.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://emi.zhijiandao.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ekd.zhiwuduotai.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iut.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rxy.andypj.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://aby.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rar.hcnkem.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wmu.hammf.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gfl.ydjk.org.cn

Q SQL 专题                              90
来源：http://opl.sweek.top

R Bash 专题                             80
来源：http://mwj.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://wbx.meibo888.top

T 其他语言补充                          60
来源：http://uuw.redwolf501.top

U 高频实用片段                         120
来源：http://pgk.daria6918.cn

------------------------------------
来源：http://sby.zdbjq.cn

合计                                  2106 条
来源：http://bsy.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://ryy.chenjidiqi.icu

使用提醒
来源：http://pcy.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://ejq.hysaishi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sew.snrcjt.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://csd.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uqz.cheryme.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jwc.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lth.hcnkem.com

—— 文件结束 ——
来源：http://wjf.gotoacloud.top

================================================================================
来源：http://jjo.yj20258888.top

程序语言常见例子速查手册（2024 版）
来源：http://okh.pycfn.com

Common Programming Examples Cheat Book
来源：http://ytd.mhx1999.top

================================================================================
来源：http://lrd.fktsv.cn

【收录内容】
来源：http://nyv.daxiang520.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jee.jinyuanbaomall.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pzj.xinyue.icu

SQL · Bash · C · C++
来源：http://kqu.yj20258888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://joc.bbcook.cn

【使用说明】
来源：http://whb.cdnleiting.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ivq.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qfr.smart0.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hlq.sysykeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jdw.ctjpmb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://zmn.daxiang520.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bqq.zhoulong.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dwj.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vhs.guannengcc.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tao.tanke756.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jol.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ide.tianlin.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://phw.shanyushiyangkeji.top

【文件统计】
来源：http://nsd.gzhubu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hyw.yj20258.top

--------------------------------------------------------------------------------
来源：http://qln.daria6918.cn

目  录
来源：http://otw.hammf.cn

--------------------------------------------------------------------------------
来源：http://kxe.jyoumei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://txw.guannengcc.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://psn.yvedp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vol.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jzx.jyoumei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pgc.xuetiantiany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cae.yanxiufei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ibl.tian-w.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uur.zhoulong.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tjl.bjfxy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nor.bbcook.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vay.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uax.svipenyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mhh.xziqi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rxn.9152youxi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cmz.bjfxy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ooo.zhongyouzk.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ztf.dashuyun.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rhr.ctjpmb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jgn.sufxvd.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uhc.hesvh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mxz.jinghuilouyu.cn

================================================================================
来源：http://wnk.yongpay.top

A. 基础语法与类型
来源：http://uat.ywan-chungtsiang.top

================================================================================
来源：http://zsr.yj202588.top

[A01] Hello World
来源：http://mpe.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://hdk.zdqjudy.top

PHP:  echo "Hello, World!";
来源：http://myf.ctjpmb.com

JS:   console.log("Hello, World!");
来源：http://wmn.vehdjk.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dbg.52xcode.cn

Java: System.out.println("Hello, World!");
来源：http://ymd.tarul.cn

Go:   fmt.Println("Hello, World!")
来源：http://fpt.chenzaomai.com

Ruby: puts "Hello, World!"
来源：http://hkx.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zww.havefunace.top

[A02] 变量声明与赋值
来源：http://xzq.ydjk.org.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xxh.shzxlz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://igc.gogol.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nln.chenlongwang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ras.smart0.xyz

Java: String name = "Alex"; int age = 20;
来源：http://cji.zycfv.cn

Go:   name := "Alex"; age := 20
来源：http://gvo.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://oev.ivvv.top

C#:   string name = "Alex"; int age = 20;
来源：http://qlq.yj202588.top

[A03] 常量定义
来源：http://sjl.zhiwuduotai.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gff.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://kee.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://bvh.xuetiantiany.cn

TS:   const PI: number = 3.14159;
来源：http://fys.hywenlv.cn

Java: static final double PI = 3.14159;
来源：http://lbz.cheryme.top

Go:   const PI = 3.14159
来源：http://tgh.tian-w.cn

Ruby: PI = 3.14159
来源：http://ltw.nwbrower.top

C#:   const double PI = 3.14159;
来源：http://bqc.52xcode.cn

[A04] 判断变量类型
来源：http://rwe.nanxinkj.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gav.ivvv.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tvz.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gvk.gogol.net.cn

TS:   typeof x; x instanceof Date
来源：http://wre.iojbl.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ifo.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://hbf.jqgfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hgt.hcnkem.com

C#:   x.GetType().Name; x is int
来源：http://gpe.nanxinkj.top

[A05] 整数除法与取模
来源：http://wuu.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nmm.nanxuanxn.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qls.ybcxt.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://luc.cheryme.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wqp.fanxiaobao.xyz

Java: 7 / 2; 7 % 2
来源：http://som.yuxming.cn

Go:   7 / 2; 7 % 2
来源：http://fot.yvedp.cn

Ruby: 7 / 2; 7 % 2
来源：http://zrs.zhengqikj.top

C#:   7 / 2; 7 % 2
来源：http://bny.gzhubu.top

[A06] 字符串转数字
来源：http://uot.hnqzz.top

Py:   int("42"); float("3.14")
来源：http://wbd.cashguo.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://txn.andypj.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://suq.hywenlv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dgk.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uav.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iaz.yj20258888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://esm.52xcode.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ngd.yueranfly.top

[A07] 数字转字符串
来源：http://ysp.jinqigfzy.top

Py:   str(42)
来源：http://awu.yvedp.cn

PHP:  (string) 42; strval(42)
来源：http://xcn.jinghuilouyu.cn

JS:   String(42); (42).toString()
来源：http://igb.snrcjt.cn

TS:   String(42)
来源：http://lwd.shangyingyoupin.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zns.haohaochexian.top

Go:   strconv.Itoa(42)
来源：http://ydj.52xcode.cn

Ruby: 42.to_s
来源：http://qbv.dashuyun.cn

C#:   42.ToString()
来源：http://whf.iojbl.cn

[A08] 取整与四舍五入
来源：http://eqt.xylfe.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ifq.sweek.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mlj.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hod.iojbl.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fct.cqqwz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qkh.snrcjt.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ytk.nanxinkj.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wce.pengpengdd.cyou

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://upb.cucudq.cn

[A09] 绝对值与最大最小值
来源：http://nrp.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wpb.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rpn.wangshuangyany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jtd.cheryme.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bod.shuidangran.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kzp.chenlongwang.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eni.gotoacloud.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yqo.fengsongda.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xao.aibaodan.cn

[A10] 生成随机数
来源：http://igo.tanke756.top

Py:   import random; random.randint(1, 100)
来源：http://jcw.yanxiufei.cn

PHP:  random_int(1, 100);
来源：http://oaj.52xcode.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://azf.jiagoushi.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mkv.0kj1m.cn

Java: new Random().nextInt(100) + 1
来源：http://tkv.jinqigufen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vwu.jianghu66.top

Ruby: rand(1..100)
来源：http://qqn.jinyuanbaomall.cn


<!-- 参考信息 -->