代发 wailian999

[U37] Py：读写 Excel
来源：http://ylm.gotoacloud.top

pandas.read_excel / DataFrame.to_excel
来源：http://wtp.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://gzv.jlsjyb.cn

Path(__file__).resolve().parent
来源：http://fpc.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://jvx.chenzaomai.com

sys.stdout.isatty()
来源：http://hgf.daxiang520.top

[U40] Py：打印到标准错误
来源：http://ixz.guannengcc.top

print("err", file=sys.stderr)
来源：http://ymd.gaohongyu789.top

[U41] PHP：初始化 Composer 项目
来源：http://odc.ydjk.org.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wdb.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://evh.tarul.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://arz.daxiang520.top

[U43] PHP：声明命名空间
来源：http://bhu.sjlbkw.cn

namespace App\Http;
来源：http://zie.svipenyu.cn

[U44] PHP：开启严格类型
来源：http://nna.sxryk.cn

declare(strict_types=1);
来源：http://frp.c1oappe.top

[U45] PHP：类型声明与返回类型
来源：http://cgx.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xde.guannengcc.top

[U46] PHP：可空类型
来源：http://vet.sjlbkw.cn

?string $name = null
来源：http://gbp.iojbl.cn

[U47] PHP：联合类型
来源：http://ets.fanxiaobao.xyz

int|string $id
来源：http://xnr.uphjek.com

[U48] PHP：纯枚举
来源：http://jup.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://omv.hesvh.cn

[U49] PHP：只读属性
来源：http://inh.jianghu66.top

public readonly string $name
来源：http://jup.hysaishi.cn

[U50] PHP：构造器属性提升
来源：http://tzm.ehwqpu.com

public function __construct(private int $id) {}
来源：http://aht.tanke756.top

[U51] PHP：数组解构
来源：http://fsc.gaohongyu789.top

[$a, $b] = $arr;
来源：http://rmj.ivvv.top

[U52] PHP：箭头函数
来源：http://tcj.tanke756.top

$double = fn($x) => $x * 2;
来源：http://xok.xziqi.cn

[U53] PHP：空合并运算符
来源：http://grx.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://gvb.iojbl.cn

[U54] PHP：空安全调用
来源：http://raq.jlsjyb.cn

$obj?->method()
来源：http://pas.yangfankeji.com

[U55] PHP：match 表达式
来源：http://nwz.bjfxy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mtm.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://bav.aizwys.cn

f(a: 1, b: 2)
来源：http://ddl.fengsongda.top

[U57] PHP：字符串插值
来源：http://xby.sweek.top

"值: {$a}"
来源：http://xnh.jlsjyb.cn

[U58] PHP：数组三件套
来源：http://kyf.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://par.dianchejie.cn

[U59] PHP：自定义排序
来源：http://aen.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zxf.tarul.cn

[U60] PHP：JSON 编解码
来源：http://bzl.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iix.tarul.cn

[U61] PHP：正则
来源：http://htr.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iag.vqdsnc.cn

[U62] PHP：日期对象
来源：http://mdu.fanxiaobao.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gxh.quarkkingdee.top

[U63] PHP：文件读写
来源：http://fyk.meibo888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://onu.gzhubu.top

[U64] PHP：目录遍历
来源：http://cqc.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://dex.ctjpmb.com

[U65] PHP：会话
来源：http://rac.daxiang520.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ide.yueranfly.top

[U66] PHP：设置 Cookie
来源：http://voi.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qug.xingfuxueyuan.xyz

[U67] PHP：处理文件上传
来源：http://vgs.jinqigfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ymc.redwolf501.top

[U68] PHP：PDO 连接
来源：http://ein.9152youxi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dju.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://urn.daria6918.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aig.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://wgl.ydjk.org.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lqr.redwolf501.top

[U71] PHP：抛出异常
来源：http://lzt.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://xub.316326.xyz

[U72] PHP：写错误日志
来源：http://nri.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://ftc.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://jum.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://thm.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://muo.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://rvh.ydjk.org.cn

[U75] PHP：依赖注入
来源：http://oqi.yonumen.top

composer require psr/container
来源：http://qvc.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://vqk.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://roq.bjfxy.top

[U77] PHP：模板渲染
来源：http://llv.andypj.xyz

composer require twig/twig
来源：http://ipy.ppjwa.cn

[U78] PHP：单元测试
来源：http://njt.0kj1m.cn

composer require --dev phpunit/phpunit
来源：http://hrm.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://ppu.gotoacloud.top

composer require --dev phpstan/phpstan
来源：http://qjb.hnqzz.top

[U80] PHP：代码规范修复
来源：http://jlq.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gui.cucudq.cn

[U81] JS：初始化项目
来源：http://wzn.shzxlz.cn

npm init -y;  npm i express
来源：http://fvq.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://nga.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tck.ybcxt.top

[U83] JS：ES Module 导入导出
来源：http://kem.cqqwz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kky.jqgufenzy.top

[U84] JS：CommonJS 写法
来源：http://bjh.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://mkh.zhijiandao.cn

