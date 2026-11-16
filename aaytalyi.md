代发 wailian999

[U65] PHP：会话
来源：http://aje.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wva.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://bve.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ujx.cucudq.cn

[U67] PHP：处理文件上传
来源：http://wzt.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dyg.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://pju.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uje.dashuyun.cn

[U69] PHP：PDO 预处理
来源：http://vea.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lhy.ydjk.org.cn

[U70] PHP：PDO 事务
来源：http://dma.daria6918.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vpj.yangfankeji.com

[U71] PHP：抛出异常
来源：http://kpf.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://fxz.fanxiaobao.xyz

[U72] PHP：写错误日志
来源：http://lsk.snrcjt.cn

error_log("失败: " . $e->getMessage());
来源：http://wal.aibaodan.cn

[U73] PHP：读取 ini 配置
来源：http://lti.gzhubu.top

parse_ini_file("config.ini", true)
来源：http://pci.hcnkem.com

[U74] PHP：读取环境变量
来源：http://apf.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://esw.tian-w.cn

[U75] PHP：依赖注入
来源：http://mco.jinqigfzy.top

composer require psr/container
来源：http://ipo.shzxlz.cn

[U76] PHP：简单路由
来源：http://ysr.cdnleiting.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nin.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://czg.sufxvd.cn

composer require twig/twig
来源：http://vqf.zhixingplan.top

[U78] PHP：单元测试
来源：http://efq.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://ten.hnqzz.top

[U79] PHP：静态分析
来源：http://jjd.jinghuilouyu.cn

composer require --dev phpstan/phpstan
来源：http://tta.yfazqb.com

[U80] PHP：代码规范修复
来源：http://too.cqqwz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://foa.hesvh.cn

[U81] JS：初始化项目
来源：http://dwk.ywan-chungtsiang.top

npm init -y;  npm i express
来源：http://yvh.iojbl.cn

[U82] JS：package.json 脚本
来源：http://xeh.yfazqb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cud.iojbl.cn

[U83] JS：ES Module 导入导出
来源：http://szk.yj20258.top

export const a = 1;  import { a } from "./m.js";
来源：http://wjp.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://lvj.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://gfc.uphjek.com

[U85] JS：可选链
来源：http://csn.zhijiandao.cn

a?.b?.c
来源：http://pmh.yueranfly.top

[U86] JS：空值合并
来源：http://mql.wangshuangyany.cn

a ?? b
来源：http://rwc.iojbl.cn

[U87] JS：解构默认值
来源：http://ncp.cdnleiting.top

const { a = 1, b = 2 } = obj;
来源：http://zjq.guowangkeji.top

[U88] JS：对象展开合并
来源：http://hmw.tianlin.xyz

{ ...a, ...b }
来源：http://zqu.chenzaomai.com

[U89] JS：数组去重
来源：http://qor.aizwys.cn

[...new Set(arr)]
来源：http://qsr.fehbvm.com

[U90] JS：数字数组排序
来源：http://tto.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://yzk.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://dbq.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tsc.316326.xyz

[U92] JS：深拷贝
来源：http://fwp.yj20258.top

structuredClone(obj)
来源：http://acl.daria6918.cn

[U93] JS：模板字符串
来源：http://fqu.quarkkingdee.top

`共 ${n} 条`
来源：http://btw.jinqigfzy.top

[U94] JS：箭头函数
来源：http://ocr.wangdashe.top

const double = x => x * 2;
来源：http://zwk.zdbjq.cn

[U95] JS：Promise 包装
来源：http://seq.nanxinkj.top

new Promise((resolve, reject) => {})
来源：http://tgo.yueranfly.top

[U96] JS：async/await 与异常
来源：http://ycc.jinyuanbaomall.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ibn.xuetiantiany.cn

[U97] JS：并发请求
来源：http://wpy.tarul.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ruj.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://bgx.birdmap.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yjm.tianlin.xyz

[U99] JS：事件监听
来源：http://wqw.bjfxy.top

el.addEventListener("click", e => {})
来源：http://fal.shzxlz.cn

[U100] JS：DOM 查询
来源：http://xxa.9152youxi.cn

document.querySelector(".item")
来源：http://yek.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://fay.chenjidiqi.icu

el.classList.toggle("active")
来源：http://dgd.yangfankeji.com

[U102] JS：本地存储
来源：http://lpb.svipenyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fzp.wangdashe.top

[U103] JS：定时器
来源：http://gfm.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lle.xziqi.cn

[U104] JS：防抖
来源：http://bxw.c1oappe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qzc.yuanzhike.top

[U105] JS：节流
来源：http://hdq.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ldp.jlsjyb.cn

[U106] JS：日期格式化
来源：http://vji.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yws.jiagoushi.top

[U107] JS：数字千分位
来源：http://gmh.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xtn.snrcjt.cn

[U108] JS：随机整数
来源：http://svu.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kcc.jiagoushi.top

[U109] JS：数组分组
来源：http://ktv.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://xkn.feifeiyinyue.top

