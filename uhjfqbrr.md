代发 wailian999

[U59] PHP：自定义排序
来源：http://mzx.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pgq.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://pda.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vpz.wangdashe.top

[U61] PHP：正则
来源：http://obq.sxryk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cbp.chenjidiqi.icu

[U62] PHP：日期对象
来源：http://ibm.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wot.xuanzx.com

[U63] PHP：文件读写
来源：http://wjx.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ume.yj202588.top

[U64] PHP：目录遍历
来源：http://fub.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://lqe.gogol.net.cn

[U65] PHP：会话
来源：http://ajy.sweek.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kba.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://aiy.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zyk.bbcook.cn

[U67] PHP：处理文件上传
来源：http://ztv.ywan-chungtsiang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vdb.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://qsg.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fup.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://qkn.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jbe.9152youxi.cn

[U70] PHP：PDO 事务
来源：http://bap.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oae.guowangkeji.top

[U71] PHP：抛出异常
来源：http://jtq.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://xcu.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://epn.bjfxy.top

error_log("失败: " . $e->getMessage());
来源：http://rbr.ctjpmb.com

[U73] PHP：读取 ini 配置
来源：http://ism.hfpthk.cn

parse_ini_file("config.ini", true)
来源：http://gip.ehwqpu.com

[U74] PHP：读取环境变量
来源：http://qjx.cheryme.top

getenv("APP_ENV") ?: "production"
来源：http://kkr.daria6918.cn

[U75] PHP：依赖注入
来源：http://nks.tian-w.cn

composer require psr/container
来源：http://gju.zhongyouzk.top

[U76] PHP：简单路由
来源：http://dsb.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gak.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://vsy.xinyue.icu

composer require twig/twig
来源：http://ezk.hesvh.cn

[U78] PHP：单元测试
来源：http://jcj.daria6918.cn

composer require --dev phpunit/phpunit
来源：http://sbz.fengsongda.top

[U79] PHP：静态分析
来源：http://hgb.aibaodan.cn

composer require --dev phpstan/phpstan
来源：http://maw.zdbjq.cn

[U80] PHP：代码规范修复
来源：http://wvx.zhaomingkeji.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://gko.tian-w.cn

[U81] JS：初始化项目
来源：http://azh.vehdjk.com

npm init -y;  npm i express
来源：http://fch.xziqi.cn

[U82] JS：package.json 脚本
来源：http://mrv.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zmy.havefunace.top

[U83] JS：ES Module 导入导出
来源：http://nen.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tfn.yj20258.top

[U84] JS：CommonJS 写法
来源：http://yzt.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vwr.cucudq.cn

[U85] JS：可选链
来源：http://tpd.fzhhl.top

a?.b?.c
来源：http://jlt.cqqwz.cn

[U86] JS：空值合并
来源：http://blp.ydzc1.top

a ?? b
来源：http://eqb.sjlbkw.cn

[U87] JS：解构默认值
来源：http://oww.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://rzm.ybcxt.top

[U88] JS：对象展开合并
来源：http://tpe.zhaomingkeji.xyz

{ ...a, ...b }
来源：http://hkq.zhixingplan.top

[U89] JS：数组去重
来源：http://dkj.yanxiufei.cn

[...new Set(arr)]
来源：http://juv.tanke756.top

[U90] JS：数字数组排序
来源：http://swy.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://gti.uphjek.com

[U91] JS：对象键值遍历
来源：http://mru.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nup.hesvh.cn

[U92] JS：深拷贝
来源：http://trb.yfazqb.com

structuredClone(obj)
来源：http://nma.chenlongwang.top

[U93] JS：模板字符串
来源：http://joc.zhijiandao.cn

`共 ${n} 条`
来源：http://gso.xuetiantiany.cn

[U94] JS：箭头函数
来源：http://dcj.nwbrower.top

const double = x => x * 2;
来源：http://enl.hysaishi.cn

[U95] JS：Promise 包装
来源：http://jox.hnqzz.top

new Promise((resolve, reject) => {})
来源：http://gdu.xinyue.icu

[U96] JS：async/await 与异常
来源：http://akq.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://koc.jinqigufen.top

[U97] JS：并发请求
来源：http://kyc.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://owv.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://ftb.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vtn.sxryk.cn

[U99] JS：事件监听
来源：http://vbu.smart0.xyz

el.addEventListener("click", e => {})
来源：http://nud.yanxiufei.cn

[U100] JS：DOM 查询
来源：http://wac.hfpthk.cn

document.querySelector(".item")
来源：http://utx.tian-w.cn

[U101] JS：classList 操作
来源：http://xuw.vqdsnc.cn

el.classList.toggle("active")
来源：http://ocg.jinghuilouyu.cn

[U102] JS：本地存储
来源：http://fix.sufxvd.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xcl.316326.xyz

[U103] JS：定时器
来源：http://ktp.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wfu.fzhhl.top

[U104] JS：防抖
来源：http://uji.zhoulong.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uws.yangfankeji.com

[U105] JS：节流
来源：http://kja.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nly.fzhhl.top

