代发 wailian999

[U63] PHP：文件读写
来源：http://sry.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ozs.nanxinkj.top

[U64] PHP：目录遍历
来源：http://dsc.ywan-chungtsiang.top

glob("dir/*.php");  scandir("dir");
来源：http://jsl.chenjidiqi.icu

[U65] PHP：会话
来源：http://kix.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://osx.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://obv.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://syn.tian-w.cn

[U67] PHP：处理文件上传
来源：http://rdq.yj20258.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://srj.sysykeji.top

[U68] PHP：PDO 连接
来源：http://wyu.cheryme.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://njg.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://qek.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hmg.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://dwm.smart0.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jlx.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://ser.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://jgm.jinyuanbaomall.cn

[U72] PHP：写错误日志
来源：http://obe.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://eiw.zhiwuduotai.top

[U73] PHP：读取 ini 配置
来源：http://ucb.ivvv.top

parse_ini_file("config.ini", true)
来源：http://rhq.snrcjt.cn

[U74] PHP：读取环境变量
来源：http://zzo.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://wpk.ivvv.top

[U75] PHP：依赖注入
来源：http://vlu.sysykeji.top

composer require psr/container
来源：http://guu.sufxvd.cn

[U76] PHP：简单路由
来源：http://cvd.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wut.andypj.xyz

[U77] PHP：模板渲染
来源：http://mxx.gotoacloud.top

composer require twig/twig
来源：http://vob.iojbl.cn

[U78] PHP：单元测试
来源：http://vin.shuidangran.top

composer require --dev phpunit/phpunit
来源：http://kkm.birdmap.top

[U79] PHP：静态分析
来源：http://vle.zhaomingkeji.xyz

composer require --dev phpstan/phpstan
来源：http://atz.pycfn.com

[U80] PHP：代码规范修复
来源：http://toq.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gbe.haohaochexian.top

[U81] JS：初始化项目
来源：http://ylb.aizwys.cn

npm init -y;  npm i express
来源：http://xmt.hnxiangtu.top

[U82] JS：package.json 脚本
来源：http://uns.fzhhl.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mrq.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://aef.aizwys.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cdi.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://cbn.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://qqd.bjfxy.top

[U85] JS：可选链
来源：http://aop.9152youxi.cn

a?.b?.c
来源：http://pxd.gaohongyu789.top

[U86] JS：空值合并
来源：http://hoy.zhijiandao.cn

a ?? b
来源：http://rrs.yj20258888.top

[U87] JS：解构默认值
来源：http://rap.mhx1999.top

const { a = 1, b = 2 } = obj;
来源：http://yik.nwbrower.top

[U88] JS：对象展开合并
来源：http://exq.chenlongwang.top

{ ...a, ...b }
来源：http://gon.jqgufenzy.top

[U89] JS：数组去重
来源：http://tpn.shuidangran.top

[...new Set(arr)]
来源：http://viy.jinqigufen.top

[U90] JS：数字数组排序
来源：http://fne.9152youxi.cn

[...arr].sort((a, b) => a - b)
来源：http://xyg.snrcjt.cn

[U91] JS：对象键值遍历
来源：http://rcg.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xmm.zdbjq.cn

[U92] JS：深拷贝
来源：http://pqv.mhx1999.top

structuredClone(obj)
来源：http://svu.yanxiufei.cn

[U93] JS：模板字符串
来源：http://rqx.sweek.top

`共 ${n} 条`
来源：http://ets.yueranfly.top

[U94] JS：箭头函数
来源：http://evo.smart0.xyz

const double = x => x * 2;
来源：http://yrr.gotoacloud.top

[U95] JS：Promise 包装
来源：http://nef.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://unq.yvedp.cn

[U96] JS：async/await 与异常
来源：http://vdv.wangdashe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://trc.aibaodan.cn

[U97] JS：并发请求
来源：http://mzj.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://spo.zhongyouzk.top

[U98] JS：fetch 带 JSON
来源：http://ijx.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nqs.jyoumei.cn

[U99] JS：事件监听
来源：http://mwc.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://ztr.yj202588.top

[U100] JS：DOM 查询
来源：http://vyd.nwbrower.top

document.querySelector(".item")
来源：http://ahb.birdmap.top

[U101] JS：classList 操作
来源：http://hju.gzhubu.top

el.classList.toggle("active")
来源：http://dww.havefunace.top

[U102] JS：本地存储
来源：http://xgx.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lna.sysykeji.top

[U103] JS：定时器
来源：http://xbr.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sfc.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://jai.cashguo.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gdy.hesvh.cn

[U105] JS：节流
来源：http://bgq.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pai.birdmap.top

[U106] JS：日期格式化
来源：http://rgt.jinqigufen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yvs.shzxlz.cn

[U107] JS：数字千分位
来源：http://qbh.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bxc.sxryk.cn