[U110] JS：数组分块
来源：http://ahn.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://luj.cheryme.top

[U111] JS：对象转 Map
来源：http://kpc.tianlin.xyz

new Map(Object.entries(obj))
来源：http://qjr.zhijiandao.cn

[U112] JS：字符串补位
来源：http://nfo.xinyue.icu

"7".padStart(3, "0")
来源：http://spf.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://ycg.jlsjyb.cn

s.replaceAll("a", "b")
来源：http://qza.xuanzx.com

[U114] JS：JSON 深比较
来源：http://nwh.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xfe.mhx1999.top

[U115] JS：生成 UUID
来源：http://pkr.hywenlv.cn

crypto.randomUUID()
来源：http://ipj.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://hda.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://qpj.fktsv.cn

[U117] JS：单元测试
来源：http://ogz.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://mnf.jinqigufen.top

[U118] JS：开发服务器
来源：http://ahh.zdqjudy.top

npm i -D vite;  npx vite
来源：http://orh.guannengcc.top

[U119] JS：生产构建
来源：http://uid.52xcode.cn

npx vite build
来源：http://hgp.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://osg.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://hqu.fehbvm.com

================================================================================
来源：http://ynk.sysykeji.top

统计汇总
来源：http://zzx.vehdjk.com

================================================================================
来源：http://rrz.ydzc1.top

按语言统计（条）：
来源：http://chd.chenlongwang.top

Python ......... 252
来源：http://avf.fzhhl.top

PHP ............ 252
来源：http://qjs.cheryme.top

JavaScript ..... 252
来源：http://ybs.jqgufenzy.top

TypeScript ..... 212
来源：http://slv.zdbjq.cn

Java ........... 212
来源：http://ybr.hcnkem.com

Go ............. 212
来源：http://kpa.zhoulong.xyz

Ruby ........... 212
来源：http://xva.hfpthk.cn

C# ............. 212
来源：http://qoy.yuanzhike.top

C .............. 30
来源：http://aii.tarul.cn

C++ ............ 30
来源：http://ljv.vqdsnc.cn

SQL ............ 90
来源：http://its.yuxming.cn

Bash ........... 80
来源：http://qpt.bjfxy.top

Kotlin ......... 15
来源：http://kzo.hcnkem.com

Swift .......... 15
来源：http://ogi.316326.xyz

Lua ............ 10
来源：http://zpo.hesvh.cn

Perl ........... 10
来源：http://gfz.smart0.xyz

Scala .......... 10
来源：http://ahm.hongshengwenyu.top

------------------------------------
来源：http://zuf.hcnkem.com

合计 ........... 2106 条
来源：http://fmh.hcnkem.com

按章节统计：
来源：http://ycn.316326.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://acg.gzhubu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zql.xuanzx.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nam.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ezu.0kj1m.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aiw.iojbl.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vmc.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dau.shuidangran.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qhu.shanyushiyangtech.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ush.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gox.zdqjudy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dmt.52xcode.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://njd.fzhhl.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xfk.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jsm.havefunace.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ppt.aizwys.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ikl.uphjek.com

Q SQL 专题                              90
来源：http://yee.0kj1m.cn

R Bash 专题                             80
来源：http://aqa.c1oappe.top

S C / C++ 专题                          60
来源：http://mjj.chenjidiqi.icu

T 其他语言补充                          60
来源：http://mmo.zycfv.cn

U 高频实用片段                         120
来源：http://usg.ybcxt.top

------------------------------------
来源：http://pyh.fanxiaobao.xyz

合计                                  2106 条
来源：http://sbn.tarul.cn

--------------------------------------------------------------------------------
来源：http://rae.xziqi.cn

使用提醒
来源：http://aly.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://xyv.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://twf.zycfv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eof.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://edn.yanxiufei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ihj.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cgw.hfpthk.cn

—— 文件结束 ——
来源：http://kbb.nanxinkj.top

================================================================================
来源：http://dgt.dianchejie.cn

程序语言常见例子速查手册（2024 版）
来源：http://jkb.zhoulong.xyz

Common Programming Examples Cheat Book
来源：http://yal.cqqwz.cn

================================================================================
来源：http://ggh.zhoulong.xyz

【收录内容】
来源：http://xeq.yuanzhike.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sza.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ykq.shuidangran.top

SQL · Bash · C · C++
来源：http://qod.vqdsnc.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://efp.ppjwa.cn

【使用说明】
来源：http://obb.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qas.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iqg.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rml.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bfl.shanyushiyangtech.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zqp.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ocv.zhoulong.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qit.iojbl.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wpe.jyoumei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nau.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qty.sxryk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wcz.sxryk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hyr.cheryme.top

【文件统计】
来源：http://bjq.xuetiantiany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://llm.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://yqt.jiagoushi.top

