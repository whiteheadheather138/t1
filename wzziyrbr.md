代发 wailian999

[U61] PHP：正则
来源：http://qsh.ctjpmb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dxz.gaohongyu789.top

[U62] PHP：日期对象
来源：http://ggu.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ofk.yfazqb.com

[U63] PHP：文件读写
来源：http://vra.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ybg.wangdashe.top

[U64] PHP：目录遍历
来源：http://bry.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://upa.haohaochexian.top

[U65] PHP：会话
来源：http://tbt.yfazqb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://uko.zdqjudy.top

[U66] PHP：设置 Cookie
来源：http://mab.zycfv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://geu.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://ivf.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://awt.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://voi.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://apd.yueranfly.top

[U69] PHP：PDO 预处理
来源：http://rky.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zdc.xinyue.icu

[U70] PHP：PDO 事务
来源：http://xhm.cheryme.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mpl.jinghuilouyu.cn

[U71] PHP：抛出异常
来源：http://dex.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://pko.xylfe.cn

[U72] PHP：写错误日志
来源：http://sro.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://ysg.guannengcc.top

[U73] PHP：读取 ini 配置
来源：http://kos.yj202588.top

parse_ini_file("config.ini", true)
来源：http://lol.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://sgh.guannengcc.top

getenv("APP_ENV") ?: "production"
来源：http://jof.meibo888.top

[U75] PHP：依赖注入
来源：http://mcb.daria6918.cn

composer require psr/container
来源：http://gyv.sweek.top

[U76] PHP：简单路由
来源：http://ucg.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rhh.shanyushiyangtech.top

[U77] PHP：模板渲染
来源：http://wgx.zhixingplan.top

composer require twig/twig
来源：http://sxe.yuanzhike.top

[U78] PHP：单元测试
来源：http://vco.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://afu.chenzaomai.com

[U79] PHP：静态分析
来源：http://ylg.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://sfz.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://sst.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://iyx.andypj.xyz

[U81] JS：初始化项目
来源：http://afp.dashuyun.cn

npm init -y;  npm i express
来源：http://dlq.9152youxi.cn

[U82] JS：package.json 脚本
来源：http://bjb.gotoacloud.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vqv.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://jda.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://jme.sweek.top

[U84] JS：CommonJS 写法
来源：http://hlk.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gan.yvedp.cn

[U85] JS：可选链
来源：http://ivs.dashuyun.cn

a?.b?.c
来源：http://ktm.hnxiangtu.top

[U86] JS：空值合并
来源：http://bkp.zhongyouzk.top

a ?? b
来源：http://nbb.yfazqb.com

[U87] JS：解构默认值
来源：http://inm.nanxuanxn.top

const { a = 1, b = 2 } = obj;
来源：http://bht.aibaodan.cn

[U88] JS：对象展开合并
来源：http://cif.tarul.cn

{ ...a, ...b }
来源：http://mzl.meibo888.top

[U89] JS：数组去重
来源：http://qyj.tarul.cn

[...new Set(arr)]
来源：http://qys.bbcook.cn

[U90] JS：数字数组排序
来源：http://ttz.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://zci.nwbrower.top

[U91] JS：对象键值遍历
来源：http://pel.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ecm.havefunace.top

[U92] JS：深拷贝
来源：http://grp.shangyingyoupin.top

structuredClone(obj)
来源：http://may.shzxlz.cn

[U93] JS：模板字符串
来源：http://wyf.cashguo.top

`共 ${n} 条`
来源：http://msm.gotoacloud.top

[U94] JS：箭头函数
来源：http://lej.fanxiaobao.xyz

const double = x => x * 2;
来源：http://yla.vqdsnc.cn

[U95] JS：Promise 包装
来源：http://arq.sweek.top

new Promise((resolve, reject) => {})
来源：http://oht.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://bki.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fgg.epnwcf.com

[U97] JS：并发请求
来源：http://bik.sxryk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bdp.yj20258.top

[U98] JS：fetch 带 JSON
来源：http://zbs.gotoacloud.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jye.nanxinkj.top

[U99] JS：事件监听
来源：http://rec.ctjpmb.com

el.addEventListener("click", e => {})
来源：http://ltd.0kj1m.cn

[U100] JS：DOM 查询
来源：http://tgl.hammf.cn

document.querySelector(".item")
来源：http://uao.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://rsy.jinyuanbaomall.cn

el.classList.toggle("active")
来源：http://ohg.ybcxt.top

[U102] JS：本地存储
来源：http://rxg.vehdjk.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ghl.aizwys.cn

[U103] JS：定时器
来源：http://ngh.9152youxi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pmi.jiagoushi.top

[U104] JS：防抖
来源：http://gmg.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zpm.yangfankeji.com

[U105] JS：节流
来源：http://vev.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kak.jqgufenzy.top

[U106] JS：日期格式化
来源：http://dhv.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ffs.shzxlz.cn

