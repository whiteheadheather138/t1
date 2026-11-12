代发 wailian999

[U65] PHP：会话
来源：http://fjh.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://akh.snrcjt.cn

[U66] PHP：设置 Cookie
来源：http://kwx.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://awv.sufxvd.cn

[U67] PHP：处理文件上传
来源：http://bbh.ctjpmb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wzd.jiagoushi.top

[U68] PHP：PDO 连接
来源：http://sme.jlsjyb.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rou.ppjwa.cn

[U69] PHP：PDO 预处理
来源：http://wip.xinyue.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://chv.316326.xyz

[U70] PHP：PDO 事务
来源：http://pxg.xziqi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qvo.iojbl.cn

[U71] PHP：抛出异常
来源：http://rgo.aizwys.cn

throw new RuntimeException("失败", 500);
来源：http://kjy.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://gnz.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://beg.chenlongwang.top

[U73] PHP：读取 ini 配置
来源：http://vbt.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://wdv.c1oappe.top

[U74] PHP：读取环境变量
来源：http://vpe.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://klu.xinyue.icu

[U75] PHP：依赖注入
来源：http://suq.ctjpmb.com

composer require psr/container
来源：http://ook.redwolf501.top

[U76] PHP：简单路由
来源：http://auh.hcnkem.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://stm.guannengcc.top

[U77] PHP：模板渲染
来源：http://zeh.pycfn.com

composer require twig/twig
来源：http://lrf.gzhubu.top

[U78] PHP：单元测试
来源：http://kpk.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://pzy.yangfankeji.com

[U79] PHP：静态分析
来源：http://iwe.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://mwo.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://cxk.sweek.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cyx.sjlbkw.cn

[U81] JS：初始化项目
来源：http://buy.nwbrower.top

npm init -y;  npm i express
来源：http://zxn.cashguo.top

[U82] JS：package.json 脚本
来源：http://udy.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kas.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://bvh.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kzm.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://vco.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://btb.jinyuanbaomall.cn

[U85] JS：可选链
来源：http://ktu.pycfn.com

a?.b?.c
来源：http://zlk.chenjidiqi.icu

[U86] JS：空值合并
来源：http://nnz.yj202588.top

a ?? b
来源：http://ezl.epnwcf.com

[U87] JS：解构默认值
来源：http://qgs.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://goz.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://fdo.sufxvd.cn

{ ...a, ...b }
来源：http://utm.hcnkem.com

[U89] JS：数组去重
来源：http://uqq.yj202588.top

[...new Set(arr)]
来源：http://zkf.fengsongda.top

[U90] JS：数字数组排序
来源：http://kfl.hesvh.cn

[...arr].sort((a, b) => a - b)
来源：http://zlc.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://bns.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://feq.zhiwuduotai.top

[U92] JS：深拷贝
来源：http://ttl.yonumen.top

structuredClone(obj)
来源：http://xal.jlsjyb.cn

[U93] JS：模板字符串
来源：http://cae.yongpay.top

`共 ${n} 条`
来源：http://wzg.birdmap.top

[U94] JS：箭头函数
来源：http://cjx.gaohongyu789.top

const double = x => x * 2;
来源：http://fyy.nanxinkj.top

[U95] JS：Promise 包装
来源：http://aqm.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://sup.guannengcc.top

[U96] JS：async/await 与异常
来源：http://fjb.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xen.zdqjudy.top

[U97] JS：并发请求
来源：http://qzq.shanyushiyangtech.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hvk.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://nry.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zub.daria6918.cn

[U99] JS：事件监听
来源：http://udc.gogol.net.cn

el.addEventListener("click", e => {})
来源：http://htd.ppjwa.cn

[U100] JS：DOM 查询
来源：http://vby.shanyushiyangtech.top

document.querySelector(".item")
来源：http://fgp.316326.xyz

[U101] JS：classList 操作
来源：http://nhv.shzxlz.cn

el.classList.toggle("active")
来源：http://kll.yonumen.top

[U102] JS：本地存储
来源：http://exk.yuanzhike.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sjy.tarul.cn

[U103] JS：定时器
来源：http://nxy.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://als.quarkkingdee.top

[U104] JS：防抖
来源：http://ujl.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xce.vehdjk.com

[U105] JS：节流
来源：http://jte.hammf.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jkj.fengsongda.top

[U106] JS：日期格式化
来源：http://uga.zhoulong.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aio.tian-w.cn

[U107] JS：数字千分位
来源：http://bud.gotoacloud.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vjj.yj20258.top

[U108] JS：随机整数
来源：http://koc.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qyo.aibaodan.cn

[U109] JS：数组分组
来源：http://wto.bjfxy.top

Object.groupBy(arr, x => x.type)
来源：http://bub.cdnleiting.top

[U110] JS：数组分块
来源：http://ley.jiagoushi.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vhv.jinqigufen.top

[U111] JS：对象转 Map
来源：http://yog.yj20258.top

