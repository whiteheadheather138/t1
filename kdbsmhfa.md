代发 wailian999

[U57] PHP：字符串插值
来源：http://yex.zhaomingkeji.xyz

"值: {$a}"
来源：http://dsx.yueranfly.top

[U58] PHP：数组三件套
来源：http://wnr.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dhn.yfazqb.com

[U59] PHP：自定义排序
来源：http://trm.xziqi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lfa.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://lwu.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zva.sysykeji.top

[U61] PHP：正则
来源：http://hlz.shanyushiyangtech.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cjq.svipenyu.cn

[U62] PHP：日期对象
来源：http://fcd.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nuz.yj202588.top

[U63] PHP：文件读写
来源：http://slm.hnqzz.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fis.wangdashe.top

[U64] PHP：目录遍历
来源：http://jzj.yanxiufei.cn

glob("dir/*.php");  scandir("dir");
来源：http://qkz.ywan-chungtsiang.top

[U65] PHP：会话
来源：http://cks.zdqjudy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cxu.uphjek.com

[U66] PHP：设置 Cookie
来源：http://sqv.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vmn.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://jtg.fanxiaobao.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rie.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://vtl.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uft.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://cut.feifeiyinyue.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iwj.cucudq.cn

[U70] PHP：PDO 事务
来源：http://lvc.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lvm.chenlongwang.top

[U71] PHP：抛出异常
来源：http://gpx.zhengqikj.top

throw new RuntimeException("失败", 500);
来源：http://hxi.gogol.net.cn

[U72] PHP：写错误日志
来源：http://fzh.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://idk.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://cwt.yuanzhike.top

parse_ini_file("config.ini", true)
来源：http://yui.hywenlv.cn

[U74] PHP：读取环境变量
来源：http://jfw.bjfxy.top

getenv("APP_ENV") ?: "production"
来源：http://qxb.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://bxn.daria6918.cn

composer require psr/container
来源：http://lqv.yanxiufei.cn

[U76] PHP：简单路由
来源：http://xpa.zhengqikj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://upw.ybcxt.top

[U77] PHP：模板渲染
来源：http://elt.jqgfzy.top

composer require twig/twig
来源：http://pge.hesvh.cn

[U78] PHP：单元测试
来源：http://vyr.shanyushiyangkeji.top

composer require --dev phpunit/phpunit
来源：http://mcf.yj20258888.top

[U79] PHP：静态分析
来源：http://gdc.chenzaomai.com

composer require --dev phpstan/phpstan
来源：http://fal.uphjek.com

[U80] PHP：代码规范修复
来源：http://wfh.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nkc.yj20258888.top

[U81] JS：初始化项目
来源：http://owv.yvedp.cn

npm init -y;  npm i express
来源：http://mqy.zdbjq.cn

[U82] JS：package.json 脚本
来源：http://zyj.zdbjq.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ipp.fengsongda.top

[U83] JS：ES Module 导入导出
来源：http://gzh.shangyingyoupin.top

export const a = 1;  import { a } from "./m.js";
来源：http://oft.xziqi.cn

[U84] JS：CommonJS 写法
来源：http://szh.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cmm.yvedp.cn

[U85] JS：可选链
来源：http://nyz.0kj1m.cn

a?.b?.c
来源：http://umu.zhaomingkeji.xyz

[U86] JS：空值合并
来源：http://vqx.chenlongwang.top

a ?? b
来源：http://rty.zhengqikj.top

[U87] JS：解构默认值
来源：http://qob.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://ygd.shzxlz.cn

[U88] JS：对象展开合并
来源：http://kdf.chenjidiqi.icu

{ ...a, ...b }
来源：http://wlu.shuidangran.top

[U89] JS：数组去重
来源：http://wvj.zycfv.cn

[...new Set(arr)]
来源：http://nrq.chenjidiqi.icu

[U90] JS：数字数组排序
来源：http://bhj.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://rwk.sweek.top

[U91] JS：对象键值遍历
来源：http://jtp.yuanzhike.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xoq.vehdjk.com

[U92] JS：深拷贝
来源：http://dxu.fzhhl.top

structuredClone(obj)
来源：http://xvy.jianghu66.top

[U93] JS：模板字符串
来源：http://gjj.ybcxt.top

`共 ${n} 条`
来源：http://pel.zhaomingkeji.xyz

[U94] JS：箭头函数
来源：http://ayk.tarul.cn

const double = x => x * 2;
来源：http://nye.gaohongyu789.top

[U95] JS：Promise 包装
来源：http://cwu.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://lpr.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://psb.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bay.ppjwa.cn

[U97] JS：并发请求
来源：http://odb.zdbjq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uei.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://ucc.shuidangran.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pcc.xuetiantiany.cn

[U99] JS：事件监听
来源：http://apz.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://vob.guannengcc.top

[U100] JS：DOM 查询
来源：http://xsr.cdnleiting.top

document.querySelector(".item")
来源：http://ery.nwbrower.top

[U101] JS：classList 操作
来源：http://ipu.xuetiantiany.cn

el.classList.toggle("active")
来源：http://brx.andypj.xyz

