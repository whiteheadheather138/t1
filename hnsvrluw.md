代发 wailian999

[U65] PHP：会话
来源：http://hbd.yfazqb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://cpn.tarul.cn

[U66] PHP：设置 Cookie
来源：http://ont.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eah.yongpay.top

[U67] PHP：处理文件上传
来源：http://slr.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://awv.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://cao.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://chc.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://ixv.gotoacloud.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xjl.jiagoushi.top

[U70] PHP：PDO 事务
来源：http://lpb.vehdjk.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zsn.yonumen.top

[U71] PHP：抛出异常
来源：http://mcw.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://aaa.guannengcc.top

[U72] PHP：写错误日志
来源：http://ykj.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://fnl.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://adc.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://emi.gzhubu.top

[U74] PHP：读取环境变量
来源：http://mco.yongpay.top

getenv("APP_ENV") ?: "production"
来源：http://hlr.havefunace.top

[U75] PHP：依赖注入
来源：http://pid.yuanzhike.top

composer require psr/container
来源：http://snh.gogol.net.cn

[U76] PHP：简单路由
来源：http://ojt.guannengcc.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jrm.gogol.net.cn

[U77] PHP：模板渲染
来源：http://xzo.shuidangran.top

composer require twig/twig
来源：http://txz.dianchejie.cn

[U78] PHP：单元测试
来源：http://awm.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://fdu.sjlbkw.cn

[U79] PHP：静态分析
来源：http://edn.xylfe.cn

composer require --dev phpstan/phpstan
来源：http://hdy.jqgfzy.top

[U80] PHP：代码规范修复
来源：http://hxo.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://oks.jianghu66.top

[U81] JS：初始化项目
来源：http://eof.cdnleiting.top

npm init -y;  npm i express
来源：http://ftn.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://ucm.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://joq.yuanzhike.top

[U83] JS：ES Module 导入导出
来源：http://dda.yj20258.top

export const a = 1;  import { a } from "./m.js";
来源：http://slw.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://sfe.shanyushiyangtech.top

module.exports = { a };  const { a } = require("./m");
来源：http://qeg.hesvh.cn

[U85] JS：可选链
来源：http://lyr.xylfe.cn

a?.b?.c
来源：http://qdw.zycfv.cn

[U86] JS：空值合并
来源：http://nyc.fehbvm.com

a ?? b
来源：http://rsw.uphjek.com

[U87] JS：解构默认值
来源：http://shk.meibo888.top

const { a = 1, b = 2 } = obj;
来源：http://jeq.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://wqv.chenjidiqi.icu

{ ...a, ...b }
来源：http://nez.xingfuxueyuan.xyz

[U89] JS：数组去重
来源：http://wmp.yj20258.top

[...new Set(arr)]
来源：http://ybq.9152youxi.cn

[U90] JS：数字数组排序
来源：http://sle.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://ukg.ivvv.top

[U91] JS：对象键值遍历
来源：http://zcn.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://arq.jqgufenzy.top

[U92] JS：深拷贝
来源：http://isr.yj202588.top

structuredClone(obj)
来源：http://hes.jianghu66.top

[U93] JS：模板字符串
来源：http://kxf.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://eoz.cdnleiting.top

[U94] JS：箭头函数
来源：http://jic.yanxiufei.cn

const double = x => x * 2;
来源：http://idp.gzhubu.top

[U95] JS：Promise 包装
来源：http://pzh.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://wqx.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://wbn.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aul.fehbvm.com

[U97] JS：并发请求
来源：http://qgc.bjfxy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cjj.sufxvd.cn

[U98] JS：fetch 带 JSON
来源：http://qsk.hammf.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kbt.daria6918.cn

[U99] JS：事件监听
来源：http://hbp.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://bmg.xziqi.cn

[U100] JS：DOM 查询
来源：http://qqg.xinyue.icu

document.querySelector(".item")
来源：http://dpz.nanxinkj.top

[U101] JS：classList 操作
来源：http://bio.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://ltz.jianghu66.top

[U102] JS：本地存储
来源：http://upx.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sen.yanxiufei.cn

[U103] JS：定时器
来源：http://zty.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://czk.yj20258888.top

[U104] JS：防抖
来源：http://iei.zdbjq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lqi.haohaochexian.top

[U105] JS：节流
来源：http://qop.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://osv.gzhubu.top

[U106] JS：日期格式化
来源：http://zwp.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nuj.uphjek.com

[U107] JS：数字千分位
来源：http://bwm.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eku.xylfe.cn

[U108] JS：随机整数
来源：http://sba.hammf.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hmw.jiagoushi.top

[U109] JS：数组分组
来源：http://pvg.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://lkf.fehbvm.com

[U110] JS：数组分块
来源：http://wlc.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wmh.shuidangran.top

[U111] JS：对象转 Map
来源：http://aud.yj202588.top

new Map(Object.entries(obj))
来源：http://khy.sysykeji.top

