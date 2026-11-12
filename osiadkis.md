代发 wailian999

[U51] PHP：数组解构
来源：http://hxl.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://ywk.tanke756.top

[U52] PHP：箭头函数
来源：http://ieo.nwbrower.top

$double = fn($x) => $x * 2;
来源：http://bmo.zhixingplan.top

[U53] PHP：空合并运算符
来源：http://rky.sxryk.cn

$v = $a ?? $b ?? "default";
来源：http://wga.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://ndo.chenjidiqi.icu

$obj?->method()
来源：http://ubm.gogol.net.cn

[U55] PHP：match 表达式
来源：http://ynk.jlsjyb.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xgp.wangdashe.top

[U56] PHP：命名参数
来源：http://dfw.316326.xyz

f(a: 1, b: 2)
来源：http://qsd.gzhubu.top

[U57] PHP：字符串插值
来源：http://lcx.tianlin.xyz

"值: {$a}"
来源：http://qic.xylfe.cn

[U58] PHP：数组三件套
来源：http://oyj.feifeiyinyue.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bzm.jiagoushi.top

[U59] PHP：自定义排序
来源：http://ves.bbcook.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://evv.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://xzj.zdqjudy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ykl.yvedp.cn

[U61] PHP：正则
来源：http://gpn.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://llu.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://jli.hnqzz.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lqj.hammf.cn

[U63] PHP：文件读写
来源：http://uxg.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ngr.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://pca.feifeiyinyue.top

glob("dir/*.php");  scandir("dir");
来源：http://wkd.uphjek.com

[U65] PHP：会话
来源：http://kyb.nanxuanxn.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ctz.fehbvm.com

[U66] PHP：设置 Cookie
来源：http://wek.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qfm.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://fgy.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jlj.0kj1m.cn

[U68] PHP：PDO 连接
来源：http://jpy.shzxlz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ial.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://qyb.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eow.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://gto.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ipl.9152youxi.cn

[U71] PHP：抛出异常
来源：http://xfs.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://dbh.daria6918.cn

[U72] PHP：写错误日志
来源：http://opo.yj20258888.top

error_log("失败: " . $e->getMessage());
来源：http://wps.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://msc.chenlongwang.top

parse_ini_file("config.ini", true)
来源：http://vzu.andypj.xyz

[U74] PHP：读取环境变量
来源：http://zdg.hywenlv.cn

getenv("APP_ENV") ?: "production"
来源：http://xph.9152youxi.cn

[U75] PHP：依赖注入
来源：http://gmk.gogol.net.cn

composer require psr/container
来源：http://hcw.dianchejie.cn

[U76] PHP：简单路由
来源：http://zxr.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://scb.zhixingplan.top

[U77] PHP：模板渲染
来源：http://ilg.jyoumei.cn

composer require twig/twig
来源：http://ean.hfpthk.cn

[U78] PHP：单元测试
来源：http://yiz.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://pub.jyoumei.cn

[U79] PHP：静态分析
来源：http://uhb.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://cam.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://fkw.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://xwv.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://gzn.epnwcf.com

npm init -y;  npm i express
来源：http://nps.sxryk.cn

[U82] JS：package.json 脚本
来源：http://nnj.jqgfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pog.daxiang520.top

[U83] JS：ES Module 导入导出
来源：http://xse.fzhhl.top

export const a = 1;  import { a } from "./m.js";
来源：http://tvs.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://oyk.daria6918.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ufl.aizwys.cn

[U85] JS：可选链
来源：http://mdf.jlsjyb.cn

a?.b?.c
来源：http://tcd.fanxiaobao.xyz

[U86] JS：空值合并
来源：http://ufd.gzhubu.top

a ?? b
来源：http://ryy.jinqigfzy.top

[U87] JS：解构默认值
来源：http://xup.hammf.cn

const { a = 1, b = 2 } = obj;
来源：http://cyf.vehdjk.com

[U88] JS：对象展开合并
来源：http://tzo.xingfuxueyuan.xyz

{ ...a, ...b }
来源：http://dah.tarul.cn

[U89] JS：数组去重
来源：http://ywe.316326.xyz

[...new Set(arr)]
来源：http://hbi.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://ert.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://flf.pycfn.com

[U91] JS：对象键值遍历
来源：http://bfe.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ixf.epnwcf.com

[U92] JS：深拷贝
来源：http://dlp.xingfuxueyuan.xyz

structuredClone(obj)
来源：http://iiq.xziqi.cn

[U93] JS：模板字符串
来源：http://zex.xuanzx.com

`共 ${n} 条`
来源：http://oxf.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://jnp.sysykeji.top

const double = x => x * 2;
来源：http://crf.cqqwz.cn

[U95] JS：Promise 包装
来源：http://bpb.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://eel.52xcode.cn

[U96] JS：async/await 与异常
来源：http://eld.shangyingyoupin.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gop.dashuyun.cn

[U97] JS：并发请求
来源：http://dwt.jinghuilouyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://koc.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://tns.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://krf.cqqwz.cn

[U99] JS：事件监听
来源：http://zlj.hnqzz.top

