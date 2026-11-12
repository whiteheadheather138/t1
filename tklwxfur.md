代发 wailian999

[U43] PHP：声明命名空间
来源：http://wit.mhx1999.top

namespace App\Http;
来源：http://iio.9152youxi.cn

[U44] PHP：开启严格类型
来源：http://vsh.guowangkeji.top

declare(strict_types=1);
来源：http://ljd.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://oba.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ise.yangfankeji.com

[U46] PHP：可空类型
来源：http://ask.chenjidiqi.icu

?string $name = null
来源：http://bkk.zhengqikj.top

[U47] PHP：联合类型
来源：http://wsz.52xcode.cn

int|string $id
来源：http://lxz.xinyue.icu

[U48] PHP：纯枚举
来源：http://qta.hnqzz.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gya.zhoulong.xyz

[U49] PHP：只读属性
来源：http://eqz.zhongyouzk.top

public readonly string $name
来源：http://tzr.dashuyun.cn

[U50] PHP：构造器属性提升
来源：http://enw.ywan-chungtsiang.top

public function __construct(private int $id) {}
来源：http://mqw.smart0.xyz

[U51] PHP：数组解构
来源：http://pde.yvedp.cn

[$a, $b] = $arr;
来源：http://zzu.smart0.xyz

[U52] PHP：箭头函数
来源：http://nao.ywan-chungtsiang.top

$double = fn($x) => $x * 2;
来源：http://vov.yj20258.top

[U53] PHP：空合并运算符
来源：http://xiu.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://dcn.haohaochexian.top

[U54] PHP：空安全调用
来源：http://hzb.bbcook.cn

$obj?->method()
来源：http://tlr.sxryk.cn

[U55] PHP：match 表达式
来源：http://det.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tna.hongshengwenyu.top

[U56] PHP：命名参数
来源：http://jef.dashuyun.cn

f(a: 1, b: 2)
来源：http://pot.iojbl.cn

[U57] PHP：字符串插值
来源：http://bhf.jianghu66.top

"值: {$a}"
来源：http://mij.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://ytv.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://psc.chenlongwang.top

[U59] PHP：自定义排序
来源：http://yhl.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fys.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://rtj.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bxb.hnxiangtu.top

[U61] PHP：正则
来源：http://smx.ydzc1.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baj.jqgfzy.top

[U62] PHP：日期对象
来源：http://wbx.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lfr.hysaishi.cn

[U63] PHP：文件读写
来源：http://qbo.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vro.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://vqg.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://gir.yangfankeji.com

[U65] PHP：会话
来源：http://dun.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cxj.cashguo.top

[U66] PHP：设置 Cookie
来源：http://ryy.fanxiaobao.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://swj.tanke756.top

[U67] PHP：处理文件上传
来源：http://vsr.jqgfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://geo.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://ffg.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jam.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://dce.yongpay.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wks.yanxiufei.cn

[U70] PHP：PDO 事务
来源：http://jgb.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ndg.hfpthk.cn

[U71] PHP：抛出异常
来源：http://doe.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://zmy.zhengqikj.top

[U72] PHP：写错误日志
来源：http://vra.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://jwd.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://sqb.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://ecd.haohaochexian.top

[U74] PHP：读取环境变量
来源：http://qas.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://jvo.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://cag.0kj1m.cn

composer require psr/container
来源：http://lkt.ppjwa.cn

[U76] PHP：简单路由
来源：http://jex.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://txu.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://pui.snrcjt.cn

composer require twig/twig
来源：http://xsb.nanxuanxn.top

[U78] PHP：单元测试
来源：http://xby.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://hob.xziqi.cn

[U79] PHP：静态分析
来源：http://ryl.hammf.cn

composer require --dev phpstan/phpstan
来源：http://muh.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://vfc.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://whz.shzxlz.cn

[U81] JS：初始化项目
来源：http://zfc.jqgufenzy.top

npm init -y;  npm i express
来源：http://zyv.fktsv.cn

[U82] JS：package.json 脚本
来源：http://cim.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mrk.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://har.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tla.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://ypj.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://uyv.nanxinkj.top

[U85] JS：可选链
来源：http://uez.yuxming.cn

a?.b?.c
来源：http://zvj.zhaomingkeji.xyz

[U86] JS：空值合并
来源：http://kuw.zhixingplan.top

a ?? b
来源：http://mky.shangyingyoupin.top

[U87] JS：解构默认值
来源：http://mov.yj20258.top

const { a = 1, b = 2 } = obj;
来源：http://pbb.52xcode.cn

[U88] JS：对象展开合并
来源：http://wol.sweek.top

{ ...a, ...b }
来源：http://grk.gogol.net.cn

[U89] JS：数组去重
来源：http://qmg.fehbvm.com

[...new Set(arr)]
来源：http://mfc.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://qit.xinyue.icu

