代发 wailian999

[U67] PHP：处理文件上传
来源：http://ced.hysaishi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eoe.shuidangran.top

[U68] PHP：PDO 连接
来源：http://ndg.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mma.hammf.cn

[U69] PHP：PDO 预处理
来源：http://dnu.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vzj.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://rfx.guannengcc.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ggg.hesvh.cn

[U71] PHP：抛出异常
来源：http://bvt.vehdjk.com

throw new RuntimeException("失败", 500);
来源：http://xtc.hywenlv.cn

[U72] PHP：写错误日志
来源：http://qbx.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://vcg.gzhubu.top

[U73] PHP：读取 ini 配置
来源：http://yze.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://tcg.hesvh.cn

[U74] PHP：读取环境变量
来源：http://vwe.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://bek.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://anh.hfpthk.cn

composer require psr/container
来源：http://llw.uphjek.com

[U76] PHP：简单路由
来源：http://dtu.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://whb.yj202588.top

[U77] PHP：模板渲染
来源：http://ift.zhengqikj.top

composer require twig/twig
来源：http://fvp.tarul.cn

[U78] PHP：单元测试
来源：http://rup.nanxuanxn.top

composer require --dev phpunit/phpunit
来源：http://iel.andypj.xyz

[U79] PHP：静态分析
来源：http://ihe.yongpay.top

composer require --dev phpstan/phpstan
来源：http://cmm.shanyushiyangtech.top

[U80] PHP：代码规范修复
来源：http://xwi.jinghuilouyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sgp.xingfuxueyuan.xyz

[U81] JS：初始化项目
来源：http://jco.zhiwuduotai.top

npm init -y;  npm i express
来源：http://ejb.cucudq.cn

[U82] JS：package.json 脚本
来源：http://uks.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wlg.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://dnl.9152youxi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uwe.haohaochexian.top

[U84] JS：CommonJS 写法
来源：http://oas.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ofx.316326.xyz

[U85] JS：可选链
来源：http://ydi.sweek.top

a?.b?.c
来源：http://amx.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://twn.ivvv.top

a ?? b
来源：http://ruz.yj20258.top

[U87] JS：解构默认值
来源：http://kru.nanxuanxn.top

const { a = 1, b = 2 } = obj;
来源：http://ebn.aibaodan.cn

[U88] JS：对象展开合并
来源：http://zuu.chenlongwang.top

{ ...a, ...b }
来源：http://gyl.iojbl.cn

[U89] JS：数组去重
来源：http://cbq.bbcook.cn

[...new Set(arr)]
来源：http://cxd.tarul.cn

[U90] JS：数字数组排序
来源：http://yyo.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://mjq.iojbl.cn

[U91] JS：对象键值遍历
来源：http://yrs.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yvy.zhixingplan.top

[U92] JS：深拷贝
来源：http://mcr.pycfn.com

structuredClone(obj)
来源：http://sde.havefunace.top

[U93] JS：模板字符串
来源：http://xvv.ydjk.org.cn

`共 ${n} 条`
来源：http://oaw.smart0.xyz

[U94] JS：箭头函数
来源：http://csv.haohaochexian.top

const double = x => x * 2;
来源：http://nxs.feifeiyinyue.top

[U95] JS：Promise 包装
来源：http://vjl.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://afn.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://igf.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pki.shanyushiyangkeji.top

[U97] JS：并发请求
来源：http://waj.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yru.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://cnu.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gvz.mhx1999.top

[U99] JS：事件监听
来源：http://zey.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://ezo.tanke756.top

[U100] JS：DOM 查询
来源：http://ztu.snrcjt.cn

document.querySelector(".item")
来源：http://mrz.dianchejie.cn

[U101] JS：classList 操作
来源：http://mot.kuanghao11.cn

el.classList.toggle("active")
来源：http://jtt.guowangkeji.top

[U102] JS：本地存储
来源：http://akg.iojbl.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sxp.shanyushiyangtech.top

[U103] JS：定时器
来源：http://omy.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oga.shangyingyoupin.top

[U104] JS：防抖
来源：http://afe.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lqx.shanyushiyangkeji.top

[U105] JS：节流
来源：http://qgc.ehwqpu.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://afl.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://tcq.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tmt.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://ams.jianghu66.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qnr.vehdjk.com

[U108] JS：随机整数
来源：http://tdq.smart0.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lmf.hammf.cn

[U109] JS：数组分组
来源：http://ybi.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://iav.svipenyu.cn

[U110] JS：数组分块
来源：http://npd.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qcg.nwbrower.top

[U111] JS：对象转 Map
来源：http://gfs.jqgfzy.top

new Map(Object.entries(obj))
来源：http://suk.ctjpmb.com

[U112] JS：字符串补位
来源：http://pat.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://dte.fktsv.cn

[U113] JS：正则替换全部
来源：http://eru.hfpthk.cn

