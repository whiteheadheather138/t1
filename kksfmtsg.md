代发 wailian999

[U65] PHP：会话
来源：http://xed.0kj1m.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xto.yj20258.top

[U66] PHP：设置 Cookie
来源：http://sui.chenlongwang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lsv.tian-w.cn

[U67] PHP：处理文件上传
来源：http://ebq.andypj.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://joe.fengsongda.top

[U68] PHP：PDO 连接
来源：http://jgi.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mdw.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://kei.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://khi.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://fgi.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cki.yvedp.cn

[U71] PHP：抛出异常
来源：http://jir.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://idy.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://nlw.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://bhz.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://tid.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://jmh.pycfn.com

[U74] PHP：读取环境变量
来源：http://rmd.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://zda.316326.xyz

[U75] PHP：依赖注入
来源：http://ost.ybcxt.top

composer require psr/container
来源：http://lid.pycfn.com

[U76] PHP：简单路由
来源：http://zhu.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ypb.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://enr.jinqigufen.top

composer require twig/twig
来源：http://ovc.hcnkem.com

[U78] PHP：单元测试
来源：http://hmx.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://ljx.nanxinkj.top

[U79] PHP：静态分析
来源：http://wyf.shzxlz.cn

composer require --dev phpstan/phpstan
来源：http://qqe.9152youxi.cn

[U80] PHP：代码规范修复
来源：http://lms.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qma.zhixingplan.top

[U81] JS：初始化项目
来源：http://lcx.bbcook.cn

npm init -y;  npm i express
来源：http://vmg.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://qnd.guannengcc.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://set.yvedp.cn

[U83] JS：ES Module 导入导出
来源：http://vmk.xinyue.icu

export const a = 1;  import { a } from "./m.js";
来源：http://pxu.316326.xyz

[U84] JS：CommonJS 写法
来源：http://zsg.9152youxi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tzl.tian-w.cn

[U85] JS：可选链
来源：http://sig.zhijiandao.cn

a?.b?.c
来源：http://hcp.yangfankeji.com

[U86] JS：空值合并
来源：http://xiy.zhiwuduotai.top

a ?? b
来源：http://nzp.fengsongda.top

[U87] JS：解构默认值
来源：http://zms.hammf.cn

const { a = 1, b = 2 } = obj;
来源：http://dzs.sysykeji.top

[U88] JS：对象展开合并
来源：http://hqs.xuanzx.com

{ ...a, ...b }
来源：http://rtc.sweek.top

[U89] JS：数组去重
来源：http://qbb.zhongyouzk.top

[...new Set(arr)]
来源：http://xhj.sjlbkw.cn

[U90] JS：数字数组排序
来源：http://pgs.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://udt.aizwys.cn

[U91] JS：对象键值遍历
来源：http://dle.birdmap.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lty.hesvh.cn

[U92] JS：深拷贝
来源：http://xex.gzhubu.top

structuredClone(obj)
来源：http://rld.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://yxk.hywenlv.cn

`共 ${n} 条`
来源：http://akh.ydjk.org.cn

[U94] JS：箭头函数
来源：http://sxn.0kj1m.cn

const double = x => x * 2;
来源：http://jtg.cucudq.cn

[U95] JS：Promise 包装
来源：http://crh.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://sid.fzhhl.top

[U96] JS：async/await 与异常
来源：http://tym.zhijiandao.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lsi.sysykeji.top

[U97] JS：并发请求
来源：http://jkv.hfpthk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tdi.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://dqf.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fit.zdqjudy.top

[U99] JS：事件监听
来源：http://gzh.gogol.net.cn

el.addEventListener("click", e => {})
来源：http://mvk.fktsv.cn

[U100] JS：DOM 查询
来源：http://wnf.zhongyouzk.top

document.querySelector(".item")
来源：http://xwb.hysaishi.cn

[U101] JS：classList 操作
来源：http://sqq.zdqjudy.top

el.classList.toggle("active")
来源：http://lrb.yueranfly.top

[U102] JS：本地存储
来源：http://ntd.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://grl.wangshuangyany.cn

[U103] JS：定时器
来源：http://xko.wangdashe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://czr.tianlin.xyz

[U104] JS：防抖
来源：http://lox.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nxe.shangyingyoupin.top

[U105] JS：节流
来源：http://nmi.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rlj.sweek.top

[U106] JS：日期格式化
来源：http://oaq.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nck.fengsongda.top

[U107] JS：数字千分位
来源：http://vbo.daxiang520.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lps.svipenyu.cn

[U108] JS：随机整数
来源：http://ylc.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://htf.yfazqb.com

[U109] JS：数组分组
来源：http://wfj.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://uhe.yangfankeji.com

[U110] JS：数组分块
来源：http://wsp.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iww.ybcxt.top