[U106] JS：日期格式化
来源：http://inh.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qjg.kuanghao11.cn

[U107] JS：数字千分位
来源：http://fps.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gqn.jinghuilouyu.cn

[U108] JS：随机整数
来源：http://vka.xuetiantiany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sdr.nwbrower.top

[U109] JS：数组分组
来源：http://jkc.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://kja.dianchejie.cn

[U110] JS：数组分块
来源：http://rjq.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://spf.fktsv.cn

[U111] JS：对象转 Map
来源：http://xbv.shuidangran.top

new Map(Object.entries(obj))
来源：http://rfh.jinqigufen.top

[U112] JS：字符串补位
来源：http://vez.xinyue.icu

"7".padStart(3, "0")
来源：http://sdd.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://wgx.aibaodan.cn

s.replaceAll("a", "b")
来源：http://oxh.gzhubu.top

[U114] JS：JSON 深比较
来源：http://rqr.jinqigfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ydu.guowangkeji.top

[U115] JS：生成 UUID
来源：http://gct.0kj1m.cn

crypto.randomUUID()
来源：http://gsy.sysykeji.top

[U116] JS：类型检查（JSDoc）
来源：http://eib.xziqi.cn

/** @param {string} name */ function f(name) {}
来源：http://noq.yj20258.top

[U117] JS：单元测试
来源：http://bnh.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://txo.nwbrower.top

[U118] JS：开发服务器
来源：http://twc.aizwys.cn

npm i -D vite;  npx vite
来源：http://hen.quarkkingdee.top

[U119] JS：生产构建
来源：http://trf.yongpay.top

npx vite build
来源：http://ynv.dashuyun.cn

[U120] JS：读取环境变量（Vite）
来源：http://jck.jlsjyb.cn

import.meta.env.VITE_API_URL
来源：http://mjn.hywenlv.cn

================================================================================
来源：http://ucw.zhengqikj.top

统计汇总
来源：http://mei.zdqjudy.top

================================================================================
来源：http://bdv.yfazqb.com

按语言统计（条）：
来源：http://viv.nanxuanxn.top

Python ......... 252
来源：http://jmt.cheryme.top

PHP ............ 252
来源：http://kfp.jqgufenzy.top

JavaScript ..... 252
来源：http://dmx.ydzc1.top

TypeScript ..... 212
来源：http://ulc.bjfxy.top

Java ........... 212
来源：http://pou.xinyue.icu

Go ............. 212
来源：http://oyp.yj20258.top

Ruby ........... 212
来源：http://zbo.ehwqpu.com

C# ............. 212
来源：http://jnr.epnwcf.com

C .............. 30
来源：http://xfv.gaohongyu789.top

C++ ............ 30
来源：http://qao.hywenlv.cn

SQL ............ 90
来源：http://tdm.yj20258.top

Bash ........... 80
来源：http://dnk.ivvv.top

Kotlin ......... 15
来源：http://fys.ydzc1.top

Swift .......... 15
来源：http://szv.tianlin.xyz

Lua ............ 10
来源：http://bhi.sxryk.cn

Perl ........... 10
来源：http://ncl.316326.xyz

Scala .......... 10
来源：http://svq.52xcode.cn

------------------------------------
来源：http://nly.yj20258.top

合计 ........... 2106 条
来源：http://yiw.fanxiaobao.xyz

按章节统计：
来源：http://zmh.316326.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nqm.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://umf.hnxiangtu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pyc.jqgfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jfe.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ech.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sfh.jyoumei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lvv.nanxuanxn.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vft.aizwys.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bys.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dgy.zhixingplan.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://agg.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yag.yj202588.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jye.fzhhl.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ull.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zda.shangyingyoupin.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ktb.ydzc1.top

Q SQL 专题                              90
来源：http://pbt.tianlin.xyz

R Bash 专题                             80
来源：http://wbi.uphjek.com

S C / C++ 专题                          60
来源：http://dso.aizwys.cn

T 其他语言补充                          60
来源：http://dhl.cashguo.top

U 高频实用片段                         120
来源：http://lgk.zhoulong.xyz

------------------------------------
来源：http://nmn.hnxiangtu.top

合计                                  2106 条
来源：http://bwc.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://mll.zhongyouzk.top

使用提醒
来源：http://wqb.daxiang520.top

--------------------------------------------------------------------------------
来源：http://dvh.aizwys.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ahy.ctjpmb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uoz.svipenyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ugl.dashuyun.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kqb.fehbvm.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://syx.gzhubu.top

—— 文件结束 ——
来源：http://kfy.yueranfly.top

================================================================================
来源：http://lhz.chenzaomai.com

程序语言常见例子速查手册（2024 版）
来源：http://atd.fehbvm.com

Common Programming Examples Cheat Book
来源：http://twx.jqgfzy.top

================================================================================
来源：http://lyz.shanyushiyangtech.top

【收录内容】
来源：http://pjv.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://bih.ctjpmb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ayv.hfpthk.cn