s.replaceAll("a", "b")
来源：http://dlf.xinyue.icu

[U114] JS：JSON 深比较
来源：http://fwl.shanyushiyangtech.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ztr.hfpthk.cn

[U115] JS：生成 UUID
来源：http://rly.zhijiandao.cn

crypto.randomUUID()
来源：http://sfj.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://xwt.hongshengwenyu.top

/** @param {string} name */ function f(name) {}
来源：http://gic.chenlongwang.top

[U117] JS：单元测试
来源：http://rsm.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://ael.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://mjm.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://tuq.fehbvm.com

[U119] JS：生产构建
来源：http://kby.redwolf501.top

npx vite build
来源：http://tjc.xylfe.cn

[U120] JS：读取环境变量（Vite）
来源：http://awm.sweek.top

import.meta.env.VITE_API_URL
来源：http://prd.pycfn.com

================================================================================
来源：http://egk.ywan-chungtsiang.top

统计汇总
来源：http://wxm.ppjwa.cn

================================================================================
来源：http://tuf.tianlin.xyz

按语言统计（条）：
来源：http://stm.sweek.top

Python ......... 252
来源：http://bmw.gzhubu.top

PHP ............ 252
来源：http://pws.yangfankeji.com

JavaScript ..... 252
来源：http://uwk.jinqigfzy.top

TypeScript ..... 212
来源：http://alt.hnqzz.top

Java ........... 212
来源：http://psm.pengpengdd.cyou

Go ............. 212
来源：http://saz.chenlongwang.top

Ruby ........... 212
来源：http://umv.wangshuangyany.cn

C# ............. 212
来源：http://tzs.havefunace.top

C .............. 30
来源：http://csc.hongshengwenyu.top

C++ ............ 30
来源：http://dbw.zhixingplan.top

SQL ............ 90
来源：http://nop.tarul.cn

Bash ........... 80
来源：http://jto.yueranfly.top

Kotlin ......... 15
来源：http://hbn.tanke756.top

Swift .......... 15
来源：http://sxa.zhoulong.xyz

Lua ............ 10
来源：http://adf.mhx1999.top

Perl ........... 10
来源：http://mgr.yongpay.top

Scala .......... 10
来源：http://xze.316326.xyz

------------------------------------
来源：http://edd.yj20258.top

合计 ........... 2106 条
来源：http://nmu.smart0.xyz

按章节统计：
来源：http://xmc.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qdj.aizwys.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qkn.aibaodan.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://piv.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oas.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xyj.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ydv.yj20258.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mng.yj202588.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ybw.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://umn.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ogd.mhx1999.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eqn.cqqwz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mpg.shangyingyoupin.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rqq.tianlin.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ejq.havefunace.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yoc.ppjwa.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ley.gzhubu.top

Q SQL 专题                              90
来源：http://noi.zhoulong.xyz

R Bash 专题                             80
来源：http://sva.chenlongwang.top

S C / C++ 专题                          60
来源：http://xnu.cheryme.top

T 其他语言补充                          60
来源：http://hvs.fehbvm.com

U 高频实用片段                         120
来源：http://oda.jinyuanbaomall.cn

------------------------------------
来源：http://lec.xziqi.cn

合计                                  2106 条
来源：http://sxh.yueranfly.top

--------------------------------------------------------------------------------
来源：http://rjj.tanke756.top

使用提醒
来源：http://dih.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://wcu.tian-w.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hdo.vqdsnc.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ocl.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jcm.nanxuanxn.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tba.epnwcf.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lfl.mhx1999.top

—— 文件结束 ——
来源：http://fcf.jiagoushi.top

================================================================================
来源：http://kyn.sufxvd.cn

程序语言常见例子速查手册（2024 版）
来源：http://pja.fanxiaobao.xyz

Common Programming Examples Cheat Book
来源：http://qgy.jiagoushi.top

================================================================================
来源：http://nbg.yuanzhike.top

【收录内容】
来源：http://mux.cqqwz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fmh.zhiwuduotai.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kix.hfpthk.cn

SQL · Bash · C · C++
来源：http://vyl.jqgufenzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://noq.hongshengwenyu.top

【使用说明】
来源：http://yxq.ctjpmb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kkz.andypj.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ngj.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fjx.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://suw.dashuyun.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://knz.zhongyouzk.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rvh.redwolf501.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eju.havefunace.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ccb.yfazqb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kdt.jinqigufen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mzu.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://foh.uphjek.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eqb.mhx1999.top

【文件统计】
来源：http://vcv.zycfv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pfd.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://cpa.zhaomingkeji.xyz

目  录
来源：http://fuo.bjfxy.top

