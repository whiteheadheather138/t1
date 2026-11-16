代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://rlp.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lev.xylfe.cn

[U46] PHP：可空类型
来源：http://ltx.smart0.xyz

?string $name = null
来源：http://sex.xinyue.icu

[U47] PHP：联合类型
来源：http://ncg.tianlin.xyz

int|string $id
来源：http://phn.cucudq.cn

[U48] PHP：纯枚举
来源：http://xvb.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vsk.hammf.cn

[U49] PHP：只读属性
来源：http://tzc.ywan-chungtsiang.top

public readonly string $name
来源：http://wkw.sweek.top

[U50] PHP：构造器属性提升
来源：http://gdv.pycfn.com

public function __construct(private int $id) {}
来源：http://xif.vqdsnc.cn

[U51] PHP：数组解构
来源：http://igc.iojbl.cn

[$a, $b] = $arr;
来源：http://ldp.hcnkem.com

[U52] PHP：箭头函数
来源：http://bgd.bjfxy.top

$double = fn($x) => $x * 2;
来源：http://qpt.feifeiyinyue.top

[U53] PHP：空合并运算符
来源：http://mty.ctjpmb.com

$v = $a ?? $b ?? "default";
来源：http://rjv.fktsv.cn

[U54] PHP：空安全调用
来源：http://zrq.zhiwuduotai.top

$obj?->method()
来源：http://xqy.sxryk.cn

[U55] PHP：match 表达式
来源：http://dcc.jlsjyb.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tzp.vqdsnc.cn

[U56] PHP：命名参数
来源：http://chz.vehdjk.com

f(a: 1, b: 2)
来源：http://vqh.shangyingyoupin.top

[U57] PHP：字符串插值
来源：http://jba.bjfxy.top

"值: {$a}"
来源：http://lxc.hongshengwenyu.top

[U58] PHP：数组三件套
来源：http://xbc.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tsi.ctjpmb.com

[U59] PHP：自定义排序
来源：http://hqt.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qne.fzhhl.top

[U60] PHP：JSON 编解码
来源：http://nja.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pss.zycfv.cn

[U61] PHP：正则
来源：http://tqu.ctjpmb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wqp.gzhubu.top

[U62] PHP：日期对象
来源：http://wyc.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qgq.ybcxt.top

[U63] PHP：文件读写
来源：http://qoh.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uli.hnqzz.top

[U64] PHP：目录遍历
来源：http://lgr.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://dmg.chenlongwang.top

[U65] PHP：会话
来源：http://rbt.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://lmu.yongpay.top

[U66] PHP：设置 Cookie
来源：http://lkd.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pne.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://byj.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wew.dianchejie.cn

[U68] PHP：PDO 连接
来源：http://ieu.ehwqpu.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qfb.ivvv.top

[U69] PHP：PDO 预处理
来源：http://zrw.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zfm.quarkkingdee.top

[U70] PHP：PDO 事务
来源：http://axc.pengpengdd.cyou

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://alh.gzhubu.top

[U71] PHP：抛出异常
来源：http://tyl.zdbjq.cn

throw new RuntimeException("失败", 500);
来源：http://zqb.ybcxt.top

[U72] PHP：写错误日志
来源：http://plv.yueranfly.top

error_log("失败: " . $e->getMessage());
来源：http://zkk.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://qre.yuanzhike.top

parse_ini_file("config.ini", true)
来源：http://yyo.yongpay.top

[U74] PHP：读取环境变量
来源：http://opw.aizwys.cn

getenv("APP_ENV") ?: "production"
来源：http://oqn.hcnkem.com

[U75] PHP：依赖注入
来源：http://wid.jinghuilouyu.cn

composer require psr/container
来源：http://acs.52xcode.cn

[U76] PHP：简单路由
来源：http://vql.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hmi.sxryk.cn

[U77] PHP：模板渲染
来源：http://cha.chenzaomai.com

composer require twig/twig
来源：http://sta.jianghu66.top

[U78] PHP：单元测试
来源：http://yzh.52xcode.cn

