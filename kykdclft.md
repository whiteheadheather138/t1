代发 wailian999

[U63] PHP：文件读写
来源：http://tul.chenjidiqi.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qps.zycfv.cn

[U64] PHP：目录遍历
来源：http://nmb.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://iwn.yueranfly.top

[U65] PHP：会话
来源：http://oso.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wow.nwbrower.top

[U66] PHP：设置 Cookie
来源：http://gdr.haohaochexian.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dbu.yonumen.top

[U67] PHP：处理文件上传
来源：http://vud.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jnc.guannengcc.top

[U68] PHP：PDO 连接
来源：http://mwa.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bdm.cashguo.top

[U69] PHP：PDO 预处理
来源：http://yii.chenzaomai.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oam.jlsjyb.cn

[U70] PHP：PDO 事务
来源：http://hon.shanyushiyangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wwh.zhengqikj.top

[U71] PHP：抛出异常
来源：http://mag.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://nxj.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://csd.bjfxy.top

error_log("失败: " . $e->getMessage());
来源：http://nlx.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://oqc.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://afk.shuidangran.top

[U74] PHP：读取环境变量
来源：http://trl.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://xwj.jyoumei.cn

[U75] PHP：依赖注入
来源：http://pkb.feifeiyinyue.top

composer require psr/container
来源：http://lib.gaohongyu789.top

[U76] PHP：简单路由
来源：http://wyo.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iim.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://rix.shzxlz.cn

composer require twig/twig
来源：http://tsj.tarul.cn

[U78] PHP：单元测试
来源：http://xfp.meibo888.top

composer require --dev phpunit/phpunit
来源：http://drv.tarul.cn

[U79] PHP：静态分析
来源：http://bqc.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://wpd.mhx1999.top

[U80] PHP：代码规范修复
来源：http://wvw.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://dic.jqgufenzy.top

[U81] JS：初始化项目
来源：http://obk.nanxinkj.top

npm init -y;  npm i express
来源：http://wjt.zycfv.cn

[U82] JS：package.json 脚本
来源：http://sly.tanke756.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lvs.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://ezk.hammf.cn

export const a = 1;  import { a } from "./m.js";
来源：http://idd.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://ery.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fsx.hesvh.cn

[U85] JS：可选链
来源：http://voy.quarkkingdee.top

a?.b?.c
来源：http://ywg.fanxiaobao.xyz

[U86] JS：空值合并
来源：http://tua.uphjek.com

a ?? b
来源：http://bdo.hesvh.cn

[U87] JS：解构默认值
来源：http://yvr.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://omw.aizwys.cn

[U88] JS：对象展开合并
来源：http://njr.jyoumei.cn

{ ...a, ...b }
来源：http://kit.52xcode.cn

[U89] JS：数组去重
来源：http://nfd.redwolf501.top

[...new Set(arr)]
来源：http://obo.daria6918.cn

[U90] JS：数字数组排序
来源：http://swv.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://wxm.hnxiangtu.top

[U91] JS：对象键值遍历
来源：http://wqp.sjlbkw.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tkw.fehbvm.com

[U92] JS：深拷贝
来源：http://hha.ivvv.top

structuredClone(obj)
来源：http://zxa.ybcxt.top

[U93] JS：模板字符串
来源：http://xgb.hongshengwenyu.top

`共 ${n} 条`
来源：http://ctv.ctjpmb.com

[U94] JS：箭头函数
来源：http://kbq.shuidangran.top

const double = x => x * 2;
来源：http://yld.haohaochexian.top

[U95] JS：Promise 包装
来源：http://psr.meibo888.top

new Promise((resolve, reject) => {})
来源：http://nwf.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://cpc.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hkk.gaohongyu789.top

[U97] JS：并发请求
来源：http://ecu.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://alm.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://jhi.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jzz.zhengqikj.top

[U99] JS：事件监听
来源：http://rpd.sysykeji.top

el.addEventListener("click", e => {})
来源：http://pxp.hesvh.cn

[U100] JS：DOM 查询
来源：http://ltg.yanxiufei.cn

document.querySelector(".item")
来源：http://ttw.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://fsr.vqdsnc.cn

el.classList.toggle("active")
来源：http://lnz.chenjidiqi.icu

[U102] JS：本地存储
来源：http://zau.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uzc.yj20258888.top

[U103] JS：定时器
来源：http://gra.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ald.cucudq.cn

[U104] JS：防抖
来源：http://try.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vxx.cdnleiting.top

[U105] JS：节流
来源：http://hky.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://njv.bbcook.cn

[U106] JS：日期格式化
来源：http://uys.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://obf.yuanzhike.top

[U107] JS：数字千分位
来源：http://qln.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://abf.fehbvm.com

[U108] JS：随机整数
来源：http://eir.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ndd.ehwqpu.com

[U109] JS：数组分组
来源：http://qpr.bbcook.cn

Object.groupBy(arr, x => x.type)
来源：http://wgn.sweek.top

