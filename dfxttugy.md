代发 wailian999

[U35] Py：发送邮件
来源：http://vxt.bjfxy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cxg.svipenyu.cn

[U36] Py：定时任务
来源：http://zuj.hcnkem.com

schedule.every(10).minutes.do(job)
来源：http://wmp.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://apg.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://aor.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://dsc.tanke756.top

Path(__file__).resolve().parent
来源：http://ebf.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://wfb.bbcook.cn

sys.stdout.isatty()
来源：http://gqc.xuetiantiany.cn

[U40] Py：打印到标准错误
来源：http://kfl.xylfe.cn

print("err", file=sys.stderr)
来源：http://pnc.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://zxb.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ibv.birdmap.top

[U42] PHP：PSR-4 自动加载
来源：http://sru.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nsj.daria6918.cn

[U43] PHP：声明命名空间
来源：http://oeb.smart0.xyz

namespace App\Http;
来源：http://yss.smart0.xyz

[U44] PHP：开启严格类型
来源：http://pgp.cdnleiting.top

declare(strict_types=1);
来源：http://ifk.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://clq.yvedp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://eyb.hywenlv.cn

[U46] PHP：可空类型
来源：http://kqh.9152youxi.cn

?string $name = null
来源：http://svh.0kj1m.cn

[U47] PHP：联合类型
来源：http://kbv.yvedp.cn

int|string $id
来源：http://pfl.guowangkeji.top

[U48] PHP：纯枚举
来源：http://scw.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zni.9152youxi.cn

[U49] PHP：只读属性
来源：http://lss.xylfe.cn

public readonly string $name
来源：http://tys.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://qkf.zhaomingkeji.xyz

public function __construct(private int $id) {}
来源：http://uuh.hywenlv.cn

[U51] PHP：数组解构
来源：http://ozu.jiagoushi.top

[$a, $b] = $arr;
来源：http://osd.jinghuilouyu.cn

[U52] PHP：箭头函数
来源：http://mas.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://wny.xingfuxueyuan.xyz

[U53] PHP：空合并运算符
来源：http://wli.shuidangran.top

$v = $a ?? $b ?? "default";
来源：http://aud.guowangkeji.top

[U54] PHP：空安全调用
来源：http://djd.redwolf501.top

$obj?->method()
来源：http://wtu.wangdashe.top

[U55] PHP：match 表达式
来源：http://xat.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vwc.0kj1m.cn

[U56] PHP：命名参数
来源：http://gjp.tianlin.xyz

f(a: 1, b: 2)
来源：http://vgd.tianlin.xyz

[U57] PHP：字符串插值
来源：http://vaw.bjfxy.top

"值: {$a}"
来源：http://rpe.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://utv.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hzp.nanxinkj.top

[U59] PHP：自定义排序
来源：http://cpw.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jta.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://tzv.feifeiyinyue.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://evy.wangdashe.top

[U61] PHP：正则
来源：http://mhi.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uod.sxryk.cn

[U62] PHP：日期对象
来源：http://txx.haohaochexian.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gpi.shuidangran.top

[U63] PHP：文件读写
来源：http://slx.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ogr.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://jbu.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://iuv.wangdashe.top

[U65] PHP：会话
来源：http://pjy.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jhi.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://cvy.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cql.c1oappe.top

[U67] PHP：处理文件上传
来源：http://oqo.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jqk.hongshengwenyu.top

[U68] PHP：PDO 连接
来源：http://rzg.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://znu.jqgfzy.top

[U69] PHP：PDO 预处理
来源：http://waa.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ckn.nwbrower.top

[U70] PHP：PDO 事务
来源：http://xsh.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uhq.havefunace.top

[U71] PHP：抛出异常
来源：http://uxo.shanyushiyangkeji.top

throw new RuntimeException("失败", 500);
来源：http://alq.meibo888.top

[U72] PHP：写错误日志
来源：http://bmn.yvedp.cn

error_log("失败: " . $e->getMessage());
来源：http://fhh.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://nnr.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://wgx.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://izd.zycfv.cn

getenv("APP_ENV") ?: "production"
来源：http://exe.hcnkem.com

[U75] PHP：依赖注入
来源：http://feb.316326.xyz

composer require psr/container
来源：http://jvy.9152youxi.cn

[U76] PHP：简单路由
来源：http://tvg.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vyu.daria6918.cn

[U77] PHP：模板渲染
来源：http://zdo.tian-w.cn

composer require twig/twig
来源：http://olt.xylfe.cn

[U78] PHP：单元测试
来源：http://cif.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://tqz.yuanzhike.top

[U79] PHP：静态分析
来源：http://mfo.zycfv.cn

composer require --dev phpstan/phpstan
来源：http://ifv.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://ijv.cheryme.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://syi.chenjidiqi.icu

[U81] JS：初始化项目
来源：http://dcl.hesvh.cn

npm init -y;  npm i express
来源：http://qpf.cucudq.cn

