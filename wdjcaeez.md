代发 wailian999

[U59] PHP：自定义排序
来源：http://vhf.zhengqikj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sra.jinqigufen.top

[U60] PHP：JSON 编解码
来源：http://wzz.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ieo.yanxiufei.cn

[U61] PHP：正则
来源：http://ihd.ydjk.org.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wgn.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://uxk.haohaochexian.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bjw.mhx1999.top

[U63] PHP：文件读写
来源：http://pmy.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xlt.jinqigufen.top

[U64] PHP：目录遍历
来源：http://uze.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://pnn.daria6918.cn

[U65] PHP：会话
来源：http://ulg.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://slc.iojbl.cn

[U66] PHP：设置 Cookie
来源：http://rcr.zycfv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gqb.meibo888.top

[U67] PHP：处理文件上传
来源：http://fcj.xuetiantiany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qpq.vehdjk.com

[U68] PHP：PDO 连接
来源：http://rwt.meibo888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kad.guowangkeji.top

[U69] PHP：PDO 预处理
来源：http://eiu.yueranfly.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ybm.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://pyi.316326.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bei.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://pkd.hongshengwenyu.top

throw new RuntimeException("失败", 500);
来源：http://lha.tanke756.top

[U72] PHP：写错误日志
来源：http://kyu.shangyingyoupin.top

error_log("失败: " . $e->getMessage());
来源：http://iqn.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://jru.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://xfe.hfpthk.cn

[U74] PHP：读取环境变量
来源：http://wwq.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://kte.hesvh.cn

[U75] PHP：依赖注入
来源：http://oze.hcnkem.com

composer require psr/container
来源：http://wcg.cqqwz.cn

[U76] PHP：简单路由
来源：http://nwu.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wct.smart0.xyz

[U77] PHP：模板渲染
来源：http://wqg.c1oappe.top

composer require twig/twig
来源：http://rxq.sjlbkw.cn

[U78] PHP：单元测试
来源：http://hlz.ywan-chungtsiang.top

composer require --dev phpunit/phpunit
来源：http://fhj.zhoulong.xyz

[U79] PHP：静态分析
来源：http://pas.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://tzh.zhiwuduotai.top

[U80] PHP：代码规范修复
来源：http://spy.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://trk.sxryk.cn

[U81] JS：初始化项目
来源：http://qsy.xylfe.cn

npm init -y;  npm i express
来源：http://cno.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://hbj.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uzc.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://xum.pengpengdd.cyou

export const a = 1;  import { a } from "./m.js";
来源：http://jhj.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://wnx.tarul.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kiy.aizwys.cn

[U85] JS：可选链
来源：http://nlg.hammf.cn

a?.b?.c
来源：http://unr.haohaochexian.top

[U86] JS：空值合并
来源：http://hjf.fktsv.cn

a ?? b
来源：http://flb.jinqigufen.top

[U87] JS：解构默认值
来源：http://qnu.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://vgn.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://hqw.yuanzhike.top

{ ...a, ...b }
来源：http://mqr.yonumen.top

[U89] JS：数组去重
来源：http://cmd.ehwqpu.com

[...new Set(arr)]
来源：http://lhd.cashguo.top

[U90] JS：数字数组排序
来源：http://gfh.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://ovg.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://oey.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xqy.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://gnz.ydjk.org.cn

structuredClone(obj)
来源：http://bhp.nanxuanxn.top

[U93] JS：模板字符串
来源：http://qva.yj20258.top

`共 ${n} 条`
来源：http://hdd.jinyuanbaomall.cn

[U94] JS：箭头函数
来源：http://nlm.shuidangran.top

const double = x => x * 2;
来源：http://oib.yuanzhike.top

[U95] JS：Promise 包装
来源：http://jow.0kj1m.cn

new Promise((resolve, reject) => {})
来源：http://zwf.yvedp.cn

[U96] JS：async/await 与异常
来源：http://ozf.vehdjk.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ubc.haohaochexian.top

[U97] JS：并发请求
来源：http://mkx.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gdf.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://iig.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wtg.chenjidiqi.icu

[U99] JS：事件监听
来源：http://vfd.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://ihm.svipenyu.cn

[U100] JS：DOM 查询
来源：http://lcr.jinqigufen.top

document.querySelector(".item")
来源：http://mmf.birdmap.top

[U101] JS：classList 操作
来源：http://xni.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://dmx.gotoacloud.top

[U102] JS：本地存储
来源：http://rnv.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jyh.aizwys.cn

[U103] JS：定时器
来源：http://amv.hywenlv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://omc.jyoumei.cn

[U104] JS：防抖
来源：http://sfp.cashguo.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sxa.nanxuanxn.top

[U105] JS：节流
来源：http://eyp.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jtc.hnqzz.top

[U106] JS：日期格式化
来源：http://mta.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qyd.0kj1m.cn

[U107] JS：数字千分位
来源：http://zzh.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ouq.xinyue.icu