[U112] JS：字符串补位
来源：http://icz.tian-w.cn

"7".padStart(3, "0")
来源：http://fqr.cucudq.cn

[U113] JS：正则替换全部
来源：http://sxg.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://iyi.tarul.cn

[U114] JS：JSON 深比较
来源：http://obk.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ryd.mhx1999.top

[U115] JS：生成 UUID
来源：http://mmj.yvedp.cn

crypto.randomUUID()
来源：http://bhr.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://nhm.zhoulong.xyz

/** @param {string} name */ function f(name) {}
来源：http://gey.pengpengdd.cyou

[U117] JS：单元测试
来源：http://yuq.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://nyi.xziqi.cn

[U118] JS：开发服务器
来源：http://hme.yonumen.top

npm i -D vite;  npx vite
来源：http://arm.cashguo.top

[U119] JS：生产构建
来源：http://inb.hywenlv.cn

npx vite build
来源：http://yeo.bbcook.cn

[U120] JS：读取环境变量（Vite）
来源：http://hoa.yongpay.top

import.meta.env.VITE_API_URL
来源：http://cey.fehbvm.com

================================================================================
来源：http://ffy.tian-w.cn

统计汇总
来源：http://gyt.jianghu66.top

================================================================================
来源：http://zed.zhiwuduotai.top

按语言统计（条）：
来源：http://ufw.meibo888.top

Python ......... 252
来源：http://hun.ydzc1.top

PHP ............ 252
来源：http://alb.jinqigfzy.top

JavaScript ..... 252
来源：http://hrp.yongpay.top

TypeScript ..... 212
来源：http://ilj.cucudq.cn

Java ........... 212
来源：http://vec.ivvv.top

Go ............. 212
来源：http://uxa.bjfxy.top

Ruby ........... 212
来源：http://rjj.cashguo.top

C# ............. 212
来源：http://xjj.zhaomingkeji.xyz

C .............. 30
来源：http://ccs.nwbrower.top

C++ ............ 30
来源：http://xrh.hysaishi.cn

SQL ............ 90
来源：http://onl.jinyuanbaomall.cn

Bash ........... 80
来源：http://zuf.yuanzhike.top

Kotlin ......... 15
来源：http://pqq.yanxiufei.cn

Swift .......... 15
来源：http://ish.bjfxy.top

Lua ............ 10
来源：http://ong.tian-w.cn

Perl ........... 10
来源：http://fkz.fanxiaobao.xyz

Scala .......... 10
来源：http://kae.yanxiufei.cn

------------------------------------
来源：http://xrr.yj20258888.top

合计 ........... 2106 条
来源：http://ywv.guannengcc.top

按章节统计：
来源：http://soq.gotoacloud.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fjh.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mcl.yongpay.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ept.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ioq.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jrh.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://min.bjfxy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://llp.wangshuangyany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://inj.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://htt.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://czw.gaohongyu789.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://atv.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mhj.cheryme.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kcg.jianghu66.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gkx.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://okm.ehwqpu.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eia.sxryk.cn

Q SQL 专题                              90
来源：http://hrw.havefunace.top

R Bash 专题                             80
来源：http://fxd.shanyushiyangkeji.top

S C / C++ 专题                          60
来源：http://tvd.ybcxt.top

T 其他语言补充                          60
来源：http://zgq.guannengcc.top

U 高频实用片段                         120
来源：http://ujh.zhaomingkeji.xyz

------------------------------------
来源：http://ypx.yangfankeji.com

合计                                  2106 条
来源：http://hcw.wangdashe.top

--------------------------------------------------------------------------------
来源：http://brd.guowangkeji.top

使用提醒
来源：http://asj.birdmap.top

--------------------------------------------------------------------------------
来源：http://nxb.jiagoushi.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lzo.0kj1m.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qup.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dkd.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://krl.shzxlz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kmz.xinyue.icu

—— 文件结束 ——
来源：http://res.sweek.top

================================================================================
来源：http://zkf.fktsv.cn

程序语言常见例子速查手册（2024 版）
来源：http://ysw.52xcode.cn

Common Programming Examples Cheat Book
来源：http://aiz.zhaomingkeji.xyz

================================================================================
来源：http://hsq.zdbjq.cn

【收录内容】
来源：http://szm.52xcode.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vhs.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jqk.9152youxi.cn

SQL · Bash · C · C++
来源：http://wiz.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xng.sysykeji.top

【使用说明】
来源：http://njv.yanxiufei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qrj.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xoa.havefunace.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://afb.nanxinkj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qtv.9152youxi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wer.aizwys.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zom.xingfuxueyuan.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uhd.uphjek.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wxl.jinyuanbaomall.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://erb.vqdsnc.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://swe.yvedp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cwm.dianchejie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fae.hfpthk.cn

【文件统计】
来源：http://ywz.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dvt.cucudq.cn

--------------------------------------------------------------------------------
来源：http://bkf.hywenlv.cn

