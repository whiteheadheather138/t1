代发 wailian999

[U69] PHP：PDO 预处理
来源：http://cos.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wyc.vehdjk.com

[U70] PHP：PDO 事务
来源：http://alh.yueranfly.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zwo.xylfe.cn

[U71] PHP：抛出异常
来源：http://uzx.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://ayy.nwbrower.top

[U72] PHP：写错误日志
来源：http://fkq.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://jhz.yangfankeji.com

[U73] PHP：读取 ini 配置
来源：http://ixb.feifeiyinyue.top

parse_ini_file("config.ini", true)
来源：http://azq.andypj.xyz

[U74] PHP：读取环境变量
来源：http://pfh.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://ssj.birdmap.top

[U75] PHP：依赖注入
来源：http://lji.xingfuxueyuan.xyz

composer require psr/container
来源：http://cuk.yonumen.top

[U76] PHP：简单路由
来源：http://qam.hongshengwenyu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://twx.jiagoushi.top

[U77] PHP：模板渲染
来源：http://euu.zhijiandao.cn

composer require twig/twig
来源：http://awb.aibaodan.cn

[U78] PHP：单元测试
来源：http://vwc.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://ddt.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://apz.guowangkeji.top

composer require --dev phpstan/phpstan
来源：http://jaq.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://fdk.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gdh.xylfe.cn

[U81] JS：初始化项目
来源：http://zxd.yj20258888.top

npm init -y;  npm i express
来源：http://yhn.52xcode.cn

[U82] JS：package.json 脚本
来源：http://tfx.xuetiantiany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ftz.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://tyr.xinyue.icu

export const a = 1;  import { a } from "./m.js";
来源：http://spm.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://kfs.fzhhl.top

module.exports = { a };  const { a } = require("./m");
来源：http://mzo.zhengqikj.top

[U85] JS：可选链
来源：http://kxz.cqqwz.cn

a?.b?.c
来源：http://vwb.dashuyun.cn

[U86] JS：空值合并
来源：http://yio.hammf.cn

a ?? b
来源：http://lou.chenlongwang.top

[U87] JS：解构默认值
来源：http://lhf.yonumen.top

const { a = 1, b = 2 } = obj;
来源：http://nqk.zhoulong.xyz

[U88] JS：对象展开合并
来源：http://ldf.hesvh.cn

{ ...a, ...b }
来源：http://fvv.hongshengwenyu.top

[U89] JS：数组去重
来源：http://dpl.iojbl.cn

[...new Set(arr)]
来源：http://two.ybcxt.top

[U90] JS：数字数组排序
来源：http://zqy.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://syl.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://jcz.guowangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hyr.hesvh.cn

[U92] JS：深拷贝
来源：http://dnz.sweek.top

structuredClone(obj)
来源：http://nhh.hcnkem.com

[U93] JS：模板字符串
来源：http://oxb.fktsv.cn

`共 ${n} 条`
来源：http://oyo.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://dlw.chenlongwang.top

const double = x => x * 2;
来源：http://cxn.shuidangran.top

[U95] JS：Promise 包装
来源：http://lxe.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://rwx.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://uqv.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ofm.vqdsnc.cn

[U97] JS：并发请求
来源：http://mzp.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://oaq.hnxiangtu.top

[U98] JS：fetch 带 JSON
来源：http://yrd.dianchejie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jit.tianlin.xyz

[U99] JS：事件监听
来源：http://beq.redwolf501.top

el.addEventListener("click", e => {})
来源：http://kej.uphjek.com

[U100] JS：DOM 查询
来源：http://sab.uphjek.com

document.querySelector(".item")
来源：http://jkk.316326.xyz

[U101] JS：classList 操作
来源：http://txe.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://faw.cucudq.cn

[U102] JS：本地存储
来源：http://qxi.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bde.zycfv.cn

[U103] JS：定时器
来源：http://gjz.hywenlv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hwc.yangfankeji.com

[U104] JS：防抖
来源：http://czq.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iit.hcnkem.com

[U105] JS：节流
来源：http://zqb.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oem.fzhhl.top

[U106] JS：日期格式化
来源：http://vkg.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lsr.aibaodan.cn

[U107] JS：数字千分位
来源：http://yyb.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vrr.fehbvm.com

[U108] JS：随机整数
来源：http://nak.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nth.haohaochexian.top

[U109] JS：数组分组
来源：http://oto.pycfn.com

Object.groupBy(arr, x => x.type)
来源：http://uck.zhaomingkeji.xyz

[U110] JS：数组分块
来源：http://zop.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zpf.ydzc1.top

[U111] JS：对象转 Map
来源：http://wkt.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://kgs.zhijiandao.cn

[U112] JS：字符串补位
来源：http://tna.fanxiaobao.xyz

"7".padStart(3, "0")
来源：http://xsi.xziqi.cn

[U113] JS：正则替换全部
来源：http://lgn.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://yyf.pengpengdd.cyou

[U114] JS：JSON 深比较
来源：http://qhv.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fev.svipenyu.cn

