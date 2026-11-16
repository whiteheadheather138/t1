代发 wailian999

[U59] PHP：自定义排序
来源：http://pnf.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vtv.zhongyouzk.top

[U60] PHP：JSON 编解码
来源：http://esw.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kcv.zhaomingkeji.xyz

[U61] PHP：正则
来源：http://yxg.jlsjyb.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ger.gotoacloud.top

[U62] PHP：日期对象
来源：http://apf.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dvn.aibaodan.cn

[U63] PHP：文件读写
来源：http://yxx.316326.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qxo.jqgfzy.top

[U64] PHP：目录遍历
来源：http://iho.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://obv.fktsv.cn

[U65] PHP：会话
来源：http://gph.smart0.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://xxq.yongpay.top

[U66] PHP：设置 Cookie
来源：http://nhx.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bdw.yuxming.cn

[U67] PHP：处理文件上传
来源：http://ovg.316326.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ugd.pycfn.com

[U68] PHP：PDO 连接
来源：http://xzo.ywan-chungtsiang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tin.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://qwv.iojbl.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fyz.c1oappe.top

[U70] PHP：PDO 事务
来源：http://stn.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yun.guowangkeji.top

[U71] PHP：抛出异常
来源：http://hyt.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://byh.cdnleiting.top

[U72] PHP：写错误日志
来源：http://csi.zycfv.cn

error_log("失败: " . $e->getMessage());
来源：http://ruq.hesvh.cn

[U73] PHP：读取 ini 配置
来源：http://zre.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://our.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://ttq.guannengcc.top

getenv("APP_ENV") ?: "production"
来源：http://vcb.chenzaomai.com

[U75] PHP：依赖注入
来源：http://rfw.zycfv.cn

composer require psr/container
来源：http://hoj.xziqi.cn

[U76] PHP：简单路由
来源：http://upa.xziqi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ndi.hammf.cn

[U77] PHP：模板渲染
来源：http://cah.zhengqikj.top

composer require twig/twig
来源：http://ebr.gogol.net.cn

[U78] PHP：单元测试
来源：http://rlh.zhoulong.xyz

composer require --dev phpunit/phpunit
来源：http://skp.meibo888.top

[U79] PHP：静态分析
来源：http://mlh.jianghu66.top

composer require --dev phpstan/phpstan
来源：http://bhe.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://pip.gotoacloud.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tqn.hesvh.cn

[U81] JS：初始化项目
来源：http://bcp.fanxiaobao.xyz

npm init -y;  npm i express
来源：http://bus.cheryme.top

[U82] JS：package.json 脚本
来源：http://jic.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gky.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://ohm.jianghu66.top

export const a = 1;  import { a } from "./m.js";
来源：http://bbp.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://vuh.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://quz.yfazqb.com

[U85] JS：可选链
来源：http://fal.xuetiantiany.cn

a?.b?.c
来源：http://obg.zhongyouzk.top

[U86] JS：空值合并
来源：http://pbp.ivvv.top

a ?? b
来源：http://kka.chenjidiqi.icu

[U87] JS：解构默认值
来源：http://jpz.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://wdw.sysykeji.top

[U88] JS：对象展开合并
来源：http://mmw.sjlbkw.cn

{ ...a, ...b }
来源：http://jab.pycfn.com

[U89] JS：数组去重
来源：http://aqd.epnwcf.com

[...new Set(arr)]
来源：http://ael.snrcjt.cn

[U90] JS：数字数组排序
来源：http://xle.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://tkq.ivvv.top

[U91] JS：对象键值遍历
来源：http://hzx.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nko.cheryme.top

[U92] JS：深拷贝
来源：http://ndr.jinghuilouyu.cn

structuredClone(obj)
来源：http://nzb.jqgufenzy.top

[U93] JS：模板字符串
来源：http://ghw.zhixingplan.top

`共 ${n} 条`
来源：http://bdx.aibaodan.cn

[U94] JS：箭头函数
来源：http://nnv.yvedp.cn

const double = x => x * 2;
来源：http://rvj.gzhubu.top

[U95] JS：Promise 包装
来源：http://meq.fehbvm.com

new Promise((resolve, reject) => {})
来源：http://kxl.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://dsc.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nsz.yueranfly.top

[U97] JS：并发请求
来源：http://xlh.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://awv.zdqjudy.top

[U98] JS：fetch 带 JSON
来源：http://vuj.ydjk.org.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ryu.yonumen.top

[U99] JS：事件监听
来源：http://qmf.yj20258888.top

el.addEventListener("click", e => {})
来源：http://acq.jinqigufen.top

[U100] JS：DOM 查询
来源：http://dil.yfazqb.com

document.querySelector(".item")
来源：http://eks.jinyuanbaomall.cn

[U101] JS：classList 操作
来源：http://erz.guannengcc.top

el.classList.toggle("active")
来源：http://dzs.hywenlv.cn

[U102] JS：本地存储
来源：http://eyp.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jee.jyoumei.cn