[U110] JS：数组分块
来源：http://xso.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eqp.yuxming.cn

[U111] JS：对象转 Map
来源：http://zyh.tanke756.top

new Map(Object.entries(obj))
来源：http://xnd.uphjek.com

[U112] JS：字符串补位
来源：http://ayg.havefunace.top

"7".padStart(3, "0")
来源：http://btj.havefunace.top

[U113] JS：正则替换全部
来源：http://cud.ctjpmb.com

s.replaceAll("a", "b")
来源：http://uin.mhx1999.top

[U114] JS：JSON 深比较
来源：http://cee.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://vhx.dashuyun.cn

[U115] JS：生成 UUID
来源：http://csm.c1oappe.top

crypto.randomUUID()
来源：http://msn.ivvv.top

[U116] JS：类型检查（JSDoc）
来源：http://dqy.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://cvg.jyoumei.cn

[U117] JS：单元测试
来源：http://yra.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://wzc.nanxinkj.top

[U118] JS：开发服务器
来源：http://ucr.iojbl.cn

npm i -D vite;  npx vite
来源：http://dpz.pengpengdd.cyou

[U119] JS：生产构建
来源：http://mmf.ywan-chungtsiang.top

npx vite build
来源：http://jba.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://qbf.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://mov.ppjwa.cn

================================================================================
来源：http://ilb.yuxming.cn

统计汇总
来源：http://abo.vehdjk.com

================================================================================
来源：http://oxz.yanxiufei.cn

按语言统计（条）：
来源：http://htx.yfazqb.com

Python ......... 252
来源：http://hss.jianghu66.top

PHP ............ 252
来源：http://pnu.hongshengwenyu.top

JavaScript ..... 252
来源：http://lge.bbcook.cn

TypeScript ..... 212
来源：http://plz.iojbl.cn

Java ........... 212
来源：http://mou.ybcxt.top

Go ............. 212
来源：http://vnn.ppjwa.cn

Ruby ........... 212
来源：http://uhx.zhongyouzk.top

C# ............. 212
来源：http://ehp.daxiang520.top

C .............. 30
来源：http://pmn.bbcook.cn

C++ ............ 30
来源：http://vbk.feifeiyinyue.top

SQL ............ 90
来源：http://atd.gotoacloud.top

Bash ........... 80
来源：http://tzg.daria6918.cn

Kotlin ......... 15
来源：http://lmp.dashuyun.cn

Swift .......... 15
来源：http://dys.tian-w.cn

Lua ............ 10
来源：http://xsz.xziqi.cn

Perl ........... 10
来源：http://ncv.sysykeji.top

Scala .......... 10
来源：http://wli.snrcjt.cn

------------------------------------
来源：http://ybd.shuidangran.top

合计 ........... 2106 条
来源：http://aap.jqgfzy.top

按章节统计：
来源：http://iue.xuetiantiany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://viw.hysaishi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zpg.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nqp.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jxb.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zvt.ppjwa.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iiq.cdnleiting.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hty.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uko.feifeiyinyue.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hjc.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yyf.hcnkem.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://evb.wangdashe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cta.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ecr.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://twp.9152youxi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://efj.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lqz.aizwys.cn

Q SQL 专题                              90
来源：http://ypq.snrcjt.cn

R Bash 专题                             80
来源：http://bqd.snrcjt.cn

S C / C++ 专题                          60
来源：http://iua.ydzc1.top

T 其他语言补充                          60
来源：http://gpq.cdnleiting.top

U 高频实用片段                         120
来源：http://pbr.hesvh.cn

------------------------------------
来源：http://xnn.sjlbkw.cn

合计                                  2106 条
来源：http://pxk.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://omc.zhixingplan.top

使用提醒
来源：http://ade.fehbvm.com

--------------------------------------------------------------------------------
来源：http://pse.havefunace.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qte.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rak.jinqigufen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zpr.dianchejie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zuy.zdbjq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cql.jqgufenzy.top

—— 文件结束 ——
来源：http://sie.ehwqpu.com

================================================================================
来源：http://scm.pengpengdd.cyou

程序语言常见例子速查手册（2024 版）
来源：http://uxd.pycfn.com

Common Programming Examples Cheat Book
来源：http://zoj.chenlongwang.top

================================================================================
来源：http://cnz.feifeiyinyue.top

【收录内容】
来源：http://qif.cdnleiting.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bkc.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qcp.wangdashe.top

SQL · Bash · C · C++
来源：http://tqz.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://aee.tian-w.cn

【使用说明】
来源：http://jsz.svipenyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vja.jinqigfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ocd.shzxlz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bwp.yanxiufei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kek.jlsjyb.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fha.zhijiandao.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ney.sufxvd.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vwi.cqqwz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://snw.jlsjyb.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://koo.shangyingyoupin.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tun.hesvh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lka.jiagoushi.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zrw.hammf.cn

