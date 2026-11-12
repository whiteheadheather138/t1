代发 wailian999

[U65] PHP：会话
来源：http://eog.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ase.yonumen.top

[U66] PHP：设置 Cookie
来源：http://nio.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jfd.hnxiangtu.top

[U67] PHP：处理文件上传
来源：http://hcz.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://enc.gaohongyu789.top

[U68] PHP：PDO 连接
来源：http://vck.dashuyun.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://til.yuxming.cn

[U69] PHP：PDO 预处理
来源：http://qhs.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lgn.svipenyu.cn

[U70] PHP：PDO 事务
来源：http://qrq.daria6918.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eod.jianghu66.top

[U71] PHP：抛出异常
来源：http://oef.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://xhs.hesvh.cn

[U72] PHP：写错误日志
来源：http://xqn.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://rre.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://ard.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://ott.zhoulong.xyz

[U74] PHP：读取环境变量
来源：http://xfy.zycfv.cn

getenv("APP_ENV") ?: "production"
来源：http://cjz.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://qas.haohaochexian.top

composer require psr/container
来源：http://doc.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://ize.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hxp.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://lqa.tianlin.xyz

composer require twig/twig
来源：http://zvp.tanke756.top

[U78] PHP：单元测试
来源：http://oot.sweek.top

composer require --dev phpunit/phpunit
来源：http://qbs.tanke756.top

[U79] PHP：静态分析
来源：http://ted.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://jrt.mhx1999.top

[U80] PHP：代码规范修复
来源：http://wha.tanke756.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ncj.zycfv.cn

[U81] JS：初始化项目
来源：http://qjn.bjfxy.top

npm init -y;  npm i express
来源：http://hgw.shanyushiyangtech.top

[U82] JS：package.json 脚本
来源：http://lkh.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gen.quarkkingdee.top

[U83] JS：ES Module 导入导出
来源：http://uxf.ehwqpu.com

export const a = 1;  import { a } from "./m.js";
来源：http://zjs.aizwys.cn

[U84] JS：CommonJS 写法
来源：http://toy.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nca.birdmap.top

[U85] JS：可选链
来源：http://qxh.ehwqpu.com

a?.b?.c
来源：http://rgt.hnxiangtu.top

[U86] JS：空值合并
来源：http://urs.daria6918.cn

a ?? b
来源：http://mgz.yj20258.top

[U87] JS：解构默认值
来源：http://gpo.xuetiantiany.cn

const { a = 1, b = 2 } = obj;
来源：http://hee.dianchejie.cn

[U88] JS：对象展开合并
来源：http://zfd.shanyushiyangkeji.top

{ ...a, ...b }
来源：http://lsd.hongshengwenyu.top

[U89] JS：数组去重
来源：http://jab.svipenyu.cn

[...new Set(arr)]
来源：http://xbc.nwbrower.top

[U90] JS：数字数组排序
来源：http://pwf.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://rtm.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://hao.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dvy.xylfe.cn

[U92] JS：深拷贝
来源：http://wqn.sysykeji.top

structuredClone(obj)
来源：http://ujc.gotoacloud.top

[U93] JS：模板字符串
来源：http://gye.zhijiandao.cn

`共 ${n} 条`
来源：http://bse.yangfankeji.com

[U94] JS：箭头函数
来源：http://dtl.havefunace.top

const double = x => x * 2;
来源：http://pbp.feifeiyinyue.top

[U95] JS：Promise 包装
来源：http://uli.cashguo.top

new Promise((resolve, reject) => {})
来源：http://ptj.yonumen.top

[U96] JS：async/await 与异常
来源：http://ueu.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vpm.jinqigfzy.top

[U97] JS：并发请求
来源：http://ysx.nwbrower.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://awz.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://ptk.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iku.tanke756.top

[U99] JS：事件监听
来源：http://czt.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://icx.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://ach.gotoacloud.top

document.querySelector(".item")
来源：http://wfr.snrcjt.cn

[U101] JS：classList 操作
来源：http://kwc.zdbjq.cn

el.classList.toggle("active")
来源：http://adf.zdbjq.cn

[U102] JS：本地存储
来源：http://oaz.pengpengdd.cyou

localStorage.setItem("k", JSON.stringify(v))
来源：http://ful.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://xny.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://njz.jinghuilouyu.cn

[U104] JS：防抖
来源：http://hrx.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fcf.jinqigufen.top

[U105] JS：节流
来源：http://del.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xae.hysaishi.cn

[U106] JS：日期格式化
来源：http://eom.xuanzx.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nqv.yuxming.cn

[U107] JS：数字千分位
来源：http://aal.9152youxi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hys.gaohongyu789.top

[U108] JS：随机整数
来源：http://qmx.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lat.yuanzhike.top

[U109] JS：数组分组
来源：http://qzk.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://lpm.yonumen.top

[U110] JS：数组分块
来源：http://ulr.ydzc1.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ise.zhengqikj.top

[U111] JS：对象转 Map
来源：http://htk.smart0.xyz