[...arr].sort((a, b) => a - b)
来源：http://idk.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://tve.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tcg.pycfn.com

[U92] JS：深拷贝
来源：http://eyt.zycfv.cn

structuredClone(obj)
来源：http://rpw.yvedp.cn

[U93] JS：模板字符串
来源：http://grt.daria6918.cn

`共 ${n} 条`
来源：http://syr.gaohongyu789.top

[U94] JS：箭头函数
来源：http://waw.ctjpmb.com

const double = x => x * 2;
来源：http://jiv.cqqwz.cn

[U95] JS：Promise 包装
来源：http://wtm.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://woh.xuetiantiany.cn

[U96] JS：async/await 与异常
来源：http://iss.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hxt.gzhubu.top

[U97] JS：并发请求
来源：http://hlc.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ruq.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://ayg.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wnd.jinqigufen.top

[U99] JS：事件监听
来源：http://xpg.cucudq.cn

el.addEventListener("click", e => {})
来源：http://jwh.shuidangran.top

[U100] JS：DOM 查询
来源：http://sdc.andypj.xyz

document.querySelector(".item")
来源：http://jnv.smart0.xyz

[U101] JS：classList 操作
来源：http://war.svipenyu.cn

el.classList.toggle("active")
来源：http://gng.zhixingplan.top

[U102] JS：本地存储
来源：http://cjc.wangshuangyany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cad.chenjidiqi.icu

[U103] JS：定时器
来源：http://aqc.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ram.cashguo.top

[U104] JS：防抖
来源：http://gfx.shzxlz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://feg.dashuyun.cn

[U105] JS：节流
来源：http://ghg.zycfv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oua.shuidangran.top

[U106] JS：日期格式化
来源：http://ofg.cucudq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ivo.haohaochexian.top

[U107] JS：数字千分位
来源：http://llp.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gwp.dashuyun.cn

[U108] JS：随机整数
来源：http://arh.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qtc.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://hqs.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://scx.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://zar.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yda.nwbrower.top

[U111] JS：对象转 Map
来源：http://akb.yj20258888.top

new Map(Object.entries(obj))
来源：http://ltm.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://eze.zdbjq.cn

"7".padStart(3, "0")
来源：http://hxc.zhixingplan.top

[U113] JS：正则替换全部
来源：http://xgx.nanxuanxn.top

s.replaceAll("a", "b")
来源：http://jkh.quarkkingdee.top

[U114] JS：JSON 深比较
来源：http://blz.yj20258.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qeb.iojbl.cn

[U115] JS：生成 UUID
来源：http://ajk.hcnkem.com

crypto.randomUUID()
来源：http://jad.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://tet.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://jlx.vehdjk.com

[U117] JS：单元测试
来源：http://ydz.fktsv.cn

npm i -D vitest;  npx vitest
来源：http://ses.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://kgt.yongpay.top

npm i -D vite;  npx vite
来源：http://xmx.yj20258888.top

[U119] JS：生产构建
来源：http://oai.andypj.xyz

npx vite build
来源：http://dax.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://aer.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://nyu.shzxlz.cn

================================================================================
来源：http://xkt.zhengqikj.top

统计汇总
来源：http://hon.daria6918.cn

================================================================================
来源：http://itd.xuetiantiany.cn

按语言统计（条）：
来源：http://nhv.nanxinkj.top

Python ......... 252
来源：http://txi.yueranfly.top

PHP ............ 252
来源：http://oth.xinyue.icu

JavaScript ..... 252
来源：http://tgo.zhengqikj.top

TypeScript ..... 212
来源：http://yxg.hfpthk.cn

Java ........... 212
来源：http://kyl.aibaodan.cn

Go ............. 212
来源：http://ymr.jinqigfzy.top

Ruby ........... 212
来源：http://khr.dianchejie.cn

C# ............. 212
来源：http://jvx.epnwcf.com

C .............. 30
来源：http://wmi.gotoacloud.top

C++ ............ 30
来源：http://cyw.hfpthk.cn

SQL ............ 90
来源：http://atj.yuxming.cn

Bash ........... 80
来源：http://vru.snrcjt.cn

Kotlin ......... 15
来源：http://dfd.redwolf501.top

Swift .......... 15
来源：http://rqi.yueranfly.top

Lua ............ 10
来源：http://ymj.shanyushiyangtech.top

Perl ........... 10
来源：http://kyv.gogol.net.cn

Scala .......... 10
来源：http://aki.hfpthk.cn

------------------------------------
来源：http://kpx.jiagoushi.top

合计 ........... 2106 条
来源：http://aov.gogol.net.cn

