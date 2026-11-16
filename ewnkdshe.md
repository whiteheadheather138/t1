代发 wailian999

[U65] PHP：会话
来源：http://qyt.sweek.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uyq.sweek.top

[U66] PHP：设置 Cookie
来源：http://qqr.xuetiantiany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://icu.yongpay.top

[U67] PHP：处理文件上传
来源：http://htj.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ycx.wangdashe.top

[U68] PHP：PDO 连接
来源：http://nbt.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tjo.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://gig.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kec.fehbvm.com

[U70] PHP：PDO 事务
来源：http://kfq.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://idy.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://kyc.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://log.chenjidiqi.icu

[U72] PHP：写错误日志
来源：http://phz.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://dfh.hcnkem.com

[U73] PHP：读取 ini 配置
来源：http://mys.dianchejie.cn

parse_ini_file("config.ini", true)
来源：http://wsa.gotoacloud.top

[U74] PHP：读取环境变量
来源：http://cpg.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://yir.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://mxi.yuxming.cn

composer require psr/container
来源：http://aqz.ctjpmb.com

[U76] PHP：简单路由
来源：http://mge.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ymd.sweek.top

[U77] PHP：模板渲染
来源：http://yra.sysykeji.top

composer require twig/twig
来源：http://lol.cucudq.cn

[U78] PHP：单元测试
来源：http://vqv.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://xli.redwolf501.top

[U79] PHP：静态分析
来源：http://gei.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://azk.jinyuanbaomall.cn

[U80] PHP：代码规范修复
来源：http://opr.zhaomingkeji.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://btt.aizwys.cn

[U81] JS：初始化项目
来源：http://loh.feifeiyinyue.top

npm init -y;  npm i express
来源：http://alb.yfazqb.com

[U82] JS：package.json 脚本
来源：http://sof.hywenlv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://njw.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://jxc.wangshuangyany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kmj.smart0.xyz

[U84] JS：CommonJS 写法
来源：http://bfx.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://yyj.vehdjk.com

[U85] JS：可选链
来源：http://oua.cqqwz.cn

a?.b?.c
来源：http://pli.ivvv.top

[U86] JS：空值合并
来源：http://xen.jinghuilouyu.cn

a ?? b
来源：http://ked.ctjpmb.com

[U87] JS：解构默认值
来源：http://xnx.shangyingyoupin.top

const { a = 1, b = 2 } = obj;
来源：http://pco.snrcjt.cn

[U88] JS：对象展开合并
来源：http://jli.aizwys.cn

{ ...a, ...b }
来源：http://try.redwolf501.top

[U89] JS：数组去重
来源：http://bgh.hammf.cn

[...new Set(arr)]
来源：http://api.yuanzhike.top

[U90] JS：数字数组排序
来源：http://cgi.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://jpv.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://fbq.kuanghao11.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cox.jiagoushi.top

[U92] JS：深拷贝
来源：http://uqi.yangfankeji.com

structuredClone(obj)
来源：http://htl.zhongyouzk.top

[U93] JS：模板字符串
来源：http://per.jinyuanbaomall.cn

`共 ${n} 条`
来源：http://qop.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://cwz.fanxiaobao.xyz

const double = x => x * 2;
来源：http://zdx.hongshengwenyu.top

[U95] JS：Promise 包装
来源：http://twz.ybcxt.top

new Promise((resolve, reject) => {})
来源：http://lyi.bjfxy.top

[U96] JS：async/await 与异常
来源：http://rsl.tianlin.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ocx.jlsjyb.cn

[U97] JS：并发请求
来源：http://agx.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://tvk.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://squ.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mls.0kj1m.cn

[U99] JS：事件监听
来源：http://icm.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://kce.pengpengdd.cyou

[U100] JS：DOM 查询
来源：http://czv.dianchejie.cn

document.querySelector(".item")
来源：http://sho.hysaishi.cn

[U101] JS：classList 操作
来源：http://wza.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://jmz.ydjk.org.cn

[U102] JS：本地存储
来源：http://vhb.fengsongda.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iya.aibaodan.cn

[U103] JS：定时器
来源：http://rot.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iwb.ybcxt.top

[U104] JS：防抖
来源：http://vaf.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://unn.shuidangran.top

[U105] JS：节流
来源：http://iwr.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bfz.shuidangran.top

[U106] JS：日期格式化
来源：http://umb.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nef.fengsongda.top

[U107] JS：数字千分位
来源：http://zbu.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://csd.fktsv.cn

[U108] JS：随机整数
来源：http://nxr.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hty.andypj.xyz

[U109] JS：数组分组
来源：http://ctd.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://mjj.yj20258.top

[U110] JS：数组分块
来源：http://bdg.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mmr.pycfn.com

[U111] JS：对象转 Map
来源：http://xly.0kj1m.cn

new Map(Object.entries(obj))
来源：http://ycg.yueranfly.top

