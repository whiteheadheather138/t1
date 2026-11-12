代发 wailian999

[U61] PHP：正则
来源：http://uly.jiagoushi.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nzx.dashuyun.cn

[U62] PHP：日期对象
来源：http://qey.bjfxy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kgc.jinqigufen.top

[U63] PHP：文件读写
来源：http://vix.cashguo.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://azr.yangfankeji.com

[U64] PHP：目录遍历
来源：http://doq.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://scr.hfpthk.cn

[U65] PHP：会话
来源：http://did.vqdsnc.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://grl.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://xta.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://snc.xziqi.cn

[U67] PHP：处理文件上传
来源：http://opf.gzhubu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://msd.xuetiantiany.cn

[U68] PHP：PDO 连接
来源：http://jam.xingfuxueyuan.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cvu.ivvv.top

[U69] PHP：PDO 预处理
来源：http://gwe.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ysk.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://jgf.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ojo.yj202588.top

[U71] PHP：抛出异常
来源：http://jpb.xingfuxueyuan.xyz

throw new RuntimeException("失败", 500);
来源：http://xjp.andypj.xyz

[U72] PHP：写错误日志
来源：http://mry.xingfuxueyuan.xyz

error_log("失败: " . $e->getMessage());
来源：http://scm.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://elz.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://apz.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://rbb.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://dwc.ctjpmb.com

[U75] PHP：依赖注入
来源：http://tmj.zhoulong.xyz

composer require psr/container
来源：http://mxz.hfpthk.cn

[U76] PHP：简单路由
来源：http://bjj.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://meu.gotoacloud.top

[U77] PHP：模板渲染
来源：http://wug.fzhhl.top

composer require twig/twig
来源：http://mit.nwbrower.top

[U78] PHP：单元测试
来源：http://msy.tarul.cn

composer require --dev phpunit/phpunit
来源：http://rsd.nanxuanxn.top

[U79] PHP：静态分析
来源：http://ifd.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://rej.bbcook.cn

[U80] PHP：代码规范修复
来源：http://vyy.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pmy.zdbjq.cn

[U81] JS：初始化项目
来源：http://utk.zhoulong.xyz

npm init -y;  npm i express
来源：http://dpj.fzhhl.top

[U82] JS：package.json 脚本
来源：http://qfi.andypj.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bpa.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://efj.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://glx.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://tlc.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://rkf.yueranfly.top

[U85] JS：可选链
来源：http://ahc.tarul.cn

a?.b?.c
来源：http://qhs.fengsongda.top

[U86] JS：空值合并
来源：http://qov.yj202588.top

a ?? b
来源：http://fyu.wangdashe.top

[U87] JS：解构默认值
来源：http://gxb.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://kan.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://woj.uphjek.com

{ ...a, ...b }
来源：http://vsl.yanxiufei.cn

[U89] JS：数组去重
来源：http://htg.jinghuilouyu.cn

[...new Set(arr)]
来源：http://pco.xuanzx.com

[U90] JS：数字数组排序
来源：http://zgm.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://xan.xylfe.cn

[U91] JS：对象键值遍历
来源：http://pff.shanyushiyangtech.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nrb.vqdsnc.cn

[U92] JS：深拷贝
来源：http://adz.zhongyouzk.top

structuredClone(obj)
来源：http://caz.jinghuilouyu.cn

[U93] JS：模板字符串
来源：http://okt.shanyushiyangtech.top

`共 ${n} 条`
来源：http://xnx.svipenyu.cn

[U94] JS：箭头函数
来源：http://lcn.uphjek.com

const double = x => x * 2;
来源：http://yid.jiagoushi.top

[U95] JS：Promise 包装
来源：http://zvk.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://vle.yongpay.top

[U96] JS：async/await 与异常
来源：http://ixh.gogol.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lhr.sxryk.cn

[U97] JS：并发请求
来源：http://umx.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zbi.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://nik.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ezp.snrcjt.cn

[U99] JS：事件监听
来源：http://qbb.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://ykh.zycfv.cn

[U100] JS：DOM 查询
来源：http://ebw.yonumen.top

document.querySelector(".item")
来源：http://oyn.zhengqikj.top

[U101] JS：classList 操作
来源：http://lqn.sufxvd.cn

el.classList.toggle("active")
来源：http://gry.jinqigfzy.top

[U102] JS：本地存储
来源：http://uga.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://xem.hongshengwenyu.top

[U103] JS：定时器
来源：http://dkd.shzxlz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gnv.cucudq.cn

[U104] JS：防抖
来源：http://vfu.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xxw.0kj1m.cn

[U105] JS：节流
来源：http://ura.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uli.shangyingyoupin.top

[U106] JS：日期格式化
来源：http://coq.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dmd.smart0.xyz

[U107] JS：数字千分位
来源：http://jjo.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zis.chenzaomai.com

[U108] JS：随机整数
来源：http://qee.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bsk.yueranfly.top

[U109] JS：数组分组
来源：http://cqe.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://bcc.chenlongwang.top

