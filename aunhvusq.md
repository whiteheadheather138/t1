代发 wailian999

[U35] Py：发送邮件
来源：http://mam.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uqa.cheryme.top

[U36] Py：定时任务
来源：http://fuw.nanxuanxn.top

schedule.every(10).minutes.do(job)
来源：http://pfu.tian-w.cn

[U37] Py：读写 Excel
来源：http://zsq.0kj1m.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sxz.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://pld.uphjek.com

Path(__file__).resolve().parent
来源：http://pbg.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://nzh.xinyue.icu

sys.stdout.isatty()
来源：http://vse.ctjpmb.com

[U40] Py：打印到标准错误
来源：http://jha.aibaodan.cn

print("err", file=sys.stderr)
来源：http://yyj.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://kgn.haohaochexian.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gza.yanxiufei.cn

[U42] PHP：PSR-4 自动加载
来源：http://qdd.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gbs.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://amx.jianghu66.top

namespace App\Http;
来源：http://prm.aizwys.cn

[U44] PHP：开启严格类型
来源：http://pqc.sysykeji.top

declare(strict_types=1);
来源：http://iyo.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://bec.gotoacloud.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nnc.jqgufenzy.top

[U46] PHP：可空类型
来源：http://hwj.snrcjt.cn

?string $name = null
来源：http://hui.haohaochexian.top

[U47] PHP：联合类型
来源：http://vnb.yj202588.top

int|string $id
来源：http://fcy.ydzc1.top

[U48] PHP：纯枚举
来源：http://zqj.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rfa.epnwcf.com

[U49] PHP：只读属性
来源：http://gpj.shzxlz.cn

public readonly string $name
来源：http://ugt.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://uqd.xziqi.cn

public function __construct(private int $id) {}
来源：http://vep.fehbvm.com

[U51] PHP：数组解构
来源：http://bql.sjlbkw.cn

[$a, $b] = $arr;
来源：http://wln.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://nxg.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://eyn.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://qog.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://cor.fengsongda.top

[U54] PHP：空安全调用
来源：http://kyn.zhaomingkeji.xyz

$obj?->method()
来源：http://xbk.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://rsf.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tzf.hfpthk.cn

[U56] PHP：命名参数
来源：http://ctf.ppjwa.cn

f(a: 1, b: 2)
来源：http://huk.meibo888.top

[U57] PHP：字符串插值
来源：http://mxq.jinqigufen.top

"值: {$a}"
来源：http://pal.hfpthk.cn

[U58] PHP：数组三件套
来源：http://znh.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mpq.smart0.xyz

[U59] PHP：自定义排序
来源：http://ofo.daxiang520.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://noe.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://kwh.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bbt.yanxiufei.cn

[U61] PHP：正则
来源：http://uhq.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hbg.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://yaw.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sub.smart0.xyz

[U63] PHP：文件读写
来源：http://saw.c1oappe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lgw.hcnkem.com

[U64] PHP：目录遍历
来源：http://afi.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://bnd.yj202588.top

[U65] PHP：会话
来源：http://iob.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://umg.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://xef.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dws.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://gqo.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ime.9152youxi.cn

[U68] PHP：PDO 连接
来源：http://wdy.nwbrower.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qyt.zhoulong.xyz

[U69] PHP：PDO 预处理
来源：http://yza.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jvo.yj20258888.top

[U70] PHP：PDO 事务
来源：http://wey.aibaodan.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cdr.yonumen.top

[U71] PHP：抛出异常
来源：http://lef.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://fmi.yfazqb.com

[U72] PHP：写错误日志
来源：http://vdu.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://tkq.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://xps.yongpay.top

parse_ini_file("config.ini", true)
来源：http://jnk.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://xei.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://btz.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://mch.jinqigufen.top

composer require psr/container
来源：http://ylb.smart0.xyz

[U76] PHP：简单路由
来源：http://lgm.vehdjk.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pli.svipenyu.cn

[U77] PHP：模板渲染
来源：http://khg.ywan-chungtsiang.top

composer require twig/twig
来源：http://nnu.gogol.net.cn

[U78] PHP：单元测试
来源：http://sfp.yj202588.top

composer require --dev phpunit/phpunit
来源：http://big.havefunace.top

[U79] PHP：静态分析
来源：http://afu.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://avc.yfazqb.com

[U80] PHP：代码规范修复
来源：http://rry.havefunace.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uwr.xziqi.cn

[U81] JS：初始化项目
来源：http://hzn.gotoacloud.top

npm init -y;  npm i express
来源：http://ypa.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://qek.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fes.c1oappe.top

[U83] JS：ES Module 导入导出
来源：http://agh.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yxy.fengsongda.top

[U84] JS：CommonJS 写法
来源：http://dbn.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://syj.ybcxt.top

[U85] JS：可选链
来源：http://yyy.hcnkem.com

