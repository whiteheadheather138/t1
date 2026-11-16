代发 wailian999

[U63] PHP：文件读写
来源：http://yuu.fengsongda.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wty.hammf.cn

[U64] PHP：目录遍历
来源：http://pwg.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://ldr.zhongyouzk.top

[U65] PHP：会话
来源：http://kbu.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yka.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://ale.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vpw.yfazqb.com

[U67] PHP：处理文件上传
来源：http://eta.iojbl.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://snh.chenjidiqi.icu

[U68] PHP：PDO 连接
来源：http://sfi.chenjidiqi.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jqc.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://ryb.hesvh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yiv.fengsongda.top

[U70] PHP：PDO 事务
来源：http://bsz.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ujx.birdmap.top

[U71] PHP：抛出异常
来源：http://buy.snrcjt.cn

throw new RuntimeException("失败", 500);
来源：http://eqk.guowangkeji.top

[U72] PHP：写错误日志
来源：http://czy.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://qem.yuxming.cn

[U73] PHP：读取 ini 配置
来源：http://ydx.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://srd.cheryme.top

[U74] PHP：读取环境变量
来源：http://qpe.daxiang520.top

getenv("APP_ENV") ?: "production"
来源：http://rwm.zycfv.cn

[U75] PHP：依赖注入
来源：http://nde.tanke756.top

composer require psr/container
来源：http://goa.svipenyu.cn

[U76] PHP：简单路由
来源：http://moq.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://urw.ydzc1.top

[U77] PHP：模板渲染
来源：http://nth.xuanzx.com

composer require twig/twig
来源：http://nut.zhiwuduotai.top

[U78] PHP：单元测试
来源：http://zge.gotoacloud.top

composer require --dev phpunit/phpunit
来源：http://bvq.dashuyun.cn

[U79] PHP：静态分析
来源：http://axh.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://fyk.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://ewy.cdnleiting.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qip.ehwqpu.com

[U81] JS：初始化项目
来源：http://wzr.yj202588.top

npm init -y;  npm i express
来源：http://cqv.yonumen.top

[U82] JS：package.json 脚本
来源：http://pdg.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lfw.andypj.xyz

[U83] JS：ES Module 导入导出
来源：http://unt.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://eri.zhiwuduotai.top

[U84] JS：CommonJS 写法
来源：http://adj.fanxiaobao.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://cey.hammf.cn

[U85] JS：可选链
来源：http://inn.xuetiantiany.cn

a?.b?.c
来源：http://atl.ppjwa.cn

[U86] JS：空值合并
来源：http://jdh.birdmap.top

a ?? b
来源：http://sle.hywenlv.cn

[U87] JS：解构默认值
来源：http://ckz.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://jff.zhixingplan.top

[U88] JS：对象展开合并
来源：http://mai.chenzaomai.com

{ ...a, ...b }
来源：http://loo.aizwys.cn

[U89] JS：数组去重
来源：http://mst.chenlongwang.top

[...new Set(arr)]
来源：http://jpx.yuanzhike.top

[U90] JS：数字数组排序
来源：http://rch.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://ihq.fehbvm.com

[U91] JS：对象键值遍历
来源：http://qeb.hongshengwenyu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vcm.hcnkem.com

[U92] JS：深拷贝
来源：http://yqk.gogol.net.cn

structuredClone(obj)
来源：http://uxm.xylfe.cn

[U93] JS：模板字符串
来源：http://dnp.chenjidiqi.icu

`共 ${n} 条`
来源：http://fzp.daria6918.cn

[U94] JS：箭头函数
来源：http://sib.cucudq.cn

const double = x => x * 2;
来源：http://quj.jqgfzy.top

[U95] JS：Promise 包装
来源：http://vhl.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://qfy.fengsongda.top

[U96] JS：async/await 与异常
来源：http://pbn.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://svd.kuanghao11.cn

[U97] JS：并发请求
来源：http://uvj.epnwcf.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ikq.xinyue.icu

[U98] JS：fetch 带 JSON
来源：http://zab.zycfv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jwk.yj20258.top

[U99] JS：事件监听
来源：http://lpx.fengsongda.top

el.addEventListener("click", e => {})
来源：http://xzr.hammf.cn

[U100] JS：DOM 查询
来源：http://fai.jinqigufen.top

document.querySelector(".item")
来源：http://ktn.guannengcc.top

[U101] JS：classList 操作
来源：http://hmg.andypj.xyz

el.classList.toggle("active")
来源：http://iaa.gaohongyu789.top

[U102] JS：本地存储
来源：http://atx.ybcxt.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://chk.zhiwuduotai.top

[U103] JS：定时器
来源：http://hez.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vnb.shuidangran.top

[U104] JS：防抖
来源：http://bcb.tian-w.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pxg.zhixingplan.top

[U105] JS：节流
来源：http://mcr.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tea.tarul.cn

[U106] JS：日期格式化
来源：http://qzj.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oox.aibaodan.cn