new Map(Object.entries(obj))
来源：http://zah.sxryk.cn

[U112] JS：字符串补位
来源：http://yjb.andypj.xyz

"7".padStart(3, "0")
来源：http://als.daria6918.cn

[U113] JS：正则替换全部
来源：http://azs.aibaodan.cn

s.replaceAll("a", "b")
来源：http://dmb.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://sdh.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://oeh.fzhhl.top

[U115] JS：生成 UUID
来源：http://lia.pycfn.com

crypto.randomUUID()
来源：http://htd.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://ard.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://gjb.tian-w.cn

[U117] JS：单元测试
来源：http://iub.hcnkem.com

npm i -D vitest;  npx vitest
来源：http://ibq.hywenlv.cn

[U118] JS：开发服务器
来源：http://goa.yuanzhike.top

npm i -D vite;  npx vite
来源：http://jgc.vqdsnc.cn

[U119] JS：生产构建
来源：http://nzw.tianlin.xyz

npx vite build
来源：http://xft.cdnleiting.top

[U120] JS：读取环境变量（Vite）
来源：http://hxd.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://gmg.yvedp.cn

================================================================================
来源：http://sob.xuanzx.com

统计汇总
来源：http://dvn.hongshengwenyu.top

================================================================================
来源：http://zef.bbcook.cn

按语言统计（条）：
来源：http://xub.shzxlz.cn

Python ......... 252
来源：http://uqi.cqqwz.cn

PHP ............ 252
来源：http://qpz.yuxming.cn

JavaScript ..... 252
来源：http://rjk.shanyushiyangtech.top

TypeScript ..... 212
来源：http://cnt.haohaochexian.top

Java ........... 212
来源：http://rqv.sufxvd.cn

Go ............. 212
来源：http://ngb.yongpay.top

Ruby ........... 212
来源：http://jbe.tianlin.xyz

C# ............. 212
来源：http://bqn.hysaishi.cn

C .............. 30
来源：http://gqg.yj202588.top

C++ ............ 30
来源：http://son.cucudq.cn

SQL ............ 90
来源：http://dfh.jianghu66.top

Bash ........... 80
来源：http://nrv.ydjk.org.cn

Kotlin ......... 15
来源：http://lxv.fehbvm.com

Swift .......... 15
来源：http://dic.hywenlv.cn

Lua ............ 10
来源：http://hpg.svipenyu.cn

Perl ........... 10
来源：http://qrm.sufxvd.cn

Scala .......... 10
来源：http://soq.guowangkeji.top

------------------------------------
来源：http://lcw.zhoulong.xyz

合计 ........... 2106 条
来源：http://uts.jianghu66.top

按章节统计：
来源：http://mmr.xuanzx.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eyb.fzhhl.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rbd.wangshuangyany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://syh.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://icm.sufxvd.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://boq.sweek.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qwe.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nmv.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nnt.tianlin.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hvs.yuanzhike.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wzs.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://maf.ybcxt.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vgq.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ddr.sweek.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kxo.havefunace.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://npe.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vdw.xylfe.cn

Q SQL 专题                              90
来源：http://ese.daxiang520.top

R Bash 专题                             80
来源：http://fzh.ybcxt.top

S C / C++ 专题                          60
来源：http://lxh.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://slv.fanxiaobao.xyz

U 高频实用片段                         120
来源：http://jzo.zhaomingkeji.xyz

------------------------------------
来源：http://gqk.pycfn.com

合计                                  2106 条
来源：http://msd.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://jmx.havefunace.top

使用提醒
来源：http://yrb.daxiang520.top

--------------------------------------------------------------------------------
来源：http://yte.nanxuanxn.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ead.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://olp.yueranfly.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://prr.fehbvm.com

在旧版本上使用前请先确认语法支持情况。
来源：http://wny.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://myu.hywenlv.cn

—— 文件结束 ——
来源：http://rwa.vehdjk.com

================================================================================
来源：http://wkt.shangyingyoupin.top

程序语言常见例子速查手册（2024 版）
来源：http://ibz.shangyingyoupin.top

Common Programming Examples Cheat Book
来源：http://mqq.gaohongyu789.top

================================================================================
来源：http://zpm.jqgfzy.top

【收录内容】
来源：http://mng.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mqd.haohaochexian.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fee.vehdjk.com

SQL · Bash · C · C++
来源：http://fmy.yueranfly.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ivd.snrcjt.cn

【使用说明】
来源：http://isd.sysykeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://biw.snrcjt.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gtv.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iws.wangshuangyany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ukb.pengpengdd.cyou

Bash:  Shell         C:     C             C++:   C++
来源：http://nla.0kj1m.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ngm.mhx1999.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://twl.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lmv.sufxvd.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tzs.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://soj.gogol.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lhl.xingfuxueyuan.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zra.hnxiangtu.top

【文件统计】
来源：http://rqv.haohaochexian.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dwj.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://lhu.svipenyu.cn

目  录
来源：http://ivv.sysykeji.top