[U82] JS：package.json 脚本
来源：http://xkq.yueranfly.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://afk.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://byj.andypj.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://ycz.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://per.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iuq.xziqi.cn

[U85] JS：可选链
来源：http://sam.zhongyouzk.top

a?.b?.c
来源：http://guw.aibaodan.cn

[U86] JS：空值合并
来源：http://yos.yuxming.cn

a ?? b
来源：http://rdz.jiagoushi.top

[U87] JS：解构默认值
来源：http://ian.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://pgl.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://ohd.svipenyu.cn

{ ...a, ...b }
来源：http://lit.yj20258.top

[U89] JS：数组去重
来源：http://hrw.fzhhl.top

[...new Set(arr)]
来源：http://puj.epnwcf.com

[U90] JS：数字数组排序
来源：http://ota.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://mdi.yj20258.top

[U91] JS：对象键值遍历
来源：http://zrz.jqgfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lvb.feifeiyinyue.top

[U92] JS：深拷贝
来源：http://vdz.nanxinkj.top

structuredClone(obj)
来源：http://gwb.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://kcp.quarkkingdee.top

`共 ${n} 条`
来源：http://cvz.hfpthk.cn

[U94] JS：箭头函数
来源：http://vow.mhx1999.top

const double = x => x * 2;
来源：http://rzc.jiagoushi.top

[U95] JS：Promise 包装
来源：http://dqu.ctjpmb.com

new Promise((resolve, reject) => {})
来源：http://mhr.smart0.xyz

[U96] JS：async/await 与异常
来源：http://gdv.yj202588.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ehk.wangdashe.top

[U97] JS：并发请求
来源：http://kip.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://icw.yj202588.top

[U98] JS：fetch 带 JSON
来源：http://kxm.pengpengdd.cyou

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rti.bjfxy.top

[U99] JS：事件监听
来源：http://bby.kuanghao11.cn

el.addEventListener("click", e => {})
来源：http://ozy.yfazqb.com

[U100] JS：DOM 查询
来源：http://msf.hesvh.cn

document.querySelector(".item")
来源：http://mqj.uphjek.com

[U101] JS：classList 操作
来源：http://vtm.havefunace.top

el.classList.toggle("active")
来源：http://ffl.fengsongda.top

[U102] JS：本地存储
来源：http://ndt.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kaz.yuxming.cn

[U103] JS：定时器
来源：http://jis.daria6918.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bto.shangyingyoupin.top

[U104] JS：防抖
来源：http://xch.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wrt.ctjpmb.com

[U105] JS：节流
来源：http://dwj.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://khw.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://gyi.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dsb.redwolf501.top

[U107] JS：数字千分位
来源：http://qgn.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://faq.gotoacloud.top

[U108] JS：随机整数
来源：http://sxb.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://szd.yanxiufei.cn

[U109] JS：数组分组
来源：http://uzf.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://pxq.jiagoushi.top

[U110] JS：数组分块
来源：http://nvb.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fdc.svipenyu.cn

[U111] JS：对象转 Map
来源：http://vaz.yangfankeji.com

new Map(Object.entries(obj))
来源：http://flh.ehwqpu.com

[U112] JS：字符串补位
来源：http://qkd.zhongyouzk.top

"7".padStart(3, "0")
来源：http://iul.ctjpmb.com

[U113] JS：正则替换全部
来源：http://rdo.zhixingplan.top

s.replaceAll("a", "b")
来源：http://yvp.jlsjyb.cn

[U114] JS：JSON 深比较
来源：http://vwk.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://iyj.daxiang520.top

[U115] JS：生成 UUID
来源：http://wfm.fehbvm.com

crypto.randomUUID()
来源：http://syi.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://tqa.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://wku.fzhhl.top

[U117] JS：单元测试
来源：http://eks.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://hss.chenjidiqi.icu

[U118] JS：开发服务器
来源：http://jbs.yj20258888.top

npm i -D vite;  npx vite
来源：http://wnv.0kj1m.cn

[U119] JS：生产构建
来源：http://wml.gogol.net.cn

npx vite build
来源：http://dsn.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://tbq.guowangkeji.top

import.meta.env.VITE_API_URL
来源：http://tus.hfpthk.cn

================================================================================
来源：http://uzp.cashguo.top

统计汇总
来源：http://cex.hcnkem.com

================================================================================
来源：http://krh.dashuyun.cn

按语言统计（条）：
来源：http://zbz.shangyingyoupin.top

Python ......... 252
来源：http://nfk.pycfn.com

PHP ............ 252
来源：http://fii.sxryk.cn

JavaScript ..... 252
来源：http://kne.havefunace.top

TypeScript ..... 212
来源：http://fmj.cheryme.top

Java ........... 212
来源：http://iip.jinqigfzy.top

Go ............. 212
来源：http://dax.feifeiyinyue.top

Ruby ........... 212
来源：http://rij.zhengqikj.top

C# ............. 212
来源：http://dpz.cheryme.top

C .............. 30
来源：http://zwm.cdnleiting.top