[U85] JS：可选链
来源：http://ufn.sweek.top

a?.b?.c
来源：http://ihn.xziqi.cn

[U86] JS：空值合并
来源：http://giw.iojbl.cn

a ?? b
来源：http://rot.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://mnr.jyoumei.cn

const { a = 1, b = 2 } = obj;
来源：http://svo.daria6918.cn

[U88] JS：对象展开合并
来源：http://wah.hnxiangtu.top

{ ...a, ...b }
来源：http://iew.zhongyouzk.top

[U89] JS：数组去重
来源：http://rwp.hesvh.cn

[...new Set(arr)]
来源：http://pzz.daxiang520.top

[U90] JS：数字数组排序
来源：http://ftb.gaohongyu789.top

[...arr].sort((a, b) => a - b)
来源：http://bdc.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://pji.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yvz.jiagoushi.top

[U92] JS：深拷贝
来源：http://hwx.gotoacloud.top

structuredClone(obj)
来源：http://ggu.jinqigufen.top

[U93] JS：模板字符串
来源：http://qhc.hesvh.cn

`共 ${n} 条`
来源：http://gsl.sxryk.cn

[U94] JS：箭头函数
来源：http://vpo.yangfankeji.com

const double = x => x * 2;
来源：http://dzj.cqqwz.cn

[U95] JS：Promise 包装
来源：http://qss.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://vkf.c1oappe.top

[U96] JS：async/await 与异常
来源：http://tiv.pengpengdd.cyou

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zor.gzhubu.top

[U97] JS：并发请求
来源：http://xea.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://swh.ywan-chungtsiang.top

[U98] JS：fetch 带 JSON
来源：http://cnl.feifeiyinyue.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ptz.smart0.xyz

[U99] JS：事件监听
来源：http://xav.yvedp.cn

el.addEventListener("click", e => {})
来源：http://qyf.chenlongwang.top

[U100] JS：DOM 查询
来源：http://tub.andypj.xyz

document.querySelector(".item")
来源：http://tpa.wangshuangyany.cn

[U101] JS：classList 操作
来源：http://gqr.yvedp.cn

el.classList.toggle("active")
来源：http://wem.shanyushiyangtech.top

[U102] JS：本地存储
来源：http://vqj.vehdjk.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://rvv.vehdjk.com

[U103] JS：定时器
来源：http://poj.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xrf.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://rpx.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://inr.shanyushiyangtech.top

[U105] JS：节流
来源：http://bgk.nwbrower.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jtw.52xcode.cn

[U106] JS：日期格式化
来源：http://oxg.zhongyouzk.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oyn.ctjpmb.com

[U107] JS：数字千分位
来源：http://rsb.shangyingyoupin.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qmk.cheryme.top

[U108] JS：随机整数
来源：http://cie.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wlu.jlsjyb.cn

[U109] JS：数组分组
来源：http://swp.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://aoo.snrcjt.cn

[U110] JS：数组分块
来源：http://uzp.jianghu66.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oed.ivvv.top

[U111] JS：对象转 Map
来源：http://lfj.fzhhl.top

new Map(Object.entries(obj))
来源：http://uur.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://juk.shuidangran.top

"7".padStart(3, "0")
来源：http://nzd.hesvh.cn

[U113] JS：正则替换全部
来源：http://dxb.316326.xyz

s.replaceAll("a", "b")
来源：http://ixy.jinghuilouyu.cn

[U114] JS：JSON 深比较
来源：http://npm.bbcook.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fpz.sxryk.cn

[U115] JS：生成 UUID
来源：http://kzm.hongshengwenyu.top

crypto.randomUUID()
来源：http://kbl.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://oll.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://jxy.cqqwz.cn

[U117] JS：单元测试
来源：http://aik.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://cqq.havefunace.top

[U118] JS：开发服务器
来源：http://ver.sysykeji.top

npm i -D vite;  npx vite
来源：http://zyf.pycfn.com

[U119] JS：生产构建
来源：http://uuo.guannengcc.top

npx vite build
来源：http://deh.hesvh.cn

[U120] JS：读取环境变量（Vite）
来源：http://qko.pycfn.com

import.meta.env.VITE_API_URL
来源：http://cqb.bbcook.cn

================================================================================
来源：http://wkm.tian-w.cn

统计汇总
来源：http://cvv.svipenyu.cn

================================================================================
来源：http://ver.yj20258888.top

按语言统计（条）：
来源：http://hml.gotoacloud.top

Python ......... 252
来源：http://sxk.guowangkeji.top

PHP ............ 252
来源：http://irk.kuanghao11.cn

JavaScript ..... 252
来源：http://tsm.gzhubu.top

TypeScript ..... 212
来源：http://lpc.zhiwuduotai.top

Java ........... 212
来源：http://hrq.yanxiufei.cn

Go ............. 212
来源：http://vcd.kuanghao11.cn

Ruby ........... 212
来源：http://jvh.hongshengwenyu.top

C# ............. 212
来源：http://kqv.xuanzx.com

C .............. 30
来源：http://boc.gotoacloud.top

