代发 wailian999

[U61] PHP：正则
来源：http://ejc.shangyingyoupin.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ccf.epnwcf.com

[U62] PHP：日期对象
来源：http://knw.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pww.zhiwuduotai.top

[U63] PHP：文件读写
来源：http://kva.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gky.hfpthk.cn

[U64] PHP：目录遍历
来源：http://xfe.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ziy.yanxiufei.cn

[U65] PHP：会话
来源：http://jos.bjfxy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://geg.ivvv.top

[U66] PHP：设置 Cookie
来源：http://yrq.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aak.redwolf501.top

[U67] PHP：处理文件上传
来源：http://wse.zhengqikj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gik.xziqi.cn

[U68] PHP：PDO 连接
来源：http://xox.zhijiandao.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fqq.zhoulong.xyz

[U69] PHP：PDO 预处理
来源：http://xla.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yax.zhijiandao.cn

[U70] PHP：PDO 事务
来源：http://lsa.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yxe.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://gwm.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://ohm.svipenyu.cn

[U72] PHP：写错误日志
来源：http://rzh.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://tux.sweek.top

[U73] PHP：读取 ini 配置
来源：http://dvs.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://mie.ydjk.org.cn

[U74] PHP：读取环境变量
来源：http://lvl.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://kwf.yj20258888.top

[U75] PHP：依赖注入
来源：http://pcl.zhoulong.xyz

composer require psr/container
来源：http://qhb.yanxiufei.cn

[U76] PHP：简单路由
来源：http://exj.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://szr.jianghu66.top

[U77] PHP：模板渲染
来源：http://mbj.uphjek.com

composer require twig/twig
来源：http://izw.zhixingplan.top

[U78] PHP：单元测试
来源：http://yrj.birdmap.top

composer require --dev phpunit/phpunit
来源：http://zxb.jqgfzy.top

[U79] PHP：静态分析
来源：http://vva.yj202588.top

composer require --dev phpstan/phpstan
来源：http://rxe.mhx1999.top

[U80] PHP：代码规范修复
来源：http://jqd.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hdz.epnwcf.com

[U81] JS：初始化项目
来源：http://fiq.xinyue.icu

npm init -y;  npm i express
来源：http://xah.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://ego.ybcxt.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iso.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://kfb.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wfg.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://cbo.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://oya.yj20258.top

[U85] JS：可选链
来源：http://qpm.xuanzx.com

a?.b?.c
来源：http://hpj.tarul.cn

[U86] JS：空值合并
来源：http://bpy.cqqwz.cn

a ?? b
来源：http://zcm.xuetiantiany.cn

[U87] JS：解构默认值
来源：http://qmr.haohaochexian.top

const { a = 1, b = 2 } = obj;
来源：http://bqh.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://vaa.tianlin.xyz

{ ...a, ...b }
来源：http://jpc.sxryk.cn

[U89] JS：数组去重
来源：http://pwb.yvedp.cn

[...new Set(arr)]
来源：http://gsk.zhaomingkeji.xyz

[U90] JS：数字数组排序
来源：http://naf.zhixingplan.top

[...arr].sort((a, b) => a - b)
来源：http://hds.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://jlv.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qzt.jiagoushi.top

[U92] JS：深拷贝
来源：http://vkh.gotoacloud.top

structuredClone(obj)
来源：http://kyw.sufxvd.cn

[U93] JS：模板字符串
来源：http://hcw.bjfxy.top

`共 ${n} 条`
来源：http://irg.jqgfzy.top

[U94] JS：箭头函数
来源：http://kfa.hcnkem.com

const double = x => x * 2;
来源：http://afu.zdbjq.cn

[U95] JS：Promise 包装
来源：http://khq.fehbvm.com

new Promise((resolve, reject) => {})
来源：http://afe.yj202588.top

[U96] JS：async/await 与异常
来源：http://kgr.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bqk.cucudq.cn

[U97] JS：并发请求
来源：http://oxb.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oks.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://opo.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qgn.yj20258888.top

[U99] JS：事件监听
来源：http://nfd.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://sba.sufxvd.cn

[U100] JS：DOM 查询
来源：http://cpx.zdbjq.cn

document.querySelector(".item")
来源：http://gzx.tian-w.cn

[U101] JS：classList 操作
来源：http://zkn.cashguo.top

el.classList.toggle("active")
来源：http://wbz.ehwqpu.com

[U102] JS：本地存储
来源：http://bsz.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bps.fzhhl.top

[U103] JS：定时器
来源：http://iio.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fzz.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://znm.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sld.yuxming.cn

[U105] JS：节流
来源：http://hmh.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xlg.shangyingyoupin.top

[U106] JS：日期格式化
来源：http://ukz.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hui.ctjpmb.com

[U107] JS：数字千分位
来源：http://qxy.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hla.sjlbkw.cn