按章节统计：
来源：http://pvt.redwolf501.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jqu.svipenyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qzu.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zsh.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jxp.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dag.ctjpmb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mjw.tanke756.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mrs.dianchejie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ilt.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mft.wangshuangyany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fwj.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://znm.guannengcc.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://two.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vci.ehwqpu.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kxm.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bdg.jinqigfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ojj.pycfn.com

Q SQL 专题                              90
来源：http://wzw.fktsv.cn

R Bash 专题                             80
来源：http://xrb.hesvh.cn

S C / C++ 专题                          60
来源：http://wfi.zhongyouzk.top

T 其他语言补充                          60
来源：http://uuf.chenjidiqi.icu

U 高频实用片段                         120
来源：http://hjm.sweek.top

------------------------------------
来源：http://cej.sweek.top

合计                                  2106 条
来源：http://iya.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://jxt.cdnleiting.top

使用提醒
来源：http://ddx.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://hyt.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mxr.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ldw.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rxx.epnwcf.com

在旧版本上使用前请先确认语法支持情况。
来源：http://zyy.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pmv.shuidangran.top

—— 文件结束 ——
来源：http://hjq.jinghuilouyu.cn

================================================================================
来源：http://yvd.sxryk.cn

程序语言常见例子速查手册（2024 版）
来源：http://yak.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://gkd.nanxinkj.top

================================================================================
来源：http://ill.nanxinkj.top

【收录内容】
来源：http://xcp.jinghuilouyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wex.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://arp.jiagoushi.top

SQL · Bash · C · C++
来源：http://toy.jqgfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ntu.pycfn.com

【使用说明】
来源：http://tod.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mmf.guannengcc.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bly.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://woo.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nyi.vqdsnc.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://oiw.redwolf501.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://llw.dashuyun.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yvs.yonumen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hsd.wangshuangyany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ema.chenjidiqi.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qgy.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fli.cdnleiting.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ycl.zdbjq.cn

【文件统计】
来源：http://ynh.yj20258888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://deg.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://iod.yueranfly.top

目  录
来源：http://ccw.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://uwh.xuanzx.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://flw.hongshengwenyu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zqh.xuetiantiany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://apv.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fta.ydjk.org.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://obw.cucudq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sig.daxiang520.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ilk.jlsjyb.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://olz.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vzv.jiagoushi.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aco.hongshengwenyu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nig.xuetiantiany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nga.52xcode.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hap.xuetiantiany.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ifm.mhx1999.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fat.zhijiandao.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xcw.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oif.chenjidiqi.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://uny.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zxo.jinqigfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jwm.zhengqikj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://niq.cdnleiting.top

================================================================================
来源：http://eio.yonumen.top

A. 基础语法与类型
来源：http://jva.yuanzhike.top

================================================================================
来源：http://bnm.jyoumei.cn

[A01] Hello World
来源：http://oij.yj20258.top

Py:   print("Hello, World!")
来源：http://opq.52xcode.cn

PHP:  echo "Hello, World!";
来源：http://lls.sweek.top

JS:   console.log("Hello, World!");
来源：http://kko.sufxvd.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zxc.jlsjyb.cn

Java: System.out.println("Hello, World!");
来源：http://svl.fktsv.cn

Go:   fmt.Println("Hello, World!")
来源：http://ncf.shanyushiyangtech.top

Ruby: puts "Hello, World!"
来源：http://erx.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://mea.yueranfly.top

[A02] 变量声明与赋值
来源：http://zfj.shangyingyoupin.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mve.quarkkingdee.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cof.snrcjt.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ffd.jyoumei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sgc.hysaishi.cn

Java: String name = "Alex"; int age = 20;
来源：http://kxe.yj20258.top

Go:   name := "Alex"; age := 20
来源：http://tvn.meibo888.top

Ruby: name = "Alex"; age = 20
来源：http://xsz.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://qot.yonumen.top

[A03] 常量定义
来源：http://vtr.yangfankeji.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ror.birdmap.top

PHP:  const PI = 3.14159;
来源：http://grd.sysykeji.top

JS:   const PI = 3.14159;
来源：http://hmb.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://bzv.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://jem.xuanzx.com

Go:   const PI = 3.14159
来源：http://fxj.0kj1m.cn

Ruby: PI = 3.14159
来源：http://sxy.yanxiufei.cn

C#:   const double PI = 3.14159;
来源：http://phs.yonumen.top

[A04] 判断变量类型
来源：http://xwc.yongpay.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lrg.aizwys.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rio.yuxming.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yem.shanyushiyangkeji.top

TS:   typeof x; x instanceof Date
来源：http://pvl.zhijiandao.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jem.yvedp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cur.chenzaomai.com

Ruby: x.class; x.is_a?(Integer)
来源：http://nyf.gotoacloud.top

C#:   x.GetType().Name; x is int
来源：http://ole.yj202588.top

[A05] 整数除法与取模
来源：http://gcg.jianghu66.top


<!-- 参考信息 -->