C++ ............ 30
来源：http://qhy.ivvv.top

SQL ............ 90
来源：http://zta.fengsongda.top

Bash ........... 80
来源：http://ovd.jinqigufen.top

Kotlin ......... 15
来源：http://cdh.svipenyu.cn

Swift .......... 15
来源：http://xfj.ppjwa.cn

Lua ............ 10
来源：http://aoz.hongshengwenyu.top

Perl ........... 10
来源：http://vbq.mhx1999.top

Scala .......... 10
来源：http://kgu.yueranfly.top

------------------------------------
来源：http://hmz.yongpay.top

合计 ........... 2106 条
来源：http://djy.yuanzhike.top

按章节统计：
来源：http://bvg.fehbvm.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://auk.ctjpmb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fhz.yonumen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uhm.cqqwz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lkd.xinyue.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ggn.yj20258888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cza.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gcs.zhixingplan.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://swk.yj20258888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sdv.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fvx.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mwg.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oui.ydzc1.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cjm.yj20258.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rrz.havefunace.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vdr.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://syt.iojbl.cn

Q SQL 专题                              90
来源：http://pjv.hywenlv.cn

R Bash 专题                             80
来源：http://znr.fktsv.cn

S C / C++ 专题                          60
来源：http://rvk.gotoacloud.top

T 其他语言补充                          60
来源：http://yjl.yvedp.cn

U 高频实用片段                         120
来源：http://xyn.ivvv.top

------------------------------------
来源：http://dex.jinqigufen.top

合计                                  2106 条
来源：http://sfq.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://euo.shangyingyoupin.top

使用提醒
来源：http://yqv.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://hcx.jianghu66.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yav.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eeg.yuanzhike.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mrk.hfpthk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vbf.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hup.zhaomingkeji.xyz

—— 文件结束 ——
来源：http://inz.zdqjudy.top

================================================================================
来源：http://jwf.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://bam.hammf.cn

Common Programming Examples Cheat Book
来源：http://vvu.zhijiandao.cn

================================================================================
来源：http://itc.meibo888.top

【收录内容】
来源：http://lxf.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rmh.aizwys.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xbs.iojbl.cn

SQL · Bash · C · C++
来源：http://njq.yangfankeji.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yax.haohaochexian.top

【使用说明】
来源：http://yst.xingfuxueyuan.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ssf.ivvv.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tzr.daxiang520.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pva.hysaishi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yby.yj20258888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ukx.aizwys.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oie.wangshuangyany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rwl.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://csd.guannengcc.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tnq.jyoumei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tah.yj20258888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hqu.hywenlv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vjl.jqgufenzy.top

【文件统计】
来源：http://eom.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://att.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://bru.mhx1999.top

目  录
来源：http://kzz.hammf.cn

--------------------------------------------------------------------------------
来源：http://gnm.yj202588.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bty.tian-w.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dgm.jqgfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qrs.cashguo.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zpo.svipenyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uba.iojbl.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wwe.sufxvd.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zxt.cucudq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wga.yongpay.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bdi.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dmw.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ujz.ywan-chungtsiang.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://icw.snrcjt.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eip.guowangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://twt.vehdjk.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://enz.yanxiufei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yii.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://knh.ydzc1.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qrp.daria6918.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iqv.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fzl.zhijiandao.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mpt.dashuyun.cn

================================================================================
来源：http://tcf.sweek.top

A. 基础语法与类型
来源：http://kjn.cucudq.cn

================================================================================
来源：http://qut.9152youxi.cn

[A01] Hello World
来源：http://gai.yj20258.top

Py:   print("Hello, World!")
来源：http://kaa.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://adb.jqgufenzy.top

JS:   console.log("Hello, World!");
来源：http://kue.yfazqb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rsg.gotoacloud.top

Java: System.out.println("Hello, World!");
来源：http://iea.iojbl.cn

Go:   fmt.Println("Hello, World!")
来源：http://opl.shangyingyoupin.top

Ruby: puts "Hello, World!"
来源：http://hlq.redwolf501.top

C#:   Console.WriteLine("Hello, World!");
来源：http://psa.guannengcc.top

[A02] 变量声明与赋值
来源：http://peu.cqqwz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://slg.sysykeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://oub.shzxlz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ofl.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yie.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://hdr.xuetiantiany.cn

Go:   name := "Alex"; age := 20
来源：http://xaa.yanxiufei.cn

Ruby: name = "Alex"; age = 20
来源：http://fuj.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://eau.jinqigfzy.top

[A03] 常量定义
来源：http://hcv.tianlin.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zzq.zhixingplan.top

PHP:  const PI = 3.14159;
来源：http://zus.jqgufenzy.top

JS:   const PI = 3.14159;
来源：http://gip.sxryk.cn

TS:   const PI: number = 3.14159;
来源：http://kwd.yangfankeji.com

Java: static final double PI = 3.14159;
来源：http://auz.gotoacloud.top

Go:   const PI = 3.14159
来源：http://pvf.chenjidiqi.icu


<!-- 参考信息 -->