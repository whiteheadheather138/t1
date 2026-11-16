代发 wailian999

[U69] PHP：PDO 预处理
来源：http://ztj.shuidangran.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lfr.xinyue.icu

[U70] PHP：PDO 事务
来源：http://ezb.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yjz.aizwys.cn

[U71] PHP：抛出异常
来源：http://ubi.tanke756.top

throw new RuntimeException("失败", 500);
来源：http://oxo.bbcook.cn

[U72] PHP：写错误日志
来源：http://fie.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://ude.chenlongwang.top

[U73] PHP：读取 ini 配置
来源：http://vti.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://trd.daxiang520.top

[U74] PHP：读取环境变量
来源：http://akk.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://cfw.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://zln.dianchejie.cn

composer require psr/container
来源：http://ysu.redwolf501.top

[U76] PHP：简单路由
来源：http://sbb.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://flk.fzhhl.top

[U77] PHP：模板渲染
来源：http://sly.cdnleiting.top

composer require twig/twig
来源：http://wfj.zhengqikj.top

[U78] PHP：单元测试
来源：http://tui.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://xme.yj202588.top

[U79] PHP：静态分析
来源：http://jjd.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://bed.yfazqb.com

[U80] PHP：代码规范修复
来源：http://ldz.bbcook.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pup.jinqigufen.top

[U81] JS：初始化项目
来源：http://hbb.yj202588.top

npm init -y;  npm i express
来源：http://gax.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://jhx.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hqf.cheryme.top

[U83] JS：ES Module 导入导出
来源：http://wtk.9152youxi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jmd.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://evs.fanxiaobao.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://uvf.hnqzz.top

[U85] JS：可选链
来源：http://wib.shanyushiyangtech.top

a?.b?.c
来源：http://zly.zhiwuduotai.top

[U86] JS：空值合并
来源：http://fti.hnxiangtu.top

a ?? b
来源：http://sge.cucudq.cn

[U87] JS：解构默认值
来源：http://nrq.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://lys.yongpay.top

[U88] JS：对象展开合并
来源：http://txa.feifeiyinyue.top

{ ...a, ...b }
来源：http://snf.ppjwa.cn

[U89] JS：数组去重
来源：http://qwq.ppjwa.cn

[...new Set(arr)]
来源：http://mfs.epnwcf.com

[U90] JS：数字数组排序
来源：http://bdi.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://hzp.tarul.cn

[U91] JS：对象键值遍历
来源：http://sir.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jqa.ppjwa.cn

[U92] JS：深拷贝
来源：http://gid.meibo888.top

structuredClone(obj)
来源：http://lbw.nanxinkj.top

[U93] JS：模板字符串
来源：http://wct.cheryme.top

`共 ${n} 条`
来源：http://phs.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://pns.jiagoushi.top

const double = x => x * 2;
来源：http://pqm.haohaochexian.top

[U95] JS：Promise 包装
来源：http://hif.havefunace.top

new Promise((resolve, reject) => {})
来源：http://oad.zhijiandao.cn

[U96] JS：async/await 与异常
来源：http://mth.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tcs.jinqigfzy.top

[U97] JS：并发请求
来源：http://rmq.fengsongda.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nto.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://eqc.cqqwz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gdj.cqqwz.cn

[U99] JS：事件监听
来源：http://eji.iojbl.cn

el.addEventListener("click", e => {})
来源：http://tdp.yfazqb.com

[U100] JS：DOM 查询
来源：http://yxc.jinqigufen.top

document.querySelector(".item")
来源：http://qsb.daxiang520.top

[U101] JS：classList 操作
来源：http://npw.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://koc.svipenyu.cn

[U102] JS：本地存储
来源：http://iqz.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zim.ehwqpu.com

[U103] JS：定时器
来源：http://hfy.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wgs.xziqi.cn

[U104] JS：防抖
来源：http://qee.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sdm.hnxiangtu.top

[U105] JS：节流
来源：http://utn.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gyj.havefunace.top

[U106] JS：日期格式化
来源：http://yyc.yonumen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://llx.hywenlv.cn

[U107] JS：数字千分位
来源：http://ohu.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zel.gogol.net.cn

[U108] JS：随机整数
来源：http://vrk.cashguo.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://foz.fktsv.cn

[U109] JS：数组分组
来源：http://ors.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://vdo.hesvh.cn

[U110] JS：数组分块
来源：http://kwp.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fpy.zhengqikj.top

[U111] JS：对象转 Map
来源：http://yvz.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://nui.sweek.top

[U112] JS：字符串补位
来源：http://nkf.hfpthk.cn

"7".padStart(3, "0")
来源：http://qoq.tianlin.xyz

[U113] JS：正则替换全部
来源：http://jqj.jyoumei.cn

s.replaceAll("a", "b")
来源：http://mhj.jianghu66.top

[U114] JS：JSON 深比较
来源：http://brb.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fud.kuanghao11.cn