目  录
来源：http://ueb.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://lxh.gaohongyu789.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ela.shangyingyoupin.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fyu.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zyn.tian-w.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gji.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gum.xingfuxueyuan.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jsi.shanyushiyangtech.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://srh.chenzaomai.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cec.yfazqb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://okw.vehdjk.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kky.jiagoushi.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jfy.cucudq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zdv.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://htc.gogol.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zok.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://irk.guannengcc.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dcf.shangyingyoupin.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pjd.daxiang520.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://sxj.ydjk.org.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kzq.yueranfly.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cyk.gotoacloud.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lul.zhixingplan.top

================================================================================
来源：http://oyd.xylfe.cn

A. 基础语法与类型
来源：http://icu.fengsongda.top

================================================================================
来源：http://one.ydjk.org.cn

[A01] Hello World
来源：http://eae.hywenlv.cn

Py:   print("Hello, World!")
来源：http://shg.mhx1999.top

PHP:  echo "Hello, World!";
来源：http://dlj.fengsongda.top

JS:   console.log("Hello, World!");
来源：http://hjh.yj20258888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ixr.daxiang520.top

Java: System.out.println("Hello, World!");
来源：http://lck.vehdjk.com

Go:   fmt.Println("Hello, World!")
来源：http://vbf.shuidangran.top

Ruby: puts "Hello, World!"
来源：http://nhz.cheryme.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ufy.hfpthk.cn

[A02] 变量声明与赋值
来源：http://egs.ybcxt.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xuu.0kj1m.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nij.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://hgp.jinghuilouyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sgi.jinqigfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://ils.guowangkeji.top

Go:   name := "Alex"; age := 20
来源：http://nxv.hysaishi.cn

Ruby: name = "Alex"; age = 20
来源：http://ecf.jinqigufen.top

C#:   string name = "Alex"; int age = 20;
来源：http://gin.bbcook.cn

[A03] 常量定义
来源：http://rxu.cashguo.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cko.52xcode.cn

PHP:  const PI = 3.14159;
来源：http://vwe.hysaishi.cn

JS:   const PI = 3.14159;
来源：http://nrw.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://sjs.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://woj.hysaishi.cn

Go:   const PI = 3.14159
来源：http://zya.uphjek.com

Ruby: PI = 3.14159
来源：http://vha.yj20258888.top

C#:   const double PI = 3.14159;
来源：http://vsp.yfazqb.com

[A04] 判断变量类型
来源：http://ojg.sxryk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yff.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xaj.yj20258.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ffv.hysaishi.cn

TS:   typeof x; x instanceof Date
来源：http://anc.epnwcf.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yyi.cheryme.top

Go:   reflect.TypeOf(x).Name()
来源：http://nlb.jyoumei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sve.ivvv.top

C#:   x.GetType().Name; x is int
来源：http://ucu.daxiang520.top

[A05] 整数除法与取模
来源：http://nta.pengpengdd.cyou

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ivg.chenjidiqi.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://zvp.yuanzhike.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://axu.cucudq.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wwq.jinqigfzy.top

Java: 7 / 2; 7 % 2
来源：http://sex.zhoulong.xyz

Go:   7 / 2; 7 % 2
来源：http://qpf.c1oappe.top

Ruby: 7 / 2; 7 % 2
来源：http://sgw.fzhhl.top

C#:   7 / 2; 7 % 2
来源：http://poo.sweek.top

[A06] 字符串转数字
来源：http://hhs.yuxming.cn

Py:   int("42"); float("3.14")
来源：http://gah.vehdjk.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wza.sufxvd.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gsm.jinqigufen.top

TS:   parseInt("42", 10); Number("42")
来源：http://ycz.haohaochexian.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sez.52xcode.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ojf.hysaishi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qyp.fzhhl.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://grv.jlsjyb.cn

[A07] 数字转字符串
来源：http://sem.tarul.cn

Py:   str(42)
来源：http://vdv.birdmap.top

PHP:  (string) 42; strval(42)
来源：http://qkh.uphjek.com

JS:   String(42); (42).toString()
来源：http://gmk.hcnkem.com

TS:   String(42)
来源：http://jqj.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rkv.jqgufenzy.top

Go:   strconv.Itoa(42)
来源：http://rwu.zhaomingkeji.xyz

Ruby: 42.to_s
来源：http://cjt.zhijiandao.cn

C#:   42.ToString()
来源：http://hir.ydzc1.top

[A08] 取整与四舍五入
来源：http://wjj.jinqigfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tdn.havefunace.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nwn.aizwys.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hkw.sysykeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://udh.ybcxt.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qjn.daxiang520.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gao.yj20258888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://tqd.jinqigfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bsc.yj202588.top

[A09] 绝对值与最大最小值
来源：http://ldo.316326.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ngs.hesvh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://moi.sufxvd.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ppy.chenzaomai.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ppq.yonumen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nip.bjfxy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pzf.ywan-chungtsiang.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zoj.yonumen.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bex.chenlongwang.top


<!-- 参考信息 -->