[U115] JS：生成 UUID
来源：http://mib.yueranfly.top

crypto.randomUUID()
来源：http://jtf.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://vnv.aibaodan.cn

/** @param {string} name */ function f(name) {}
来源：http://ejn.smart0.xyz

[U117] JS：单元测试
来源：http://umv.0kj1m.cn

npm i -D vitest;  npx vitest
来源：http://nxs.yuanzhike.top

[U118] JS：开发服务器
来源：http://uhg.hysaishi.cn

npm i -D vite;  npx vite
来源：http://hcy.nanxinkj.top

[U119] JS：生产构建
来源：http://oid.feifeiyinyue.top

npx vite build
来源：http://cnf.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://plf.c1oappe.top

import.meta.env.VITE_API_URL
来源：http://uku.wangdashe.top

================================================================================
来源：http://ggm.zhongyouzk.top

统计汇总
来源：http://hww.svipenyu.cn

================================================================================
来源：http://bqc.yvedp.cn

按语言统计（条）：
来源：http://xea.52xcode.cn

Python ......... 252
来源：http://bon.redwolf501.top

PHP ............ 252
来源：http://npe.xylfe.cn

JavaScript ..... 252
来源：http://juq.guowangkeji.top

TypeScript ..... 212
来源：http://cbc.xuanzx.com

Java ........... 212
来源：http://fwi.jinghuilouyu.cn

Go ............. 212
来源：http://rht.svipenyu.cn

Ruby ........... 212
来源：http://pwa.hongshengwenyu.top

C# ............. 212
来源：http://nit.bjfxy.top

C .............. 30
来源：http://bht.zhaomingkeji.xyz

C++ ............ 30
来源：http://ksm.shuidangran.top

SQL ............ 90
来源：http://bro.hysaishi.cn

Bash ........... 80
来源：http://pnx.gzhubu.top

Kotlin ......... 15
来源：http://jyo.meibo888.top

Swift .......... 15
来源：http://pgz.nanxinkj.top

Lua ............ 10
来源：http://omw.zhongyouzk.top

Perl ........... 10
来源：http://voo.zdbjq.cn

Scala .......... 10
来源：http://dzd.yueranfly.top

------------------------------------
来源：http://wmd.tarul.cn

合计 ........... 2106 条
来源：http://tso.meibo888.top

按章节统计：
来源：http://efz.316326.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://alo.aizwys.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dep.xuanzx.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ijn.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xgd.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ogn.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bbh.pengpengdd.cyou

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ssy.jqgfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://luu.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jfh.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ljv.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cmz.pycfn.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ryw.aizwys.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lqv.wangdashe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://esz.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://imy.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://msr.yangfankeji.com

Q SQL 专题                              90
来源：http://dnv.ydjk.org.cn

R Bash 专题                             80
来源：http://lfv.tianlin.xyz

S C / C++ 专题                          60
来源：http://ewy.jlsjyb.cn

T 其他语言补充                          60
来源：http://yfu.dianchejie.cn

U 高频实用片段                         120
来源：http://myz.dashuyun.cn

------------------------------------
来源：http://wgi.meibo888.top

合计                                  2106 条
来源：http://zpg.uphjek.com

--------------------------------------------------------------------------------
来源：http://ddy.guowangkeji.top

使用提醒
来源：http://yhe.yonumen.top

--------------------------------------------------------------------------------
来源：http://zyj.xylfe.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zch.jiagoushi.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qnt.gogol.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kwu.zhaomingkeji.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://pmr.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dfc.chenlongwang.top

—— 文件结束 ——
来源：http://hyx.yueranfly.top

================================================================================
来源：http://mqv.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://mmx.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://jfn.yj20258888.top

================================================================================
来源：http://zec.chenjidiqi.icu

【收录内容】
来源：http://sxz.hammf.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://spt.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jfh.yanxiufei.cn

SQL · Bash · C · C++
来源：http://ddx.zhaomingkeji.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ijb.ybcxt.top

【使用说明】
来源：http://iqy.uphjek.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oel.fzhhl.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://syf.gogol.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bcc.gotoacloud.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qyx.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yzg.wangshuangyany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ekp.gaohongyu789.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xtj.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ixr.9152youxi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vwn.52xcode.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ldg.shangyingyoupin.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ofk.ybcxt.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yzx.zdqjudy.top

【文件统计】
来源：http://mim.hcnkem.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ksk.guannengcc.top

--------------------------------------------------------------------------------
来源：http://cad.snrcjt.cn

目  录
来源：http://rzx.tian-w.cn

--------------------------------------------------------------------------------
来源：http://vxn.zhijiandao.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zbw.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xfz.meibo888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://upt.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cyq.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qyp.nanxuanxn.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fol.zhoulong.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jdy.bbcook.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://plr.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nvo.sufxvd.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ipo.jyoumei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hnq.yangfankeji.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cbz.316326.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ugn.gaohongyu789.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rkp.bjfxy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fvl.cqqwz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qtv.yangfankeji.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lru.hnxiangtu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://acs.zdbjq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uuq.9152youxi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blq.hysaishi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mgh.ybcxt.top

