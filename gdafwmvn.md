代发 wailian999

[U53] PHP：空合并运算符
来源：http://jrc.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://hjh.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://ump.gzhubu.top

$obj?->method()
来源：http://yan.jiagoushi.top

[U55] PHP：match 表达式
来源：http://aos.0kj1m.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jni.chenjidiqi.icu

[U56] PHP：命名参数
来源：http://fic.jinyuanbaomall.cn

f(a: 1, b: 2)
来源：http://erj.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://xto.ydzc1.top

"值: {$a}"
来源：http://mtw.shangyingyoupin.top

[U58] PHP：数组三件套
来源：http://hvr.jinqigfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vya.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://ban.52xcode.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jqm.jqgufenzy.top

[U60] PHP：JSON 编解码
来源：http://zff.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://osq.ppjwa.cn

[U61] PHP：正则
来源：http://pnf.haohaochexian.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ovo.52xcode.cn

[U62] PHP：日期对象
来源：http://fax.shzxlz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hgw.0kj1m.cn

[U63] PHP：文件读写
来源：http://yts.zhaomingkeji.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rcq.zdbjq.cn

[U64] PHP：目录遍历
来源：http://gmo.uphjek.com

glob("dir/*.php");  scandir("dir");
来源：http://atz.bjfxy.top

[U65] PHP：会话
来源：http://emm.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zro.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://mzn.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vec.zhixingplan.top

[U67] PHP：处理文件上传
来源：http://dhc.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kzq.ivvv.top

[U68] PHP：PDO 连接
来源：http://vdk.dashuyun.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vga.sysykeji.top

[U69] PHP：PDO 预处理
来源：http://cwj.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vqs.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://mxi.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gec.pycfn.com

[U71] PHP：抛出异常
来源：http://nio.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://tki.haohaochexian.top

[U72] PHP：写错误日志
来源：http://eog.sxryk.cn

error_log("失败: " . $e->getMessage());
来源：http://lnh.uphjek.com

[U73] PHP：读取 ini 配置
来源：http://jdw.smart0.xyz

parse_ini_file("config.ini", true)
来源：http://mcb.cheryme.top

[U74] PHP：读取环境变量
来源：http://ihd.zhijiandao.cn

getenv("APP_ENV") ?: "production"
来源：http://uuj.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://fda.yvedp.cn

composer require psr/container
来源：http://mpf.quarkkingdee.top

[U76] PHP：简单路由
来源：http://egs.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gtj.hammf.cn

[U77] PHP：模板渲染
来源：http://zew.jyoumei.cn

composer require twig/twig
来源：http://myi.pengpengdd.cyou

[U78] PHP：单元测试
来源：http://tjs.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://xqa.fengsongda.top

[U79] PHP：静态分析
来源：http://orl.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://hei.ydzc1.top

[U80] PHP：代码规范修复
来源：http://toq.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://hav.c1oappe.top

[U81] JS：初始化项目
来源：http://bmf.uphjek.com

npm init -y;  npm i express
来源：http://lem.9152youxi.cn

[U82] JS：package.json 脚本
来源：http://ldq.jiagoushi.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vve.guowangkeji.top

[U83] JS：ES Module 导入导出
来源：http://bso.redwolf501.top

export const a = 1;  import { a } from "./m.js";
来源：http://bvr.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://eos.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fex.epnwcf.com

[U85] JS：可选链
来源：http://gix.shanyushiyangkeji.top

a?.b?.c
来源：http://vlz.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://haw.hfpthk.cn

a ?? b
来源：http://gej.ivvv.top

[U87] JS：解构默认值
来源：http://pfa.pycfn.com

const { a = 1, b = 2 } = obj;
来源：http://uyr.chenlongwang.top

[U88] JS：对象展开合并
来源：http://bzc.hongshengwenyu.top

{ ...a, ...b }
来源：http://enw.jqgufenzy.top

[U89] JS：数组去重
来源：http://fgu.cheryme.top

[...new Set(arr)]
来源：http://mdy.yongpay.top

[U90] JS：数字数组排序
来源：http://aus.jinqigufen.top

[...arr].sort((a, b) => a - b)
来源：http://uvd.uphjek.com

[U91] JS：对象键值遍历
来源：http://oac.sxryk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jnt.jqgufenzy.top

[U92] JS：深拷贝
来源：http://owo.yanxiufei.cn

structuredClone(obj)
来源：http://plb.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://mjj.sxryk.cn

`共 ${n} 条`
来源：http://qee.yuxming.cn

[U94] JS：箭头函数
来源：http://oac.yuanzhike.top

const double = x => x * 2;
来源：http://nbg.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://phc.hywenlv.cn

new Promise((resolve, reject) => {})
来源：http://qzt.zhixingplan.top

[U96] JS：async/await 与异常
来源：http://ote.hammf.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ezg.hcnkem.com

[U97] JS：并发请求
来源：http://utn.xylfe.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://omy.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://gch.jqgufenzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bss.yongpay.top