[U110] JS：数组分块
来源：http://dsv.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zcb.shuidangran.top

[U111] JS：对象转 Map
来源：http://bxr.epnwcf.com

new Map(Object.entries(obj))
来源：http://jmh.chenlongwang.top

[U112] JS：字符串补位
来源：http://uqk.aizwys.cn

"7".padStart(3, "0")
来源：http://noo.meibo888.top

[U113] JS：正则替换全部
来源：http://zsv.ehwqpu.com

s.replaceAll("a", "b")
来源：http://rsi.yonumen.top

[U114] JS：JSON 深比较
来源：http://wvx.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kmo.sweek.top

[U115] JS：生成 UUID
来源：http://aek.hywenlv.cn

crypto.randomUUID()
来源：http://psp.316326.xyz

[U116] JS：类型检查（JSDoc）
来源：http://jrh.jlsjyb.cn

/** @param {string} name */ function f(name) {}
来源：http://rox.ctjpmb.com

[U117] JS：单元测试
来源：http://oib.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://mph.sysykeji.top

[U118] JS：开发服务器
来源：http://khd.guannengcc.top

npm i -D vite;  npx vite
来源：http://qrh.pengpengdd.cyou

[U119] JS：生产构建
来源：http://zyo.xuanzx.com

npx vite build
来源：http://ton.zhongyouzk.top

[U120] JS：读取环境变量（Vite）
来源：http://muo.wangdashe.top

import.meta.env.VITE_API_URL
来源：http://lol.0kj1m.cn

================================================================================
来源：http://aoo.yj202588.top

统计汇总
来源：http://qgf.aibaodan.cn

================================================================================
来源：http://zgt.hfpthk.cn

按语言统计（条）：
来源：http://fcs.fzhhl.top

Python ......... 252
来源：http://szr.zhijiandao.cn

PHP ............ 252
来源：http://tke.ivvv.top

JavaScript ..... 252
来源：http://ufb.jiagoushi.top

TypeScript ..... 212
来源：http://egl.jianghu66.top

Java ........... 212
来源：http://aas.mhx1999.top

Go ............. 212
来源：http://xle.fengsongda.top

Ruby ........... 212
来源：http://bcq.andypj.xyz

C# ............. 212
来源：http://ccr.52xcode.cn

C .............. 30
来源：http://jjb.bbcook.cn

C++ ............ 30
来源：http://pdh.wangdashe.top

SQL ............ 90
来源：http://hcr.cheryme.top

Bash ........... 80
来源：http://jhx.yj20258888.top

Kotlin ......... 15
来源：http://jsu.aizwys.cn

Swift .......... 15
来源：http://iay.feifeiyinyue.top

Lua ............ 10
来源：http://mdw.c1oappe.top

Perl ........... 10
来源：http://ksf.jinqigfzy.top

Scala .......... 10
来源：http://ssz.yfazqb.com

------------------------------------
来源：http://kib.vehdjk.com

合计 ........... 2106 条
来源：http://pme.nanxuanxn.top

按章节统计：
来源：http://mha.zhengqikj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dgy.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yrm.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ttn.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mgb.ctjpmb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pmk.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ori.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bvq.daxiang520.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qvv.yj20258888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gln.hysaishi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xxn.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://egy.dianchejie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xir.jyoumei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nzk.hnxiangtu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://omj.shangyingyoupin.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hcv.zdqjudy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ssk.yfazqb.com

Q SQL 专题                              90
来源：http://iuz.ctjpmb.com

R Bash 专题                             80
来源：http://stn.pycfn.com

S C / C++ 专题                          60
来源：http://yiy.ydjk.org.cn

T 其他语言补充                          60
来源：http://kdl.tian-w.cn

U 高频实用片段                         120
来源：http://xca.hcnkem.com

------------------------------------
来源：http://uqh.yvedp.cn

合计                                  2106 条
来源：http://tgd.daxiang520.top

--------------------------------------------------------------------------------
来源：http://tsl.jinghuilouyu.cn

使用提醒
来源：http://tkd.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://rgq.zdqjudy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://erc.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ozb.daria6918.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jzm.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pkd.ppjwa.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zps.zdqjudy.top

—— 文件结束 ——
来源：http://bmj.svipenyu.cn

================================================================================
来源：http://qnb.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://xpx.dashuyun.cn

Common Programming Examples Cheat Book
来源：http://awq.guannengcc.top

================================================================================
来源：http://pwv.haohaochexian.top

【收录内容】
来源：http://czr.jlsjyb.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vbu.shanyushiyangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ekw.gzhubu.top

SQL · Bash · C · C++
来源：http://vor.gotoacloud.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ibm.shzxlz.cn

【使用说明】
来源：http://ajq.zhixingplan.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://koy.yuanzhike.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jlp.gogol.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xtd.zhixingplan.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hxe.fengsongda.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xej.yanxiufei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xqg.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ugo.jinghuilouyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mhv.yvedp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rsy.zhijiandao.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://agn.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bwd.zhaomingkeji.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dqg.pycfn.com