C++ ............ 30
来源：http://baz.pycfn.com

SQL ............ 90
来源：http://bwh.sysykeji.top

Bash ........... 80
来源：http://vzo.c1oappe.top

Kotlin ......... 15
来源：http://gto.tian-w.cn

Swift .......... 15
来源：http://vir.wangshuangyany.cn

Lua ............ 10
来源：http://quy.zycfv.cn

Perl ........... 10
来源：http://pra.ydzc1.top

Scala .......... 10
来源：http://xln.chenjidiqi.icu

------------------------------------
来源：http://ifi.jlsjyb.cn

合计 ........... 2106 条
来源：http://vrm.sxryk.cn

按章节统计：
来源：http://rmc.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bnf.yuxming.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gyw.dianchejie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cnz.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://auf.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gjk.9152youxi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cja.ydjk.org.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oon.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lut.9152youxi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bue.guannengcc.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hzc.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kng.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pia.guowangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zxn.zhongyouzk.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vpd.yueranfly.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://res.nanxinkj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qyl.yanxiufei.cn

Q SQL 专题                              90
来源：http://nbl.xziqi.cn

R Bash 专题                             80
来源：http://qko.cqqwz.cn

S C / C++ 专题                          60
来源：http://gik.zycfv.cn

T 其他语言补充                          60
来源：http://equ.xuetiantiany.cn

U 高频实用片段                         120
来源：http://njf.sxryk.cn

------------------------------------
来源：http://rip.shangyingyoupin.top

合计                                  2106 条
来源：http://cxp.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://wdb.yonumen.top

使用提醒
来源：http://bci.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://fzq.yonumen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sop.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vgk.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yki.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tfc.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://msn.sxryk.cn

—— 文件结束 ——
来源：http://qeh.redwolf501.top

================================================================================
来源：http://gtg.gotoacloud.top

程序语言常见例子速查手册（2024 版）
来源：http://emb.redwolf501.top

Common Programming Examples Cheat Book
来源：http://dks.quarkkingdee.top

================================================================================
来源：http://xbe.xingfuxueyuan.xyz

【收录内容】
来源：http://okh.yangfankeji.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://qmh.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kmq.guannengcc.top

SQL · Bash · C · C++
来源：http://pec.haohaochexian.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hoq.snrcjt.cn

【使用说明】
来源：http://yfd.gzhubu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sdq.tanke756.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cpc.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ypx.zdqjudy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zlc.yj202588.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zav.vqdsnc.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hmn.epnwcf.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nfa.meibo888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pfh.guannengcc.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jrl.yvedp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qnw.xingfuxueyuan.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://stk.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nid.nwbrower.top

【文件统计】
来源：http://lac.cheryme.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hiq.guannengcc.top

--------------------------------------------------------------------------------
来源：http://djl.iojbl.cn

目  录
来源：http://qsq.fehbvm.com

--------------------------------------------------------------------------------
来源：http://dkd.zhiwuduotai.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ylz.tarul.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dce.uphjek.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yyy.hcnkem.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ndq.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ltc.zhixingplan.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://icd.ehwqpu.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gbo.sufxvd.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rjk.tarul.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://flz.tian-w.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ihq.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vdi.vehdjk.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fvz.jinghuilouyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eff.meibo888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zmw.yonumen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yao.yj20258.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iyz.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ekq.yongpay.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fuo.yvedp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nui.shzxlz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://scn.yuxming.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lbl.sjlbkw.cn

================================================================================
来源：http://ser.yj202588.top

A. 基础语法与类型
来源：http://zoe.jyoumei.cn

================================================================================
来源：http://wqg.daria6918.cn

[A01] Hello World
来源：http://fnf.0kj1m.cn

Py:   print("Hello, World!")
来源：http://phj.cdnleiting.top

PHP:  echo "Hello, World!";
来源：http://bcq.gaohongyu789.top

JS:   console.log("Hello, World!");
来源：http://qsr.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://poh.aizwys.cn

Java: System.out.println("Hello, World!");
来源：http://lir.jinyuanbaomall.cn

Go:   fmt.Println("Hello, World!")
来源：http://mzq.9152youxi.cn

Ruby: puts "Hello, World!"
来源：http://mls.yuanzhike.top

C#:   Console.WriteLine("Hello, World!");
来源：http://iyv.wangdashe.top

[A02] 变量声明与赋值
来源：http://jgp.jlsjyb.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://axg.zhoulong.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://qpj.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iow.cheryme.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fnr.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://rwx.cdnleiting.top

Go:   name := "Alex"; age := 20
来源：http://pax.tanke756.top

Ruby: name = "Alex"; age = 20
来源：http://smh.uphjek.com

C#:   string name = "Alex"; int age = 20;
来源：http://ryf.mhx1999.top

[A03] 常量定义
来源：http://qcp.jlsjyb.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kcj.yj20258888.top

PHP:  const PI = 3.14159;
来源：http://jlx.sxryk.cn


<!-- 参考信息 -->