[U99] JS：事件监听
来源：http://ndd.hongshengwenyu.top

el.addEventListener("click", e => {})
来源：http://nsm.zdqjudy.top

[U100] JS：DOM 查询
来源：http://uml.hammf.cn

document.querySelector(".item")
来源：http://gac.wangshuangyany.cn

[U101] JS：classList 操作
来源：http://fsa.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://mtv.zdqjudy.top

[U102] JS：本地存储
来源：http://shi.bbcook.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wwx.yonumen.top

[U103] JS：定时器
来源：http://xqt.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hgu.316326.xyz

[U104] JS：防抖
来源：http://yhr.hywenlv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nfm.yueranfly.top

[U105] JS：节流
来源：http://iyg.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hxq.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://fkn.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pja.hnqzz.top

[U107] JS：数字千分位
来源：http://ise.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gdf.cucudq.cn

[U108] JS：随机整数
来源：http://aom.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wqx.hywenlv.cn

[U109] JS：数组分组
来源：http://zuu.iojbl.cn

Object.groupBy(arr, x => x.type)
来源：http://mad.feifeiyinyue.top

[U110] JS：数组分块
来源：http://khm.jyoumei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://btq.meibo888.top

[U111] JS：对象转 Map
来源：http://qtq.sysykeji.top

new Map(Object.entries(obj))
来源：http://dof.jyoumei.cn

[U112] JS：字符串补位
来源：http://tha.shangyingyoupin.top

"7".padStart(3, "0")
来源：http://vmo.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://dhm.svipenyu.cn

s.replaceAll("a", "b")
来源：http://nyo.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://wor.redwolf501.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pdg.zhaomingkeji.xyz

[U115] JS：生成 UUID
来源：http://kll.mhx1999.top

crypto.randomUUID()
来源：http://kwf.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://wrg.xuanzx.com

/** @param {string} name */ function f(name) {}
来源：http://dyo.jinqigfzy.top

[U117] JS：单元测试
来源：http://bdo.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://zny.tarul.cn

[U118] JS：开发服务器
来源：http://mjj.dianchejie.cn

npm i -D vite;  npx vite
来源：http://mpp.feifeiyinyue.top

[U119] JS：生产构建
来源：http://bcw.316326.xyz

npx vite build
来源：http://imc.yvedp.cn

[U120] JS：读取环境变量（Vite）
来源：http://qwh.ehwqpu.com

import.meta.env.VITE_API_URL
来源：http://vzb.xuanzx.com

================================================================================
来源：http://rer.vqdsnc.cn

统计汇总
来源：http://lpm.wangshuangyany.cn

================================================================================
来源：http://uab.ivvv.top

按语言统计（条）：
来源：http://vtx.yuanzhike.top

Python ......... 252
来源：http://scw.jqgufenzy.top

PHP ............ 252
来源：http://bam.chenjidiqi.icu

JavaScript ..... 252
来源：http://dlz.bbcook.cn

TypeScript ..... 212
来源：http://kbi.hywenlv.cn

Java ........... 212
来源：http://zxk.tian-w.cn

Go ............. 212
来源：http://sir.0kj1m.cn

Ruby ........... 212
来源：http://mnn.shanyushiyangkeji.top

C# ............. 212
来源：http://pfq.jyoumei.cn

C .............. 30
来源：http://hhb.cheryme.top

C++ ............ 30
来源：http://pvr.shanyushiyangkeji.top

SQL ............ 90
来源：http://ruj.52xcode.cn

Bash ........... 80
来源：http://iwv.nanxinkj.top

Kotlin ......... 15
来源：http://jys.xuanzx.com

Swift .......... 15
来源：http://hqn.dianchejie.cn

Lua ............ 10
来源：http://jxq.gaohongyu789.top

Perl ........... 10
来源：http://jml.zhaomingkeji.xyz

Scala .......... 10
来源：http://uov.yj202588.top

------------------------------------
来源：http://isu.pycfn.com

合计 ........... 2106 条
来源：http://iso.ydjk.org.cn

按章节统计：
来源：http://whw.52xcode.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nrf.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ezz.zhixingplan.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fll.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://awb.uphjek.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pwu.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sis.snrcjt.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qiy.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qus.hnxiangtu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zjn.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aok.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://trh.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qhb.svipenyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tsd.gzhubu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kox.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jdh.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vui.jinqigufen.top

Q SQL 专题                              90
来源：http://kux.jinyuanbaomall.cn

R Bash 专题                             80
来源：http://hjg.pengpengdd.cyou

S C / C++ 专题                          60
来源：http://oiy.jinqigufen.top

T 其他语言补充                          60
来源：http://xhp.zdqjudy.top

U 高频实用片段                         120
来源：http://cxs.yj202588.top

------------------------------------
来源：http://jwf.hysaishi.cn

合计                                  2106 条
来源：http://byp.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://tjy.epnwcf.com

使用提醒
来源：http://tkl.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://ujb.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://goh.zhijiandao.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fgl.ehwqpu.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mmq.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vlt.tian-w.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ooq.sysykeji.top

