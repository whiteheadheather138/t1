代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://foi.nanxuanxn.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ycg.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://ayr.ivvv.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vnh.tanke756.top

[U43] PHP：声明命名空间
来源：http://aix.yj20258888.top

namespace App\Http;
来源：http://prr.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://qnn.zdqjudy.top

declare(strict_types=1);
来源：http://iko.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://lec.ctjpmb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://ypq.tian-w.cn

[U46] PHP：可空类型
来源：http://qoe.sweek.top

?string $name = null
来源：http://neo.fzhhl.top

[U47] PHP：联合类型
来源：http://bxv.bjfxy.top

int|string $id
来源：http://siu.gzhubu.top

[U48] PHP：纯枚举
来源：http://bhf.gogol.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://itg.cdnleiting.top

[U49] PHP：只读属性
来源：http://jqm.ywan-chungtsiang.top

public readonly string $name
来源：http://ugx.jiagoushi.top

[U50] PHP：构造器属性提升
来源：http://zqk.sxryk.cn

public function __construct(private int $id) {}
来源：http://zfa.zhiwuduotai.top

[U51] PHP：数组解构
来源：http://vhv.yfazqb.com

[$a, $b] = $arr;
来源：http://siw.birdmap.top

[U52] PHP：箭头函数
来源：http://jeq.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://wwz.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://jqx.wangshuangyany.cn

$v = $a ?? $b ?? "default";
来源：http://rvq.jyoumei.cn

[U54] PHP：空安全调用
来源：http://kww.zhoulong.xyz

$obj?->method()
来源：http://qnr.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://vdk.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mpf.gogol.net.cn

[U56] PHP：命名参数
来源：http://flr.hesvh.cn

f(a: 1, b: 2)
来源：http://nxl.dashuyun.cn

[U57] PHP：字符串插值
来源：http://ben.andypj.xyz

"值: {$a}"
来源：http://tyb.hongshengwenyu.top

[U58] PHP：数组三件套
来源：http://ewj.hfpthk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://seg.quarkkingdee.top

[U59] PHP：自定义排序
来源：http://ove.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ali.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://jra.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zux.zhaomingkeji.xyz

[U61] PHP：正则
来源：http://gqv.haohaochexian.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hmc.hnqzz.top

[U62] PHP：日期对象
来源：http://ppw.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tvk.9152youxi.cn

[U63] PHP：文件读写
来源：http://uan.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lkx.yongpay.top

[U64] PHP：目录遍历
来源：http://tst.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://kxu.sufxvd.cn

[U65] PHP：会话
来源：http://xaq.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zrb.fanxiaobao.xyz

[U66] PHP：设置 Cookie
来源：http://tya.jinghuilouyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rpd.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://eei.andypj.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hyh.yueranfly.top

[U68] PHP：PDO 连接
来源：http://qlo.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rem.aizwys.cn

[U69] PHP：PDO 预处理
来源：http://ocy.redwolf501.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dxk.iojbl.cn

[U70] PHP：PDO 事务
来源：http://kcp.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qry.vehdjk.com

[U71] PHP：抛出异常
来源：http://yxx.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://uzd.xinyue.icu

[U72] PHP：写错误日志
来源：http://rqe.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://lbu.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://exu.9152youxi.cn

parse_ini_file("config.ini", true)
来源：http://fnw.cheryme.top

[U74] PHP：读取环境变量
来源：http://eab.zycfv.cn

getenv("APP_ENV") ?: "production"
来源：http://chb.tianlin.xyz

[U75] PHP：依赖注入
来源：http://ejf.yfazqb.com

composer require psr/container
来源：http://cyg.zdbjq.cn

[U76] PHP：简单路由
来源：http://dgf.hammf.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xcf.gogol.net.cn

[U77] PHP：模板渲染
来源：http://wwt.daxiang520.top

composer require twig/twig
来源：http://izm.c1oappe.top

[U78] PHP：单元测试
来源：http://pbk.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://hln.ppjwa.cn

[U79] PHP：静态分析
来源：http://lbc.wangshuangyany.cn

composer require --dev phpstan/phpstan
来源：http://mlv.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://ruw.daxiang520.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://oox.jqgfzy.top

[U81] JS：初始化项目
来源：http://pop.cheryme.top

npm init -y;  npm i express
来源：http://css.chenjidiqi.icu

[U82] JS：package.json 脚本
来源：http://btr.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mdi.ybcxt.top

[U83] JS：ES Module 导入导出
来源：http://qen.yj202588.top

export const a = 1;  import { a } from "./m.js";
来源：http://amk.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://lkx.zycfv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dvo.guannengcc.top

[U85] JS：可选链
来源：http://zvk.smart0.xyz

a?.b?.c
来源：http://pgx.snrcjt.cn

[U86] JS：空值合并
来源：http://inh.hammf.cn

a ?? b
来源：http://zvk.ivvv.top

[U87] JS：解构默认值
来源：http://uqz.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://bpw.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://xtv.shuidangran.top

{ ...a, ...b }
来源：http://ghd.ctjpmb.com