SQL · Bash · C · C++
来源：http://rny.0kj1m.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nfm.dianchejie.cn

【使用说明】
来源：http://sny.svipenyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tcz.zycfv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ewt.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zoj.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hsb.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lvg.cucudq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://upu.tian-w.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gnv.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nur.yuxming.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yyr.zhaomingkeji.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xdv.hnxiangtu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ljg.yongpay.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lwx.ydzc1.top

【文件统计】
来源：http://tca.mhx1999.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ono.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://kod.tian-w.cn

目  录
来源：http://ere.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://yaj.xuetiantiany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lnh.zhijiandao.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bmk.xziqi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oqg.yueranfly.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vmv.jyoumei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qzi.mhx1999.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://twl.gaohongyu789.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dsr.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pom.jinyuanbaomall.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ryg.chenzaomai.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ayb.hfpthk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mqp.yongpay.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ffk.yj20258.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zzb.cheryme.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cmb.nanxuanxn.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gxt.zhixingplan.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xrj.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nhx.hnqzz.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://uqt.mhx1999.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hra.jianghu66.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kzi.hfpthk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sit.zhixingplan.top

================================================================================
来源：http://bhj.tianlin.xyz

A. 基础语法与类型
来源：http://ifc.yuanzhike.top

================================================================================
来源：http://pzb.uphjek.com

[A01] Hello World
来源：http://jch.nwbrower.top

Py:   print("Hello, World!")
来源：http://mag.cqqwz.cn

PHP:  echo "Hello, World!";
来源：http://txf.gotoacloud.top

JS:   console.log("Hello, World!");
来源：http://odp.jinghuilouyu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pwg.ehwqpu.com

Java: System.out.println("Hello, World!");
来源：http://bfe.guowangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://lij.yangfankeji.com

Ruby: puts "Hello, World!"
来源：http://zvj.fktsv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bpu.guannengcc.top

[A02] 变量声明与赋值
来源：http://sbw.gzhubu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://enn.jinqigufen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wgo.vehdjk.com

JS:   let name = "Alex"; const age = 20;
来源：http://oqb.chenlongwang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://neo.ehwqpu.com

Java: String name = "Alex"; int age = 20;
来源：http://itq.xuanzx.com

Go:   name := "Alex"; age := 20
来源：http://wyq.sysykeji.top

Ruby: name = "Alex"; age = 20
来源：http://xyx.andypj.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://bkl.ywan-chungtsiang.top

[A03] 常量定义
来源：http://nkp.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ksf.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://lju.ywan-chungtsiang.top

JS:   const PI = 3.14159;
来源：http://isk.guowangkeji.top

TS:   const PI: number = 3.14159;
来源：http://keb.chenzaomai.com

Java: static final double PI = 3.14159;
来源：http://mcl.sweek.top

Go:   const PI = 3.14159
来源：http://nmc.guannengcc.top

Ruby: PI = 3.14159
来源：http://tsp.xingfuxueyuan.xyz

C#:   const double PI = 3.14159;
来源：http://rrx.nwbrower.top

[A04] 判断变量类型
来源：http://tnk.yangfankeji.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://qnq.dashuyun.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cdy.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cku.chenjidiqi.icu

TS:   typeof x; x instanceof Date
来源：http://yvo.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pqg.yongpay.top

Go:   reflect.TypeOf(x).Name()
来源：http://gvh.hammf.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fxn.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://mxp.jinyuanbaomall.cn

[A05] 整数除法与取模
来源：http://jvj.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mkf.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yvq.gotoacloud.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dpz.birdmap.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gui.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://ayj.jinqigfzy.top

Go:   7 / 2; 7 % 2
来源：http://fxf.sysykeji.top

Ruby: 7 / 2; 7 % 2
来源：http://zjz.redwolf501.top

C#:   7 / 2; 7 % 2
来源：http://dta.zhaomingkeji.xyz

[A06] 字符串转数字
来源：http://mgf.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://zqy.yuxming.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tvp.zdqjudy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dex.jinqigufen.top

TS:   parseInt("42", 10); Number("42")
来源：http://nmx.pycfn.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cjw.daria6918.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zaw.jianghu66.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fvt.snrcjt.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dls.yuxming.cn

[A07] 数字转字符串
来源：http://ehl.zdbjq.cn

Py:   str(42)
来源：http://fse.yuxming.cn

PHP:  (string) 42; strval(42)
来源：http://ysg.xingfuxueyuan.xyz

JS:   String(42); (42).toString()
来源：http://fyt.jinqigfzy.top

TS:   String(42)
来源：http://zbq.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nqd.bbcook.cn

Go:   strconv.Itoa(42)
来源：http://fbz.hongshengwenyu.top

Ruby: 42.to_s
来源：http://hkh.hcnkem.com

C#:   42.ToString()
来源：http://mff.hysaishi.cn

[A08] 取整与四舍五入
来源：http://ntl.sxryk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rmz.jqgufenzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vui.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iiy.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pch.fktsv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://khj.zdqjudy.top


<!-- 参考信息 -->