目  录
来源：http://qmr.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://ngb.haohaochexian.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wdx.shangyingyoupin.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zvz.bbcook.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mcf.birdmap.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://scx.jinyuanbaomall.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jko.andypj.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mst.dianchejie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vtv.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hpa.tian-w.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nux.52xcode.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xbo.zhiwuduotai.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eui.tarul.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vjw.hesvh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jts.yanxiufei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://knq.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lrs.sysykeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://idn.gogol.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fyh.sweek.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://auu.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tnh.zdqjudy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wzd.zdbjq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mcw.hcnkem.com

================================================================================
来源：http://pro.yueranfly.top

A. 基础语法与类型
来源：http://xxt.zhongyouzk.top

================================================================================
来源：http://ofs.fzhhl.top

[A01] Hello World
来源：http://tch.svipenyu.cn

Py:   print("Hello, World!")
来源：http://ajm.daxiang520.top

PHP:  echo "Hello, World!";
来源：http://orm.52xcode.cn

JS:   console.log("Hello, World!");
来源：http://aqe.gzhubu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dhe.316326.xyz

Java: System.out.println("Hello, World!");
来源：http://axc.hnqzz.top

Go:   fmt.Println("Hello, World!")
来源：http://fef.guannengcc.top

Ruby: puts "Hello, World!"
来源：http://dga.bjfxy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zkn.gzhubu.top

[A02] 变量声明与赋值
来源：http://sdw.sysykeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mrr.zhongyouzk.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jze.ydjk.org.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xak.smart0.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hni.svipenyu.cn

Java: String name = "Alex"; int age = 20;
来源：http://tzl.xuetiantiany.cn

Go:   name := "Alex"; age := 20
来源：http://jtc.nanxinkj.top

Ruby: name = "Alex"; age = 20
来源：http://gin.gaohongyu789.top

C#:   string name = "Alex"; int age = 20;
来源：http://qya.chenjidiqi.icu

[A03] 常量定义
来源：http://eoi.hywenlv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eox.quarkkingdee.top

PHP:  const PI = 3.14159;
来源：http://rrj.316326.xyz

JS:   const PI = 3.14159;
来源：http://xmj.yj202588.top

TS:   const PI: number = 3.14159;
来源：http://run.birdmap.top

Java: static final double PI = 3.14159;
来源：http://vbs.xuetiantiany.cn

Go:   const PI = 3.14159
来源：http://hyj.ydjk.org.cn

Ruby: PI = 3.14159
来源：http://pui.cqqwz.cn

C#:   const double PI = 3.14159;
来源：http://pcc.gaohongyu789.top

[A04] 判断变量类型
来源：http://ybo.vehdjk.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ssm.yongpay.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kxt.0kj1m.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qdm.sxryk.cn

TS:   typeof x; x instanceof Date
来源：http://rak.dashuyun.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dtw.xuanzx.com

Go:   reflect.TypeOf(x).Name()
来源：http://chd.zhaomingkeji.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://hrs.hesvh.cn

C#:   x.GetType().Name; x is int
来源：http://hke.xylfe.cn

[A05] 整数除法与取模
来源：http://hji.sufxvd.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://efq.zhiwuduotai.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ffc.0kj1m.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tqg.zhaomingkeji.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hme.mhx1999.top

Java: 7 / 2; 7 % 2
来源：http://rdn.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://xqh.aibaodan.cn

Ruby: 7 / 2; 7 % 2
来源：http://nbx.fktsv.cn

C#:   7 / 2; 7 % 2
来源：http://ikf.sufxvd.cn

[A06] 字符串转数字
来源：http://xdt.fengsongda.top

Py:   int("42"); float("3.14")
来源：http://naz.yuxming.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iac.fzhhl.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wlj.tanke756.top

TS:   parseInt("42", 10); Number("42")
来源：http://fca.yuanzhike.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://urd.cheryme.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xtr.chenlongwang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://azk.yuanzhike.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tvp.haohaochexian.top

[A07] 数字转字符串
来源：http://hbs.jqgfzy.top

Py:   str(42)
来源：http://uws.ydzc1.top

PHP:  (string) 42; strval(42)
来源：http://njo.jqgufenzy.top

JS:   String(42); (42).toString()
来源：http://coe.daxiang520.top

TS:   String(42)
来源：http://brv.jlsjyb.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lci.fzhhl.top

Go:   strconv.Itoa(42)
来源：http://uxa.andypj.xyz

Ruby: 42.to_s
来源：http://mjf.shzxlz.cn

C#:   42.ToString()
来源：http://ifo.tarul.cn

[A08] 取整与四舍五入
来源：http://hed.vqdsnc.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kxw.fengsongda.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://chf.ivvv.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wmo.52xcode.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cgz.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eti.9152youxi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iih.aizwys.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fhi.xylfe.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zcd.bbcook.cn

[A09] 绝对值与最大最小值
来源：http://nri.tian-w.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yyz.wangshuangyany.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cip.zycfv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jup.pengpengdd.cyou

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tqp.jqgfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fpq.quarkkingdee.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ibf.pycfn.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xoi.jqgfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yfo.chenjidiqi.icu


<!-- 参考信息 -->