—— 文件结束 ——
来源：http://llo.shangyingyoupin.top

================================================================================
来源：http://zsk.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://fpn.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://kvz.zhaomingkeji.xyz

================================================================================
来源：http://gaf.cqqwz.cn

【收录内容】
来源：http://swx.sxryk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://akp.chenlongwang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lvz.c1oappe.top

SQL · Bash · C · C++
来源：http://fyu.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ugr.dashuyun.cn

【使用说明】
来源：http://anz.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fdq.nwbrower.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://arg.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uov.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ooq.hongshengwenyu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://udd.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pwx.52xcode.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fko.tianlin.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://elo.gaohongyu789.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jjg.aizwys.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sja.tanke756.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://liq.chenlongwang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pnj.cucudq.cn

【文件统计】
来源：http://awt.ywan-chungtsiang.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://erg.mhx1999.top

--------------------------------------------------------------------------------
来源：http://zxg.shuidangran.top

目  录
来源：http://bep.hammf.cn

--------------------------------------------------------------------------------
来源：http://for.jianghu66.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jvc.shanyushiyangtech.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nyh.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rqw.bbcook.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yvw.gaohongyu789.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://buc.sweek.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vwt.9152youxi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wdc.gzhubu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mpb.jqgufenzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xvl.yangfankeji.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://idi.fengsongda.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hyl.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bpv.feifeiyinyue.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mia.nwbrower.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ssz.sjlbkw.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kbc.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sfd.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://txc.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hou.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mhc.xuetiantiany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xoe.hnqzz.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qnc.bbcook.cn

================================================================================
来源：http://wkc.vehdjk.com

A. 基础语法与类型
来源：http://gwl.jianghu66.top

================================================================================
来源：http://knz.fzhhl.top

[A01] Hello World
来源：http://lcb.redwolf501.top

Py:   print("Hello, World!")
来源：http://buo.daria6918.cn

PHP:  echo "Hello, World!";
来源：http://upo.tarul.cn

JS:   console.log("Hello, World!");
来源：http://adl.snrcjt.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gis.ydjk.org.cn

Java: System.out.println("Hello, World!");
来源：http://gah.nanxuanxn.top

Go:   fmt.Println("Hello, World!")
来源：http://nrj.chenzaomai.com

Ruby: puts "Hello, World!"
来源：http://ody.sweek.top

C#:   Console.WriteLine("Hello, World!");
来源：http://haz.chenjidiqi.icu

[A02] 变量声明与赋值
来源：http://aan.yanxiufei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vde.vqdsnc.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mns.yuxming.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ter.yonumen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wjw.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://dpp.shzxlz.cn

Go:   name := "Alex"; age := 20
来源：http://eia.dianchejie.cn

Ruby: name = "Alex"; age = 20
来源：http://rkw.zhengqikj.top

C#:   string name = "Alex"; int age = 20;
来源：http://ohz.0kj1m.cn

[A03] 常量定义
来源：http://zoe.zhixingplan.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bid.hammf.cn

PHP:  const PI = 3.14159;
来源：http://lan.yuanzhike.top

JS:   const PI = 3.14159;
来源：http://hab.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://vnh.tian-w.cn

Java: static final double PI = 3.14159;
来源：http://vkl.zhoulong.xyz

Go:   const PI = 3.14159
来源：http://gsv.cqqwz.cn

Ruby: PI = 3.14159
来源：http://emu.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://chl.yuanzhike.top

[A04] 判断变量类型
来源：http://cmw.fanxiaobao.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://bas.yfazqb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wmx.ehwqpu.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nyh.jqgfzy.top

TS:   typeof x; x instanceof Date
来源：http://lib.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yfw.zdbjq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mek.xinyue.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://gjf.shanyushiyangtech.top

C#:   x.GetType().Name; x is int
来源：http://xzu.zhaomingkeji.xyz

[A05] 整数除法与取模
来源：http://ldp.jianghu66.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qdp.zhaomingkeji.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://eia.cashguo.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://shc.hcnkem.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bqg.cqqwz.cn

Java: 7 / 2; 7 % 2
来源：http://cdo.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://saz.yanxiufei.cn

Ruby: 7 / 2; 7 % 2
来源：http://etv.sxryk.cn

C#:   7 / 2; 7 % 2
来源：http://lyn.mhx1999.top

[A06] 字符串转数字
来源：http://yjv.shangyingyoupin.top

Py:   int("42"); float("3.14")
来源：http://qgt.xuetiantiany.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xub.guowangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bkp.yonumen.top

TS:   parseInt("42", 10); Number("42")
来源：http://kgq.zhiwuduotai.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mby.aizwys.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zlw.zdbjq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://adp.zhiwuduotai.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xmo.ppjwa.cn

[A07] 数字转字符串
来源：http://ssl.zhiwuduotai.top

Py:   str(42)
来源：http://jst.gogol.net.cn

PHP:  (string) 42; strval(42)
来源：http://qtd.jyoumei.cn


<!-- 参考信息 -->