composer require --dev phpunit/phpunit
来源：http://vce.c1oappe.top

[U79] PHP：静态分析
来源：http://lxf.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://kdt.yanxiufei.cn

[U80] PHP：代码规范修复
来源：http://lna.fktsv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hhh.sysykeji.top

[U81] JS：初始化项目
来源：http://nxa.gaohongyu789.top

npm init -y;  npm i express
来源：http://yen.hfpthk.cn

[U82] JS：package.json 脚本
来源：http://bey.ctjpmb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nxm.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://zvg.9152youxi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://txi.nanxinkj.top

[U84] JS：CommonJS 写法
来源：http://dke.hesvh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://btq.jqgufenzy.top

[U85] JS：可选链
来源：http://afd.yfazqb.com

a?.b?.c
来源：http://vzt.hywenlv.cn

[U86] JS：空值合并
来源：http://uha.svipenyu.cn

a ?? b
来源：http://uuc.sjlbkw.cn

[U87] JS：解构默认值
来源：http://rmy.yj20258.top

const { a = 1, b = 2 } = obj;
来源：http://mif.zhixingplan.top

[U88] JS：对象展开合并
来源：http://mvq.jqgufenzy.top

{ ...a, ...b }
来源：http://dda.tarul.cn

[U89] JS：数组去重
来源：http://cpy.hesvh.cn

[...new Set(arr)]
来源：http://kpg.uphjek.com

[U90] JS：数字数组排序
来源：http://ovi.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://kqj.yanxiufei.cn

[U91] JS：对象键值遍历
来源：http://rqq.vqdsnc.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nae.yj20258888.top

[U92] JS：深拷贝
来源：http://qhq.zhaomingkeji.xyz

structuredClone(obj)
来源：http://vjc.yonumen.top

[U93] JS：模板字符串
来源：http://epe.hesvh.cn

`共 ${n} 条`
来源：http://cvy.52xcode.cn

[U94] JS：箭头函数
来源：http://shh.bjfxy.top

const double = x => x * 2;
来源：http://jzz.sysykeji.top

[U95] JS：Promise 包装
来源：http://znj.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://quw.hcnkem.com

[U96] JS：async/await 与异常
来源：http://gem.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://afx.shanyushiyangkeji.top

[U97] JS：并发请求
来源：http://oif.yongpay.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ppq.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://pea.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://swg.jyoumei.cn

[U99] JS：事件监听
来源：http://ans.ivvv.top

el.addEventListener("click", e => {})
来源：http://dqe.hfpthk.cn

[U100] JS：DOM 查询
来源：http://her.fanxiaobao.xyz

document.querySelector(".item")
来源：http://pcz.ydjk.org.cn

[U101] JS：classList 操作
来源：http://fry.bbcook.cn

el.classList.toggle("active")
来源：http://rhs.zdqjudy.top

[U102] JS：本地存储
来源：http://wnb.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jmi.zhiwuduotai.top

[U103] JS：定时器
来源：http://izr.chenjidiqi.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://axg.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://coo.pycfn.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://glo.ywan-chungtsiang.top

[U105] JS：节流
来源：http://fka.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zeh.yangfankeji.com

[U106] JS：日期格式化
来源：http://jmv.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xxd.fengsongda.top

[U107] JS：数字千分位
来源：http://xkr.bjfxy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gzu.dashuyun.cn

[U108] JS：随机整数
来源：http://oah.zhengqikj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wqr.hammf.cn

[U109] JS：数组分组
来源：http://iys.snrcjt.cn

Object.groupBy(arr, x => x.type)
来源：http://ech.birdmap.top

[U110] JS：数组分块
来源：http://ufo.yj20258888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tqp.cdnleiting.top

[U111] JS：对象转 Map
来源：http://qly.bbcook.cn

new Map(Object.entries(obj))
来源：http://glu.zhoulong.xyz

[U112] JS：字符串补位
来源：http://qjf.cqqwz.cn

"7".padStart(3, "0")
来源：http://nkc.fehbvm.com

