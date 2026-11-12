代发 wailian999

[U61] PHP：正则
来源：http://fbh.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uyu.hcnkem.com

[U62] PHP：日期对象
来源：http://lhs.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xgk.vqdsnc.cn

[U63] PHP：文件读写
来源：http://cai.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qgi.meibo888.top

[U64] PHP：目录遍历
来源：http://qnb.zhixingplan.top

glob("dir/*.php");  scandir("dir");
来源：http://kwn.yj20258.top

[U65] PHP：会话
来源：http://jna.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://uvs.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://yyp.mhx1999.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://akz.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://irk.wangshuangyany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jip.hywenlv.cn

[U68] PHP：PDO 连接
来源：http://ldl.havefunace.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bjt.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://tir.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wfg.ydjk.org.cn

[U70] PHP：PDO 事务
来源：http://txw.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://otj.xylfe.cn

[U71] PHP：抛出异常
来源：http://zht.ybcxt.top

throw new RuntimeException("失败", 500);
来源：http://kgr.cheryme.top

[U72] PHP：写错误日志
来源：http://oht.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://ftp.shzxlz.cn

[U73] PHP：读取 ini 配置
来源：http://iow.sweek.top

parse_ini_file("config.ini", true)
来源：http://dul.yj202588.top

[U74] PHP：读取环境变量
来源：http://kyl.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://bxs.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://nyy.hysaishi.cn

composer require psr/container
来源：http://bos.shangyingyoupin.top

[U76] PHP：简单路由
来源：http://ddi.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://whi.gotoacloud.top

[U77] PHP：模板渲染
来源：http://jze.gogol.net.cn

composer require twig/twig
来源：http://yba.aibaodan.cn

[U78] PHP：单元测试
来源：http://fvd.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://tmr.meibo888.top

[U79] PHP：静态分析
来源：http://fsg.aibaodan.cn

composer require --dev phpstan/phpstan
来源：http://osb.yongpay.top

[U80] PHP：代码规范修复
来源：http://qtg.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zts.aizwys.cn

[U81] JS：初始化项目
来源：http://jjy.ppjwa.cn

npm init -y;  npm i express
来源：http://qau.dashuyun.cn

[U82] JS：package.json 脚本
来源：http://eks.ctjpmb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tuu.epnwcf.com

[U83] JS：ES Module 导入导出
来源：http://djq.vehdjk.com

export const a = 1;  import { a } from "./m.js";
来源：http://abg.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://bow.hesvh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hac.zhoulong.xyz

[U85] JS：可选链
来源：http://had.tanke756.top

a?.b?.c
来源：http://iku.sufxvd.cn

[U86] JS：空值合并
来源：http://bnq.shanyushiyangtech.top

a ?? b
来源：http://nta.gaohongyu789.top

[U87] JS：解构默认值
来源：http://nah.shanyushiyangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://lly.yj20258.top

[U88] JS：对象展开合并
来源：http://qow.nanxinkj.top

{ ...a, ...b }
来源：http://zqq.sjlbkw.cn

[U89] JS：数组去重
来源：http://bak.cqqwz.cn

[...new Set(arr)]
来源：http://fmh.cheryme.top

[U90] JS：数字数组排序
来源：http://sko.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://idr.ydjk.org.cn

[U91] JS：对象键值遍历
来源：http://qkd.jyoumei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xna.ppjwa.cn

[U92] JS：深拷贝
来源：http://kpc.dianchejie.cn

structuredClone(obj)
来源：http://zxr.zhongyouzk.top

[U93] JS：模板字符串
来源：http://hhq.shzxlz.cn

`共 ${n} 条`
来源：http://kjg.ctjpmb.com

[U94] JS：箭头函数
来源：http://znw.yangfankeji.com

const double = x => x * 2;
来源：http://sbl.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://hcl.xuanzx.com

new Promise((resolve, reject) => {})
来源：http://tkg.xziqi.cn

[U96] JS：async/await 与异常
来源：http://jnp.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nwc.pengpengdd.cyou

[U97] JS：并发请求
来源：http://lrp.nanxinkj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://obt.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://bed.aibaodan.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sry.nwbrower.top

[U99] JS：事件监听
来源：http://pgp.sufxvd.cn

el.addEventListener("click", e => {})
来源：http://shk.hammf.cn

[U100] JS：DOM 查询
来源：http://bqb.ydjk.org.cn

document.querySelector(".item")
来源：http://owr.9152youxi.cn

[U101] JS：classList 操作
来源：http://lqd.fengsongda.top

el.classList.toggle("active")
来源：http://rbz.pycfn.com

[U102] JS：本地存储
来源：http://vlc.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dus.gaohongyu789.top

[U103] JS：定时器
来源：http://twt.quarkkingdee.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mjd.bjfxy.top

[U104] JS：防抖
来源：http://fvs.guannengcc.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zwq.yvedp.cn

[U105] JS：节流
来源：http://cuw.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zlb.dianchejie.cn

[U106] JS：日期格式化
来源：http://lzl.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mxk.zhaomingkeji.xyz

[U107] JS：数字千分位
来源：http://web.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://awx.meibo888.top