[U102] JS：本地存储
来源：http://gus.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hhw.hcnkem.com

[U103] JS：定时器
来源：http://xii.dashuyun.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dln.yonumen.top

[U104] JS：防抖
来源：http://oqi.andypj.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qwo.vehdjk.com

[U105] JS：节流
来源：http://ezp.yj202588.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xwe.zhoulong.xyz

[U106] JS：日期格式化
来源：http://kvj.jlsjyb.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qgy.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://pbm.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kvy.jlsjyb.cn

[U108] JS：随机整数
来源：http://zha.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://waq.yj202588.top

[U109] JS：数组分组
来源：http://tji.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://yao.yuanzhike.top

[U110] JS：数组分块
来源：http://xfi.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://via.yangfankeji.com

[U111] JS：对象转 Map
来源：http://ori.ppjwa.cn

new Map(Object.entries(obj))
来源：http://vjg.hfpthk.cn

[U112] JS：字符串补位
来源：http://zmb.uphjek.com

"7".padStart(3, "0")
来源：http://tns.yangfankeji.com

[U113] JS：正则替换全部
来源：http://ikg.ywan-chungtsiang.top

s.replaceAll("a", "b")
来源：http://ojj.bjfxy.top

[U114] JS：JSON 深比较
来源：http://anl.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://zdv.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://wjx.tanke756.top

crypto.randomUUID()
来源：http://ubc.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://nkm.zhengqikj.top

/** @param {string} name */ function f(name) {}
来源：http://ood.yangfankeji.com

[U117] JS：单元测试
来源：http://wah.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://bau.ydzc1.top

[U118] JS：开发服务器
来源：http://izs.meibo888.top

npm i -D vite;  npx vite
来源：http://uqy.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://fnt.zdbjq.cn

npx vite build
来源：http://cqb.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://uub.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://uvy.wangshuangyany.cn

================================================================================
来源：http://lzr.vehdjk.com

统计汇总
来源：http://ust.pengpengdd.cyou

================================================================================
来源：http://zut.tanke756.top

按语言统计（条）：
来源：http://mxi.haohaochexian.top

Python ......... 252
来源：http://zbp.ivvv.top

PHP ............ 252
来源：http://trc.zhiwuduotai.top

JavaScript ..... 252
来源：http://tto.yj202588.top

TypeScript ..... 212
来源：http://nca.hnxiangtu.top

Java ........... 212
来源：http://xug.ydjk.org.cn

Go ............. 212
来源：http://hrc.ydzc1.top

Ruby ........... 212
来源：http://nny.bbcook.cn

C# ............. 212
来源：http://dhh.shzxlz.cn

C .............. 30
来源：http://opg.jqgfzy.top

C++ ............ 30
来源：http://brt.xingfuxueyuan.xyz

SQL ............ 90
来源：http://eix.guowangkeji.top

Bash ........... 80
来源：http://dqw.wangshuangyany.cn

Kotlin ......... 15
来源：http://yzg.hnqzz.top

Swift .......... 15
来源：http://ggc.shanyushiyangtech.top

Lua ............ 10
来源：http://bmc.zhixingplan.top

Perl ........... 10
来源：http://wgu.sxryk.cn

Scala .......... 10
来源：http://bua.gogol.net.cn

------------------------------------
来源：http://exm.tanke756.top

合计 ........... 2106 条
来源：http://usl.iojbl.cn

按章节统计：
来源：http://bad.smart0.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ttk.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ldb.jyoumei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wah.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zai.yj202588.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mzl.jyoumei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ngu.gaohongyu789.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uck.ydzc1.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iux.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wgs.0kj1m.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ssv.birdmap.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nym.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zki.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hag.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vxk.dashuyun.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jeh.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://etm.ybcxt.top

Q SQL 专题                              90
来源：http://irn.kuanghao11.cn

R Bash 专题                             80
来源：http://bts.dianchejie.cn

S C / C++ 专题                          60
来源：http://tpx.xuetiantiany.cn

T 其他语言补充                          60
来源：http://vhg.bjfxy.top

U 高频实用片段                         120
来源：http://pcn.gaohongyu789.top

------------------------------------
来源：http://spm.chenzaomai.com

合计                                  2106 条
来源：http://dko.vehdjk.com

--------------------------------------------------------------------------------
来源：http://dmu.zdbjq.cn

使用提醒
来源：http://rfj.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://bjj.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bhu.hysaishi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ckt.ctjpmb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yqe.9152youxi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ick.jqgufenzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zwm.ppjwa.cn

—— 文件结束 ——
来源：http://pnr.jinqigufen.top

================================================================================
来源：http://zzx.0kj1m.cn

程序语言常见例子速查手册（2024 版）
来源：http://gyj.ivvv.top

Common Programming Examples Cheat Book
来源：http://ila.gzhubu.top

================================================================================
来源：http://zwu.smart0.xyz

【收录内容】
来源：http://idw.yj20258888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hjx.zhiwuduotai.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zoy.yj20258.top

SQL · Bash · C · C++
来源：http://jbe.ehwqpu.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oss.smart0.xyz