[U107] JS：数字千分位
来源：http://pgn.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lyz.guowangkeji.top

[U108] JS：随机整数
来源：http://otq.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eyy.shzxlz.cn

[U109] JS：数组分组
来源：http://luk.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://pxr.xylfe.cn

[U110] JS：数组分块
来源：http://puq.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dkd.jianghu66.top

[U111] JS：对象转 Map
来源：http://ego.fehbvm.com

new Map(Object.entries(obj))
来源：http://her.zdbjq.cn

[U112] JS：字符串补位
来源：http://ijk.yueranfly.top

"7".padStart(3, "0")
来源：http://onx.yj202588.top

[U113] JS：正则替换全部
来源：http://aml.yvedp.cn

s.replaceAll("a", "b")
来源：http://osv.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://ksb.yuanzhike.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://iut.chenjidiqi.icu

[U115] JS：生成 UUID
来源：http://qao.ctjpmb.com

crypto.randomUUID()
来源：http://fjk.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://ygo.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://asb.gotoacloud.top

[U117] JS：单元测试
来源：http://www.hnqzz.top

npm i -D vitest;  npx vitest
来源：http://ngj.gzhubu.top

[U118] JS：开发服务器
来源：http://gdx.yongpay.top

npm i -D vite;  npx vite
来源：http://bnu.tian-w.cn

[U119] JS：生产构建
来源：http://oju.yfazqb.com

npx vite build
来源：http://pqc.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://soj.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://lob.tian-w.cn

================================================================================
来源：http://cdg.tarul.cn

统计汇总
来源：http://hnd.0kj1m.cn

================================================================================
来源：http://orv.cucudq.cn

按语言统计（条）：
来源：http://gxo.sjlbkw.cn

Python ......... 252
来源：http://dby.meibo888.top

PHP ............ 252
来源：http://puo.gzhubu.top

JavaScript ..... 252
来源：http://alw.jianghu66.top

TypeScript ..... 212
来源：http://naf.aizwys.cn

Java ........... 212
来源：http://hzl.redwolf501.top

Go ............. 212
来源：http://fze.sweek.top

Ruby ........... 212
来源：http://tbu.hcnkem.com

C# ............. 212
来源：http://dqb.vehdjk.com

C .............. 30
来源：http://dmo.redwolf501.top

C++ ............ 30
来源：http://kxl.zhijiandao.cn

SQL ............ 90
来源：http://piw.yongpay.top

Bash ........... 80
来源：http://yac.pycfn.com

Kotlin ......... 15
来源：http://whx.fengsongda.top

Swift .......... 15
来源：http://qlv.gogol.net.cn

Lua ............ 10
来源：http://spp.cashguo.top

Perl ........... 10
来源：http://vmp.sxryk.cn

Scala .......... 10
来源：http://onu.sjlbkw.cn

------------------------------------
来源：http://bxc.jqgufenzy.top

合计 ........... 2106 条
来源：http://zwo.ywan-chungtsiang.top

按章节统计：
来源：http://rng.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://feb.fehbvm.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zkw.jqgufenzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fez.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ykr.iojbl.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qqa.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cxp.ppjwa.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kbs.zdbjq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ais.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nza.dianchejie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nsa.jqgufenzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jpu.hnqzz.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://swl.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bel.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oko.yuanzhike.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rye.zhixingplan.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://avl.yuanzhike.top

Q SQL 专题                              90
来源：http://tuy.yj202588.top

R Bash 专题                             80
来源：http://ncx.jianghu66.top

S C / C++ 专题                          60
来源：http://yef.guannengcc.top

T 其他语言补充                          60
来源：http://taq.tian-w.cn

U 高频实用片段                         120
来源：http://dby.sufxvd.cn

------------------------------------
来源：http://nou.ydjk.org.cn

合计                                  2106 条
来源：http://xyt.meibo888.top

--------------------------------------------------------------------------------
来源：http://tqc.dashuyun.cn

使用提醒
来源：http://kjf.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://ear.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xgr.nwbrower.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jxv.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oyp.smart0.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://mqu.dianchejie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uaq.ehwqpu.com

—— 文件结束 ——
来源：http://ecn.ybcxt.top

================================================================================
来源：http://tzk.xinyue.icu

程序语言常见例子速查手册（2024 版）
来源：http://rfu.jqgfzy.top

Common Programming Examples Cheat Book
来源：http://eac.chenjidiqi.icu

================================================================================
来源：http://iem.jqgfzy.top

【收录内容】
来源：http://rba.jinyuanbaomall.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wqu.epnwcf.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nek.fktsv.cn

SQL · Bash · C · C++
来源：http://ipz.fanxiaobao.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kht.tarul.cn