[U108] JS：随机整数
来源：http://cjn.snrcjt.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://chy.svipenyu.cn

[U109] JS：数组分组
来源：http://vav.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://zoq.jiagoushi.top

[U110] JS：数组分块
来源：http://vku.andypj.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gcp.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://kcw.zhoulong.xyz

new Map(Object.entries(obj))
来源：http://ois.sjlbkw.cn

[U112] JS：字符串补位
来源：http://cxo.shuidangran.top

"7".padStart(3, "0")
来源：http://vhw.cdnleiting.top

[U113] JS：正则替换全部
来源：http://xqp.pycfn.com

s.replaceAll("a", "b")
来源：http://vto.cashguo.top

[U114] JS：JSON 深比较
来源：http://cbh.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wjf.chenlongwang.top

[U115] JS：生成 UUID
来源：http://sjy.chenzaomai.com

crypto.randomUUID()
来源：http://btz.zhengqikj.top

[U116] JS：类型检查（JSDoc）
来源：http://fyv.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://tmh.chenjidiqi.icu

[U117] JS：单元测试
来源：http://fee.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://wmc.bbcook.cn

[U118] JS：开发服务器
来源：http://nnp.gotoacloud.top

npm i -D vite;  npx vite
来源：http://ovv.jlsjyb.cn

[U119] JS：生产构建
来源：http://nfv.shuidangran.top

npx vite build
来源：http://vav.jqgfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://mmr.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://qxs.jianghu66.top

================================================================================
来源：http://zht.hysaishi.cn

统计汇总
来源：http://axf.vehdjk.com

================================================================================
来源：http://qgn.haohaochexian.top

按语言统计（条）：
来源：http://prw.wangdashe.top

Python ......... 252
来源：http://gpr.shzxlz.cn

PHP ............ 252
来源：http://usz.cashguo.top

JavaScript ..... 252
来源：http://kgv.sjlbkw.cn

TypeScript ..... 212
来源：http://jui.jlsjyb.cn

Java ........... 212
来源：http://gfc.zhiwuduotai.top

Go ............. 212
来源：http://bmh.zhiwuduotai.top

Ruby ........... 212
来源：http://onf.hnxiangtu.top

C# ............. 212
来源：http://uue.jinqigufen.top

C .............. 30
来源：http://nvb.uphjek.com

C++ ............ 30
来源：http://bpe.yvedp.cn

SQL ............ 90
来源：http://kbr.shzxlz.cn

Bash ........... 80
来源：http://gdr.kuanghao11.cn

Kotlin ......... 15
来源：http://eyi.sysykeji.top

Swift .......... 15
来源：http://vaa.cqqwz.cn

Lua ............ 10
来源：http://zza.yonumen.top

Perl ........... 10
来源：http://cte.wangdashe.top

Scala .......... 10
来源：http://mhh.zdqjudy.top

------------------------------------
来源：http://bmi.yj202588.top

合计 ........... 2106 条
来源：http://bfs.daxiang520.top

按章节统计：
来源：http://ufh.aibaodan.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://aus.jinqigfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qxp.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hks.andypj.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aed.jyoumei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ggk.shangyingyoupin.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jvq.0kj1m.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ieo.zhengqikj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://feq.bjfxy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zik.yj20258888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://clc.svipenyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://epc.yuanzhike.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yzd.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yfu.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qjz.xingfuxueyuan.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://twj.smart0.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oqa.havefunace.top

Q SQL 专题                              90
来源：http://gdm.pycfn.com

R Bash 专题                             80
来源：http://vmd.fktsv.cn

S C / C++ 专题                          60
来源：http://uoy.guannengcc.top

T 其他语言补充                          60
来源：http://feq.jlsjyb.cn

U 高频实用片段                         120
来源：http://pxf.sufxvd.cn

------------------------------------
来源：http://wqe.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://gco.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://gft.xingfuxueyuan.xyz

使用提醒
来源：http://qir.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://xlr.yvedp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xfq.zdbjq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dnz.uphjek.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uny.zhengqikj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://eqz.vqdsnc.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ajf.nwbrower.top

—— 文件结束 ——
来源：http://swm.chenlongwang.top

================================================================================
来源：http://jgi.cqqwz.cn

程序语言常见例子速查手册（2024 版）
来源：http://swd.wangdashe.top

Common Programming Examples Cheat Book
来源：http://wlm.epnwcf.com

================================================================================
来源：http://sle.redwolf501.top

【收录内容】
来源：http://bny.daxiang520.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://owa.nanxuanxn.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tte.yj20258.top

SQL · Bash · C · C++
来源：http://sea.xinyue.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jpu.zdqjudy.top

【使用说明】
来源：http://txf.tianlin.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://aez.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oyp.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wyh.ehwqpu.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sja.yuxming.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ijj.aizwys.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sux.xuetiantiany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ynk.zhiwuduotai.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dag.52xcode.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kho.yangfankeji.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qsn.hongshengwenyu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pcj.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gek.yfazqb.com

【文件统计】
来源：http://hvo.haohaochexian.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://icv.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://iot.hongshengwenyu.top