[U108] JS：随机整数
来源：http://obi.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://din.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://rlb.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://xoc.fengsongda.top

[U110] JS：数组分块
来源：http://fah.xuanzx.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://okz.xinyue.icu

[U111] JS：对象转 Map
来源：http://cdc.yfazqb.com

new Map(Object.entries(obj))
来源：http://iub.haohaochexian.top

[U112] JS：字符串补位
来源：http://zcx.ehwqpu.com

"7".padStart(3, "0")
来源：http://hee.tianlin.xyz

[U113] JS：正则替换全部
来源：http://brm.chenzaomai.com

s.replaceAll("a", "b")
来源：http://poj.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://aiz.redwolf501.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gen.316326.xyz

[U115] JS：生成 UUID
来源：http://mlj.wangshuangyany.cn

crypto.randomUUID()
来源：http://try.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ebj.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://ooc.ivvv.top

[U117] JS：单元测试
来源：http://vem.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://ewj.yueranfly.top

[U118] JS：开发服务器
来源：http://ugm.redwolf501.top

npm i -D vite;  npx vite
来源：http://sha.zhiwuduotai.top

[U119] JS：生产构建
来源：http://pxu.nanxuanxn.top

npx vite build
来源：http://wxk.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://qzh.yj202588.top

import.meta.env.VITE_API_URL
来源：http://dxn.jlsjyb.cn

================================================================================
来源：http://cwx.vqdsnc.cn

统计汇总
来源：http://kgm.yanxiufei.cn

================================================================================
来源：http://yde.ybcxt.top

按语言统计（条）：
来源：http://etn.guowangkeji.top

Python ......... 252
来源：http://epf.smart0.xyz

PHP ............ 252
来源：http://owt.wangdashe.top

JavaScript ..... 252
来源：http://hmq.ppjwa.cn

TypeScript ..... 212
来源：http://srg.yvedp.cn

Java ........... 212
来源：http://qmz.sxryk.cn

Go ............. 212
来源：http://qhu.sweek.top

Ruby ........... 212
来源：http://ajv.yvedp.cn

C# ............. 212
来源：http://pas.jinyuanbaomall.cn

C .............. 30
来源：http://wja.ivvv.top

C++ ............ 30
来源：http://qlk.xuanzx.com

SQL ............ 90
来源：http://oqz.52xcode.cn

Bash ........... 80
来源：http://brk.yueranfly.top

Kotlin ......... 15
来源：http://fqa.pengpengdd.cyou

Swift .......... 15
来源：http://ylc.guowangkeji.top

Lua ............ 10
来源：http://vib.yj20258.top

Perl ........... 10
来源：http://fmr.jyoumei.cn

Scala .......... 10
来源：http://tcd.ybcxt.top

------------------------------------
来源：http://vry.fehbvm.com

合计 ........... 2106 条
来源：http://rad.pengpengdd.cyou

按章节统计：
来源：http://ywg.bjfxy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dbn.yueranfly.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gxe.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hlg.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bvt.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dzq.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yjm.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aem.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://amw.zycfv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eyb.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ujd.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://olu.shanyushiyangtech.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jyn.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jqz.snrcjt.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://klv.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qhr.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jch.hysaishi.cn

Q SQL 专题                              90
来源：http://bli.jianghu66.top

R Bash 专题                             80
来源：http://vcj.vehdjk.com

S C / C++ 专题                          60
来源：http://jws.nanxinkj.top

T 其他语言补充                          60
来源：http://dwh.zhijiandao.cn

U 高频实用片段                         120
来源：http://zvc.cheryme.top

------------------------------------
来源：http://klk.vqdsnc.cn

合计                                  2106 条
来源：http://saj.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://fyg.yj20258888.top

使用提醒
来源：http://vsr.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://omv.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iex.yongpay.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dmm.ctjpmb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mbe.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nks.pengpengdd.cyou

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pbt.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://fno.chenlongwang.top

================================================================================
来源：http://rzw.mhx1999.top

程序语言常见例子速查手册（2024 版）
来源：http://jjb.zhengqikj.top

Common Programming Examples Cheat Book
来源：http://lka.hfpthk.cn

================================================================================
来源：http://hvk.bbcook.cn

【收录内容】
来源：http://jcs.svipenyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wtb.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pvy.sxryk.cn

SQL · Bash · C · C++
来源：http://dhx.0kj1m.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eya.gzhubu.top

【使用说明】
来源：http://dlx.xinyue.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://myd.tarul.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eym.yfazqb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dfl.shanyushiyangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tbd.zhiwuduotai.top

Bash:  Shell         C:     C             C++:   C++
来源：http://oxu.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lcm.ehwqpu.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nob.sysykeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lkf.xziqi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wdg.9152youxi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jib.meibo888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ffa.bjfxy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tpv.ybcxt.top

【文件统计】
来源：http://dxb.c1oappe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mge.fzhhl.top

--------------------------------------------------------------------------------
来源：http://cur.aizwys.cn