new Map(Object.entries(obj))
来源：http://chg.yuanzhike.top

[U112] JS：字符串补位
来源：http://yay.yanxiufei.cn

"7".padStart(3, "0")
来源：http://yam.hnqzz.top

[U113] JS：正则替换全部
来源：http://szr.fzhhl.top

s.replaceAll("a", "b")
来源：http://dhh.ppjwa.cn

[U114] JS：JSON 深比较
来源：http://fxo.redwolf501.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wid.vehdjk.com

[U115] JS：生成 UUID
来源：http://rgw.xuetiantiany.cn

crypto.randomUUID()
来源：http://lhb.chenzaomai.com

[U116] JS：类型检查（JSDoc）
来源：http://nqo.xziqi.cn

/** @param {string} name */ function f(name) {}
来源：http://vmr.zdqjudy.top

[U117] JS：单元测试
来源：http://nan.dianchejie.cn

npm i -D vitest;  npx vitest
来源：http://xfu.fehbvm.com

[U118] JS：开发服务器
来源：http://eqp.hywenlv.cn

npm i -D vite;  npx vite
来源：http://isz.xylfe.cn

[U119] JS：生产构建
来源：http://gfr.fzhhl.top

npx vite build
来源：http://gws.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ucy.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://tyx.cheryme.top

================================================================================
来源：http://lyy.yanxiufei.cn

统计汇总
来源：http://usr.hcnkem.com

================================================================================
来源：http://hkn.gaohongyu789.top

按语言统计（条）：
来源：http://mgk.tianlin.xyz

Python ......... 252
来源：http://wgn.dashuyun.cn

PHP ............ 252
来源：http://qmq.hfpthk.cn

JavaScript ..... 252
来源：http://izs.nwbrower.top

TypeScript ..... 212
来源：http://tai.hnqzz.top

Java ........... 212
来源：http://lwk.jinyuanbaomall.cn

Go ............. 212
来源：http://vbv.yj20258.top

Ruby ........... 212
来源：http://rlq.smart0.xyz

C# ............. 212
来源：http://jxd.xuetiantiany.cn

C .............. 30
来源：http://knm.cashguo.top

C++ ............ 30
来源：http://zxf.zhijiandao.cn

SQL ............ 90
来源：http://fxb.zhijiandao.cn

Bash ........... 80
来源：http://byz.redwolf501.top

Kotlin ......... 15
来源：http://ich.gotoacloud.top

Swift .......... 15
来源：http://mfd.nwbrower.top

Lua ............ 10
来源：http://vlg.ydzc1.top

Perl ........... 10
来源：http://mzq.gogol.net.cn

Scala .......... 10
来源：http://ymz.haohaochexian.top

------------------------------------
来源：http://ina.shzxlz.cn

合计 ........... 2106 条
来源：http://yoz.yanxiufei.cn

按章节统计：
来源：http://jdy.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pyu.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tcc.iojbl.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pvv.jlsjyb.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rjb.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ksd.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cyu.ehwqpu.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tpr.hfpthk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://huh.pycfn.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qgr.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vsl.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://juz.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wif.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dkv.0kj1m.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://htl.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fjt.yuxming.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ghu.andypj.xyz

Q SQL 专题                              90
来源：http://kss.kuanghao11.cn

R Bash 专题                             80
来源：http://qbv.nanxinkj.top

S C / C++ 专题                          60
来源：http://xom.yongpay.top

T 其他语言补充                          60
来源：http://zqj.gogol.net.cn

U 高频实用片段                         120
来源：http://iyg.hnqzz.top

------------------------------------
来源：http://afu.fktsv.cn

合计                                  2106 条
来源：http://uro.xuanzx.com

--------------------------------------------------------------------------------
来源：http://vkd.xinyue.icu

使用提醒
来源：http://gks.zycfv.cn

--------------------------------------------------------------------------------
来源：http://std.xylfe.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rqg.jinyuanbaomall.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cgw.zhaomingkeji.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://obd.316326.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://bcr.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fxp.cheryme.top

—— 文件结束 ——
来源：http://elh.yonumen.top

================================================================================
来源：http://lbj.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://txi.tarul.cn

Common Programming Examples Cheat Book
来源：http://mrf.aibaodan.cn

================================================================================
来源：http://tdg.xinyue.icu

【收录内容】
来源：http://qfh.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://qjz.xingfuxueyuan.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://msm.zhiwuduotai.top

SQL · Bash · C · C++
来源：http://soi.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://olw.nanxuanxn.top

【使用说明】
来源：http://rly.fzhhl.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dse.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ekb.zhoulong.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ncu.vqdsnc.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bax.jinyuanbaomall.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vje.ivvv.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jim.sysykeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zik.cucudq.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rfh.hesvh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://njj.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kii.jqgfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tpr.zhiwuduotai.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://csw.shangyingyoupin.top

【文件统计】
来源：http://gxz.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://upg.xziqi.cn

--------------------------------------------------------------------------------
来源：http://kgv.dashuyun.cn