【文件统计】
来源：http://jnc.yangfankeji.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jut.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://lrm.dianchejie.cn

目  录
来源：http://eql.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://vly.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mul.0kj1m.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dgk.hongshengwenyu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mdd.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mff.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gie.yj20258888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://duf.sweek.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eas.uphjek.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xdj.chenzaomai.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mkv.ehwqpu.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jiw.daria6918.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uxe.nanxuanxn.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zva.xylfe.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://szh.jyoumei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wbn.cucudq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gnl.hysaishi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kbm.shzxlz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ser.shanyushiyangtech.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xzx.redwolf501.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://syv.aibaodan.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ubq.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xgr.vqdsnc.cn

================================================================================
来源：http://fxw.cashguo.top

A. 基础语法与类型
来源：http://irr.ehwqpu.com

================================================================================
来源：http://ajj.hammf.cn

[A01] Hello World
来源：http://nsw.yj20258.top

Py:   print("Hello, World!")
来源：http://mhr.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://djh.guannengcc.top

JS:   console.log("Hello, World!");
来源：http://npk.epnwcf.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dpi.redwolf501.top

Java: System.out.println("Hello, World!");
来源：http://vdp.nanxinkj.top

Go:   fmt.Println("Hello, World!")
来源：http://jug.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://leo.zycfv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mtt.andypj.xyz

[A02] 变量声明与赋值
来源：http://axn.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rnd.shuidangran.top

PHP:  $name = "Alex"; $age = 20;
来源：http://oom.meibo888.top

JS:   let name = "Alex"; const age = 20;
来源：http://dlm.zhongyouzk.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ibo.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://lop.gotoacloud.top

Go:   name := "Alex"; age := 20
来源：http://ysh.ctjpmb.com

Ruby: name = "Alex"; age = 20
来源：http://qfv.vehdjk.com

C#:   string name = "Alex"; int age = 20;
来源：http://lht.ydzc1.top

[A03] 常量定义
来源：http://rxv.zhengqikj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gcp.hammf.cn

PHP:  const PI = 3.14159;
来源：http://weo.gotoacloud.top

JS:   const PI = 3.14159;
来源：http://hoa.shanyushiyangtech.top

TS:   const PI: number = 3.14159;
来源：http://srn.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://hzq.jqgufenzy.top

Go:   const PI = 3.14159
来源：http://fgz.meibo888.top

Ruby: PI = 3.14159
来源：http://fpi.yj202588.top

C#:   const double PI = 3.14159;
来源：http://pwt.vehdjk.com

[A04] 判断变量类型
来源：http://abl.feifeiyinyue.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gvc.hammf.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uqf.snrcjt.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gsv.dianchejie.cn

TS:   typeof x; x instanceof Date
来源：http://qwt.jianghu66.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rxf.zhiwuduotai.top

Go:   reflect.TypeOf(x).Name()
来源：http://nvn.epnwcf.com

Ruby: x.class; x.is_a?(Integer)
来源：http://khv.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://dzb.smart0.xyz

[A05] 整数除法与取模
来源：http://qpa.chenjidiqi.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://spv.c1oappe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kvh.yvedp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jln.daxiang520.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pbr.ctjpmb.com

Java: 7 / 2; 7 % 2
来源：http://yte.dashuyun.cn

Go:   7 / 2; 7 % 2
来源：http://grb.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://dqt.shuidangran.top

C#:   7 / 2; 7 % 2
来源：http://kug.ctjpmb.com

[A06] 字符串转数字
来源：http://jcb.vehdjk.com

Py:   int("42"); float("3.14")
来源：http://juu.zhengqikj.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lxr.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cgi.jinghuilouyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uop.yanxiufei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ewx.wangdashe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cbc.fzhhl.top

Ruby: "42".to_i; "3.14".to_f
来源：http://tzb.bbcook.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dvl.quarkkingdee.top

[A07] 数字转字符串
来源：http://pxn.feifeiyinyue.top

Py:   str(42)
来源：http://lgk.yfazqb.com

PHP:  (string) 42; strval(42)
来源：http://cqy.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://kya.hnxiangtu.top

TS:   String(42)
来源：http://wfg.c1oappe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mab.zhengqikj.top

Go:   strconv.Itoa(42)
来源：http://isf.fzhhl.top

Ruby: 42.to_s
来源：http://ooq.dianchejie.cn

C#:   42.ToString()
来源：http://igw.xziqi.cn

[A08] 取整与四舍五入
来源：http://ohx.cheryme.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xdw.ybcxt.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vmk.sjlbkw.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jaa.yj20258888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cij.gzhubu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wab.fengsongda.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qvy.wangdashe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ugj.hongshengwenyu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hmb.jyoumei.cn

[A09] 绝对值与最大最小值
来源：http://afc.xingfuxueyuan.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://erw.hesvh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ufl.tianlin.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ovh.ywan-chungtsiang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qca.dashuyun.cn


<!-- 参考信息 -->