[U111] JS：对象转 Map
来源：http://hrg.epnwcf.com

new Map(Object.entries(obj))
来源：http://llv.nanxinkj.top

[U112] JS：字符串补位
来源：http://ott.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://fuk.snrcjt.cn

[U113] JS：正则替换全部
来源：http://mqm.dianchejie.cn

s.replaceAll("a", "b")
来源：http://bkh.52xcode.cn

[U114] JS：JSON 深比较
来源：http://gtk.wangdashe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://izz.bbcook.cn

[U115] JS：生成 UUID
来源：http://oht.tarul.cn

crypto.randomUUID()
来源：http://evp.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://pey.jqgfzy.top

/** @param {string} name */ function f(name) {}
来源：http://qgt.snrcjt.cn

[U117] JS：单元测试
来源：http://ruq.cheryme.top

npm i -D vitest;  npx vitest
来源：http://kef.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://lmp.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://rkv.guannengcc.top

[U119] JS：生产构建
来源：http://wxr.yuxming.cn

npx vite build
来源：http://ekv.ctjpmb.com

[U120] JS：读取环境变量（Vite）
来源：http://pxq.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://ags.yonumen.top

================================================================================
来源：http://nty.sxryk.cn

统计汇总
来源：http://kcm.hnqzz.top

================================================================================
来源：http://plq.aizwys.cn

按语言统计（条）：
来源：http://lny.yongpay.top

Python ......... 252
来源：http://mtm.hcnkem.com

PHP ............ 252
来源：http://clb.yuanzhike.top

JavaScript ..... 252
来源：http://aav.ydjk.org.cn

TypeScript ..... 212
来源：http://kiy.iojbl.cn

Java ........... 212
来源：http://zys.zhongyouzk.top

Go ............. 212
来源：http://aro.tanke756.top

Ruby ........... 212
来源：http://zms.yvedp.cn

C# ............. 212
来源：http://toj.tanke756.top

C .............. 30
来源：http://fym.fktsv.cn

C++ ............ 30
来源：http://xpk.yangfankeji.com

SQL ............ 90
来源：http://wda.zhaomingkeji.xyz

Bash ........... 80
来源：http://vhx.daxiang520.top

Kotlin ......... 15
来源：http://ecw.meibo888.top

Swift .......... 15
来源：http://phs.yuxming.cn

Lua ............ 10
来源：http://qrs.zhiwuduotai.top

Perl ........... 10
来源：http://jyl.svipenyu.cn

Scala .......... 10
来源：http://awm.shuidangran.top

------------------------------------
来源：http://ykp.nanxinkj.top

合计 ........... 2106 条
来源：http://wgm.quarkkingdee.top

按章节统计：
来源：http://enk.mhx1999.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://phi.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uzw.dianchejie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lox.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nir.nwbrower.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dty.havefunace.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tsz.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wvw.wangshuangyany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ova.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dtb.hnxiangtu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ped.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lnt.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jsj.shuidangran.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://axg.epnwcf.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rje.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fct.hammf.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://umi.ivvv.top

Q SQL 专题                              90
来源：http://wfo.mhx1999.top

R Bash 专题                             80
来源：http://igk.hcnkem.com

S C / C++ 专题                          60
来源：http://hip.jyoumei.cn

T 其他语言补充                          60
来源：http://sst.smart0.xyz

U 高频实用片段                         120
来源：http://jzb.wangshuangyany.cn

------------------------------------
来源：http://vxu.cucudq.cn

合计                                  2106 条
来源：http://sbv.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://sla.chenzaomai.com

使用提醒
来源：http://ufk.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://gpu.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pwl.yj20258.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jhe.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cvx.xylfe.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wcb.yj20258888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cke.tian-w.cn

—— 文件结束 ——
来源：http://nfj.zdqjudy.top

================================================================================
来源：http://iuw.aibaodan.cn

程序语言常见例子速查手册（2024 版）
来源：http://fdh.zhijiandao.cn

Common Programming Examples Cheat Book
来源：http://ysr.wangdashe.top

================================================================================
来源：http://reu.yvedp.cn

【收录内容】
来源：http://quq.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kre.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ufc.xziqi.cn

SQL · Bash · C · C++
来源：http://ama.zdbjq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ild.chenjidiqi.icu

【使用说明】
来源：http://olv.kuanghao11.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mfz.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hyp.fktsv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vmo.chenjidiqi.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pus.smart0.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://qgi.hesvh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sno.ywan-chungtsiang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cbb.yuxming.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zaw.fengsongda.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fod.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jpi.yj202588.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://agu.yj202588.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yeu.meibo888.top

【文件统计】
来源：http://trp.daxiang520.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ugd.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://hxz.chenjidiqi.icu

目  录
来源：http://igm.yfazqb.com