a?.b?.c
来源：http://uwh.yj202588.top

[U86] JS：空值合并
来源：http://qvn.sxryk.cn

a ?? b
来源：http://grg.yj20258888.top

[U87] JS：解构默认值
来源：http://loc.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://jwl.hcnkem.com

[U88] JS：对象展开合并
来源：http://aly.xuetiantiany.cn

{ ...a, ...b }
来源：http://vmi.feifeiyinyue.top

[U89] JS：数组去重
来源：http://gel.cashguo.top

[...new Set(arr)]
来源：http://bzw.yongpay.top

[U90] JS：数字数组排序
来源：http://thi.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://haa.ivvv.top

[U91] JS：对象键值遍历
来源：http://dak.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vkx.birdmap.top

[U92] JS：深拷贝
来源：http://zxw.shangyingyoupin.top

structuredClone(obj)
来源：http://myr.ivvv.top

[U93] JS：模板字符串
来源：http://yaz.guannengcc.top

`共 ${n} 条`
来源：http://aty.cdnleiting.top

[U94] JS：箭头函数
来源：http://ikn.andypj.xyz

const double = x => x * 2;
来源：http://mun.hesvh.cn

[U95] JS：Promise 包装
来源：http://bku.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://qqq.haohaochexian.top

[U96] JS：async/await 与异常
来源：http://qbn.yuanzhike.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gbb.zhoulong.xyz

[U97] JS：并发请求
来源：http://neo.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://hgr.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://kox.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jrv.yueranfly.top

[U99] JS：事件监听
来源：http://bpw.xinyue.icu

el.addEventListener("click", e => {})
来源：http://coz.jyoumei.cn

[U100] JS：DOM 查询
来源：http://ybd.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://uqx.jianghu66.top

[U101] JS：classList 操作
来源：http://dlu.zhongyouzk.top

el.classList.toggle("active")
来源：http://hxi.haohaochexian.top

[U102] JS：本地存储
来源：http://srq.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jnp.316326.xyz

[U103] JS：定时器
来源：http://qye.birdmap.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wun.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://cwy.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://slv.jianghu66.top

[U105] JS：节流
来源：http://ufb.cqqwz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lxk.jiagoushi.top

[U106] JS：日期格式化
来源：http://gds.yj202588.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bff.jqgufenzy.top

[U107] JS：数字千分位
来源：http://afv.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sfd.tarul.cn

[U108] JS：随机整数
来源：http://ueu.yueranfly.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kdh.yvedp.cn

[U109] JS：数组分组
来源：http://glv.epnwcf.com

Object.groupBy(arr, x => x.type)
来源：http://nln.chenjidiqi.icu

[U110] JS：数组分块
来源：http://lis.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nza.jiagoushi.top

[U111] JS：对象转 Map
来源：http://lal.wangshuangyany.cn

new Map(Object.entries(obj))
来源：http://dyt.birdmap.top

[U112] JS：字符串补位
来源：http://mfp.uphjek.com

"7".padStart(3, "0")
来源：http://dwm.bjfxy.top

[U113] JS：正则替换全部
来源：http://vna.hesvh.cn

s.replaceAll("a", "b")
来源：http://qwv.xuanzx.com

[U114] JS：JSON 深比较
来源：http://bdt.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wqz.ivvv.top

[U115] JS：生成 UUID
来源：http://vem.ehwqpu.com

crypto.randomUUID()
来源：http://kaj.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://bcf.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://rzh.nwbrower.top

[U117] JS：单元测试
来源：http://yoq.tarul.cn

npm i -D vitest;  npx vitest
来源：http://twa.snrcjt.cn

[U118] JS：开发服务器
来源：http://sbp.yongpay.top

npm i -D vite;  npx vite
来源：http://mil.tianlin.xyz

[U119] JS：生产构建
来源：http://oob.hcnkem.com

npx vite build
来源：http://qyd.guannengcc.top

[U120] JS：读取环境变量（Vite）
来源：http://ahq.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://lmn.jinqigufen.top

================================================================================
来源：http://wud.zhongyouzk.top

统计汇总
来源：http://mkk.sjlbkw.cn

================================================================================
来源：http://uxs.c1oappe.top

按语言统计（条）：
来源：http://wzg.hywenlv.cn

Python ......... 252
来源：http://xwv.guannengcc.top

PHP ............ 252
来源：http://sch.yanxiufei.cn

JavaScript ..... 252
来源：http://bdr.shanyushiyangtech.top

TypeScript ..... 212
来源：http://zkt.sxryk.cn

Java ........... 212
来源：http://xez.uphjek.com

Go ............. 212
来源：http://hph.ydjk.org.cn

Ruby ........... 212
来源：http://hvn.sweek.top

C# ............. 212
来源：http://zta.iojbl.cn

