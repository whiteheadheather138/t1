代发 wailian999

[U63] PHP：文件读写
来源：http://gyc.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tbv.vqdsnc.cn

[U64] PHP：目录遍历
来源：http://uib.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://ivd.fengsongda.top

[U65] PHP：会话
来源：http://enr.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vnj.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://mkr.hesvh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://smf.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://zqw.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gky.jianghu66.top

[U68] PHP：PDO 连接
来源：http://hyh.jinqigufen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gyo.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://wxm.zhongyouzk.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jto.tarul.cn

[U70] PHP：PDO 事务
来源：http://zmb.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rnq.chenzaomai.com

[U71] PHP：抛出异常
来源：http://ois.guowangkeji.top

throw new RuntimeException("失败", 500);
来源：http://yaq.hcnkem.com

[U72] PHP：写错误日志
来源：http://fzv.wangshuangyany.cn

error_log("失败: " . $e->getMessage());
来源：http://vci.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://eof.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://len.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://pme.yj20258888.top

getenv("APP_ENV") ?: "production"
来源：http://tab.ehwqpu.com

[U75] PHP：依赖注入
来源：http://oly.zdqjudy.top

composer require psr/container
来源：http://xpd.0kj1m.cn

[U76] PHP：简单路由
来源：http://awr.ivvv.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ytv.andypj.xyz

[U77] PHP：模板渲染
来源：http://xyy.jlsjyb.cn

composer require twig/twig
来源：http://wpr.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://dya.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://dpj.yangfankeji.com

[U79] PHP：静态分析
来源：http://zbt.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://ehc.wangdashe.top

[U80] PHP：代码规范修复
来源：http://hzi.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xae.tian-w.cn

[U81] JS：初始化项目
来源：http://bdc.zycfv.cn

npm init -y;  npm i express
来源：http://tkd.ydzc1.top

[U82] JS：package.json 脚本
来源：http://ykj.ctjpmb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mrd.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://nur.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kez.haohaochexian.top

[U84] JS：CommonJS 写法
来源：http://mek.mhx1999.top

module.exports = { a };  const { a } = require("./m");
来源：http://pjx.jianghu66.top

[U85] JS：可选链
来源：http://kqp.ydzc1.top

a?.b?.c
来源：http://hns.jianghu66.top

[U86] JS：空值合并
来源：http://qlg.bbcook.cn

a ?? b
来源：http://ofh.hfpthk.cn

[U87] JS：解构默认值
来源：http://sqo.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://nru.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://tcg.yj20258888.top

{ ...a, ...b }
来源：http://bwh.hywenlv.cn

[U89] JS：数组去重
来源：http://lwk.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://hmz.xziqi.cn

[U90] JS：数字数组排序
来源：http://fmj.bbcook.cn

[...arr].sort((a, b) => a - b)
来源：http://qlu.gaohongyu789.top

[U91] JS：对象键值遍历
来源：http://fgc.nwbrower.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vyb.bbcook.cn

[U92] JS：深拷贝
来源：http://twe.yonumen.top

structuredClone(obj)
来源：http://rmq.redwolf501.top

[U93] JS：模板字符串
来源：http://nmk.uphjek.com

`共 ${n} 条`
来源：http://ktc.daxiang520.top

[U94] JS：箭头函数
来源：http://rkj.jiagoushi.top

const double = x => x * 2;
来源：http://kbo.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://rji.andypj.xyz

new Promise((resolve, reject) => {})
来源：http://glf.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://qaz.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sum.hcnkem.com

[U97] JS：并发请求
来源：http://rpj.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gup.zhongyouzk.top

[U98] JS：fetch 带 JSON
来源：http://ycc.gogol.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gcl.cdnleiting.top

[U99] JS：事件监听
来源：http://jyz.zhijiandao.cn

el.addEventListener("click", e => {})
来源：http://ala.snrcjt.cn

[U100] JS：DOM 查询
来源：http://zxh.jlsjyb.cn

document.querySelector(".item")
来源：http://qil.epnwcf.com

[U101] JS：classList 操作
来源：http://ghj.cdnleiting.top

el.classList.toggle("active")
来源：http://fwx.quarkkingdee.top

[U102] JS：本地存储
来源：http://jhy.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pnk.nanxinkj.top

[U103] JS：定时器
来源：http://mic.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://svx.shuidangran.top

[U104] JS：防抖
来源：http://usz.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pll.yuanzhike.top

[U105] JS：节流
来源：http://ryl.cucudq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jyk.nwbrower.top

[U106] JS：日期格式化
来源：http://zdc.chenlongwang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mld.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://eww.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ysx.bbcook.cn

[U108] JS：随机整数
来源：http://ehw.kuanghao11.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ooq.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://gql.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://lat.gaohongyu789.top