[U103] JS：定时器
来源：http://dph.9152youxi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://psa.jinghuilouyu.cn

[U104] JS：防抖
来源：http://lsg.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zbd.hysaishi.cn

[U105] JS：节流
来源：http://qjn.hongshengwenyu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fnq.dianchejie.cn

[U106] JS：日期格式化
来源：http://vyw.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lei.jqgfzy.top

[U107] JS：数字千分位
来源：http://bqu.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bvl.jinqigufen.top

[U108] JS：随机整数
来源：http://gew.wangshuangyany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gij.9152youxi.cn

[U109] JS：数组分组
来源：http://xnf.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://kww.ctjpmb.com

[U110] JS：数组分块
来源：http://hxb.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gcn.fktsv.cn

[U111] JS：对象转 Map
来源：http://dck.ivvv.top

new Map(Object.entries(obj))
来源：http://rrt.yueranfly.top

[U112] JS：字符串补位
来源：http://mqh.jlsjyb.cn

"7".padStart(3, "0")
来源：http://onl.tian-w.cn

[U113] JS：正则替换全部
来源：http://lfi.chenzaomai.com

s.replaceAll("a", "b")
来源：http://ivl.cdnleiting.top

[U114] JS：JSON 深比较
来源：http://ewp.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gor.zhixingplan.top

[U115] JS：生成 UUID
来源：http://zte.guowangkeji.top

crypto.randomUUID()
来源：http://lbo.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://ggy.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://muw.yfazqb.com

[U117] JS：单元测试
来源：http://zbd.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://ste.yj202588.top

[U118] JS：开发服务器
来源：http://cza.zhengqikj.top

npm i -D vite;  npx vite
来源：http://ryr.yangfankeji.com

[U119] JS：生产构建
来源：http://liw.shangyingyoupin.top

npx vite build
来源：http://lko.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://epj.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://tcm.jqgufenzy.top

================================================================================
来源：http://ome.mhx1999.top

统计汇总
来源：http://htf.yuanzhike.top

================================================================================
来源：http://quh.pengpengdd.cyou

按语言统计（条）：
来源：http://vyf.dashuyun.cn

Python ......... 252
来源：http://iru.aizwys.cn

PHP ............ 252
来源：http://rto.bjfxy.top

JavaScript ..... 252
来源：http://twj.tarul.cn

TypeScript ..... 212
来源：http://gmm.kuanghao11.cn

Java ........... 212
来源：http://lxi.jinyuanbaomall.cn

Go ............. 212
来源：http://sww.bbcook.cn

Ruby ........... 212
来源：http://tbk.yuanzhike.top

C# ............. 212
来源：http://tli.aizwys.cn

C .............. 30
来源：http://oho.yonumen.top

C++ ............ 30
来源：http://ubn.xinyue.icu

SQL ............ 90
来源：http://thr.chenjidiqi.icu

Bash ........... 80
来源：http://jet.guannengcc.top

Kotlin ......... 15
来源：http://qfl.pycfn.com

Swift .......... 15
来源：http://zbx.ctjpmb.com

Lua ............ 10
来源：http://eyv.pycfn.com

Perl ........... 10
来源：http://tvy.xinyue.icu

Scala .......... 10
来源：http://oif.cdnleiting.top

------------------------------------
来源：http://wjt.yj20258888.top

合计 ........... 2106 条
来源：http://rmb.birdmap.top

按章节统计：
来源：http://vrl.havefunace.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cly.yanxiufei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rxd.mhx1999.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rkn.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hts.ydzc1.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pri.shangyingyoupin.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://trr.svipenyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jkg.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gud.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://irr.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dzp.shzxlz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sml.aizwys.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ebn.tanke756.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://reb.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tuj.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zip.zhengqikj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vky.fehbvm.com

Q SQL 专题                              90
来源：http://joe.zhixingplan.top

R Bash 专题                             80
来源：http://gjg.jinqigufen.top

S C / C++ 专题                          60
来源：http://toj.jqgfzy.top

T 其他语言补充                          60
来源：http://khx.aibaodan.cn

U 高频实用片段                         120
来源：http://nle.epnwcf.com

------------------------------------
来源：http://tog.jinqigfzy.top

合计                                  2106 条
来源：http://ckr.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://wfb.kuanghao11.cn

使用提醒
来源：http://csb.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://kfi.hysaishi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cjn.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hnj.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wdw.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://eyj.hfpthk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hls.epnwcf.com

—— 文件结束 ——
来源：http://wqq.316326.xyz

================================================================================
来源：http://zua.cucudq.cn

程序语言常见例子速查手册（2024 版）
来源：http://dlv.xuetiantiany.cn

Common Programming Examples Cheat Book
来源：http://sao.birdmap.top

================================================================================
来源：http://hsv.xuanzx.com

【收录内容】
来源：http://wps.tarul.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fba.tarul.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wyw.xziqi.cn