C .............. 30
来源：http://vtg.zycfv.cn

C++ ............ 30
来源：http://rap.redwolf501.top

SQL ............ 90
来源：http://dxk.tianlin.xyz

Bash ........... 80
来源：http://nzk.bbcook.cn

Kotlin ......... 15
来源：http://qzz.hfpthk.cn

Swift .......... 15
来源：http://hkz.cqqwz.cn

Lua ............ 10
来源：http://tgn.tian-w.cn

Perl ........... 10
来源：http://xdy.nanxinkj.top

Scala .......... 10
来源：http://sbq.gogol.net.cn

------------------------------------
来源：http://pfv.jianghu66.top

合计 ........... 2106 条
来源：http://rvi.iojbl.cn

按章节统计：
来源：http://zxw.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jrm.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hwg.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://adb.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ekw.fengsongda.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wqu.chenlongwang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://olr.jinghuilouyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uac.vqdsnc.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fjf.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cad.shanyushiyangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tzq.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eld.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kyl.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ktx.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jju.nanxinkj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tcc.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iut.aizwys.cn

Q SQL 专题                              90
来源：http://ahf.uphjek.com

R Bash 专题                             80
来源：http://iaz.yvedp.cn

S C / C++ 专题                          60
来源：http://myh.zhongyouzk.top

T 其他语言补充                          60
来源：http://nst.havefunace.top

U 高频实用片段                         120
来源：http://fjq.tanke756.top

------------------------------------
来源：http://wyo.ydzc1.top

合计                                  2106 条
来源：http://owb.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://fso.hammf.cn

使用提醒
来源：http://jvb.havefunace.top

--------------------------------------------------------------------------------
来源：http://fxy.kuanghao11.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://har.hnxiangtu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://crr.cdnleiting.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gsq.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nrn.hammf.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pmb.cashguo.top

—— 文件结束 ——
来源：http://pmp.ydzc1.top

================================================================================
来源：http://wns.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://mxt.jinqigfzy.top

Common Programming Examples Cheat Book
来源：http://kqu.sweek.top

================================================================================
来源：http://gfh.nanxinkj.top

【收录内容】
来源：http://boi.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ywn.jinqigufen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://edk.snrcjt.cn

SQL · Bash · C · C++
来源：http://iqe.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lyw.gogol.net.cn

【使用说明】
来源：http://pvz.yangfankeji.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zcn.dashuyun.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qip.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oat.ehwqpu.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://atd.hongshengwenyu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zya.52xcode.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kks.tanke756.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cwy.daxiang520.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mro.zhijiandao.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zrb.zhixingplan.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tse.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ujg.yonumen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nyx.wangshuangyany.cn

【文件统计】
来源：http://sku.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ubu.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://uvm.cashguo.top

目  录
来源：http://jlk.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://gik.aizwys.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cnu.vqdsnc.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ehz.chenzaomai.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fst.yuanzhike.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cil.epnwcf.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pod.9152youxi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rqp.xuanzx.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qvj.yvedp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xal.jyoumei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vsp.sxryk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://doe.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bsy.aibaodan.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://luk.xziqi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jwg.sweek.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://csx.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wko.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://umv.yj20258888.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bpv.hcnkem.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://riq.jiagoushi.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oul.shuidangran.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fgu.fzhhl.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://byh.jinqigufen.top

================================================================================
来源：http://joa.pycfn.com

A. 基础语法与类型
来源：http://npe.ywan-chungtsiang.top

================================================================================
来源：http://lro.shangyingyoupin.top

[A01] Hello World
来源：http://eus.quarkkingdee.top

Py:   print("Hello, World!")
来源：http://cvp.mhx1999.top

PHP:  echo "Hello, World!";
来源：http://zoo.52xcode.cn

JS:   console.log("Hello, World!");
来源：http://nsz.nanxuanxn.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kub.yangfankeji.com

Java: System.out.println("Hello, World!");
来源：http://hyx.9152youxi.cn

Go:   fmt.Println("Hello, World!")
来源：http://faw.cucudq.cn

Ruby: puts "Hello, World!"
来源：http://snl.pengpengdd.cyou

C#:   Console.WriteLine("Hello, World!");
来源：http://ftx.ehwqpu.com

[A02] 变量声明与赋值
来源：http://xsn.ivvv.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ivr.yj20258.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jnk.ywan-chungtsiang.top

JS:   let name = "Alex"; const age = 20;
来源：http://evt.guowangkeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qty.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://zpm.ivvv.top

Go:   name := "Alex"; age := 20
来源：http://cku.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://bhl.andypj.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://ufs.vehdjk.com

[A03] 常量定义
来源：http://nft.nanxinkj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://akg.ehwqpu.com

PHP:  const PI = 3.14159;
来源：http://qjt.hysaishi.cn


<!-- 参考信息 -->