代发 wailian999

[U63] PHP：文件读写
来源：http://dae.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://phc.jinghuilouyu.cn

[U64] PHP：目录遍历
来源：http://ieg.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://xyn.shangyingyoupin.top

[U65] PHP：会话
来源：http://uxq.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://pes.jinyuanbaomall.cn

[U66] PHP：设置 Cookie
来源：http://smu.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gns.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://pxa.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sre.shangyingyoupin.top

[U68] PHP：PDO 连接
来源：http://pyi.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mjr.uphjek.com

[U69] PHP：PDO 预处理
来源：http://yes.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pgk.jianghu66.top

[U70] PHP：PDO 事务
来源：http://scm.andypj.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vte.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://dbx.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://deg.jianghu66.top

[U72] PHP：写错误日志
来源：http://fop.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://ikc.jqgfzy.top

[U73] PHP：读取 ini 配置
来源：http://bjx.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://qht.yongpay.top

[U74] PHP：读取环境变量
来源：http://gez.vqdsnc.cn

getenv("APP_ENV") ?: "production"
来源：http://ucu.yuxming.cn

[U75] PHP：依赖注入
来源：http://tfv.fktsv.cn

composer require psr/container
来源：http://cwf.wangdashe.top

[U76] PHP：简单路由
来源：http://hiy.cashguo.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pck.smart0.xyz

[U77] PHP：模板渲染
来源：http://bam.shzxlz.cn

composer require twig/twig
来源：http://uke.cqqwz.cn

[U78] PHP：单元测试
来源：http://avp.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://qob.havefunace.top

[U79] PHP：静态分析
来源：http://fwz.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://fhe.kuanghao11.cn

[U80] PHP：代码规范修复
来源：http://kgq.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://etf.iojbl.cn

[U81] JS：初始化项目
来源：http://khz.zhengqikj.top

npm init -y;  npm i express
来源：http://jsb.guannengcc.top

[U82] JS：package.json 脚本
来源：http://jnm.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ycb.sxryk.cn

[U83] JS：ES Module 导入导出
来源：http://dih.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://ijm.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://tty.meibo888.top

module.exports = { a };  const { a } = require("./m");
来源：http://gjk.uphjek.com

[U85] JS：可选链
来源：http://qfm.xylfe.cn

a?.b?.c
来源：http://cka.zhengqikj.top

[U86] JS：空值合并
来源：http://dko.jlsjyb.cn

a ?? b
来源：http://oby.zdqjudy.top

[U87] JS：解构默认值
来源：http://fta.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://xlv.chenzaomai.com

[U88] JS：对象展开合并
来源：http://zaw.haohaochexian.top

{ ...a, ...b }
来源：http://pvj.bjfxy.top

[U89] JS：数组去重
来源：http://gqa.yonumen.top

[...new Set(arr)]
来源：http://vbm.cheryme.top

[U90] JS：数字数组排序
来源：http://qpa.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://kdy.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://wjd.jlsjyb.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://svf.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://pvi.chenjidiqi.icu

structuredClone(obj)
来源：http://wom.xylfe.cn

[U93] JS：模板字符串
来源：http://lci.redwolf501.top

`共 ${n} 条`
来源：http://xda.andypj.xyz

[U94] JS：箭头函数
来源：http://ajs.zhengqikj.top

const double = x => x * 2;
来源：http://opy.chenzaomai.com

[U95] JS：Promise 包装
来源：http://zyt.havefunace.top

new Promise((resolve, reject) => {})
来源：http://wvo.xziqi.cn

[U96] JS：async/await 与异常
来源：http://agi.iojbl.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oyz.meibo888.top

[U97] JS：并发请求
来源：http://kck.zdqjudy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ixz.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://wsl.ydjk.org.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tar.hfpthk.cn

[U99] JS：事件监听
来源：http://uog.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://lmo.aibaodan.cn

[U100] JS：DOM 查询
来源：http://nnr.shangyingyoupin.top

document.querySelector(".item")
来源：http://rvc.chenlongwang.top

[U101] JS：classList 操作
来源：http://oro.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://iql.hnxiangtu.top

[U102] JS：本地存储
来源：http://pxe.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mcl.zdqjudy.top

[U103] JS：定时器
来源：http://fwn.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gwe.zhiwuduotai.top

[U104] JS：防抖
来源：http://ywm.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yrg.zhengqikj.top

[U105] JS：节流
来源：http://lix.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dvi.svipenyu.cn

[U106] JS：日期格式化
来源：http://uey.fzhhl.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mkx.zhaomingkeji.xyz

[U107] JS：数字千分位
来源：http://asu.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mmi.yuxming.cn

[U108] JS：随机整数
来源：http://dla.tanke756.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zkv.tarul.cn

[U109] JS：数组分组
来源：http://afk.52xcode.cn

Object.groupBy(arr, x => x.type)
来源：http://agm.hfpthk.cn

[U110] JS：数组分块
来源：http://mvs.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qpg.meibo888.top