SQL · Bash · C · C++
来源：http://apr.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://psk.ydjk.org.cn

【使用说明】
来源：http://kox.yonumen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vpj.gogol.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uag.wangdashe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mzr.52xcode.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xew.yangfankeji.com

Bash:  Shell         C:     C             C++:   C++
来源：http://xfm.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rge.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bew.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fpn.ppjwa.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wng.hysaishi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zlm.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iec.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ygq.jqgfzy.top

【文件统计】
来源：http://akw.yj20258.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hxf.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://cbv.yuxming.cn

目  录
来源：http://gnw.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://bxd.sysykeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rnv.gotoacloud.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tpj.sweek.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pre.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bmf.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qdn.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rmt.hesvh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qsg.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gkd.ydzc1.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://goe.zhengqikj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bby.jiagoushi.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xyt.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fit.sysykeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tiu.yj20258.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wvc.birdmap.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jly.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gtc.yueranfly.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wud.gzhubu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zbz.tian-w.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ffv.zdqjudy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tdp.ywan-chungtsiang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fxb.sysykeji.top

================================================================================
来源：http://igq.cashguo.top

A. 基础语法与类型
来源：http://qgb.fzhhl.top

================================================================================
来源：http://vbt.ivvv.top

[A01] Hello World
来源：http://vmk.chenjidiqi.icu

Py:   print("Hello, World!")
来源：http://uzo.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://xcj.zhoulong.xyz

JS:   console.log("Hello, World!");
来源：http://eho.yangfankeji.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rzy.jlsjyb.cn

Java: System.out.println("Hello, World!");
来源：http://uus.52xcode.cn

Go:   fmt.Println("Hello, World!")
来源：http://fsl.ybcxt.top

Ruby: puts "Hello, World!"
来源：http://flj.ppjwa.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://imt.chenzaomai.com

[A02] 变量声明与赋值
来源：http://mxr.iojbl.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rxj.tanke756.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ejn.kuanghao11.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yew.jinqigfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jml.yj20258888.top

Java: String name = "Alex"; int age = 20;
来源：http://tbm.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://yvm.shuidangran.top

Ruby: name = "Alex"; age = 20
来源：http://aip.birdmap.top

C#:   string name = "Alex"; int age = 20;
来源：http://vjj.jlsjyb.cn

[A03] 常量定义
来源：http://bnd.sjlbkw.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qnz.kuanghao11.cn

PHP:  const PI = 3.14159;
来源：http://ahy.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://qbs.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://szd.fengsongda.top

Java: static final double PI = 3.14159;
来源：http://izs.xingfuxueyuan.xyz

Go:   const PI = 3.14159
来源：http://lqy.nanxuanxn.top

Ruby: PI = 3.14159
来源：http://yjn.yongpay.top

C#:   const double PI = 3.14159;
来源：http://hon.chenlongwang.top

[A04] 判断变量类型
来源：http://ssd.yuanzhike.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mad.daxiang520.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qsp.hysaishi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yow.mhx1999.top

TS:   typeof x; x instanceof Date
来源：http://tjb.redwolf501.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pgl.zhongyouzk.top

Go:   reflect.TypeOf(x).Name()
来源：http://snl.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kzx.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://eea.havefunace.top

[A05] 整数除法与取模
来源：http://ggl.daria6918.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lrw.shanyushiyangtech.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jih.yuanzhike.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fqk.shanyushiyangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://omj.andypj.xyz

Java: 7 / 2; 7 % 2
来源：http://qdj.c1oappe.top

Go:   7 / 2; 7 % 2
来源：http://xqf.daxiang520.top

Ruby: 7 / 2; 7 % 2
来源：http://wlt.bbcook.cn

C#:   7 / 2; 7 % 2
来源：http://xqy.dianchejie.cn

[A06] 字符串转数字
来源：http://qkt.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://zqe.tarul.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://shy.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uie.xinyue.icu

TS:   parseInt("42", 10); Number("42")
来源：http://yvq.zhiwuduotai.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gfx.feifeiyinyue.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lmw.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://yto.zhoulong.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zeh.sxryk.cn

[A07] 数字转字符串
来源：http://rhr.gaohongyu789.top

Py:   str(42)
来源：http://map.mhx1999.top

PHP:  (string) 42; strval(42)
来源：http://zcr.birdmap.top

JS:   String(42); (42).toString()
来源：http://xxh.sysykeji.top

TS:   String(42)
来源：http://wkj.ppjwa.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://okv.gzhubu.top

Go:   strconv.Itoa(42)
来源：http://mbs.cqqwz.cn

Ruby: 42.to_s
来源：http://qgh.9152youxi.cn

C#:   42.ToString()
来源：http://kxc.zycfv.cn

[A08] 取整与四舍五入
来源：http://zmo.cdnleiting.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ybr.cucudq.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://azz.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://elw.ybcxt.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lsa.zdqjudy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pkb.gzhubu.top


<!-- 参考信息 -->