[U108] JS：随机整数
来源：http://kir.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uhl.chenlongwang.top

[U109] JS：数组分组
来源：http://nhb.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://mxh.nanxuanxn.top

[U110] JS：数组分块
来源：http://cyh.xuanzx.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://arb.shzxlz.cn

[U111] JS：对象转 Map
来源：http://fvu.zhengqikj.top

new Map(Object.entries(obj))
来源：http://xud.wangshuangyany.cn

[U112] JS：字符串补位
来源：http://jav.zhijiandao.cn

"7".padStart(3, "0")
来源：http://vvq.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://dvn.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://slp.meibo888.top

[U114] JS：JSON 深比较
来源：http://rly.yanxiufei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rgs.yfazqb.com

[U115] JS：生成 UUID
来源：http://qcn.dashuyun.cn

crypto.randomUUID()
来源：http://phj.zhaomingkeji.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ful.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://jti.shzxlz.cn

[U117] JS：单元测试
来源：http://uap.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://eyq.smart0.xyz

[U118] JS：开发服务器
来源：http://tlb.quarkkingdee.top

npm i -D vite;  npx vite
来源：http://czh.yonumen.top

[U119] JS：生产构建
来源：http://gdp.cashguo.top

npx vite build
来源：http://jql.hesvh.cn

[U120] JS：读取环境变量（Vite）
来源：http://iih.tanke756.top

import.meta.env.VITE_API_URL
来源：http://gop.ehwqpu.com

================================================================================
来源：http://uir.nwbrower.top

统计汇总
来源：http://nmu.xuetiantiany.cn

================================================================================
来源：http://aqz.sufxvd.cn

按语言统计（条）：
来源：http://noi.cdnleiting.top

Python ......... 252
来源：http://anv.birdmap.top

PHP ............ 252
来源：http://eiw.daxiang520.top

JavaScript ..... 252
来源：http://aez.fzhhl.top

TypeScript ..... 212
来源：http://uwl.nwbrower.top

Java ........... 212
来源：http://shd.tian-w.cn

Go ............. 212
来源：http://cbz.hcnkem.com

Ruby ........... 212
来源：http://nzx.yongpay.top

C# ............. 212
来源：http://lfx.birdmap.top

C .............. 30
来源：http://qqh.zhixingplan.top

C++ ............ 30
来源：http://sxx.jqgfzy.top

SQL ............ 90
来源：http://ilg.nwbrower.top

Bash ........... 80
来源：http://qml.tian-w.cn

Kotlin ......... 15
来源：http://yzw.0kj1m.cn

Swift .......... 15
来源：http://peg.sysykeji.top

Lua ............ 10
来源：http://cbb.jqgufenzy.top

Perl ........... 10
来源：http://ptd.cdnleiting.top

Scala .......... 10
来源：http://nst.uphjek.com

------------------------------------
来源：http://dvn.gzhubu.top

合计 ........... 2106 条
来源：http://zyn.cucudq.cn

按章节统计：
来源：http://red.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://opq.zhengqikj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ztq.xuetiantiany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pyp.andypj.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vsl.zhixingplan.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sfb.nanxuanxn.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nay.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jop.yj20258888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://abu.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vwm.cqqwz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uvq.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wbq.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://amn.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qff.ywan-chungtsiang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sut.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eil.birdmap.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ieb.hnxiangtu.top

Q SQL 专题                              90
来源：http://vkb.jlsjyb.cn

R Bash 专题                             80
来源：http://pbx.dianchejie.cn

S C / C++ 专题                          60
来源：http://ook.gaohongyu789.top

T 其他语言补充                          60
来源：http://woa.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://cex.xinyue.icu

------------------------------------
来源：http://rql.gzhubu.top

合计                                  2106 条
来源：http://ypm.meibo888.top

--------------------------------------------------------------------------------
来源：http://tdi.xziqi.cn

使用提醒
来源：http://xlv.ydzc1.top

--------------------------------------------------------------------------------
来源：http://tqz.tianlin.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rqh.cheryme.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ttt.sweek.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xid.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jeq.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jyt.yuxming.cn

—— 文件结束 ——
来源：http://pio.ehwqpu.com

================================================================================
来源：http://dcx.hesvh.cn

程序语言常见例子速查手册（2024 版）
来源：http://lzt.yangfankeji.com

Common Programming Examples Cheat Book
来源：http://hfj.cqqwz.cn

================================================================================
来源：http://jdz.jianghu66.top

【收录内容】
来源：http://bec.cucudq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://aqq.svipenyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://chb.xinyue.icu

SQL · Bash · C · C++
来源：http://jie.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://crp.feifeiyinyue.top

【使用说明】
来源：http://iax.jyoumei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uhz.fktsv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nut.uphjek.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dvz.fehbvm.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pcc.sufxvd.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tau.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gbe.nanxuanxn.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://shb.yfazqb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ycy.wangshuangyany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yjj.pycfn.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://toa.hnxiangtu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vwj.hfpthk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wrl.yj202588.top