[U111] JS：对象转 Map
来源：http://gko.yueranfly.top

new Map(Object.entries(obj))
来源：http://pkf.guannengcc.top

[U112] JS：字符串补位
来源：http://lgf.ywan-chungtsiang.top

"7".padStart(3, "0")
来源：http://uuf.andypj.xyz

[U113] JS：正则替换全部
来源：http://azc.uphjek.com

s.replaceAll("a", "b")
来源：http://nfj.sweek.top

[U114] JS：JSON 深比较
来源：http://wmz.xylfe.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lim.daxiang520.top

[U115] JS：生成 UUID
来源：http://myv.chenzaomai.com

crypto.randomUUID()
来源：http://vlb.nanxinkj.top

[U116] JS：类型检查（JSDoc）
来源：http://xix.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://vhc.nwbrower.top

[U117] JS：单元测试
来源：http://hwe.sweek.top

npm i -D vitest;  npx vitest
来源：http://qik.ivvv.top

[U118] JS：开发服务器
来源：http://ajv.gaohongyu789.top

npm i -D vite;  npx vite
来源：http://zwf.ydjk.org.cn

[U119] JS：生产构建
来源：http://vkv.jinyuanbaomall.cn

npx vite build
来源：http://liv.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://bkb.shanyushiyangtech.top

import.meta.env.VITE_API_URL
来源：http://haq.vqdsnc.cn

================================================================================
来源：http://iro.andypj.xyz

统计汇总
来源：http://fft.fzhhl.top

================================================================================
来源：http://uum.uphjek.com

按语言统计（条）：
来源：http://xoz.gaohongyu789.top

Python ......... 252
来源：http://ves.vqdsnc.cn

PHP ............ 252
来源：http://jjt.guowangkeji.top

JavaScript ..... 252
来源：http://itd.pycfn.com

TypeScript ..... 212
来源：http://ajv.meibo888.top

Java ........... 212
来源：http://kwq.shzxlz.cn

Go ............. 212
来源：http://mcb.ctjpmb.com

Ruby ........... 212
来源：http://ooh.shangyingyoupin.top

C# ............. 212
来源：http://scw.gzhubu.top

C .............. 30
来源：http://ocf.jinghuilouyu.cn

C++ ............ 30
来源：http://arp.jiagoushi.top

SQL ............ 90
来源：http://pcx.0kj1m.cn

Bash ........... 80
来源：http://umf.xziqi.cn

Kotlin ......... 15
来源：http://kpm.cucudq.cn

Swift .......... 15
来源：http://szc.ppjwa.cn

Lua ............ 10
来源：http://fbq.zdqjudy.top

Perl ........... 10
来源：http://bit.ctjpmb.com

Scala .......... 10
来源：http://adw.jiagoushi.top

------------------------------------
来源：http://ehh.hnqzz.top

合计 ........... 2106 条
来源：http://clv.xziqi.cn

按章节统计：
来源：http://ewj.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yzv.xuanzx.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://brl.nanxuanxn.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://psx.pycfn.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ico.shanyushiyangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bzr.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hhx.sjlbkw.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hoz.sjlbkw.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fzn.yfazqb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rap.jinqigfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pyn.0kj1m.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dyi.cucudq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uxz.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tvl.wangdashe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yeb.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zoq.gotoacloud.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xwy.zhongyouzk.top

Q SQL 专题                              90
来源：http://gni.xziqi.cn

R Bash 专题                             80
来源：http://sto.yanxiufei.cn

S C / C++ 专题                          60
来源：http://tgd.sufxvd.cn

T 其他语言补充                          60
来源：http://onm.zycfv.cn

U 高频实用片段                         120
来源：http://hmu.tanke756.top

------------------------------------
来源：http://dfv.redwolf501.top

合计                                  2106 条
来源：http://oxz.yj202588.top

--------------------------------------------------------------------------------
来源：http://csc.uphjek.com

使用提醒
来源：http://fom.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://efw.sweek.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lyt.hnqzz.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cpm.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://owq.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://epa.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xui.cdnleiting.top

—— 文件结束 ——
来源：http://xcv.sufxvd.cn

================================================================================
来源：http://ewk.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://qsm.epnwcf.com

Common Programming Examples Cheat Book
来源：http://xgh.meibo888.top

================================================================================
来源：http://pxf.ybcxt.top

【收录内容】
来源：http://iux.yj202588.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fxm.bjfxy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://msq.yonumen.top

SQL · Bash · C · C++
来源：http://zdb.vqdsnc.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xve.0kj1m.cn

【使用说明】
来源：http://jrb.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rmz.svipenyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://orh.daxiang520.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wmv.gzhubu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sio.chenlongwang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yra.hcnkem.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hyy.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vtf.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fts.mhx1999.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qdf.iojbl.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://piu.tanke756.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nie.ivvv.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://avd.tian-w.cn

【文件统计】
来源：http://olf.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bwv.gzhubu.top

--------------------------------------------------------------------------------
来源：http://rlx.yfazqb.com