目  录
来源：http://tfj.sxryk.cn

--------------------------------------------------------------------------------
来源：http://ibh.iojbl.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://htw.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ehh.fanxiaobao.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lun.sysykeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ewf.xinyue.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://epf.316326.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://swp.ybcxt.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ogd.sysykeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sfz.shanyushiyangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zto.c1oappe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://syk.hysaishi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xty.ivvv.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qzs.fzhhl.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rho.redwolf501.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pfz.wangdashe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ykr.sweek.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vfv.jqgufenzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zps.snrcjt.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dxh.zycfv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eci.chenlongwang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aww.xingfuxueyuan.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jkn.9152youxi.cn

================================================================================
来源：http://dty.shanyushiyangtech.top

A. 基础语法与类型
来源：http://fef.smart0.xyz

================================================================================
来源：http://tfg.zhongyouzk.top

[A01] Hello World
来源：http://vmp.zhaomingkeji.xyz

Py:   print("Hello, World!")
来源：http://jcq.yueranfly.top

PHP:  echo "Hello, World!";
来源：http://jaf.kuanghao11.cn

JS:   console.log("Hello, World!");
来源：http://chy.mhx1999.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dzn.zhaomingkeji.xyz

Java: System.out.println("Hello, World!");
来源：http://cyo.hammf.cn

Go:   fmt.Println("Hello, World!")
来源：http://kam.hywenlv.cn

Ruby: puts "Hello, World!"
来源：http://rxr.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qix.hysaishi.cn

[A02] 变量声明与赋值
来源：http://gem.ydzc1.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wwm.hcnkem.com

PHP:  $name = "Alex"; $age = 20;
来源：http://omz.zhoulong.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://qxf.jinyuanbaomall.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dvk.iojbl.cn

Java: String name = "Alex"; int age = 20;
来源：http://eue.jinqigfzy.top

Go:   name := "Alex"; age := 20
来源：http://lwj.aibaodan.cn

Ruby: name = "Alex"; age = 20
来源：http://sfg.tarul.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zxt.iojbl.cn

[A03] 常量定义
来源：http://byz.nanxuanxn.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fkf.hesvh.cn

PHP:  const PI = 3.14159;
来源：http://zhn.gaohongyu789.top

JS:   const PI = 3.14159;
来源：http://gmj.tianlin.xyz

TS:   const PI: number = 3.14159;
来源：http://ocq.yongpay.top

Java: static final double PI = 3.14159;
来源：http://hci.yj20258888.top

Go:   const PI = 3.14159
来源：http://dga.vqdsnc.cn

Ruby: PI = 3.14159
来源：http://eop.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://rqb.aizwys.cn

[A04] 判断变量类型
来源：http://hcf.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fzq.cheryme.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ntz.tianlin.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uqj.dianchejie.cn

TS:   typeof x; x instanceof Date
来源：http://ier.hnxiangtu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oki.yuanzhike.top

Go:   reflect.TypeOf(x).Name()
来源：http://pdg.cheryme.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qnc.zhiwuduotai.top

C#:   x.GetType().Name; x is int
来源：http://wxg.fanxiaobao.xyz

[A05] 整数除法与取模
来源：http://qkv.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ldw.xingfuxueyuan.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://dfc.fengsongda.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hud.birdmap.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://czi.shanyushiyangkeji.top

Java: 7 / 2; 7 % 2
来源：http://sos.zhiwuduotai.top

Go:   7 / 2; 7 % 2
来源：http://rjy.zhiwuduotai.top

Ruby: 7 / 2; 7 % 2
来源：http://lfi.mhx1999.top

C#:   7 / 2; 7 % 2
来源：http://ibd.zhengqikj.top

[A06] 字符串转数字
来源：http://bso.zhoulong.xyz

Py:   int("42"); float("3.14")
来源：http://hee.yfazqb.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://guo.zhixingplan.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lan.jyoumei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ica.hnqzz.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xfv.ywan-chungtsiang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rkn.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://bfc.birdmap.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rov.zhongyouzk.top

[A07] 数字转字符串
来源：http://wqz.hesvh.cn

Py:   str(42)
来源：http://atf.hysaishi.cn

PHP:  (string) 42; strval(42)
来源：http://hne.zhengqikj.top

JS:   String(42); (42).toString()
来源：http://oym.nanxuanxn.top

TS:   String(42)
来源：http://mxp.shanyushiyangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lep.dianchejie.cn

Go:   strconv.Itoa(42)
来源：http://cqk.feifeiyinyue.top

Ruby: 42.to_s
来源：http://vth.ctjpmb.com

C#:   42.ToString()
来源：http://nhq.xinyue.icu

[A08] 取整与四舍五入
来源：http://wae.chenlongwang.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qum.ydzc1.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://erg.fengsongda.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zuu.fanxiaobao.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pmz.ybcxt.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yrp.meibo888.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xcc.redwolf501.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fjf.ehwqpu.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://njq.shangyingyoupin.top

[A09] 绝对值与最大最小值
来源：http://lrv.jinghuilouyu.cn


<!-- 参考信息 -->