================================================================================
来源：http://jls.hnxiangtu.top

A. 基础语法与类型
来源：http://roh.c1oappe.top

================================================================================
来源：http://srd.0kj1m.cn

[A01] Hello World
来源：http://zsj.yj202588.top

Py:   print("Hello, World!")
来源：http://cyq.havefunace.top

PHP:  echo "Hello, World!";
来源：http://lhb.hywenlv.cn

JS:   console.log("Hello, World!");
来源：http://xuu.tanke756.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rfe.sysykeji.top

Java: System.out.println("Hello, World!");
来源：http://zvg.c1oappe.top

Go:   fmt.Println("Hello, World!")
来源：http://yka.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://hhh.zhengqikj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://blu.quarkkingdee.top

[A02] 变量声明与赋值
来源：http://ohm.ywan-chungtsiang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ddn.zdbjq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zay.xylfe.cn

JS:   let name = "Alex"; const age = 20;
来源：http://biw.c1oappe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dfg.kuanghao11.cn

Java: String name = "Alex"; int age = 20;
来源：http://bsi.andypj.xyz

Go:   name := "Alex"; age := 20
来源：http://tpk.sysykeji.top

Ruby: name = "Alex"; age = 20
来源：http://hfz.chenzaomai.com

C#:   string name = "Alex"; int age = 20;
来源：http://ewn.zhixingplan.top

[A03] 常量定义
来源：http://ovx.shangyingyoupin.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mza.aibaodan.cn

PHP:  const PI = 3.14159;
来源：http://upd.dashuyun.cn

JS:   const PI = 3.14159;
来源：http://taw.cqqwz.cn

TS:   const PI: number = 3.14159;
来源：http://fah.zhixingplan.top

Java: static final double PI = 3.14159;
来源：http://qsd.sysykeji.top

Go:   const PI = 3.14159
来源：http://blp.jlsjyb.cn

Ruby: PI = 3.14159
来源：http://qpo.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://uca.sjlbkw.cn

[A04] 判断变量类型
来源：http://ieg.hywenlv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tki.gotoacloud.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://stq.xuetiantiany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pvn.xuetiantiany.cn

TS:   typeof x; x instanceof Date
来源：http://igv.jlsjyb.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ujc.epnwcf.com

Go:   reflect.TypeOf(x).Name()
来源：http://icn.sysykeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cwv.hongshengwenyu.top

C#:   x.GetType().Name; x is int
来源：http://bzs.yangfankeji.com

[A05] 整数除法与取模
来源：http://lef.tian-w.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wyk.jyoumei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bwo.ehwqpu.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lbx.yfazqb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tiw.haohaochexian.top

Java: 7 / 2; 7 % 2
来源：http://pmr.yueranfly.top

Go:   7 / 2; 7 % 2
来源：http://ynn.zhijiandao.cn

Ruby: 7 / 2; 7 % 2
来源：http://fli.wangdashe.top

C#:   7 / 2; 7 % 2
来源：http://bha.yuxming.cn

[A06] 字符串转数字
来源：http://ghu.xuetiantiany.cn

Py:   int("42"); float("3.14")
来源：http://sei.zdqjudy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hym.guowangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rpq.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vjw.jqgufenzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zzf.chenjidiqi.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rgo.yonumen.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gsi.jianghu66.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hdd.zhixingplan.top

[A07] 数字转字符串
来源：http://mlk.yj202588.top

Py:   str(42)
来源：http://fpl.fzhhl.top

PHP:  (string) 42; strval(42)
来源：http://udp.xylfe.cn

JS:   String(42); (42).toString()
来源：http://uas.vqdsnc.cn

TS:   String(42)
来源：http://owk.guowangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://kww.vqdsnc.cn

Go:   strconv.Itoa(42)
来源：http://pbh.ehwqpu.com

Ruby: 42.to_s
来源：http://dfk.jyoumei.cn

C#:   42.ToString()
来源：http://wcv.daria6918.cn

[A08] 取整与四舍五入
来源：http://zax.hongshengwenyu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dgq.zhengqikj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://edc.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pzh.ivvv.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wxe.jqgfzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://djy.316326.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wjq.zhixingplan.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://biz.yj20258.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ucv.xziqi.cn

[A09] 绝对值与最大最小值
来源：http://zlp.sjlbkw.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jxv.yj202588.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://htv.jyoumei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vad.0kj1m.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tzz.chenjidiqi.icu

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xnd.hesvh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://isl.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zmu.yangfankeji.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lwf.gaohongyu789.top

[A10] 生成随机数
来源：http://hdw.jinqigufen.top

Py:   import random; random.randint(1, 100)
来源：http://ycd.haohaochexian.top

PHP:  random_int(1, 100);
来源：http://ukg.52xcode.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://iek.snrcjt.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ixw.316326.xyz

Java: new Random().nextInt(100) + 1
来源：http://zvh.0kj1m.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://msc.yvedp.cn

Ruby: rand(1..100)
来源：http://cmy.tianlin.xyz


<!-- 参考信息 -->