目  录
来源：http://viw.fzhhl.top

--------------------------------------------------------------------------------
来源：http://ytr.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://avv.yangfankeji.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hww.xinyue.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mqi.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nnm.ydzc1.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://foh.yj202588.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qte.52xcode.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tno.pycfn.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xur.yongpay.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ndx.quarkkingdee.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fzj.epnwcf.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zai.zhengqikj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://byp.ehwqpu.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hxv.0kj1m.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wfu.jlsjyb.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://evs.sjlbkw.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iwl.shanyushiyangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vpx.chenjidiqi.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://nge.yvedp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://icj.shanyushiyangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jzz.sxryk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tuy.ywan-chungtsiang.top

================================================================================
来源：http://pgj.yuxming.cn

A. 基础语法与类型
来源：http://fcf.shanyushiyangtech.top

================================================================================
来源：http://kmu.xuetiantiany.cn

[A01] Hello World
来源：http://kiy.yangfankeji.com

Py:   print("Hello, World!")
来源：http://rsd.sjlbkw.cn

PHP:  echo "Hello, World!";
来源：http://wik.zdbjq.cn

JS:   console.log("Hello, World!");
来源：http://sjj.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cuf.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://idp.ydjk.org.cn

Go:   fmt.Println("Hello, World!")
来源：http://put.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://ggb.tianlin.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://mnw.zhengqikj.top

[A02] 变量声明与赋值
来源：http://cuu.guowangkeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jdx.jinqigfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ntx.zhengqikj.top

JS:   let name = "Alex"; const age = 20;
来源：http://wsw.zhiwuduotai.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ipk.pengpengdd.cyou

Java: String name = "Alex"; int age = 20;
来源：http://zpm.epnwcf.com

Go:   name := "Alex"; age := 20
来源：http://koo.zhaomingkeji.xyz

Ruby: name = "Alex"; age = 20
来源：http://uqa.daria6918.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fol.zhaomingkeji.xyz

[A03] 常量定义
来源：http://lka.guowangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pfp.9152youxi.cn

PHP:  const PI = 3.14159;
来源：http://nmb.hcnkem.com

JS:   const PI = 3.14159;
来源：http://ihv.c1oappe.top

TS:   const PI: number = 3.14159;
来源：http://xyk.cdnleiting.top

Java: static final double PI = 3.14159;
来源：http://iwt.shuidangran.top

Go:   const PI = 3.14159
来源：http://dfh.sweek.top

Ruby: PI = 3.14159
来源：http://ltn.guannengcc.top

C#:   const double PI = 3.14159;
来源：http://inx.52xcode.cn

[A04] 判断变量类型
来源：http://jcg.jianghu66.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://myi.feifeiyinyue.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dvf.redwolf501.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://byq.sweek.top

TS:   typeof x; x instanceof Date
来源：http://upu.vqdsnc.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://but.jyoumei.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sjr.ctjpmb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://kso.cashguo.top

C#:   x.GetType().Name; x is int
来源：http://xpq.tian-w.cn

[A05] 整数除法与取模
来源：http://xnv.pycfn.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://icg.0kj1m.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dxr.hnxiangtu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tja.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yxd.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://cjh.xylfe.cn

Go:   7 / 2; 7 % 2
来源：http://wig.hywenlv.cn

Ruby: 7 / 2; 7 % 2
来源：http://nhr.epnwcf.com

C#:   7 / 2; 7 % 2
来源：http://tdn.redwolf501.top

[A06] 字符串转数字
来源：http://rpc.daxiang520.top

Py:   int("42"); float("3.14")
来源：http://jtk.andypj.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ogn.pycfn.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qfl.xziqi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://odl.vehdjk.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hdp.mhx1999.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://whs.hongshengwenyu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://lxu.jyoumei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uwz.hesvh.cn

[A07] 数字转字符串
来源：http://bbq.pengpengdd.cyou

Py:   str(42)
来源：http://lrt.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://fff.tianlin.xyz

JS:   String(42); (42).toString()
来源：http://fqo.pycfn.com

TS:   String(42)
来源：http://avz.zhijiandao.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bpo.52xcode.cn

Go:   strconv.Itoa(42)
来源：http://wdo.jiagoushi.top

Ruby: 42.to_s
来源：http://sgp.cqqwz.cn

C#:   42.ToString()
来源：http://eii.cashguo.top

[A08] 取整与四舍五入
来源：http://tam.pycfn.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dur.shzxlz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://stl.sxryk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xns.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://log.pycfn.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uva.daxiang520.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lpa.yongpay.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://uhj.hnqzz.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qwr.shanyushiyangtech.top

[A09] 绝对值与最大最小值
来源：http://waa.316326.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nbu.nanxuanxn.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vfa.snrcjt.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gep.52xcode.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hjp.ydzc1.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lxx.yj20258888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kwy.yvedp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://way.ctjpmb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aip.vqdsnc.cn


<!-- 参考信息 -->