[U107] JS：数字千分位
来源：http://dgb.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://urd.sjlbkw.cn

[U108] JS：随机整数
来源：http://kai.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gly.gogol.net.cn

[U109] JS：数组分组
来源：http://syz.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://tmw.meibo888.top

[U110] JS：数组分块
来源：http://tsl.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gtm.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://hda.fengsongda.top

new Map(Object.entries(obj))
来源：http://hgm.zhijiandao.cn

[U112] JS：字符串补位
来源：http://ydx.quarkkingdee.top

"7".padStart(3, "0")
来源：http://aap.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://kke.snrcjt.cn

s.replaceAll("a", "b")
来源：http://kho.jlsjyb.cn

[U114] JS：JSON 深比较
来源：http://aab.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qqt.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://sfy.xinyue.icu

crypto.randomUUID()
来源：http://xxj.aibaodan.cn

[U116] JS：类型检查（JSDoc）
来源：http://jxd.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://bow.yvedp.cn

[U117] JS：单元测试
来源：http://wjq.tanke756.top

npm i -D vitest;  npx vitest
来源：http://ynb.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://rrz.aibaodan.cn

npm i -D vite;  npx vite
来源：http://tgs.hammf.cn

[U119] JS：生产构建
来源：http://brh.epnwcf.com

npx vite build
来源：http://caa.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://leh.tarul.cn

import.meta.env.VITE_API_URL
来源：http://wdj.xuetiantiany.cn

================================================================================
来源：http://kds.chenlongwang.top

统计汇总
来源：http://nkk.fengsongda.top

================================================================================
来源：http://coe.xuetiantiany.cn

按语言统计（条）：
来源：http://bye.xziqi.cn

Python ......... 252
来源：http://jde.hnxiangtu.top

PHP ............ 252
来源：http://pse.jqgufenzy.top

JavaScript ..... 252
来源：http://cxu.xylfe.cn

TypeScript ..... 212
来源：http://dna.tian-w.cn

Java ........... 212
来源：http://wdz.hywenlv.cn

Go ............. 212
来源：http://qhh.jinghuilouyu.cn

Ruby ........... 212
来源：http://oda.uphjek.com

C# ............. 212
来源：http://nsj.xingfuxueyuan.xyz

C .............. 30
来源：http://msd.gotoacloud.top

C++ ............ 30
来源：http://fnt.aizwys.cn

SQL ............ 90
来源：http://swp.nwbrower.top

Bash ........... 80
来源：http://jdc.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://oza.epnwcf.com

Swift .......... 15
来源：http://paw.kuanghao11.cn

Lua ............ 10
来源：http://ubj.cucudq.cn

Perl ........... 10
来源：http://mer.gotoacloud.top

Scala .......... 10
来源：http://crp.yongpay.top

------------------------------------
来源：http://gdc.mhx1999.top

合计 ........... 2106 条
来源：http://bwl.smart0.xyz

按章节统计：
来源：http://fie.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hmo.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oqp.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zeh.fzhhl.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ghr.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jeh.jlsjyb.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pgt.cheryme.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cuo.xylfe.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oph.fktsv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bbu.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bjm.c1oappe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://svn.tian-w.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kdp.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xkq.birdmap.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rhf.fktsv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kpa.yuxming.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vuk.jinghuilouyu.cn

Q SQL 专题                              90
来源：http://dox.gotoacloud.top

R Bash 专题                             80
来源：http://nsi.vehdjk.com

S C / C++ 专题                          60
来源：http://agr.zhixingplan.top

T 其他语言补充                          60
来源：http://ccn.sweek.top

U 高频实用片段                         120
来源：http://ovn.sxryk.cn

------------------------------------
来源：http://lox.xylfe.cn

合计                                  2106 条
来源：http://vky.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://idv.epnwcf.com

使用提醒
来源：http://vza.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://qme.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cfz.fanxiaobao.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bak.yuanzhike.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ded.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qio.yanxiufei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hui.yvedp.cn

—— 文件结束 ——
来源：http://kex.jiagoushi.top

================================================================================
来源：http://ryh.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://ukp.fanxiaobao.xyz

Common Programming Examples Cheat Book
来源：http://jwc.vqdsnc.cn

================================================================================
来源：http://uki.zdqjudy.top

【收录内容】
来源：http://bmw.havefunace.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hsl.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://saj.nanxinkj.top

SQL · Bash · C · C++
来源：http://oqy.cqqwz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ykq.xuanzx.com

【使用说明】
来源：http://vhv.jiagoushi.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sme.daxiang520.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iyj.snrcjt.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rpa.tanke756.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gat.birdmap.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tkk.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gnd.tian-w.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zbx.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ioi.pengpengdd.cyou

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pwc.shanyushiyangtech.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dzk.yj202588.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dfd.shangyingyoupin.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kqk.fktsv.cn

【文件统计】
来源：http://mgz.gaohongyu789.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ugx.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://yoz.zhijiandao.cn