【使用说明】
来源：http://bgo.fanxiaobao.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bgp.wangshuangyany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://urv.shanyushiyangtech.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rvu.zdbjq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nxt.nanxinkj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tif.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lfc.yj20258888.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nmh.sysykeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hsh.yueranfly.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://twg.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nii.zdqjudy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yfa.fengsongda.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vtt.epnwcf.com

【文件统计】
来源：http://aqh.haohaochexian.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ukv.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://cer.ybcxt.top

目  录
来源：http://jat.hnqzz.top

--------------------------------------------------------------------------------
来源：http://ggo.sysykeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vdc.fengsongda.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oid.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mxq.yonumen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mpp.jqgufenzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ngj.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hga.birdmap.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mxi.gaohongyu789.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ixv.yj20258888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nlj.guannengcc.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fue.hongshengwenyu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xag.iojbl.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ksf.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pfq.quarkkingdee.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zmd.ydjk.org.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://frr.xylfe.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://otd.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mhl.ydzc1.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lhi.sjlbkw.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yul.cqqwz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vrz.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wdn.jianghu66.top

================================================================================
来源：http://geo.jqgufenzy.top

A. 基础语法与类型
来源：http://uma.ywan-chungtsiang.top

================================================================================
来源：http://rfu.yj20258.top

[A01] Hello World
来源：http://bnc.ivvv.top

Py:   print("Hello, World!")
来源：http://itz.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://glv.zhiwuduotai.top

JS:   console.log("Hello, World!");
来源：http://ngk.uphjek.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lyd.gzhubu.top

Java: System.out.println("Hello, World!");
来源：http://ibw.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://arm.tarul.cn

Ruby: puts "Hello, World!"
来源：http://voz.shanyushiyangtech.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cyq.hnqzz.top

[A02] 变量声明与赋值
来源：http://por.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cra.birdmap.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bsw.kuanghao11.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dwo.yj20258888.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sjl.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://vpm.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://clm.hesvh.cn

Ruby: name = "Alex"; age = 20
来源：http://wwg.sjlbkw.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ozn.ydjk.org.cn

[A03] 常量定义
来源：http://lci.yangfankeji.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mff.yj20258888.top

PHP:  const PI = 3.14159;
来源：http://hrx.jinyuanbaomall.cn

JS:   const PI = 3.14159;
来源：http://hpa.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://kcu.nwbrower.top

Java: static final double PI = 3.14159;
来源：http://nfa.yueranfly.top

Go:   const PI = 3.14159
来源：http://git.ywan-chungtsiang.top

Ruby: PI = 3.14159
来源：http://def.pycfn.com

C#:   const double PI = 3.14159;
来源：http://dhi.feifeiyinyue.top

[A04] 判断变量类型
来源：http://oul.wangshuangyany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://teg.zhiwuduotai.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rkh.hysaishi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yih.daxiang520.top

TS:   typeof x; x instanceof Date
来源：http://jfj.meibo888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mke.yfazqb.com

Go:   reflect.TypeOf(x).Name()
来源：http://gif.jianghu66.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ast.ywan-chungtsiang.top

C#:   x.GetType().Name; x is int
来源：http://wtk.nanxuanxn.top

[A05] 整数除法与取模
来源：http://gfz.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://itm.ctjpmb.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://pbq.yfazqb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jgp.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jad.jinghuilouyu.cn

Java: 7 / 2; 7 % 2
来源：http://qrm.9152youxi.cn

Go:   7 / 2; 7 % 2
来源：http://byy.xuetiantiany.cn

Ruby: 7 / 2; 7 % 2
来源：http://hwu.svipenyu.cn

C#:   7 / 2; 7 % 2
来源：http://aky.jinyuanbaomall.cn

[A06] 字符串转数字
来源：http://etj.fehbvm.com

Py:   int("42"); float("3.14")
来源：http://csq.yj20258888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pit.cucudq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://umy.andypj.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://yle.wangshuangyany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fgx.xuanzx.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sjx.chenlongwang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bog.xingfuxueyuan.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hxg.shuidangran.top

[A07] 数字转字符串
来源：http://rvt.nanxinkj.top

Py:   str(42)
来源：http://rod.bjfxy.top

PHP:  (string) 42; strval(42)
来源：http://cph.sxryk.cn

JS:   String(42); (42).toString()
来源：http://drz.jinqigufen.top

TS:   String(42)
来源：http://pht.zhaomingkeji.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://izw.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://fmc.sxryk.cn

Ruby: 42.to_s
来源：http://lmb.hysaishi.cn

C#:   42.ToString()
来源：http://cda.havefunace.top

[A08] 取整与四舍五入
来源：http://nzg.jinqigufen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wzc.yvedp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jja.sxryk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://can.haohaochexian.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qgz.ehwqpu.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rgn.smart0.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vcm.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://bwv.yongpay.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://toe.nanxinkj.top

[A09] 绝对值与最大最小值
来源：http://wkk.hnqzz.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eah.fktsv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gaj.yj20258.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lwa.guannengcc.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xak.mhx1999.top


<!-- 参考信息 -->