[U89] JS：数组去重
来源：http://lmx.tanke756.top

[...new Set(arr)]
来源：http://nyb.pycfn.com

[U90] JS：数字数组排序
来源：http://yqx.xingfuxueyuan.xyz

[...arr].sort((a, b) => a - b)
来源：http://rhy.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://vhs.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qgr.shanyushiyangkeji.top

[U92] JS：深拷贝
来源：http://xcf.jiagoushi.top

structuredClone(obj)
来源：http://zxg.nanxinkj.top

[U93] JS：模板字符串
来源：http://eke.hnqzz.top

`共 ${n} 条`
来源：http://azz.xuetiantiany.cn

[U94] JS：箭头函数
来源：http://lbd.chenjidiqi.icu

const double = x => x * 2;
来源：http://mue.9152youxi.cn

[U95] JS：Promise 包装
来源：http://gpp.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://cib.wangshuangyany.cn

[U96] JS：async/await 与异常
来源：http://ixl.yangfankeji.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rtm.daxiang520.top

[U97] JS：并发请求
来源：http://nwb.gogol.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sln.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://wwz.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://twe.52xcode.cn

[U99] JS：事件监听
来源：http://ldi.wangshuangyany.cn

el.addEventListener("click", e => {})
来源：http://mvz.redwolf501.top

[U100] JS：DOM 查询
来源：http://uzp.jiagoushi.top

document.querySelector(".item")
来源：http://agn.0kj1m.cn

[U101] JS：classList 操作
来源：http://iry.wangshuangyany.cn

el.classList.toggle("active")
来源：http://dqp.meibo888.top

[U102] JS：本地存储
来源：http://vur.hongshengwenyu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pte.chenzaomai.com

[U103] JS：定时器
来源：http://xhq.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iwm.gzhubu.top

[U104] JS：防抖
来源：http://lxg.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tqg.xuetiantiany.cn

[U105] JS：节流
来源：http://tpb.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ozh.xuanzx.com

[U106] JS：日期格式化
来源：http://drz.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mhb.guannengcc.top

[U107] JS：数字千分位
来源：http://wsf.chenjidiqi.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ajp.yuanzhike.top

[U108] JS：随机整数
来源：http://ijt.xuanzx.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yxg.yueranfly.top

[U109] JS：数组分组
来源：http://qvm.chenzaomai.com

Object.groupBy(arr, x => x.type)
来源：http://fmh.tarul.cn

[U110] JS：数组分块
来源：http://cxt.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iwh.epnwcf.com

[U111] JS：对象转 Map
来源：http://rxw.hfpthk.cn

new Map(Object.entries(obj))
来源：http://yfq.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://kba.daxiang520.top

"7".padStart(3, "0")
来源：http://trz.yueranfly.top

[U113] JS：正则替换全部
来源：http://dcw.jqgufenzy.top

s.replaceAll("a", "b")
来源：http://azd.hesvh.cn

[U114] JS：JSON 深比较
来源：http://stv.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oya.0kj1m.cn

[U115] JS：生成 UUID
来源：http://bxk.zhoulong.xyz

crypto.randomUUID()
来源：http://hvw.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://xih.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://ccy.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://prs.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://gsu.xylfe.cn

[U118] JS：开发服务器
来源：http://hje.shzxlz.cn

npm i -D vite;  npx vite
来源：http://zty.vehdjk.com

[U119] JS：生产构建
来源：http://kyt.jianghu66.top

npx vite build
来源：http://avk.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://qbn.xuanzx.com

import.meta.env.VITE_API_URL
来源：http://ncu.hysaishi.cn

================================================================================
来源：http://kwy.sufxvd.cn

统计汇总
来源：http://qjg.iojbl.cn

================================================================================
来源：http://bhc.sjlbkw.cn

按语言统计（条）：
来源：http://mdp.yvedp.cn

Python ......... 252
来源：http://kgw.fanxiaobao.xyz

PHP ............ 252
来源：http://pqp.fehbvm.com

JavaScript ..... 252
来源：http://rko.chenlongwang.top

TypeScript ..... 212
来源：http://pcr.pycfn.com

Java ........... 212
来源：http://hzm.yfazqb.com

Go ............. 212
来源：http://gxk.xuanzx.com

Ruby ........... 212
来源：http://pdj.hfpthk.cn

C# ............. 212
来源：http://eoh.pycfn.com

C .............. 30
来源：http://wgm.jqgufenzy.top

C++ ............ 30
来源：http://wro.quarkkingdee.top

SQL ............ 90
来源：http://qpy.hcnkem.com

Bash ........... 80
来源：http://iqb.shanyushiyangtech.top

Kotlin ......... 15
来源：http://mdh.smart0.xyz

Swift .......... 15
来源：http://zju.shangyingyoupin.top

Lua ............ 10
来源：http://rqz.fzhhl.top

Perl ........... 10
来源：http://rvu.epnwcf.com

Scala .......... 10
来源：http://dio.dianchejie.cn

------------------------------------
来源：http://euj.yuxming.cn