[U108] JS：随机整数
来源：http://mck.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://unj.daxiang520.top

[U109] JS：数组分组
来源：http://btz.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://ife.yuxming.cn

[U110] JS：数组分块
来源：http://wwb.jqgufenzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bhx.yueranfly.top

[U111] JS：对象转 Map
来源：http://ycw.tianlin.xyz

new Map(Object.entries(obj))
来源：http://zog.tianlin.xyz

[U112] JS：字符串补位
来源：http://etv.tian-w.cn

"7".padStart(3, "0")
来源：http://rel.yj20258888.top

[U113] JS：正则替换全部
来源：http://vfc.hammf.cn

s.replaceAll("a", "b")
来源：http://kwn.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://dwc.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zoy.yueranfly.top

[U115] JS：生成 UUID
来源：http://zic.jyoumei.cn

crypto.randomUUID()
来源：http://ccm.shanyushiyangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://pmm.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://qjd.gogol.net.cn

[U117] JS：单元测试
来源：http://aik.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://wcj.chenzaomai.com

[U118] JS：开发服务器
来源：http://dta.iojbl.cn

npm i -D vite;  npx vite
来源：http://enb.havefunace.top

[U119] JS：生产构建
来源：http://upx.hfpthk.cn

npx vite build
来源：http://nqh.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://olm.chenjidiqi.icu

import.meta.env.VITE_API_URL
来源：http://ypa.svipenyu.cn

================================================================================
来源：http://roe.chenlongwang.top

统计汇总
来源：http://vwd.yuxming.cn

================================================================================
来源：http://ljo.chenlongwang.top

按语言统计（条）：
来源：http://pzz.svipenyu.cn

Python ......... 252
来源：http://gla.tian-w.cn

PHP ............ 252
来源：http://zdy.svipenyu.cn

JavaScript ..... 252
来源：http://bvs.gotoacloud.top

TypeScript ..... 212
来源：http://crx.c1oappe.top

Java ........... 212
来源：http://vts.0kj1m.cn

Go ............. 212
来源：http://umv.yuanzhike.top

Ruby ........... 212
来源：http://cxs.yj20258.top

C# ............. 212
来源：http://zns.9152youxi.cn

C .............. 30
来源：http://ovs.tanke756.top

C++ ............ 30
来源：http://vmn.jqgufenzy.top

SQL ............ 90
来源：http://yjo.zhixingplan.top

Bash ........... 80
来源：http://vpw.jyoumei.cn

Kotlin ......... 15
来源：http://gjv.0kj1m.cn

Swift .......... 15
来源：http://gzi.yuxming.cn

Lua ............ 10
来源：http://koe.zdqjudy.top

Perl ........... 10
来源：http://nll.hammf.cn

Scala .......... 10
来源：http://rkm.zhixingplan.top

------------------------------------
来源：http://rvu.shangyingyoupin.top

合计 ........... 2106 条
来源：http://tff.hysaishi.cn

按章节统计：
来源：http://igc.nanxinkj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rwd.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nyq.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lse.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ekj.wangdashe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fnf.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mje.chenlongwang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ixw.chenzaomai.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ocl.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sgq.ctjpmb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://urk.nanxinkj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gpa.hammf.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dhv.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zjc.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iwp.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gik.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rqy.dashuyun.cn

Q SQL 专题                              90
来源：http://ida.gzhubu.top

R Bash 专题                             80
来源：http://soe.gzhubu.top

S C / C++ 专题                          60
来源：http://eqg.jyoumei.cn

T 其他语言补充                          60
来源：http://esm.hongshengwenyu.top

U 高频实用片段                         120
来源：http://pel.shzxlz.cn

------------------------------------
来源：http://dfl.9152youxi.cn

合计                                  2106 条
来源：http://yav.smart0.xyz

--------------------------------------------------------------------------------
来源：http://elj.tianlin.xyz

使用提醒
来源：http://euo.tanke756.top

--------------------------------------------------------------------------------
来源：http://qyu.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ivh.pycfn.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zup.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hkr.chenzaomai.com

在旧版本上使用前请先确认语法支持情况。
来源：http://gwb.shuidangran.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://syx.zhengqikj.top

—— 文件结束 ——
来源：http://ixw.tianlin.xyz

================================================================================
来源：http://zbh.ppjwa.cn

程序语言常见例子速查手册（2024 版）
来源：http://bum.zhaomingkeji.xyz

Common Programming Examples Cheat Book
来源：http://fcq.jyoumei.cn

================================================================================
来源：http://ffb.zhengqikj.top

【收录内容】
来源：http://rms.hongshengwenyu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hdt.sxryk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mbi.jianghu66.top

SQL · Bash · C · C++
来源：http://gxw.cashguo.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kmm.yuxming.cn

【使用说明】
来源：http://ynv.jianghu66.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://alr.snrcjt.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kef.ctjpmb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qik.shanyushiyangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cpx.jinghuilouyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kda.hnqzz.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ebo.gogol.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://svd.aibaodan.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://smu.aibaodan.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xes.gogol.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zlj.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vos.bjfxy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zsa.jinyuanbaomall.cn

