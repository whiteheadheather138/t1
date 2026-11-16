代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://cem.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wnr.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://yld.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qyp.jqgufenzy.top

[U43] PHP：声明命名空间
来源：http://lvr.yangfankeji.com

namespace App\Http;
来源：http://iqq.ehwqpu.com

[U44] PHP：开启严格类型
来源：http://hhk.fehbvm.com

declare(strict_types=1);
来源：http://udc.xingfuxueyuan.xyz

[U45] PHP：类型声明与返回类型
来源：http://eil.jinyuanbaomall.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://csg.uphjek.com

[U46] PHP：可空类型
来源：http://bfv.ybcxt.top

?string $name = null
来源：http://mcd.c1oappe.top

[U47] PHP：联合类型
来源：http://gml.ybcxt.top

int|string $id
来源：http://hks.bjfxy.top

[U48] PHP：纯枚举
来源：http://tgs.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://klp.bjfxy.top

[U49] PHP：只读属性
来源：http://fea.chenzaomai.com

public readonly string $name
来源：http://nnf.jiagoushi.top

[U50] PHP：构造器属性提升
来源：http://ery.meibo888.top

public function __construct(private int $id) {}
来源：http://cyq.yueranfly.top

[U51] PHP：数组解构
来源：http://pyx.aibaodan.cn

[$a, $b] = $arr;
来源：http://uhb.jqgufenzy.top

[U52] PHP：箭头函数
来源：http://nwi.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://isv.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://mrh.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://pcz.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://taq.birdmap.top

$obj?->method()
来源：http://inz.yangfankeji.com

[U55] PHP：match 表达式
来源：http://ufw.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lyq.tianlin.xyz

[U56] PHP：命名参数
来源：http://kwh.zhijiandao.cn

f(a: 1, b: 2)
来源：http://hhw.tanke756.top

[U57] PHP：字符串插值
来源：http://pns.hnqzz.top

"值: {$a}"
来源：http://dss.zhixingplan.top

[U58] PHP：数组三件套
来源：http://tol.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rlr.jiagoushi.top

[U59] PHP：自定义排序
来源：http://suu.chenlongwang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zaq.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://wjl.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://unp.hnqzz.top

[U61] PHP：正则
来源：http://rhj.meibo888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hkf.sweek.top

[U62] PHP：日期对象
来源：http://vge.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iol.hnxiangtu.top

[U63] PHP：文件读写
来源：http://kgi.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jjg.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://dgr.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://rtd.snrcjt.cn

[U65] PHP：会话
来源：http://dyo.nanxinkj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hpv.sjlbkw.cn

[U66] PHP：设置 Cookie
来源：http://jjn.sysykeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://deo.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://tac.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://csa.yuxming.cn

[U68] PHP：PDO 连接
来源：http://afk.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jxp.sweek.top

[U69] PHP：PDO 预处理
来源：http://ufx.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gjs.wangdashe.top

[U70] PHP：PDO 事务
来源：http://ypc.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qlq.zycfv.cn

[U71] PHP：抛出异常
来源：http://jvo.316326.xyz

throw new RuntimeException("失败", 500);
来源：http://rpi.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://bhf.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://efw.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://sad.c1oappe.top

parse_ini_file("config.ini", true)
来源：http://vje.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://lzm.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://qzb.hysaishi.cn

[U75] PHP：依赖注入
来源：http://yso.quarkkingdee.top

composer require psr/container
来源：http://gtn.jianghu66.top

[U76] PHP：简单路由
来源：http://krg.fehbvm.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://irn.pycfn.com

[U77] PHP：模板渲染
来源：http://ind.yongpay.top

composer require twig/twig
来源：http://oeg.chenzaomai.com

[U78] PHP：单元测试
来源：http://pmh.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://oim.chenzaomai.com

[U79] PHP：静态分析
来源：http://egq.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://jmt.birdmap.top

[U80] PHP：代码规范修复
来源：http://gtt.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://caf.shuidangran.top

[U81] JS：初始化项目
来源：http://vrn.smart0.xyz

npm init -y;  npm i express
来源：http://jke.xylfe.cn

[U82] JS：package.json 脚本
来源：http://wtt.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xlq.0kj1m.cn

[U83] JS：ES Module 导入导出
来源：http://jtd.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://klf.kuanghao11.cn

[U84] JS：CommonJS 写法
来源：http://aav.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://ksz.dianchejie.cn

[U85] JS：可选链
来源：http://zbz.fehbvm.com

a?.b?.c
来源：http://ymq.zhiwuduotai.top

[U86] JS：空值合并
来源：http://bei.ctjpmb.com

a ?? b
来源：http://icj.hnxiangtu.top

[U87] JS：解构默认值
来源：http://msr.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://lod.daria6918.cn

[U88] JS：对象展开合并
来源：http://ddz.gogol.net.cn

{ ...a, ...b }
来源：http://opi.daria6918.cn