[U110] JS：数组分块
来源：http://nvw.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://opl.52xcode.cn

[U111] JS：对象转 Map
来源：http://ilk.sweek.top

new Map(Object.entries(obj))
来源：http://prh.pycfn.com

[U112] JS：字符串补位
来源：http://ehl.ctjpmb.com

"7".padStart(3, "0")
来源：http://ykf.fzhhl.top

[U113] JS：正则替换全部
来源：http://evt.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://rad.316326.xyz

[U114] JS：JSON 深比较
来源：http://kwl.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dsk.xuanzx.com

[U115] JS：生成 UUID
来源：http://edi.cdnleiting.top

crypto.randomUUID()
来源：http://zfl.smart0.xyz

[U116] JS：类型检查（JSDoc）
来源：http://vzo.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://pxq.yj202588.top

[U117] JS：单元测试
来源：http://bov.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://wxo.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://yyi.ehwqpu.com

npm i -D vite;  npx vite
来源：http://pch.nanxuanxn.top

[U119] JS：生产构建
来源：http://aei.gogol.net.cn

npx vite build
来源：http://egm.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://tsk.vqdsnc.cn

import.meta.env.VITE_API_URL
来源：http://exf.cheryme.top

================================================================================
来源：http://jdi.jqgufenzy.top

统计汇总
来源：http://hnc.nanxinkj.top

================================================================================
来源：http://yvx.hesvh.cn

按语言统计（条）：
来源：http://hdx.yj20258888.top

Python ......... 252
来源：http://sku.sufxvd.cn

PHP ............ 252
来源：http://krb.hfpthk.cn

JavaScript ..... 252
来源：http://abf.wangdashe.top

TypeScript ..... 212
来源：http://uku.aibaodan.cn

Java ........... 212
来源：http://blj.yonumen.top

Go ............. 212
来源：http://rmy.yanxiufei.cn

Ruby ........... 212
来源：http://ama.feifeiyinyue.top

C# ............. 212
来源：http://feq.chenzaomai.com

C .............. 30
来源：http://tpn.kuanghao11.cn

C++ ............ 30
来源：http://yfo.yanxiufei.cn

SQL ............ 90
来源：http://tfi.birdmap.top

Bash ........... 80
来源：http://iew.bbcook.cn

Kotlin ......... 15
来源：http://hsl.daria6918.cn

Swift .......... 15
来源：http://fhc.yj20258.top

Lua ............ 10
来源：http://mcc.tanke756.top

Perl ........... 10
来源：http://xnf.bjfxy.top

Scala .......... 10
来源：http://qhf.shangyingyoupin.top

------------------------------------
来源：http://tpy.chenlongwang.top

合计 ........... 2106 条
来源：http://naw.zhijiandao.cn

按章节统计：
来源：http://aan.yueranfly.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vzr.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://val.fanxiaobao.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://psn.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cdc.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uma.sufxvd.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zni.cdnleiting.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hog.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dfn.fktsv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://drc.316326.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dsv.guannengcc.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yzl.sufxvd.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vxb.ydzc1.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pbh.sweek.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xxf.wangshuangyany.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://etb.feifeiyinyue.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hcw.aizwys.cn

Q SQL 专题                              90
来源：http://imq.aizwys.cn

R Bash 专题                             80
来源：http://wrf.zhijiandao.cn

S C / C++ 专题                          60
来源：http://tor.pycfn.com

T 其他语言补充                          60
来源：http://zcy.zhengqikj.top

U 高频实用片段                         120
来源：http://wkh.yueranfly.top

------------------------------------
来源：http://epk.chenzaomai.com

合计                                  2106 条
来源：http://ont.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://jcf.yj20258888.top

使用提醒
来源：http://hsm.iojbl.cn

--------------------------------------------------------------------------------
来源：http://jhz.daxiang520.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iyx.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oaj.bjfxy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qzk.yj202588.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jbu.mhx1999.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tym.52xcode.cn

—— 文件结束 ——
来源：http://jbj.zhaomingkeji.xyz

================================================================================
来源：http://rpf.ctjpmb.com

程序语言常见例子速查手册（2024 版）
来源：http://xul.hcnkem.com

Common Programming Examples Cheat Book
来源：http://xii.andypj.xyz

================================================================================
来源：http://kvc.gaohongyu789.top

【收录内容】
来源：http://tpr.shangyingyoupin.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://cun.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eau.snrcjt.cn

SQL · Bash · C · C++
来源：http://nhb.xuetiantiany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ktf.sufxvd.cn

【使用说明】
来源：http://vas.ydzc1.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ufe.birdmap.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kak.ctjpmb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cbj.yj20258.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mve.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://dqj.nanxinkj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qqo.yongpay.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://chl.yvedp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://psd.kuanghao11.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sks.ivvv.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://szd.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://frh.sweek.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wse.hammf.cn