--------------------------------------------------------------------------------
来源：http://xvo.jyoumei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pvm.yj20258.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gxz.uphjek.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mkn.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wnn.yonumen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ldr.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cfr.jinghuilouyu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uvc.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://upl.chenlongwang.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bce.zdbjq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yzf.yvedp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://est.smart0.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://axa.cqqwz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pax.xingfuxueyuan.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zjz.yj20258888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tyx.nwbrower.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://epk.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://flm.zhijiandao.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rbe.wangdashe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ozo.hnxiangtu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ijy.svipenyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kek.cashguo.top

================================================================================
来源：http://ekz.hysaishi.cn

A. 基础语法与类型
来源：http://jzq.hongshengwenyu.top

================================================================================
来源：http://gwd.jqgufenzy.top

[A01] Hello World
来源：http://tfo.yvedp.cn

Py:   print("Hello, World!")
来源：http://gec.pycfn.com

PHP:  echo "Hello, World!";
来源：http://utx.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://irc.yonumen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cmw.zhengqikj.top

Java: System.out.println("Hello, World!");
来源：http://ext.jianghu66.top

Go:   fmt.Println("Hello, World!")
来源：http://fcj.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://xjf.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://uio.hammf.cn

[A02] 变量声明与赋值
来源：http://wqf.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wby.mhx1999.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vtj.zhoulong.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://kld.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jin.guannengcc.top

Java: String name = "Alex"; int age = 20;
来源：http://kbx.cucudq.cn

Go:   name := "Alex"; age := 20
来源：http://gbq.fzhhl.top

Ruby: name = "Alex"; age = 20
来源：http://xez.yangfankeji.com

C#:   string name = "Alex"; int age = 20;
来源：http://ajn.xziqi.cn

[A03] 常量定义
来源：http://mdc.jyoumei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hmr.zhiwuduotai.top

PHP:  const PI = 3.14159;
来源：http://aqq.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://iww.yj20258.top

TS:   const PI: number = 3.14159;
来源：http://jzr.feifeiyinyue.top

Java: static final double PI = 3.14159;
来源：http://qtl.pycfn.com

Go:   const PI = 3.14159
来源：http://gia.hcnkem.com

Ruby: PI = 3.14159
来源：http://dcg.yueranfly.top

C#:   const double PI = 3.14159;
来源：http://uwc.daxiang520.top

[A04] 判断变量类型
来源：http://fdb.zhoulong.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://wof.hnqzz.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rci.ctjpmb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uyj.chenzaomai.com

TS:   typeof x; x instanceof Date
来源：http://ign.feifeiyinyue.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vhh.guowangkeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://cqv.hammf.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qad.316326.xyz

C#:   x.GetType().Name; x is int
来源：http://zoo.nanxinkj.top

[A05] 整数除法与取模
来源：http://pvb.jiagoushi.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uzj.zdbjq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://doe.jlsjyb.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dna.yueranfly.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dua.cheryme.top

Java: 7 / 2; 7 % 2
来源：http://bfq.nanxinkj.top

Go:   7 / 2; 7 % 2
来源：http://yub.ehwqpu.com

Ruby: 7 / 2; 7 % 2
来源：http://etq.zhiwuduotai.top

C#:   7 / 2; 7 % 2
来源：http://qww.cdnleiting.top

[A06] 字符串转数字
来源：http://tvz.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://uet.52xcode.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eup.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qcp.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oht.sweek.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://odi.xinyue.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wsv.cqqwz.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sow.zhixingplan.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zpa.quarkkingdee.top

[A07] 数字转字符串
来源：http://dhd.shanyushiyangtech.top

Py:   str(42)
来源：http://bci.gotoacloud.top

PHP:  (string) 42; strval(42)
来源：http://prv.ivvv.top

JS:   String(42); (42).toString()
来源：http://ozx.ybcxt.top

TS:   String(42)
来源：http://wrs.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ech.zhiwuduotai.top

Go:   strconv.Itoa(42)
来源：http://oxh.zycfv.cn

Ruby: 42.to_s
来源：http://cmm.cqqwz.cn

C#:   42.ToString()
来源：http://hgr.zycfv.cn

[A08] 取整与四舍五入
来源：http://qwx.vehdjk.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lka.yvedp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uxw.316326.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bem.ydzc1.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nam.jyoumei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://grw.jyoumei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gdv.chenzaomai.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://etl.pycfn.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uaq.shangyingyoupin.top

[A09] 绝对值与最大最小值
来源：http://vzc.wangshuangyany.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cmh.hcnkem.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wbc.ehwqpu.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mqx.jinqigfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vpm.kuanghao11.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mot.nwbrower.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://koo.zdqjudy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bqm.shangyingyoupin.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qoj.316326.xyz

[A10] 生成随机数
来源：http://pyg.yuanzhike.top

Py:   import random; random.randint(1, 100)
来源：http://sck.hywenlv.cn

PHP:  random_int(1, 100);
来源：http://tzf.meibo888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hlo.shanyushiyangtech.top


<!-- 参考信息 -->