[U89] JS：数组去重
来源：http://pot.yueranfly.top

[...new Set(arr)]
来源：http://pjc.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://hiq.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://buh.hfpthk.cn

[U91] JS：对象键值遍历
来源：http://ush.jqgfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ija.xziqi.cn

[U92] JS：深拷贝
来源：http://vwr.jyoumei.cn

structuredClone(obj)
来源：http://fwh.xinyue.icu

[U93] JS：模板字符串
来源：http://csp.smart0.xyz

`共 ${n} 条`
来源：http://vcm.mhx1999.top

[U94] JS：箭头函数
来源：http://hwl.fengsongda.top

const double = x => x * 2;
来源：http://tao.jqgufenzy.top

[U95] JS：Promise 包装
来源：http://koh.gzhubu.top

new Promise((resolve, reject) => {})
来源：http://fbi.cqqwz.cn

[U96] JS：async/await 与异常
来源：http://liy.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wuj.fktsv.cn

[U97] JS：并发请求
来源：http://yjx.pycfn.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://egx.hongshengwenyu.top

[U98] JS：fetch 带 JSON
来源：http://vfv.aizwys.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lcc.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://pju.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://pmu.sufxvd.cn

[U100] JS：DOM 查询
来源：http://pme.tarul.cn

document.querySelector(".item")
来源：http://jcn.wangshuangyany.cn

[U101] JS：classList 操作
来源：http://lit.316326.xyz

el.classList.toggle("active")
来源：http://pud.xingfuxueyuan.xyz

[U102] JS：本地存储
来源：http://tjg.vehdjk.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://bkt.gogol.net.cn

[U103] JS：定时器
来源：http://veg.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nef.epnwcf.com

[U104] JS：防抖
来源：http://otc.hywenlv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://euq.fzhhl.top

[U105] JS：节流
来源：http://qyb.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vnw.sweek.top

[U106] JS：日期格式化
来源：http://gts.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zvb.0kj1m.cn

[U107] JS：数字千分位
来源：http://prt.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ajd.dianchejie.cn

[U108] JS：随机整数
来源：http://uoo.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://apw.pengpengdd.cyou

[U109] JS：数组分组
来源：http://eml.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://tbc.fengsongda.top

[U110] JS：数组分块
来源：http://ssr.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oog.chenzaomai.com

[U111] JS：对象转 Map
来源：http://twe.cashguo.top

new Map(Object.entries(obj))
来源：http://rds.yueranfly.top

[U112] JS：字符串补位
来源：http://hkv.316326.xyz

"7".padStart(3, "0")
来源：http://jni.c1oappe.top

[U113] JS：正则替换全部
来源：http://jdf.c1oappe.top

s.replaceAll("a", "b")
来源：http://eie.dianchejie.cn

[U114] JS：JSON 深比较
来源：http://bcp.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dgc.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://pke.iojbl.cn

crypto.randomUUID()
来源：http://wnr.yangfankeji.com

[U116] JS：类型检查（JSDoc）
来源：http://cyr.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://ago.meibo888.top

[U117] JS：单元测试
来源：http://pev.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://fqs.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://roj.0kj1m.cn

npm i -D vite;  npx vite
来源：http://cxe.hywenlv.cn

[U119] JS：生产构建
来源：http://byx.ctjpmb.com

npx vite build
来源：http://vyk.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://wiy.jqgfzy.top

import.meta.env.VITE_API_URL
来源：http://pvb.cheryme.top

================================================================================
来源：http://cxv.hfpthk.cn

统计汇总
来源：http://whq.hnqzz.top

================================================================================
来源：http://bji.chenjidiqi.icu

按语言统计（条）：
来源：http://amy.yuxming.cn

Python ......... 252
来源：http://tef.andypj.xyz

PHP ............ 252
来源：http://trp.sxryk.cn

JavaScript ..... 252
来源：http://txb.sxryk.cn

TypeScript ..... 212
来源：http://xza.jinqigfzy.top

Java ........... 212
来源：http://gbp.iojbl.cn

Go ............. 212
来源：http://wst.gzhubu.top

Ruby ........... 212
来源：http://ozy.shuidangran.top

C# ............. 212
来源：http://wpn.cashguo.top

C .............. 30
来源：http://ale.nwbrower.top

C++ ............ 30
来源：http://mbx.jinghuilouyu.cn

SQL ............ 90
来源：http://jpl.wangdashe.top

Bash ........... 80
来源：http://ugm.cucudq.cn

Kotlin ......... 15
来源：http://kvd.wangdashe.top

Swift .......... 15
来源：http://zjx.ybcxt.top

Lua ............ 10
来源：http://fbj.vehdjk.com

Perl ........... 10
来源：http://kkh.jlsjyb.cn

Scala .......... 10
来源：http://cpm.0kj1m.cn

------------------------------------
来源：http://idm.zhijiandao.cn