【文件统计】
来源：http://ezj.nanxinkj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qqp.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://lta.hysaishi.cn

目  录
来源：http://jkv.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://xey.iojbl.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tca.zhijiandao.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xyq.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://quq.hnxiangtu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tyk.c1oappe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vts.jinqigufen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kjv.sweek.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xjy.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://csj.tarul.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://muo.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kby.bbcook.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ftd.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://loq.yuanzhike.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yhx.xuanzx.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hnd.yangfankeji.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rpe.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tje.tanke756.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hjp.gaohongyu789.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ivl.aizwys.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fny.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fij.xingfuxueyuan.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vyw.hcnkem.com

================================================================================
来源：http://ilg.ehwqpu.com

A. 基础语法与类型
来源：http://ugk.zdbjq.cn

================================================================================
来源：http://ich.birdmap.top

[A01] Hello World
来源：http://bsq.zhongyouzk.top

Py:   print("Hello, World!")
来源：http://fbf.jinghuilouyu.cn

PHP:  echo "Hello, World!";
来源：http://opp.hysaishi.cn

JS:   console.log("Hello, World!");
来源：http://unw.fzhhl.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gym.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://mxa.ppjwa.cn

Go:   fmt.Println("Hello, World!")
来源：http://vjy.xuetiantiany.cn

Ruby: puts "Hello, World!"
来源：http://yln.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ttf.hcnkem.com

[A02] 变量声明与赋值
来源：http://jeu.chenzaomai.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mbn.uphjek.com

PHP:  $name = "Alex"; $age = 20;
来源：http://hxf.guannengcc.top

JS:   let name = "Alex"; const age = 20;
来源：http://vpv.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jge.yangfankeji.com

Java: String name = "Alex"; int age = 20;
来源：http://uwv.quarkkingdee.top

Go:   name := "Alex"; age := 20
来源：http://vxn.52xcode.cn

Ruby: name = "Alex"; age = 20
来源：http://wpb.zdqjudy.top

C#:   string name = "Alex"; int age = 20;
来源：http://zfv.316326.xyz

[A03] 常量定义
来源：http://thz.ydjk.org.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ngn.zhongyouzk.top

PHP:  const PI = 3.14159;
来源：http://zed.daxiang520.top

JS:   const PI = 3.14159;
来源：http://dth.hammf.cn

TS:   const PI: number = 3.14159;
来源：http://mtk.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://lao.cdnleiting.top

Go:   const PI = 3.14159
来源：http://oxd.ppjwa.cn

Ruby: PI = 3.14159
来源：http://eoc.zhixingplan.top

C#:   const double PI = 3.14159;
来源：http://dti.mhx1999.top

[A04] 判断变量类型
来源：http://ewd.bjfxy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://uvq.pengpengdd.cyou

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qel.fanxiaobao.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://woy.nwbrower.top

TS:   typeof x; x instanceof Date
来源：http://znq.52xcode.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ssr.c1oappe.top

Go:   reflect.TypeOf(x).Name()
来源：http://iea.zhixingplan.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ncz.hnxiangtu.top

C#:   x.GetType().Name; x is int
来源：http://ikk.cdnleiting.top

[A05] 整数除法与取模
来源：http://fpy.ivvv.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gez.xuanzx.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://bia.ydzc1.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://opq.yuanzhike.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gvk.zdbjq.cn

Java: 7 / 2; 7 % 2
来源：http://pvp.shangyingyoupin.top

Go:   7 / 2; 7 % 2
来源：http://jmv.gogol.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://zka.hesvh.cn

C#:   7 / 2; 7 % 2
来源：http://efj.hnqzz.top

[A06] 字符串转数字
来源：http://ydg.hnqzz.top

Py:   int("42"); float("3.14")
来源：http://vfq.cdnleiting.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tro.hywenlv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://djl.vehdjk.com

TS:   parseInt("42", 10); Number("42")
来源：http://vfv.andypj.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://poi.havefunace.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tlf.aibaodan.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bsu.cqqwz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vwn.xziqi.cn

[A07] 数字转字符串
来源：http://efy.sweek.top

Py:   str(42)
来源：http://chg.0kj1m.cn

PHP:  (string) 42; strval(42)
来源：http://jmj.ivvv.top

JS:   String(42); (42).toString()
来源：http://qyp.zhaomingkeji.xyz

TS:   String(42)
来源：http://yka.vehdjk.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://utm.fktsv.cn

Go:   strconv.Itoa(42)
来源：http://tne.yonumen.top

Ruby: 42.to_s
来源：http://fpi.gzhubu.top

C#:   42.ToString()
来源：http://cvh.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://bff.xinyue.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ktz.zhoulong.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://btg.gzhubu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zui.daria6918.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ann.shanyushiyangtech.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nff.sxryk.cn


<!-- 参考信息 -->