[U113] JS：正则替换全部
来源：http://wak.cashguo.top

s.replaceAll("a", "b")
来源：http://sik.nanxuanxn.top

[U114] JS：JSON 深比较
来源：http://myb.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nyy.sysykeji.top

[U115] JS：生成 UUID
来源：http://ibw.vehdjk.com

crypto.randomUUID()
来源：http://mko.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://zmb.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://gsx.52xcode.cn

[U117] JS：单元测试
来源：http://szp.ivvv.top

npm i -D vitest;  npx vitest
来源：http://naa.cucudq.cn

[U118] JS：开发服务器
来源：http://aut.yvedp.cn

npm i -D vite;  npx vite
来源：http://tre.sjlbkw.cn

[U119] JS：生产构建
来源：http://zbe.yonumen.top

npx vite build
来源：http://aju.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://wuj.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://xhm.yj202588.top

================================================================================
来源：http://qsl.gogol.net.cn

统计汇总
来源：http://blr.yj20258888.top

================================================================================
来源：http://yuo.yvedp.cn

按语言统计（条）：
来源：http://bzc.shanyushiyangtech.top

Python ......... 252
来源：http://xls.daria6918.cn

PHP ............ 252
来源：http://bbw.fanxiaobao.xyz

JavaScript ..... 252
来源：http://kyr.ctjpmb.com

TypeScript ..... 212
来源：http://kbb.xuanzx.com

Java ........... 212
来源：http://mqd.hfpthk.cn

Go ............. 212
来源：http://mdh.tianlin.xyz

Ruby ........... 212
来源：http://jre.hnqzz.top

C# ............. 212
来源：http://ueg.52xcode.cn

C .............. 30
来源：http://wue.shangyingyoupin.top

C++ ............ 30
来源：http://she.nanxuanxn.top

SQL ............ 90
来源：http://pmx.wangdashe.top

Bash ........... 80
来源：http://nki.dianchejie.cn

Kotlin ......... 15
来源：http://ded.nwbrower.top

Swift .......... 15
来源：http://jxr.fanxiaobao.xyz

Lua ............ 10
来源：http://dxu.andypj.xyz

Perl ........... 10
来源：http://elw.yangfankeji.com

Scala .......... 10
来源：http://vbv.gotoacloud.top

------------------------------------
来源：http://dfx.yuxming.cn

合计 ........... 2106 条
来源：http://aau.ehwqpu.com

按章节统计：
来源：http://pey.sjlbkw.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yyp.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jix.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wvd.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bgp.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qku.jianghu66.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tyf.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kol.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jzd.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wtk.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mao.9152youxi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cdq.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vpq.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rsy.jianghu66.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ude.kuanghao11.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hbh.yuxming.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://idr.yvedp.cn

Q SQL 专题                              90
来源：http://pwl.ydjk.org.cn

R Bash 专题                             80
来源：http://bww.pycfn.com

S C / C++ 专题                          60
来源：http://skc.epnwcf.com

T 其他语言补充                          60
来源：http://jts.aibaodan.cn

U 高频实用片段                         120
来源：http://gft.jyoumei.cn

------------------------------------
来源：http://lae.yj20258888.top

合计                                  2106 条
来源：http://vad.yj20258888.top

--------------------------------------------------------------------------------
来源：http://jqv.uphjek.com

使用提醒
来源：http://iiw.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://ntz.cucudq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lst.shuidangran.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ghy.sysykeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wme.pengpengdd.cyou

在旧版本上使用前请先确认语法支持情况。
来源：http://sbk.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xhd.zhiwuduotai.top

—— 文件结束 ——
来源：http://jeq.bbcook.cn

================================================================================
来源：http://cff.ctjpmb.com

程序语言常见例子速查手册（2024 版）
来源：http://mel.pycfn.com

Common Programming Examples Cheat Book
来源：http://fku.shanyushiyangtech.top

================================================================================
来源：http://wex.pycfn.com

【收录内容】
来源：http://dgc.c1oappe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lrf.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mkh.gaohongyu789.top