合计 ........... 2106 条
来源：http://uzw.zhiwuduotai.top

按章节统计：
来源：http://zhr.yangfankeji.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://crm.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qcq.shangyingyoupin.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vpi.shanyushiyangtech.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zxd.jinghuilouyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://diy.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bav.jqgfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://owr.sweek.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ccx.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ibu.zhengqikj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oln.cqqwz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cap.jqgufenzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kwr.sxryk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vin.fanxiaobao.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yfy.dashuyun.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dew.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hsz.52xcode.cn

Q SQL 专题                              90
来源：http://oxe.nwbrower.top

R Bash 专题                             80
来源：http://bdh.shuidangran.top

S C / C++ 专题                          60
来源：http://pee.nwbrower.top

T 其他语言补充                          60
来源：http://iqt.tian-w.cn

U 高频实用片段                         120
来源：http://cte.yj20258.top

------------------------------------
来源：http://hfe.quarkkingdee.top

合计                                  2106 条
来源：http://efg.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://swk.smart0.xyz

使用提醒
来源：http://nde.daria6918.cn

--------------------------------------------------------------------------------
来源：http://hgt.0kj1m.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hdm.xuetiantiany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://exu.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zap.sxryk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rdo.ivvv.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ewp.tanke756.top

—— 文件结束 ——
来源：http://doe.guannengcc.top

================================================================================
来源：http://kca.uphjek.com

程序语言常见例子速查手册（2024 版）
来源：http://dwt.xuanzx.com

Common Programming Examples Cheat Book
来源：http://roi.jlsjyb.cn

================================================================================
来源：http://hmj.chenjidiqi.icu

【收录内容】
来源：http://pfr.vehdjk.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://hxa.c1oappe.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qmr.hesvh.cn

SQL · Bash · C · C++
来源：http://rup.haohaochexian.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zph.aibaodan.cn

【使用说明】
来源：http://tha.jqgfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://maz.andypj.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nni.pengpengdd.cyou

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dow.ybcxt.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uwl.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rth.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uvo.iojbl.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sap.fktsv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nti.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mcy.zdbjq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://opv.meibo888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iqw.jinqigfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xxa.xylfe.cn

【文件统计】
来源：http://aqs.tianlin.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ekn.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://bqz.gogol.net.cn

目  录
来源：http://rpg.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://nne.shuidangran.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qfc.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hbf.nanxuanxn.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://koz.daria6918.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wzx.nanxinkj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://drs.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://onp.smart0.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gwt.feifeiyinyue.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vkr.hysaishi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hzb.jlsjyb.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://map.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hyy.yongpay.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yqu.uphjek.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://frr.daria6918.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lrs.cashguo.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zdm.cucudq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hgb.bbcook.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nqj.fanxiaobao.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://vuj.xingfuxueyuan.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fwz.xuetiantiany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wzy.ehwqpu.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wlh.zhongyouzk.top

================================================================================
来源：http://svq.hammf.cn

A. 基础语法与类型
来源：http://mjh.aibaodan.cn

================================================================================
来源：http://khg.xylfe.cn

[A01] Hello World
来源：http://lrg.iojbl.cn

Py:   print("Hello, World!")
来源：http://owj.havefunace.top

PHP:  echo "Hello, World!";
来源：http://efq.vehdjk.com

JS:   console.log("Hello, World!");
来源：http://ytj.tian-w.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jjm.zhiwuduotai.top

Java: System.out.println("Hello, World!");
来源：http://abd.kuanghao11.cn

Go:   fmt.Println("Hello, World!")
来源：http://bvs.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://tkp.xinyue.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://gwt.sweek.top

[A02] 变量声明与赋值
来源：http://zae.fengsongda.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qhi.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://ema.yanxiufei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pjj.havefunace.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fig.aizwys.cn

Java: String name = "Alex"; int age = 20;
来源：http://gak.ctjpmb.com

Go:   name := "Alex"; age := 20
来源：http://smt.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://oim.yvedp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kgs.gotoacloud.top

[A03] 常量定义
来源：http://lvy.chenzaomai.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kvv.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://qvt.fktsv.cn

JS:   const PI = 3.14159;
来源：http://ehk.hnqzz.top

TS:   const PI: number = 3.14159;
来源：http://jgo.0kj1m.cn

Java: static final double PI = 3.14159;
来源：http://gmb.quarkkingdee.top

Go:   const PI = 3.14159
来源：http://emu.sufxvd.cn

Ruby: PI = 3.14159
来源：http://hxg.tarul.cn

C#:   const double PI = 3.14159;
来源：http://qef.yuanzhike.top

[A04] 判断变量类型
来源：http://jkj.havefunace.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zey.uphjek.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qbz.chenlongwang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kro.chenjidiqi.icu

TS:   typeof x; x instanceof Date
来源：http://sim.vehdjk.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://klb.jinqigufen.top


<!-- 参考信息 -->