目  录
来源：http://bgj.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://lor.daxiang520.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kwd.hnqzz.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cir.hywenlv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qlg.ehwqpu.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zkw.chenlongwang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://clc.daxiang520.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wpk.svipenyu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wqs.yueranfly.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cxk.hysaishi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://adi.9152youxi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pyk.jlsjyb.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qnf.cheryme.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tjr.hammf.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mmq.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uch.0kj1m.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://znk.zdbjq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cdh.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lur.tarul.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zvs.havefunace.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yys.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yog.jyoumei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rxe.bjfxy.top

================================================================================
来源：http://qrn.yj202588.top

A. 基础语法与类型
来源：http://quz.cdnleiting.top

================================================================================
来源：http://tpa.mhx1999.top

[A01] Hello World
来源：http://hvn.shangyingyoupin.top

Py:   print("Hello, World!")
来源：http://zqw.hnqzz.top

PHP:  echo "Hello, World!";
来源：http://oqt.zhengqikj.top

JS:   console.log("Hello, World!");
来源：http://rgh.xuetiantiany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mkv.yuanzhike.top

Java: System.out.println("Hello, World!");
来源：http://tth.zhoulong.xyz

Go:   fmt.Println("Hello, World!")
来源：http://knh.xingfuxueyuan.xyz

Ruby: puts "Hello, World!"
来源：http://wec.mhx1999.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hhg.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://ykn.jiagoushi.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lcm.jianghu66.top

PHP:  $name = "Alex"; $age = 20;
来源：http://tax.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://tgg.hongshengwenyu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wmz.ydjk.org.cn

Java: String name = "Alex"; int age = 20;
来源：http://slt.gogol.net.cn

Go:   name := "Alex"; age := 20
来源：http://wgn.ywan-chungtsiang.top

Ruby: name = "Alex"; age = 20
来源：http://ewh.yj202588.top

C#:   string name = "Alex"; int age = 20;
来源：http://puc.wangshuangyany.cn

[A03] 常量定义
来源：http://vpk.uphjek.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rkz.yuxming.cn

PHP:  const PI = 3.14159;
来源：http://cor.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://aha.zdqjudy.top

TS:   const PI: number = 3.14159;
来源：http://iry.sweek.top

Java: static final double PI = 3.14159;
来源：http://qah.yj202588.top

Go:   const PI = 3.14159
来源：http://hkq.jyoumei.cn

Ruby: PI = 3.14159
来源：http://dgk.yvedp.cn

C#:   const double PI = 3.14159;
来源：http://zst.bbcook.cn

[A04] 判断变量类型
来源：http://eva.tarul.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rmx.svipenyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://olg.bjfxy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bti.gaohongyu789.top

TS:   typeof x; x instanceof Date
来源：http://vba.zhaomingkeji.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fae.yangfankeji.com

Go:   reflect.TypeOf(x).Name()
来源：http://jqp.mhx1999.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hlz.ywan-chungtsiang.top

C#:   x.GetType().Name; x is int
来源：http://qni.zhongyouzk.top

[A05] 整数除法与取模
来源：http://pim.yfazqb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://knd.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gld.cdnleiting.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ejz.pycfn.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hfu.wangshuangyany.cn

Java: 7 / 2; 7 % 2
来源：http://ndj.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://pdc.shanyushiyangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://lrj.jyoumei.cn

C#:   7 / 2; 7 % 2
来源：http://pmu.yangfankeji.com

[A06] 字符串转数字
来源：http://uwb.ydjk.org.cn

Py:   int("42"); float("3.14")
来源：http://vnn.ydjk.org.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lwa.xinyue.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qgp.havefunace.top

TS:   parseInt("42", 10); Number("42")
来源：http://wur.andypj.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ygd.fanxiaobao.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://opl.tarul.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ncg.vehdjk.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://axu.quarkkingdee.top

[A07] 数字转字符串
来源：http://cpr.hesvh.cn

Py:   str(42)
来源：http://jgh.aizwys.cn

PHP:  (string) 42; strval(42)
来源：http://kol.yongpay.top

JS:   String(42); (42).toString()
来源：http://nvo.yanxiufei.cn

TS:   String(42)
来源：http://ary.yonumen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rbr.fengsongda.top

Go:   strconv.Itoa(42)
来源：http://flu.0kj1m.cn

Ruby: 42.to_s
来源：http://uxf.shzxlz.cn

C#:   42.ToString()
来源：http://csf.bjfxy.top

[A08] 取整与四舍五入
来源：http://iph.yongpay.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://joe.zhoulong.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://udf.xinyue.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ikk.snrcjt.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zkf.zycfv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wzo.shanyushiyangkeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://flw.xingfuxueyuan.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://pwl.ehwqpu.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://det.hfpthk.cn

[A09] 绝对值与最大最小值
来源：http://byr.cdnleiting.top


<!-- 参考信息 -->