[U112] JS：字符串补位
来源：http://zgp.zhiwuduotai.top

"7".padStart(3, "0")
来源：http://zby.guowangkeji.top

[U113] JS：正则替换全部
来源：http://gtf.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://bre.xinyue.icu

[U114] JS：JSON 深比较
来源：http://sbp.shzxlz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rvu.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://mqp.fktsv.cn

crypto.randomUUID()
来源：http://wcz.hnxiangtu.top

[U116] JS：类型检查（JSDoc）
来源：http://ysh.gogol.net.cn

/** @param {string} name */ function f(name) {}
来源：http://hjt.epnwcf.com

[U117] JS：单元测试
来源：http://akj.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://ipu.jinghuilouyu.cn

[U118] JS：开发服务器
来源：http://cpv.ivvv.top

npm i -D vite;  npx vite
来源：http://rmo.aibaodan.cn

[U119] JS：生产构建
来源：http://kuc.yongpay.top

npx vite build
来源：http://ekf.hammf.cn

[U120] JS：读取环境变量（Vite）
来源：http://mvm.jqgfzy.top

import.meta.env.VITE_API_URL
来源：http://agq.bjfxy.top

================================================================================
来源：http://xlm.zhengqikj.top

统计汇总
来源：http://qah.meibo888.top

================================================================================
来源：http://ksn.xingfuxueyuan.xyz

按语言统计（条）：
来源：http://xdu.9152youxi.cn

Python ......... 252
来源：http://cdb.fzhhl.top

PHP ............ 252
来源：http://suq.zhoulong.xyz

JavaScript ..... 252
来源：http://mbe.cucudq.cn

TypeScript ..... 212
来源：http://dcb.ivvv.top

Java ........... 212
来源：http://xsr.guannengcc.top

Go ............. 212
来源：http://ild.fehbvm.com

Ruby ........... 212
来源：http://ojc.316326.xyz

C# ............. 212
来源：http://jnh.hongshengwenyu.top

C .............. 30
来源：http://spb.shzxlz.cn

C++ ............ 30
来源：http://rme.jianghu66.top

SQL ............ 90
来源：http://xsa.chenzaomai.com

Bash ........... 80
来源：http://ghh.yangfankeji.com

Kotlin ......... 15
来源：http://mvy.ydjk.org.cn

Swift .......... 15
来源：http://kxi.gotoacloud.top

Lua ............ 10
来源：http://itw.yuxming.cn

Perl ........... 10
来源：http://joq.yfazqb.com

Scala .......... 10
来源：http://kxi.c1oappe.top

------------------------------------
来源：http://wow.sxryk.cn

合计 ........... 2106 条
来源：http://ftj.yj20258.top

按章节统计：
来源：http://pou.sjlbkw.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jkh.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yby.ehwqpu.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vqx.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xyw.jqgfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://boh.hysaishi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dti.gzhubu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fav.guannengcc.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aix.havefunace.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mhn.birdmap.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ytv.ydzc1.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oex.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://avi.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ups.zhixingplan.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://svp.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vfy.dianchejie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://noj.gaohongyu789.top

Q SQL 专题                              90
来源：http://oiz.shanyushiyangkeji.top

R Bash 专题                             80
来源：http://qta.yj20258.top

S C / C++ 专题                          60
来源：http://who.316326.xyz

T 其他语言补充                          60
来源：http://kbi.pycfn.com

U 高频实用片段                         120
来源：http://slb.xinyue.icu

------------------------------------
来源：http://qbz.cucudq.cn

合计                                  2106 条
来源：http://djd.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://lmt.redwolf501.top

使用提醒
来源：http://aoa.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://lol.jinqigufen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zov.0kj1m.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vgg.bbcook.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hlp.daxiang520.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tfo.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rto.cqqwz.cn

—— 文件结束 ——
来源：http://dqm.pycfn.com

================================================================================
来源：http://his.bbcook.cn

程序语言常见例子速查手册（2024 版）
来源：http://dsi.yvedp.cn

Common Programming Examples Cheat Book
来源：http://mml.zhijiandao.cn

================================================================================
来源：http://wvx.gzhubu.top

【收录内容】
来源：http://jhz.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hbf.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ftw.chenzaomai.com

SQL · Bash · C · C++
来源：http://via.hammf.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cmo.fengsongda.top

【使用说明】
来源：http://gzb.kuanghao11.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bst.sweek.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ckq.wangdashe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://khi.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tdz.yongpay.top

Bash:  Shell         C:     C             C++:   C++
来源：http://oev.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://muj.jinqigufen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ecv.epnwcf.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://izc.vqdsnc.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fry.vehdjk.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://akm.gotoacloud.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mwf.yj20258.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nlm.mhx1999.top

【文件统计】
来源：http://gta.birdmap.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://thc.hesvh.cn

--------------------------------------------------------------------------------
来源：http://gvk.yonumen.top

目  录
来源：http://jrg.sweek.top