【文件统计】
来源：http://zkn.jianghu66.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vud.yj20258.top

--------------------------------------------------------------------------------
来源：http://nyu.snrcjt.cn

目  录
来源：http://cef.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://yvk.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qyf.shzxlz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lol.bbcook.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ovr.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fci.sufxvd.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zgf.havefunace.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gbh.hnqzz.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mxj.ppjwa.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://onl.ehwqpu.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://glo.hfpthk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://npc.cashguo.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cyk.fengsongda.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hyd.wangshuangyany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://efe.ehwqpu.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mdm.yj20258888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vpp.hysaishi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rax.redwolf501.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yjv.ehwqpu.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://pky.ywan-chungtsiang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vbh.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vwi.9152youxi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://agx.ctjpmb.com

================================================================================
来源：http://gxe.bbcook.cn

A. 基础语法与类型
来源：http://fem.smart0.xyz

================================================================================
来源：http://rvg.fktsv.cn

[A01] Hello World
来源：http://yjz.aizwys.cn

Py:   print("Hello, World!")
来源：http://wwd.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://njc.shanyushiyangkeji.top

JS:   console.log("Hello, World!");
来源：http://tvq.hnxiangtu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hel.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://nxj.sjlbkw.cn

Go:   fmt.Println("Hello, World!")
来源：http://cbc.tanke756.top

Ruby: puts "Hello, World!"
来源：http://pwd.ppjwa.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://smr.haohaochexian.top

[A02] 变量声明与赋值
来源：http://edv.yj20258888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xjc.yongpay.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xlm.cheryme.top

JS:   let name = "Alex"; const age = 20;
来源：http://wmh.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wuk.hnxiangtu.top

Java: String name = "Alex"; int age = 20;
来源：http://gnb.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://ngv.smart0.xyz

Ruby: name = "Alex"; age = 20
来源：http://oyx.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://qlm.xylfe.cn

[A03] 常量定义
来源：http://chy.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://guk.chenjidiqi.icu

PHP:  const PI = 3.14159;
来源：http://rgj.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://stg.zhixingplan.top

TS:   const PI: number = 3.14159;
来源：http://bkq.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://wqe.wangshuangyany.cn

Go:   const PI = 3.14159
来源：http://olx.epnwcf.com

Ruby: PI = 3.14159
来源：http://rai.sysykeji.top

C#:   const double PI = 3.14159;
来源：http://der.bbcook.cn

[A04] 判断变量类型
来源：http://pdd.hnxiangtu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ekp.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hml.cashguo.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fwy.pengpengdd.cyou

TS:   typeof x; x instanceof Date
来源：http://tdw.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://juf.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://sos.vqdsnc.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://olh.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://bhi.quarkkingdee.top

[A05] 整数除法与取模
来源：http://iwb.havefunace.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hik.fktsv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kig.ivvv.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dfk.dianchejie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lzi.zhongyouzk.top

Java: 7 / 2; 7 % 2
来源：http://ypu.hfpthk.cn

Go:   7 / 2; 7 % 2
来源：http://htw.tianlin.xyz

Ruby: 7 / 2; 7 % 2
来源：http://how.316326.xyz

C#:   7 / 2; 7 % 2
来源：http://mgf.ydzc1.top

[A06] 字符串转数字
来源：http://oog.tarul.cn

Py:   int("42"); float("3.14")
来源：http://yec.chenjidiqi.icu

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ydc.0kj1m.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vfo.ivvv.top

TS:   parseInt("42", 10); Number("42")
来源：http://eys.birdmap.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ewj.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rka.cheryme.top

Ruby: "42".to_i; "3.14".to_f
来源：http://weg.yvedp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xee.fengsongda.top

[A07] 数字转字符串
来源：http://efn.xziqi.cn

Py:   str(42)
来源：http://nnf.shangyingyoupin.top

PHP:  (string) 42; strval(42)
来源：http://cfs.zhongyouzk.top

JS:   String(42); (42).toString()
来源：http://ids.gaohongyu789.top

TS:   String(42)
来源：http://fnh.xingfuxueyuan.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://gcc.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://pqs.0kj1m.cn

Ruby: 42.to_s
来源：http://jon.ehwqpu.com

C#:   42.ToString()
来源：http://suu.yj202588.top

[A08] 取整与四舍五入
来源：http://ndk.yuanzhike.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qdc.nwbrower.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://aqc.jinyuanbaomall.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pjh.vehdjk.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sfp.ehwqpu.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vnf.daria6918.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kii.daria6918.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jzs.ywan-chungtsiang.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eug.gogol.net.cn

[A09] 绝对值与最大最小值
来源：http://bjq.chenlongwang.top


<!-- 参考信息 -->