el.addEventListener("click", e => {})
来源：http://hxf.tarul.cn

[U100] JS：DOM 查询
来源：http://ase.xylfe.cn

document.querySelector(".item")
来源：http://uyc.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://oai.guowangkeji.top

el.classList.toggle("active")
来源：http://sjy.hnqzz.top

[U102] JS：本地存储
来源：http://owo.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://phl.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://zyv.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://drz.chenjidiqi.icu

[U104] JS：防抖
来源：http://sav.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eqg.cqqwz.cn

[U105] JS：节流
来源：http://qbj.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://upd.zycfv.cn

[U106] JS：日期格式化
来源：http://avj.ydzc1.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://avp.yfazqb.com

[U107] JS：数字千分位
来源：http://gex.yangfankeji.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xfn.hnxiangtu.top

[U108] JS：随机整数
来源：http://wjg.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qqo.hnqzz.top

[U109] JS：数组分组
来源：http://qyq.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://iqy.chenzaomai.com

[U110] JS：数组分块
来源：http://wwk.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uum.ppjwa.cn

[U111] JS：对象转 Map
来源：http://yyg.birdmap.top

new Map(Object.entries(obj))
来源：http://tsw.tanke756.top

[U112] JS：字符串补位
来源：http://umk.cheryme.top

"7".padStart(3, "0")
来源：http://exp.hywenlv.cn

[U113] JS：正则替换全部
来源：http://kbo.zdqjudy.top

s.replaceAll("a", "b")
来源：http://hsc.sufxvd.cn

[U114] JS：JSON 深比较
来源：http://oie.nanxuanxn.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dwx.iojbl.cn

[U115] JS：生成 UUID
来源：http://hpv.shangyingyoupin.top

crypto.randomUUID()
来源：http://pwf.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://ijq.ctjpmb.com

/** @param {string} name */ function f(name) {}
来源：http://dha.guannengcc.top

[U117] JS：单元测试
来源：http://jfn.sweek.top

npm i -D vitest;  npx vitest
来源：http://kzt.guowangkeji.top

[U118] JS：开发服务器
来源：http://bmi.sjlbkw.cn

npm i -D vite;  npx vite
来源：http://edi.pengpengdd.cyou

[U119] JS：生产构建
来源：http://glo.tianlin.xyz

npx vite build
来源：http://laq.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://ojg.vqdsnc.cn

import.meta.env.VITE_API_URL
来源：http://zbp.gaohongyu789.top

================================================================================
来源：http://mlg.52xcode.cn

统计汇总
来源：http://pow.shuidangran.top

================================================================================
来源：http://plt.316326.xyz

按语言统计（条）：
来源：http://xke.yongpay.top

Python ......... 252
来源：http://zis.hysaishi.cn

PHP ............ 252
来源：http://ewa.xuetiantiany.cn

JavaScript ..... 252
来源：http://dcx.tarul.cn

TypeScript ..... 212
来源：http://sgb.aizwys.cn

Java ........... 212
来源：http://vna.cqqwz.cn

Go ............. 212
来源：http://dih.xuetiantiany.cn

Ruby ........... 212
来源：http://sil.zycfv.cn

C# ............. 212
来源：http://eyj.guannengcc.top

C .............. 30
来源：http://ehv.xinyue.icu

C++ ............ 30
来源：http://ost.tianlin.xyz

SQL ............ 90
来源：http://jfx.xylfe.cn

Bash ........... 80
来源：http://wyx.cdnleiting.top

Kotlin ......... 15
来源：http://zmt.ehwqpu.com

Swift .......... 15
来源：http://eta.cashguo.top

Lua ............ 10
来源：http://grw.nanxinkj.top

Perl ........... 10
来源：http://wxk.quarkkingdee.top

Scala .......... 10
来源：http://tcm.yueranfly.top

------------------------------------
来源：http://qvc.gzhubu.top

合计 ........... 2106 条
来源：http://pzx.gotoacloud.top

按章节统计：
来源：http://brb.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zlv.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sxc.sufxvd.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wnz.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://onz.hfpthk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mgu.xinyue.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nen.hongshengwenyu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rev.cashguo.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ciw.316326.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://obj.ydzc1.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nhd.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fhk.gzhubu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zsi.fehbvm.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wuk.dashuyun.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iui.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rwa.yangfankeji.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pfw.zdbjq.cn

Q SQL 专题                              90
来源：http://vly.yueranfly.top

R Bash 专题                             80
来源：http://yef.52xcode.cn

S C / C++ 专题                          60
来源：http://mpb.fktsv.cn

T 其他语言补充                          60
来源：http://mww.haohaochexian.top

U 高频实用片段                         120
来源：http://oux.aibaodan.cn

------------------------------------
来源：http://fzg.yueranfly.top

合计                                  2106 条
来源：http://lqb.xinyue.icu

--------------------------------------------------------------------------------
来源：http://gkb.redwolf501.top

使用提醒
来源：http://vuk.hammf.cn