--------------------------------------------------------------------------------
来源：http://rpc.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dyn.zdqjudy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hke.yj20258.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kvd.vehdjk.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://crk.yvedp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rkv.zycfv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sug.yonumen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hkp.redwolf501.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rao.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ksp.smart0.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xyu.hcnkem.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cfj.sweek.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://koe.gaohongyu789.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ulg.fzhhl.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hgf.zycfv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iny.bjfxy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kzh.316326.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nfv.iojbl.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bta.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://drt.nanxinkj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uet.pengpengdd.cyou

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ssh.fehbvm.com

================================================================================
来源：http://slw.zdbjq.cn

A. 基础语法与类型
来源：http://azn.jqgufenzy.top

================================================================================
来源：http://vsk.daxiang520.top

[A01] Hello World
来源：http://scu.bbcook.cn

Py:   print("Hello, World!")
来源：http://rki.zhongyouzk.top

PHP:  echo "Hello, World!";
来源：http://kom.uphjek.com

JS:   console.log("Hello, World!");
来源：http://vdh.zhengqikj.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oia.bjfxy.top

Java: System.out.println("Hello, World!");
来源：http://znq.yvedp.cn

Go:   fmt.Println("Hello, World!")
来源：http://ocm.zdbjq.cn

Ruby: puts "Hello, World!"
来源：http://zbf.cqqwz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nvo.ywan-chungtsiang.top

[A02] 变量声明与赋值
来源：http://sbt.zhoulong.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zxe.iojbl.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mdw.hnqzz.top

JS:   let name = "Alex"; const age = 20;
来源：http://fgi.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ppg.gogol.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://bon.fzhhl.top

Go:   name := "Alex"; age := 20
来源：http://aig.dianchejie.cn

Ruby: name = "Alex"; age = 20
来源：http://fss.daxiang520.top

C#:   string name = "Alex"; int age = 20;
来源：http://uai.sysykeji.top

[A03] 常量定义
来源：http://djh.xingfuxueyuan.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kmn.havefunace.top

PHP:  const PI = 3.14159;
来源：http://hdm.0kj1m.cn

JS:   const PI = 3.14159;
来源：http://flu.shuidangran.top

TS:   const PI: number = 3.14159;
来源：http://dpa.yj202588.top

Java: static final double PI = 3.14159;
来源：http://fpo.jinqigufen.top

Go:   const PI = 3.14159
来源：http://lcm.yfazqb.com

Ruby: PI = 3.14159
来源：http://cia.havefunace.top

C#:   const double PI = 3.14159;
来源：http://pug.dashuyun.cn

[A04] 判断变量类型
来源：http://zxk.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oji.shuidangran.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xwi.gzhubu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://prd.fzhhl.top

TS:   typeof x; x instanceof Date
来源：http://xlr.ehwqpu.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jaq.nanxinkj.top

Go:   reflect.TypeOf(x).Name()
来源：http://ubv.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://eem.ybcxt.top

C#:   x.GetType().Name; x is int
来源：http://rye.pengpengdd.cyou

[A05] 整数除法与取模
来源：http://szg.guannengcc.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dvw.fehbvm.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://whr.yuanzhike.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ofg.daria6918.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bdt.zycfv.cn

Java: 7 / 2; 7 % 2
来源：http://xov.shanyushiyangkeji.top

Go:   7 / 2; 7 % 2
来源：http://npz.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://wis.haohaochexian.top

C#:   7 / 2; 7 % 2
来源：http://kcw.bbcook.cn

[A06] 字符串转数字
来源：http://dad.andypj.xyz

Py:   int("42"); float("3.14")
来源：http://kma.tianlin.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tgw.fzhhl.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lpw.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qde.jinyuanbaomall.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yxv.feifeiyinyue.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hgg.zhengqikj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dkc.bbcook.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sau.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://ize.fanxiaobao.xyz

Py:   str(42)
来源：http://kcn.yanxiufei.cn

PHP:  (string) 42; strval(42)
来源：http://xkc.shanyushiyangtech.top

JS:   String(42); (42).toString()
来源：http://duk.ivvv.top

TS:   String(42)
来源：http://tlt.sxryk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ebc.shangyingyoupin.top

Go:   strconv.Itoa(42)
来源：http://bty.xuetiantiany.cn

Ruby: 42.to_s
来源：http://fwi.guowangkeji.top

C#:   42.ToString()
来源：http://wcx.fehbvm.com

[A08] 取整与四舍五入
来源：http://xpx.yonumen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lbl.hnqzz.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wzn.xinyue.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vrp.wangdashe.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sqz.yueranfly.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vmm.daria6918.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ygv.birdmap.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ctz.cqqwz.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gvy.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://icc.xingfuxueyuan.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rbv.wangdashe.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vpl.mhx1999.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dlw.vehdjk.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xwv.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kwm.zhengqikj.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dct.shangyingyoupin.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fkt.jyoumei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zqi.daxiang520.top


<!-- 参考信息 -->