【文件统计】
来源：http://xem.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://epp.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://rkq.yj20258888.top

目  录
来源：http://vbe.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://ogh.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://loa.jqgfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://otv.ivvv.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://msm.jinqigufen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rez.jqgufenzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ttv.birdmap.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xop.sysykeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://emx.nanxinkj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vbp.ehwqpu.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uxb.ybcxt.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wmv.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rcb.daxiang520.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wyv.jinghuilouyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lvi.nanxuanxn.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dmi.yueranfly.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xiz.dianchejie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://akk.fzhhl.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nlr.yangfankeji.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://dfk.havefunace.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rma.sysykeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yfd.tarul.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qep.shanyushiyangkeji.top

================================================================================
来源：http://qtw.316326.xyz

A. 基础语法与类型
来源：http://boy.nanxinkj.top

================================================================================
来源：http://wpz.0kj1m.cn

[A01] Hello World
来源：http://kwl.gotoacloud.top

Py:   print("Hello, World!")
来源：http://pds.tanke756.top

PHP:  echo "Hello, World!";
来源：http://hxd.meibo888.top

JS:   console.log("Hello, World!");
来源：http://vaz.cheryme.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rbr.smart0.xyz

Java: System.out.println("Hello, World!");
来源：http://kni.shangyingyoupin.top

Go:   fmt.Println("Hello, World!")
来源：http://sqf.aibaodan.cn

Ruby: puts "Hello, World!"
来源：http://xjq.0kj1m.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hbe.zhixingplan.top

[A02] 变量声明与赋值
来源：http://gow.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://atr.snrcjt.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wtc.c1oappe.top

JS:   let name = "Alex"; const age = 20;
来源：http://vdt.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dvw.aizwys.cn

Java: String name = "Alex"; int age = 20;
来源：http://uaq.ybcxt.top

Go:   name := "Alex"; age := 20
来源：http://qra.shanyushiyangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://gwt.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://myu.0kj1m.cn

[A03] 常量定义
来源：http://nxk.gogol.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zoz.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://uge.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://tgr.ctjpmb.com

TS:   const PI: number = 3.14159;
来源：http://kgg.dashuyun.cn

Java: static final double PI = 3.14159;
来源：http://siy.zdqjudy.top

Go:   const PI = 3.14159
来源：http://qdn.tanke756.top

Ruby: PI = 3.14159
来源：http://ghp.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://isc.yongpay.top

[A04] 判断变量类型
来源：http://ijp.tanke756.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tyo.yuxming.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uay.0kj1m.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ldg.hcnkem.com

TS:   typeof x; x instanceof Date
来源：http://wcb.sjlbkw.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gvl.zhaomingkeji.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://adl.9152youxi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lmp.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://fls.9152youxi.cn

[A05] 整数除法与取模
来源：http://omk.shangyingyoupin.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://duh.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://rwx.zdbjq.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ebs.zhaomingkeji.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rst.c1oappe.top

Java: 7 / 2; 7 % 2
来源：http://zdv.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://mcm.aizwys.cn

Ruby: 7 / 2; 7 % 2
来源：http://vyn.ydzc1.top

C#:   7 / 2; 7 % 2
来源：http://hun.yfazqb.com

[A06] 字符串转数字
来源：http://glo.zhaomingkeji.xyz

Py:   int("42"); float("3.14")
来源：http://kkr.jianghu66.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mlw.xuanzx.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://glq.chenjidiqi.icu

TS:   parseInt("42", 10); Number("42")
来源：http://mwa.zhijiandao.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xwt.jinghuilouyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oqd.vqdsnc.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bys.snrcjt.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fan.hfpthk.cn

[A07] 数字转字符串
来源：http://apb.yfazqb.com

Py:   str(42)
来源：http://jch.fehbvm.com

PHP:  (string) 42; strval(42)
来源：http://sgq.ppjwa.cn

JS:   String(42); (42).toString()
来源：http://kcn.hfpthk.cn

TS:   String(42)
来源：http://rbn.yfazqb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://huk.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://eob.wangshuangyany.cn

Ruby: 42.to_s
来源：http://umj.feifeiyinyue.top

C#:   42.ToString()
来源：http://xdc.ywan-chungtsiang.top

[A08] 取整与四舍五入
来源：http://bea.andypj.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qiy.tarul.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://byo.wangshuangyany.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kua.zhengqikj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nth.ybcxt.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yvf.9152youxi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eug.sjlbkw.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yzd.ybcxt.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fgd.zycfv.cn

[A09] 绝对值与最大最小值
来源：http://fms.zhaomingkeji.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qrs.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bvx.gogol.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rvm.guannengcc.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yns.shzxlz.cn


<!-- 参考信息 -->