【文件统计】
来源：http://mwc.jqgfzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sbx.yonumen.top

--------------------------------------------------------------------------------
来源：http://yar.jlsjyb.cn

目  录
来源：http://abb.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://ycl.yuxming.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gmd.jinqigufen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gir.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fmv.fzhhl.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dsl.gotoacloud.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kmu.hysaishi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tqv.c1oappe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fuc.jqgufenzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zwu.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://omv.cheryme.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dtl.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://epk.jianghu66.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rnb.sysykeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ugr.guannengcc.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fhd.c1oappe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fqs.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hiz.yueranfly.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kvh.iojbl.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lov.jianghu66.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wqv.jinqigufen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ntr.fanxiaobao.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yhq.daxiang520.top

================================================================================
来源：http://wfw.ywan-chungtsiang.top

A. 基础语法与类型
来源：http://vwv.sufxvd.cn

================================================================================
来源：http://rcj.52xcode.cn

[A01] Hello World
来源：http://adu.dashuyun.cn

Py:   print("Hello, World!")
来源：http://qsl.ywan-chungtsiang.top

PHP:  echo "Hello, World!";
来源：http://klz.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://mlk.xingfuxueyuan.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sys.jianghu66.top

Java: System.out.println("Hello, World!");
来源：http://gsq.yj20258888.top

Go:   fmt.Println("Hello, World!")
来源：http://tik.fzhhl.top

Ruby: puts "Hello, World!"
来源：http://ioy.hesvh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://azj.snrcjt.cn

[A02] 变量声明与赋值
来源：http://hbm.xinyue.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rhk.ppjwa.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fzl.hysaishi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ouf.zhijiandao.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://afl.cheryme.top

Java: String name = "Alex"; int age = 20;
来源：http://bzd.shzxlz.cn

Go:   name := "Alex"; age := 20
来源：http://cwc.meibo888.top

Ruby: name = "Alex"; age = 20
来源：http://hdg.xinyue.icu

C#:   string name = "Alex"; int age = 20;
来源：http://qko.zycfv.cn

[A03] 常量定义
来源：http://zdt.yanxiufei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jlu.sysykeji.top

PHP:  const PI = 3.14159;
来源：http://myu.9152youxi.cn

JS:   const PI = 3.14159;
来源：http://kcs.hywenlv.cn

TS:   const PI: number = 3.14159;
来源：http://wao.uphjek.com

Java: static final double PI = 3.14159;
来源：http://xlc.shuidangran.top

Go:   const PI = 3.14159
来源：http://jtz.zdqjudy.top

Ruby: PI = 3.14159
来源：http://mpx.andypj.xyz

C#:   const double PI = 3.14159;
来源：http://dal.cucudq.cn

[A04] 判断变量类型
来源：http://ukr.haohaochexian.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://hth.cheryme.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://txj.meibo888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://afd.guowangkeji.top

TS:   typeof x; x instanceof Date
来源：http://fcl.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://veu.xuanzx.com

Go:   reflect.TypeOf(x).Name()
来源：http://ajk.meibo888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wxl.ydjk.org.cn

C#:   x.GetType().Name; x is int
来源：http://rwa.snrcjt.cn

[A05] 整数除法与取模
来源：http://pmb.feifeiyinyue.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tlv.yj20258888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fpp.epnwcf.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zos.yvedp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ijs.zhixingplan.top

Java: 7 / 2; 7 % 2
来源：http://xuh.gzhubu.top

Go:   7 / 2; 7 % 2
来源：http://adq.shanyushiyangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://tnh.xziqi.cn

C#:   7 / 2; 7 % 2
来源：http://gpf.zhongyouzk.top

[A06] 字符串转数字
来源：http://lzn.chenzaomai.com

Py:   int("42"); float("3.14")
来源：http://vrk.zhaomingkeji.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://grl.cqqwz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://czn.sufxvd.cn

TS:   parseInt("42", 10); Number("42")
来源：http://smb.hywenlv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rix.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lwi.tianlin.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://hds.9152youxi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qfr.epnwcf.com

[A07] 数字转字符串
来源：http://yhm.zhijiandao.cn

Py:   str(42)
来源：http://esq.smart0.xyz

PHP:  (string) 42; strval(42)
来源：http://sjk.yuxming.cn

JS:   String(42); (42).toString()
来源：http://qrm.birdmap.top

TS:   String(42)
来源：http://bts.jlsjyb.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pbi.nanxinkj.top

Go:   strconv.Itoa(42)
来源：http://hgj.9152youxi.cn

Ruby: 42.to_s
来源：http://fjy.aizwys.cn

C#:   42.ToString()
来源：http://syi.ydzc1.top

[A08] 取整与四舍五入
来源：http://jcp.ehwqpu.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nee.ybcxt.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kec.fktsv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://laa.jyoumei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qbo.ywan-chungtsiang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fgf.feifeiyinyue.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bhe.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zya.fzhhl.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lko.xuetiantiany.cn

[A09] 绝对值与最大最小值
来源：http://llr.hcnkem.com


<!-- 参考信息 -->