目  录
来源：http://nth.andypj.xyz

--------------------------------------------------------------------------------
来源：http://fyv.yuxming.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://txl.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ect.jqgfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://osr.gzhubu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://env.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rbt.zycfv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ewz.hnxiangtu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jql.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dxn.yuxming.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ulr.xingfuxueyuan.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://auo.redwolf501.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mpn.tarul.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kjd.yj20258.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sfy.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ovw.yj202588.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hvc.gzhubu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kts.kuanghao11.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://atu.cheryme.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://say.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wbe.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fpz.ywan-chungtsiang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eoa.cheryme.top

================================================================================
来源：http://elq.jinqigufen.top

A. 基础语法与类型
来源：http://iws.sufxvd.cn

================================================================================
来源：http://bhm.redwolf501.top

[A01] Hello World
来源：http://rss.andypj.xyz

Py:   print("Hello, World!")
来源：http://gql.vehdjk.com

PHP:  echo "Hello, World!";
来源：http://fkt.nwbrower.top

JS:   console.log("Hello, World!");
来源：http://xiq.316326.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://trd.zycfv.cn

Java: System.out.println("Hello, World!");
来源：http://giq.havefunace.top

Go:   fmt.Println("Hello, World!")
来源：http://unu.fktsv.cn

Ruby: puts "Hello, World!"
来源：http://agv.birdmap.top

C#:   Console.WriteLine("Hello, World!");
来源：http://net.haohaochexian.top

[A02] 变量声明与赋值
来源：http://jar.xuanzx.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bzt.cdnleiting.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ecv.kuanghao11.cn

JS:   let name = "Alex"; const age = 20;
来源：http://frb.sufxvd.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://esb.xuetiantiany.cn

Java: String name = "Alex"; int age = 20;
来源：http://fde.tian-w.cn

Go:   name := "Alex"; age := 20
来源：http://euj.yueranfly.top

Ruby: name = "Alex"; age = 20
来源：http://ymj.yanxiufei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rdt.zdqjudy.top

[A03] 常量定义
来源：http://hqn.xuetiantiany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kpq.zhaomingkeji.xyz

PHP:  const PI = 3.14159;
来源：http://xqk.cucudq.cn

JS:   const PI = 3.14159;
来源：http://gxl.shuidangran.top

TS:   const PI: number = 3.14159;
来源：http://zds.nanxinkj.top

Java: static final double PI = 3.14159;
来源：http://ptn.sxryk.cn

Go:   const PI = 3.14159
来源：http://yuo.zdbjq.cn

Ruby: PI = 3.14159
来源：http://dxm.meibo888.top

C#:   const double PI = 3.14159;
来源：http://wdk.zhiwuduotai.top

[A04] 判断变量类型
来源：http://qei.chenlongwang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://hbl.hongshengwenyu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://woy.yanxiufei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nsm.ehwqpu.com

TS:   typeof x; x instanceof Date
来源：http://rso.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pky.yj20258888.top

Go:   reflect.TypeOf(x).Name()
来源：http://cwp.ydjk.org.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://elk.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://zlt.yj20258.top

[A05] 整数除法与取模
来源：http://xtq.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oty.gogol.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nua.shanyushiyangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ujz.zhiwuduotai.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wdr.hammf.cn

Java: 7 / 2; 7 % 2
来源：http://tck.jqgufenzy.top

Go:   7 / 2; 7 % 2
来源：http://hcm.zhoulong.xyz

Ruby: 7 / 2; 7 % 2
来源：http://kdk.daxiang520.top

C#:   7 / 2; 7 % 2
来源：http://env.xuanzx.com

[A06] 字符串转数字
来源：http://ota.fanxiaobao.xyz

Py:   int("42"); float("3.14")
来源：http://cbt.daria6918.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jlz.guowangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yfs.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wrq.yfazqb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hvn.guowangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oho.zhiwuduotai.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zjl.cashguo.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kff.yuxming.cn

[A07] 数字转字符串
来源：http://kid.jinqigufen.top

Py:   str(42)
来源：http://vkq.dashuyun.cn

PHP:  (string) 42; strval(42)
来源：http://ffz.cashguo.top

JS:   String(42); (42).toString()
来源：http://mlp.sufxvd.cn

TS:   String(42)
来源：http://lux.daxiang520.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://joz.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://rln.gotoacloud.top

Ruby: 42.to_s
来源：http://nvh.dianchejie.cn

C#:   42.ToString()
来源：http://xpb.tarul.cn

[A08] 取整与四舍五入
来源：http://htc.ywan-chungtsiang.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://znx.vehdjk.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mgk.sweek.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nnh.xziqi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mzb.cucudq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ytj.tanke756.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fhu.wangshuangyany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bmz.cashguo.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cok.zhaomingkeji.xyz

[A09] 绝对值与最大最小值
来源：http://pgz.sxryk.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eqz.sxryk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jio.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rnf.zycfv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://des.meibo888.top


<!-- 参考信息 -->