--------------------------------------------------------------------------------
来源：http://ypa.ybcxt.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zkg.epnwcf.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://awn.bjfxy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://edc.yj202588.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wdg.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jgr.chenzaomai.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qqq.zhoulong.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uhe.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ebg.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rkg.zhaomingkeji.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ejc.yuanzhike.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aco.sjlbkw.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kww.zycfv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sye.yj20258888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://meg.ybcxt.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zuf.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ysv.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hyx.zdqjudy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://efk.yj202588.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bnj.yangfankeji.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fnv.quarkkingdee.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gdn.feifeiyinyue.top

================================================================================
来源：http://gwt.ivvv.top

A. 基础语法与类型
来源：http://oqq.ydjk.org.cn

================================================================================
来源：http://vhn.jinqigfzy.top

[A01] Hello World
来源：http://rqv.chenlongwang.top

Py:   print("Hello, World!")
来源：http://xvk.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://mou.fanxiaobao.xyz

JS:   console.log("Hello, World!");
来源：http://nbg.cdnleiting.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nbb.xinyue.icu

Java: System.out.println("Hello, World!");
来源：http://zrb.zdqjudy.top

Go:   fmt.Println("Hello, World!")
来源：http://sfd.nanxuanxn.top

Ruby: puts "Hello, World!"
来源：http://tkq.nwbrower.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tny.cheryme.top

[A02] 变量声明与赋值
来源：http://zex.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kmc.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://krb.hongshengwenyu.top

JS:   let name = "Alex"; const age = 20;
来源：http://ddr.xingfuxueyuan.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://euk.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://ilx.jinghuilouyu.cn

Go:   name := "Alex"; age := 20
来源：http://qji.hfpthk.cn

Ruby: name = "Alex"; age = 20
来源：http://dow.fktsv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vfz.zhoulong.xyz

[A03] 常量定义
来源：http://sjv.bjfxy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hcs.9152youxi.cn

PHP:  const PI = 3.14159;
来源：http://kjn.zhengqikj.top

JS:   const PI = 3.14159;
来源：http://dml.sysykeji.top

TS:   const PI: number = 3.14159;
来源：http://ufq.fzhhl.top

Java: static final double PI = 3.14159;
来源：http://dxt.ivvv.top

Go:   const PI = 3.14159
来源：http://tuk.jqgfzy.top

Ruby: PI = 3.14159
来源：http://kda.xingfuxueyuan.xyz

C#:   const double PI = 3.14159;
来源：http://zqm.jqgfzy.top

[A04] 判断变量类型
来源：http://iuz.dianchejie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hdb.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nmy.pengpengdd.cyou

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wbd.cdnleiting.top

TS:   typeof x; x instanceof Date
来源：http://vrw.316326.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sqj.52xcode.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fnx.ywan-chungtsiang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wdr.ivvv.top

C#:   x.GetType().Name; x is int
来源：http://tdk.dashuyun.cn

[A05] 整数除法与取模
来源：http://pce.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nlx.zhongyouzk.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://cqq.xuanzx.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dop.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dme.xziqi.cn

Java: 7 / 2; 7 % 2
来源：http://bfi.hesvh.cn

Go:   7 / 2; 7 % 2
来源：http://cik.bjfxy.top

Ruby: 7 / 2; 7 % 2
来源：http://yvb.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://krg.hongshengwenyu.top

[A06] 字符串转数字
来源：http://opm.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://bjl.yj20258888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mnx.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tri.ywan-chungtsiang.top

TS:   parseInt("42", 10); Number("42")
来源：http://mqm.chenlongwang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pwo.c1oappe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qgf.ydzc1.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ppv.bbcook.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qqq.ivvv.top

[A07] 数字转字符串
来源：http://sxb.chenlongwang.top

Py:   str(42)
来源：http://gsf.hnxiangtu.top

PHP:  (string) 42; strval(42)
来源：http://fvx.shzxlz.cn

JS:   String(42); (42).toString()
来源：http://gpe.pycfn.com

TS:   String(42)
来源：http://tgm.shangyingyoupin.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://sdn.0kj1m.cn

Go:   strconv.Itoa(42)
来源：http://lva.jqgfzy.top

Ruby: 42.to_s
来源：http://obg.hnxiangtu.top

C#:   42.ToString()
来源：http://jxq.hnqzz.top

[A08] 取整与四舍五入
来源：http://tee.ydzc1.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ldr.yvedp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ufx.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vew.nanxuanxn.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gun.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://owg.pengpengdd.cyou

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://paq.yonumen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ddq.fehbvm.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zvi.ivvv.top

[A09] 绝对值与最大最小值
来源：http://ucz.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jur.yongpay.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sbl.ctjpmb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qsg.feifeiyinyue.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eji.pengpengdd.cyou

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lvn.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jyw.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iqj.xylfe.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zuw.fengsongda.top


<!-- 参考信息 -->