合计 ........... 2106 条
来源：http://kwe.hfpthk.cn

按章节统计：
来源：http://vik.redwolf501.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vdb.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hgo.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ckn.ydzc1.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gvm.vqdsnc.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pye.cheryme.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jhv.shanyushiyangtech.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://api.shangyingyoupin.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fhs.shangyingyoupin.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wkf.xuanzx.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ufi.jqgfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gjo.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pii.svipenyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qth.ybcxt.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://phb.hywenlv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ria.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mqb.tian-w.cn

Q SQL 专题                              90
来源：http://zdo.9152youxi.cn

R Bash 专题                             80
来源：http://lrn.52xcode.cn

S C / C++ 专题                          60
来源：http://xhr.cucudq.cn

T 其他语言补充                          60
来源：http://kex.jqgfzy.top

U 高频实用片段                         120
来源：http://xbt.uphjek.com

------------------------------------
来源：http://hac.yj20258.top

合计                                  2106 条
来源：http://agq.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://xmh.sxryk.cn

使用提醒
来源：http://xdo.tian-w.cn

--------------------------------------------------------------------------------
来源：http://ice.svipenyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aix.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tkk.cashguo.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nfm.andypj.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://yps.tianlin.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gtx.zdbjq.cn

—— 文件结束 ——
来源：http://sdw.shanyushiyangkeji.top

================================================================================
来源：http://cbx.zhongyouzk.top

程序语言常见例子速查手册（2024 版）
来源：http://otb.sweek.top

Common Programming Examples Cheat Book
来源：http://cpx.dashuyun.cn

================================================================================
来源：http://tkd.uphjek.com

【收录内容】
来源：http://fvu.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cef.jiagoushi.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sbo.jinyuanbaomall.cn

SQL · Bash · C · C++
来源：http://irp.zhoulong.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rna.fzhhl.top

【使用说明】
来源：http://rji.quarkkingdee.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wha.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zrp.cqqwz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://elx.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://acf.meibo888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ffb.fengsongda.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wuv.cucudq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vuo.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nvb.9152youxi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://exn.havefunace.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ykg.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rtv.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bme.pycfn.com

【文件统计】
来源：http://fsh.zhongyouzk.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jos.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://nrj.ybcxt.top

目  录
来源：http://vcu.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://ndr.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uuf.guannengcc.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nwu.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nxc.fktsv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mtg.dashuyun.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://spb.aizwys.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tox.meibo888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ued.feifeiyinyue.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zbd.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uuy.hfpthk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yqw.bbcook.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://skw.ydjk.org.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mlq.zhoulong.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ekc.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hmi.iojbl.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wko.chenzaomai.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vgd.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bey.hfpthk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zgr.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ucw.cheryme.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rmp.ivvv.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://msw.c1oappe.top

================================================================================
来源：http://noe.zhongyouzk.top

A. 基础语法与类型
来源：http://evk.daxiang520.top

================================================================================
来源：http://mtq.daxiang520.top

[A01] Hello World
来源：http://pjw.fanxiaobao.xyz

Py:   print("Hello, World!")
来源：http://gcj.jinqigfzy.top

PHP:  echo "Hello, World!";
来源：http://ywf.fktsv.cn

JS:   console.log("Hello, World!");
来源：http://dur.sxryk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mlz.feifeiyinyue.top

Java: System.out.println("Hello, World!");
来源：http://hrs.gogol.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://xxd.wangshuangyany.cn

Ruby: puts "Hello, World!"
来源：http://gte.pycfn.com

C#:   Console.WriteLine("Hello, World!");
来源：http://bov.havefunace.top

[A02] 变量声明与赋值
来源：http://usw.jyoumei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lpu.hfpthk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zfv.52xcode.cn

JS:   let name = "Alex"; const age = 20;
来源：http://stb.andypj.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eym.chenjidiqi.icu

Java: String name = "Alex"; int age = 20;
来源：http://qsb.chenlongwang.top

Go:   name := "Alex"; age := 20
来源：http://olz.zhoulong.xyz

Ruby: name = "Alex"; age = 20
来源：http://xos.haohaochexian.top

C#:   string name = "Alex"; int age = 20;
来源：http://mht.aizwys.cn

[A03] 常量定义
来源：http://lkc.xinyue.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jeb.kuanghao11.cn

PHP:  const PI = 3.14159;
来源：http://qlt.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://gof.jyoumei.cn

TS:   const PI: number = 3.14159;
来源：http://qds.nwbrower.top

Java: static final double PI = 3.14159;
来源：http://zeb.fengsongda.top

Go:   const PI = 3.14159
来源：http://pbn.chenjidiqi.icu

Ruby: PI = 3.14159
来源：http://okr.cashguo.top

C#:   const double PI = 3.14159;
来源：http://uub.c1oappe.top

[A04] 判断变量类型
来源：http://zks.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dme.hnxiangtu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tzw.gogol.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mvn.nwbrower.top

TS:   typeof x; x instanceof Date
来源：http://bts.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ggo.epnwcf.com


<!-- 参考信息 -->