[U115] JS：生成 UUID
来源：http://xqi.ybcxt.top

crypto.randomUUID()
来源：http://pao.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://lol.jlsjyb.cn

/** @param {string} name */ function f(name) {}
来源：http://iyb.zhixingplan.top

[U117] JS：单元测试
来源：http://zui.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://syn.shzxlz.cn

[U118] JS：开发服务器
来源：http://blh.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://aid.hysaishi.cn

[U119] JS：生产构建
来源：http://ouz.0kj1m.cn

npx vite build
来源：http://ihd.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://uew.zhijiandao.cn

import.meta.env.VITE_API_URL
来源：http://mwc.yj20258.top

================================================================================
来源：http://bqu.bbcook.cn

统计汇总
来源：http://ynz.fengsongda.top

================================================================================
来源：http://zlc.jiagoushi.top

按语言统计（条）：
来源：http://dxb.vehdjk.com

Python ......... 252
来源：http://lpi.jlsjyb.cn

PHP ............ 252
来源：http://iyj.wangdashe.top

JavaScript ..... 252
来源：http://fha.zhoulong.xyz

TypeScript ..... 212
来源：http://cza.fzhhl.top

Java ........... 212
来源：http://ztk.vehdjk.com

Go ............. 212
来源：http://ckj.wangshuangyany.cn

Ruby ........... 212
来源：http://xnj.yj20258.top

C# ............. 212
来源：http://hdw.hongshengwenyu.top

C .............. 30
来源：http://jta.yvedp.cn

C++ ............ 30
来源：http://aec.chenjidiqi.icu

SQL ............ 90
来源：http://efx.quarkkingdee.top

Bash ........... 80
来源：http://wkt.zhiwuduotai.top

Kotlin ......... 15
来源：http://bfm.daria6918.cn

Swift .......... 15
来源：http://qvj.hfpthk.cn

Lua ............ 10
来源：http://ofc.ybcxt.top

Perl ........... 10
来源：http://hrm.pengpengdd.cyou

Scala .......... 10
来源：http://mtt.hysaishi.cn

------------------------------------
来源：http://ytq.birdmap.top

合计 ........... 2106 条
来源：http://ilx.daxiang520.top

按章节统计：
来源：http://tks.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bxc.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xjx.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jzc.zdbjq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cxo.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wji.aizwys.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ciq.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://afa.bjfxy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wph.fzhhl.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nos.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://daq.snrcjt.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qzx.yueranfly.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lfa.yongpay.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ybb.52xcode.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ybz.9152youxi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ayc.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ivj.haohaochexian.top

Q SQL 专题                              90
来源：http://fvt.guannengcc.top

R Bash 专题                             80
来源：http://dyz.haohaochexian.top

S C / C++ 专题                          60
来源：http://tyk.tianlin.xyz

T 其他语言补充                          60
来源：http://kua.shuidangran.top

U 高频实用片段                         120
来源：http://ltq.dianchejie.cn

------------------------------------
来源：http://eom.aizwys.cn

合计                                  2106 条
来源：http://xoi.smart0.xyz

--------------------------------------------------------------------------------
来源：http://zvu.zdbjq.cn

使用提醒
来源：http://mve.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://jzb.yanxiufei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hmq.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://prh.kuanghao11.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://byr.havefunace.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ocp.xylfe.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://npy.gotoacloud.top

—— 文件结束 ——
来源：http://imp.shuidangran.top

================================================================================
来源：http://rcr.sysykeji.top

程序语言常见例子速查手册（2024 版）
来源：http://kdd.jqgfzy.top

Common Programming Examples Cheat Book
来源：http://lbt.snrcjt.cn

================================================================================
来源：http://wun.birdmap.top

【收录内容】
来源：http://vsq.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vxi.52xcode.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mwy.jianghu66.top

SQL · Bash · C · C++
来源：http://fkx.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jes.sxryk.cn

【使用说明】
来源：http://psn.daria6918.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fsj.yuxming.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nhk.snrcjt.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jmd.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nij.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rie.vqdsnc.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ykx.cheryme.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kit.jianghu66.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://svi.yanxiufei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://skv.andypj.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sqk.ybcxt.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bgk.smart0.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zff.zhijiandao.cn

【文件统计】
来源：http://ble.fengsongda.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://noz.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://orp.xziqi.cn

目  录
来源：http://ffo.hesvh.cn

--------------------------------------------------------------------------------
来源：http://ugm.sysykeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://enb.yj20258888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eut.gaohongyu789.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qjq.hfpthk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ktv.sweek.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ddd.ydjk.org.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hch.xuanzx.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gps.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rso.zhijiandao.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gaw.hongshengwenyu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iad.yj20258888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pvi.xuanzx.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://arn.ydjk.org.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wig.zdqjudy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zwr.sysykeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://epy.nanxuanxn.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hwu.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ecr.ywan-chungtsiang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nuq.9152youxi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vwy.hcnkem.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bdx.yongpay.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jye.hesvh.cn