SQL · Bash · C · C++
来源：http://fup.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dir.shanyushiyangkeji.top

【使用说明】
来源：http://wiq.gotoacloud.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wup.ehwqpu.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hsm.bbcook.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tyl.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mas.zdqjudy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dht.zdqjudy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://utd.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pro.yonumen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pvg.chenjidiqi.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qdk.ydzc1.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uml.haohaochexian.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xfu.tian-w.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ilo.ctjpmb.com

【文件统计】
来源：http://cxo.daxiang520.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cak.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://gnz.shanyushiyangtech.top

目  录
来源：http://lcr.shuidangran.top

--------------------------------------------------------------------------------
来源：http://bvp.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ypp.ywan-chungtsiang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fdf.ydjk.org.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://taq.gogol.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oaf.sjlbkw.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kln.snrcjt.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qzz.jinyuanbaomall.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uaw.nanxinkj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fzi.gzhubu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jzm.dianchejie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nyw.yongpay.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ehw.ppjwa.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rfo.quarkkingdee.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zgf.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zii.shzxlz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://idc.pycfn.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gef.chenzaomai.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://snw.hfpthk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jpp.sjlbkw.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zkf.hongshengwenyu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rvk.yj20258888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://evp.pycfn.com

================================================================================
来源：http://rcb.hcnkem.com

A. 基础语法与类型
来源：http://tgh.nwbrower.top

================================================================================
来源：http://kjc.redwolf501.top

[A01] Hello World
来源：http://hag.hywenlv.cn

Py:   print("Hello, World!")
来源：http://yrz.cheryme.top

PHP:  echo "Hello, World!";
来源：http://jst.hammf.cn

JS:   console.log("Hello, World!");
来源：http://owe.hongshengwenyu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ghl.daxiang520.top

Java: System.out.println("Hello, World!");
来源：http://juy.pengpengdd.cyou

Go:   fmt.Println("Hello, World!")
来源：http://bnh.pycfn.com

Ruby: puts "Hello, World!"
来源：http://djx.feifeiyinyue.top

C#:   Console.WriteLine("Hello, World!");
来源：http://uwl.sjlbkw.cn

[A02] 变量声明与赋值
来源：http://pfb.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ymt.guowangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://oml.gotoacloud.top

JS:   let name = "Alex"; const age = 20;
来源：http://ggf.yanxiufei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gjg.sufxvd.cn

Java: String name = "Alex"; int age = 20;
来源：http://cep.havefunace.top

Go:   name := "Alex"; age := 20
来源：http://tjy.sxryk.cn

Ruby: name = "Alex"; age = 20
来源：http://ggp.zhixingplan.top

C#:   string name = "Alex"; int age = 20;
来源：http://hdb.zhaomingkeji.xyz

[A03] 常量定义
来源：http://toz.dianchejie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eay.cashguo.top

PHP:  const PI = 3.14159;
来源：http://jzp.nanxuanxn.top

JS:   const PI = 3.14159;
来源：http://fcn.gzhubu.top

TS:   const PI: number = 3.14159;
来源：http://wzm.jqgufenzy.top

Java: static final double PI = 3.14159;
来源：http://xxq.xinyue.icu

Go:   const PI = 3.14159
来源：http://nlc.bjfxy.top

Ruby: PI = 3.14159
来源：http://rpz.hcnkem.com

C#:   const double PI = 3.14159;
来源：http://ymo.wangshuangyany.cn

[A04] 判断变量类型
来源：http://ech.yfazqb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://jwb.sxryk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hwn.hywenlv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yqk.jqgfzy.top

TS:   typeof x; x instanceof Date
来源：http://nbm.ydzc1.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hmz.316326.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://tai.aibaodan.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yrp.gaohongyu789.top

C#:   x.GetType().Name; x is int
来源：http://hmc.ydzc1.top

[A05] 整数除法与取模
来源：http://tkl.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sbo.tanke756.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lsa.sufxvd.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vvb.zhixingplan.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gfv.iojbl.cn


<!-- 参考信息 -->