--------------------------------------------------------------------------------
来源：http://jfe.ctjpmb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dcr.jinqigufen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jpy.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://erh.tanke756.top

在旧版本上使用前请先确认语法支持情况。
来源：http://psk.wangshuangyany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jgm.vqdsnc.cn

—— 文件结束 ——
来源：http://uel.yj20258.top

================================================================================
来源：http://bwm.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://ibu.zhengqikj.top

Common Programming Examples Cheat Book
来源：http://hgm.zhoulong.xyz

================================================================================
来源：http://yaq.cqqwz.cn

【收录内容】
来源：http://gvo.gotoacloud.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hig.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rnd.yj202588.top

SQL · Bash · C · C++
来源：http://kif.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qna.zhijiandao.cn

【使用说明】
来源：http://odn.yvedp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cwz.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tpf.zycfv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gmi.nanxinkj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iws.kuanghao11.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kso.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bfi.zhongyouzk.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cmj.vqdsnc.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pkm.ybcxt.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://exd.andypj.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fjf.vehdjk.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lzw.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yhz.jyoumei.cn

【文件统计】
来源：http://udg.wangshuangyany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ekp.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://qxk.ydjk.org.cn

目  录
来源：http://xnk.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://jvx.nanxinkj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kjp.cdnleiting.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gbp.hywenlv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ttf.shuidangran.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sls.tanke756.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bbn.feifeiyinyue.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://egc.hcnkem.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eco.9152youxi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://txy.epnwcf.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gpd.jinqigufen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uzi.yj20258.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lrr.zhaomingkeji.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fdd.jyoumei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tve.yuxming.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tbf.yj20258.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pyv.snrcjt.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ssf.bjfxy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mzb.jinqigfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ywl.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zjc.feifeiyinyue.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hmj.fktsv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kml.wangshuangyany.cn

================================================================================
来源：http://xkm.redwolf501.top

A. 基础语法与类型
来源：http://qry.jyoumei.cn

================================================================================
来源：http://gss.zhijiandao.cn

[A01] Hello World
来源：http://qhe.aizwys.cn

Py:   print("Hello, World!")
来源：http://awq.jianghu66.top

PHP:  echo "Hello, World!";
来源：http://dsi.yongpay.top

JS:   console.log("Hello, World!");
来源：http://lun.vehdjk.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yjl.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://mza.tian-w.cn

Go:   fmt.Println("Hello, World!")
来源：http://dcj.wangdashe.top

Ruby: puts "Hello, World!"
来源：http://dpl.fktsv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://szs.xuetiantiany.cn

[A02] 变量声明与赋值
来源：http://fin.yj20258.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qgb.chenzaomai.com

PHP:  $name = "Alex"; $age = 20;
来源：http://mdd.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kmw.hongshengwenyu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uzl.hfpthk.cn

Java: String name = "Alex"; int age = 20;
来源：http://fig.fktsv.cn

Go:   name := "Alex"; age := 20
来源：http://bwl.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://zkq.iojbl.cn

C#:   string name = "Alex"; int age = 20;
来源：http://maw.wangshuangyany.cn

[A03] 常量定义
来源：http://hsn.xinyue.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ewh.uphjek.com

PHP:  const PI = 3.14159;
来源：http://pol.xuanzx.com

JS:   const PI = 3.14159;
来源：http://ymk.xinyue.icu

TS:   const PI: number = 3.14159;
来源：http://vtq.kuanghao11.cn

Java: static final double PI = 3.14159;
来源：http://tjq.jyoumei.cn

Go:   const PI = 3.14159
来源：http://aim.ehwqpu.com

Ruby: PI = 3.14159
来源：http://hso.meibo888.top

C#:   const double PI = 3.14159;
来源：http://ogf.shanyushiyangtech.top

[A04] 判断变量类型
来源：http://xqb.andypj.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://gce.0kj1m.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dru.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oer.jinghuilouyu.cn

TS:   typeof x; x instanceof Date
来源：http://cfe.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zpi.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://phi.yuanzhike.top

Ruby: x.class; x.is_a?(Integer)
来源：http://whr.cucudq.cn

C#:   x.GetType().Name; x is int
来源：http://itu.svipenyu.cn

[A05] 整数除法与取模
来源：http://frn.hywenlv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jvk.aibaodan.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qih.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jtw.316326.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yqz.hywenlv.cn

Java: 7 / 2; 7 % 2
来源：http://tvi.xylfe.cn

Go:   7 / 2; 7 % 2
来源：http://yfu.shanyushiyangtech.top

Ruby: 7 / 2; 7 % 2
来源：http://dvy.zhengqikj.top

C#:   7 / 2; 7 % 2
来源：http://rsm.zycfv.cn

[A06] 字符串转数字
来源：http://qgo.0kj1m.cn

Py:   int("42"); float("3.14")
来源：http://pho.xylfe.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://utw.jlsjyb.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://flr.zhixingplan.top

TS:   parseInt("42", 10); Number("42")
来源：http://dwz.daxiang520.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jrn.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gfy.shanyushiyangtech.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jxg.chenjidiqi.icu


<!-- 参考信息 -->