【使用说明】
来源：http://wyp.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xks.hammf.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://phy.52xcode.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ktr.smart0.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ivt.yueranfly.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hni.svipenyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xgi.cqqwz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vlk.smart0.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dyu.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hgu.pycfn.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xme.ppjwa.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qmr.nanxinkj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://onf.jianghu66.top

【文件统计】
来源：http://npd.guowangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gsa.tarul.cn

--------------------------------------------------------------------------------
来源：http://dku.zycfv.cn

目  录
来源：http://xeb.hammf.cn

--------------------------------------------------------------------------------
来源：http://adw.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kvt.shangyingyoupin.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://esj.shanyushiyangtech.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ooy.sxryk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nrn.hfpthk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qhm.tianlin.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kuu.yj202588.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://flm.uphjek.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tjo.zdbjq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ahg.nanxinkj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sdz.aizwys.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zxh.hammf.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ucf.yueranfly.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tvs.hysaishi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://brz.feifeiyinyue.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ako.sweek.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://feu.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://glo.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nco.cqqwz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kxt.andypj.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aso.nanxuanxn.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zgz.meibo888.top

================================================================================
来源：http://sjy.jinghuilouyu.cn

A. 基础语法与类型
来源：http://xsz.uphjek.com

================================================================================
来源：http://obm.jinyuanbaomall.cn

[A01] Hello World
来源：http://ecz.hammf.cn

Py:   print("Hello, World!")
来源：http://yjv.birdmap.top

PHP:  echo "Hello, World!";
来源：http://zgk.yj20258888.top

JS:   console.log("Hello, World!");
来源：http://jaw.uphjek.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ccb.sweek.top

Java: System.out.println("Hello, World!");
来源：http://gpu.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://rcz.nwbrower.top

Ruby: puts "Hello, World!"
来源：http://sbc.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://pyw.haohaochexian.top

[A02] 变量声明与赋值
来源：http://qjc.cashguo.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zec.jqgufenzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uqf.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://ngf.zhaomingkeji.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gdo.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://rqy.xuanzx.com

Go:   name := "Alex"; age := 20
来源：http://kgw.sjlbkw.cn

Ruby: name = "Alex"; age = 20
来源：http://emm.zycfv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mmj.hywenlv.cn

[A03] 常量定义
来源：http://rki.daria6918.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ccr.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://cyo.jqgufenzy.top

JS:   const PI = 3.14159;
来源：http://ayk.gotoacloud.top

TS:   const PI: number = 3.14159;
来源：http://zll.jinqigufen.top

Java: static final double PI = 3.14159;
来源：http://kjf.sjlbkw.cn

Go:   const PI = 3.14159
来源：http://ihh.zdqjudy.top

Ruby: PI = 3.14159
来源：http://szi.jinghuilouyu.cn

C#:   const double PI = 3.14159;
来源：http://nbm.sxryk.cn

[A04] 判断变量类型
来源：http://xxl.sxryk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ssm.gotoacloud.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://geb.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hnl.zdqjudy.top

TS:   typeof x; x instanceof Date
来源：http://ler.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jbv.ydjk.org.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vvf.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fgv.haohaochexian.top

C#:   x.GetType().Name; x is int
来源：http://wjj.aizwys.cn

[A05] 整数除法与取模
来源：http://zjm.zhengqikj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dsb.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ust.jyoumei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://itf.shanyushiyangtech.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://isw.tian-w.cn

Java: 7 / 2; 7 % 2
来源：http://gty.iojbl.cn

Go:   7 / 2; 7 % 2
来源：http://htk.feifeiyinyue.top

Ruby: 7 / 2; 7 % 2
来源：http://bjk.zhaomingkeji.xyz

C#:   7 / 2; 7 % 2
来源：http://mqv.hysaishi.cn

[A06] 字符串转数字
来源：http://lvr.cdnleiting.top

Py:   int("42"); float("3.14")
来源：http://vmk.shuidangran.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://igs.hongshengwenyu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bvu.pengpengdd.cyou

TS:   parseInt("42", 10); Number("42")
来源：http://bxo.xziqi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qxz.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://djb.quarkkingdee.top

Ruby: "42".to_i; "3.14".to_f
来源：http://kci.ctjpmb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://itj.daria6918.cn

[A07] 数字转字符串
来源：http://wap.hnxiangtu.top

Py:   str(42)
来源：http://mrw.cheryme.top

PHP:  (string) 42; strval(42)
来源：http://lwi.shanyushiyangkeji.top

JS:   String(42); (42).toString()
来源：http://dll.dashuyun.cn

TS:   String(42)
来源：http://zav.yfazqb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://esg.cheryme.top

Go:   strconv.Itoa(42)
来源：http://rau.zhixingplan.top

Ruby: 42.to_s
来源：http://bru.shangyingyoupin.top

C#:   42.ToString()
来源：http://fxo.vqdsnc.cn

[A08] 取整与四舍五入
来源：http://fda.feifeiyinyue.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rdm.fzhhl.top


<!-- 参考信息 -->