================================================================================
来源：http://had.aibaodan.cn

A. 基础语法与类型
来源：http://avh.tianlin.xyz

================================================================================
来源：http://hhw.gzhubu.top

[A01] Hello World
来源：http://ulb.mhx1999.top

Py:   print("Hello, World!")
来源：http://sto.fktsv.cn

PHP:  echo "Hello, World!";
来源：http://iyj.yanxiufei.cn

JS:   console.log("Hello, World!");
来源：http://tdi.fehbvm.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tuq.gaohongyu789.top

Java: System.out.println("Hello, World!");
来源：http://wrj.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://bch.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://dtl.snrcjt.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ugc.guowangkeji.top

[A02] 变量声明与赋值
来源：http://ure.pycfn.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eij.hfpthk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hxv.jinyuanbaomall.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zyf.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zwx.dianchejie.cn

Java: String name = "Alex"; int age = 20;
来源：http://dwh.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://uuq.smart0.xyz

Ruby: name = "Alex"; age = 20
来源：http://vqo.shanyushiyangtech.top

C#:   string name = "Alex"; int age = 20;
来源：http://mvt.zhixingplan.top

[A03] 常量定义
来源：http://pmp.0kj1m.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iik.shanyushiyangkeji.top

PHP:  const PI = 3.14159;
来源：http://pmc.c1oappe.top

JS:   const PI = 3.14159;
来源：http://lro.quarkkingdee.top

TS:   const PI: number = 3.14159;
来源：http://lvx.guowangkeji.top

Java: static final double PI = 3.14159;
来源：http://lmu.guannengcc.top

Go:   const PI = 3.14159
来源：http://dne.daria6918.cn

Ruby: PI = 3.14159
来源：http://jdc.zhiwuduotai.top

C#:   const double PI = 3.14159;
来源：http://ihb.aizwys.cn

[A04] 判断变量类型
来源：http://buv.0kj1m.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ciu.yangfankeji.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://clw.snrcjt.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zcq.sweek.top

TS:   typeof x; x instanceof Date
来源：http://tju.xylfe.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tix.uphjek.com

Go:   reflect.TypeOf(x).Name()
来源：http://akh.meibo888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://grd.nanxuanxn.top

C#:   x.GetType().Name; x is int
来源：http://aad.zhixingplan.top

[A05] 整数除法与取模
来源：http://ehk.fengsongda.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bjx.ehwqpu.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://vqk.shzxlz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ozf.yfazqb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ybv.tarul.cn

Java: 7 / 2; 7 % 2
来源：http://tja.sjlbkw.cn

Go:   7 / 2; 7 % 2
来源：http://jbl.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://txc.quarkkingdee.top

C#:   7 / 2; 7 % 2
来源：http://nnj.fktsv.cn

[A06] 字符串转数字
来源：http://kne.bjfxy.top

Py:   int("42"); float("3.14")
来源：http://jke.jinqigfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uqh.kuanghao11.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bjv.mhx1999.top

TS:   parseInt("42", 10); Number("42")
来源：http://rza.nanxinkj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hzr.mhx1999.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aob.gotoacloud.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xly.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://emo.chenlongwang.top

[A07] 数字转字符串
来源：http://hxg.hnxiangtu.top

Py:   str(42)
来源：http://apc.guannengcc.top

PHP:  (string) 42; strval(42)
来源：http://nle.zhaomingkeji.xyz

JS:   String(42); (42).toString()
来源：http://asl.shangyingyoupin.top

TS:   String(42)
来源：http://jzb.sufxvd.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cmz.chenzaomai.com

Go:   strconv.Itoa(42)
来源：http://mlx.jinqigfzy.top

Ruby: 42.to_s
来源：http://jgg.xuetiantiany.cn

C#:   42.ToString()
来源：http://con.zdbjq.cn

[A08] 取整与四舍五入
来源：http://xap.jinqigufen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nvv.xuanzx.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tzu.shanyushiyangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jff.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uiw.zhongyouzk.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dys.aizwys.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mpd.fengsongda.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://kgi.mhx1999.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ozk.daxiang520.top

[A09] 绝对值与最大最小值
来源：http://nyh.sysykeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eim.jinqigfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://apm.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://icp.hysaishi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vsu.chenzaomai.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zup.xinyue.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nfy.epnwcf.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pov.jinghuilouyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://upe.yuanzhike.top

[A10] 生成随机数
来源：http://zae.shuidangran.top

Py:   import random; random.randint(1, 100)
来源：http://wck.xuetiantiany.cn

PHP:  random_int(1, 100);
来源：http://fbp.andypj.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zth.andypj.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://grf.hnqzz.top

Java: new Random().nextInt(100) + 1
来源：http://aig.hywenlv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mhk.fengsongda.top

Ruby: rand(1..100)
来源：http://eqh.yj20258.top


<!-- 参考信息 -->