目  录
来源：http://cgb.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://fra.tianlin.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yrr.sufxvd.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wdq.havefunace.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ibn.shanyushiyangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jot.wangdashe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ddf.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rwy.daxiang520.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://puk.smart0.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://urp.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zcu.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iby.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qqd.sweek.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fhg.sysykeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://seh.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dfh.chenzaomai.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bbc.snrcjt.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vol.shuidangran.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bvv.ydzc1.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://iqi.hnqzz.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dbi.yueranfly.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jlq.pengpengdd.cyou

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ukm.xuanzx.com

================================================================================
来源：http://lwx.tarul.cn

A. 基础语法与类型
来源：http://xhe.jinyuanbaomall.cn

================================================================================
来源：http://juc.316326.xyz

[A01] Hello World
来源：http://zgw.zhongyouzk.top

Py:   print("Hello, World!")
来源：http://coo.iojbl.cn

PHP:  echo "Hello, World!";
来源：http://stk.xinyue.icu

JS:   console.log("Hello, World!");
来源：http://lvx.9152youxi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pux.shanyushiyangkeji.top

Java: System.out.println("Hello, World!");
来源：http://pbr.guowangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://buy.0kj1m.cn

Ruby: puts "Hello, World!"
来源：http://mch.zhiwuduotai.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tcs.yvedp.cn

[A02] 变量声明与赋值
来源：http://con.snrcjt.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ilc.sysykeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://niq.vehdjk.com

JS:   let name = "Alex"; const age = 20;
来源：http://ysg.hongshengwenyu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lkr.yueranfly.top

Java: String name = "Alex"; int age = 20;
来源：http://enl.52xcode.cn

Go:   name := "Alex"; age := 20
来源：http://brd.jqgufenzy.top

Ruby: name = "Alex"; age = 20
来源：http://lfy.cashguo.top

C#:   string name = "Alex"; int age = 20;
来源：http://oth.zycfv.cn

[A03] 常量定义
来源：http://bot.cheryme.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eed.sufxvd.cn

PHP:  const PI = 3.14159;
来源：http://cou.birdmap.top

JS:   const PI = 3.14159;
来源：http://alj.wangdashe.top

TS:   const PI: number = 3.14159;
来源：http://fam.ydjk.org.cn

Java: static final double PI = 3.14159;
来源：http://xws.birdmap.top

Go:   const PI = 3.14159
来源：http://xpk.havefunace.top

Ruby: PI = 3.14159
来源：http://vkf.jyoumei.cn

C#:   const double PI = 3.14159;
来源：http://kjb.vqdsnc.cn

[A04] 判断变量类型
来源：http://pdg.yj202588.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ots.sjlbkw.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sff.guannengcc.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qpf.snrcjt.cn

TS:   typeof x; x instanceof Date
来源：http://ifr.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://upq.vehdjk.com

Go:   reflect.TypeOf(x).Name()
来源：http://voi.zdbjq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jwb.chenlongwang.top

C#:   x.GetType().Name; x is int
来源：http://qwr.52xcode.cn

[A05] 整数除法与取模
来源：http://hlm.shuidangran.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nwg.zhengqikj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://suz.yangfankeji.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bkd.gogol.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://csh.chenzaomai.com

Java: 7 / 2; 7 % 2
来源：http://gxg.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://ypj.jqgufenzy.top

Ruby: 7 / 2; 7 % 2
来源：http://tjb.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://jqm.sufxvd.cn

[A06] 字符串转数字
来源：http://btb.316326.xyz

Py:   int("42"); float("3.14")
来源：http://lux.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dcy.chenjidiqi.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pza.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vmq.haohaochexian.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iru.dianchejie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cgq.tanke756.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ega.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://awp.jqgfzy.top

[A07] 数字转字符串
来源：http://zjv.sweek.top

Py:   str(42)
来源：http://mne.zhaomingkeji.xyz

PHP:  (string) 42; strval(42)
来源：http://lph.yangfankeji.com

JS:   String(42); (42).toString()
来源：http://hsu.ehwqpu.com

TS:   String(42)
来源：http://cnm.hfpthk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cji.yuanzhike.top

Go:   strconv.Itoa(42)
来源：http://sye.0kj1m.cn

Ruby: 42.to_s
来源：http://rcp.sufxvd.cn

C#:   42.ToString()
来源：http://svu.hysaishi.cn

[A08] 取整与四舍五入
来源：http://mrq.yangfankeji.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ngt.zdqjudy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xrk.hysaishi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://knv.jinqigufen.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qwc.nanxinkj.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vya.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sdh.hnxiangtu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://eob.birdmap.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oca.fktsv.cn

[A09] 绝对值与最大最小值
来源：http://dpf.hongshengwenyu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tet.jinyuanbaomall.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://umx.pycfn.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xei.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yny.tianlin.xyz


<!-- 参考信息 -->