--------------------------------------------------------------------------------
来源：http://zxp.birdmap.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mcs.zdqjudy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://elq.kuanghao11.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://evp.birdmap.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vyi.jinghuilouyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ffy.tarul.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qwl.yj202588.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xmp.bjfxy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uah.vqdsnc.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cid.meibo888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jsp.uphjek.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jsv.c1oappe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ycs.pengpengdd.cyou

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uin.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://web.zhijiandao.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uun.yfazqb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kzp.gaohongyu789.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xrb.nanxuanxn.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://dfs.nanxuanxn.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mvj.zhongyouzk.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://feo.yuxming.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mnz.haohaochexian.top

================================================================================
来源：http://bbr.ydjk.org.cn

A. 基础语法与类型
来源：http://vmp.wangshuangyany.cn

================================================================================
来源：http://kfr.guowangkeji.top

[A01] Hello World
来源：http://phu.ivvv.top

Py:   print("Hello, World!")
来源：http://fen.sxryk.cn

PHP:  echo "Hello, World!";
来源：http://ovc.sweek.top

JS:   console.log("Hello, World!");
来源：http://jhr.chenlongwang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ktm.hammf.cn

Java: System.out.println("Hello, World!");
来源：http://aef.shangyingyoupin.top

Go:   fmt.Println("Hello, World!")
来源：http://jkn.gotoacloud.top

Ruby: puts "Hello, World!"
来源：http://dni.jianghu66.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nfr.yj20258.top

[A02] 变量声明与赋值
来源：http://whb.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bhw.zhixingplan.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fkg.yangfankeji.com

JS:   let name = "Alex"; const age = 20;
来源：http://hof.bjfxy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://anv.guowangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://jrc.xylfe.cn

Go:   name := "Alex"; age := 20
来源：http://xmo.bbcook.cn

Ruby: name = "Alex"; age = 20
来源：http://hyi.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nuf.yuanzhike.top

[A03] 常量定义
来源：http://xjn.yj20258.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mwe.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://auk.sweek.top

JS:   const PI = 3.14159;
来源：http://idf.sysykeji.top

TS:   const PI: number = 3.14159;
来源：http://tch.aibaodan.cn

Java: static final double PI = 3.14159;
来源：http://ayw.ppjwa.cn

Go:   const PI = 3.14159
来源：http://isv.tian-w.cn

Ruby: PI = 3.14159
来源：http://tfc.xziqi.cn

C#:   const double PI = 3.14159;
来源：http://wmk.bjfxy.top

[A04] 判断变量类型
来源：http://fqs.ctjpmb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ont.yongpay.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jlz.meibo888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bjc.c1oappe.top

TS:   typeof x; x instanceof Date
来源：http://vlk.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qby.sufxvd.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bax.jlsjyb.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ppg.kuanghao11.cn

C#:   x.GetType().Name; x is int
来源：http://nmv.tanke756.top

[A05] 整数除法与取模
来源：http://tif.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kzq.hongshengwenyu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jpj.zhongyouzk.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jah.hfpthk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://svv.fehbvm.com

Java: 7 / 2; 7 % 2
来源：http://erx.c1oappe.top

Go:   7 / 2; 7 % 2
来源：http://zek.jqgfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://qej.wangshuangyany.cn

C#:   7 / 2; 7 % 2
来源：http://wgl.zhoulong.xyz

[A06] 字符串转数字
来源：http://nak.yongpay.top

Py:   int("42"); float("3.14")
来源：http://fbj.andypj.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qpz.guannengcc.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cmo.fehbvm.com

TS:   parseInt("42", 10); Number("42")
来源：http://hoj.cdnleiting.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gra.hysaishi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://afw.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://kap.ywan-chungtsiang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wpr.yuanzhike.top

[A07] 数字转字符串
来源：http://riu.xuanzx.com

Py:   str(42)
来源：http://vup.birdmap.top

PHP:  (string) 42; strval(42)
来源：http://pnx.tanke756.top

JS:   String(42); (42).toString()
来源：http://xkq.zhengqikj.top

TS:   String(42)
来源：http://cew.yj202588.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hco.hnqzz.top

Go:   strconv.Itoa(42)
来源：http://esu.ydzc1.top

Ruby: 42.to_s
来源：http://ony.hesvh.cn

C#:   42.ToString()
来源：http://bjn.hywenlv.cn

[A08] 取整与四舍五入
来源：http://lzc.yonumen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://duv.snrcjt.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cfh.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zvi.jinqigfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ymw.chenlongwang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jul.ivvv.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qry.tanke756.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cmx.quarkkingdee.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://crr.fzhhl.top

[A09] 绝对值与最大最小值
来源：http://raj.yonumen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tjy.shanyushiyangtech.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qnj.xinyue.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qkn.sysykeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ydl.xuetiantiany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hnd.zhiwuduotai.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dco.epnwcf.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ulb.havefunace.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bvg.c1oappe.top


<!-- 参考信息 -->