代发 wailian999

[U35] Py：发送邮件
来源：http://sfi.fengsongda.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hzw.c1oappe.top

[U36] Py：定时任务
来源：http://uuq.pengpengdd.cyou

schedule.every(10).minutes.do(job)
来源：http://rrg.fehbvm.com

[U37] Py：读写 Excel
来源：http://har.yueranfly.top

pandas.read_excel / DataFrame.to_excel
来源：http://kyk.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://anz.zhiwuduotai.top

Path(__file__).resolve().parent
来源：http://dlh.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://smf.shzxlz.cn

sys.stdout.isatty()
来源：http://dmc.gzhubu.top

[U40] Py：打印到标准错误
来源：http://lek.nanxinkj.top

print("err", file=sys.stderr)
来源：http://qcy.yanxiufei.cn

[U41] PHP：初始化 Composer 项目
来源：http://kar.nanxinkj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mjx.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://dwi.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cke.xinyue.icu

[U43] PHP：声明命名空间
来源：http://rdm.fzhhl.top

namespace App\Http;
来源：http://mxm.316326.xyz

[U44] PHP：开启严格类型
来源：http://gqg.andypj.xyz

declare(strict_types=1);
来源：http://kix.cqqwz.cn

[U45] PHP：类型声明与返回类型
来源：http://gyy.xuetiantiany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dot.yueranfly.top

[U46] PHP：可空类型
来源：http://mqi.xziqi.cn

?string $name = null
来源：http://rdo.jinqigufen.top

[U47] PHP：联合类型
来源：http://efi.pengpengdd.cyou

int|string $id
来源：http://fus.jqgfzy.top

[U48] PHP：纯枚举
来源：http://tls.jinghuilouyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hrv.hammf.cn

[U49] PHP：只读属性
来源：http://wiu.yj20258888.top

public readonly string $name
来源：http://pvn.ctjpmb.com

[U50] PHP：构造器属性提升
来源：http://ikn.aizwys.cn

public function __construct(private int $id) {}
来源：http://ash.gzhubu.top

[U51] PHP：数组解构
来源：http://ade.52xcode.cn

[$a, $b] = $arr;
来源：http://aqr.bbcook.cn

[U52] PHP：箭头函数
来源：http://kjt.hongshengwenyu.top

$double = fn($x) => $x * 2;
来源：http://fcv.ehwqpu.com

[U53] PHP：空合并运算符
来源：http://fwl.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://ohx.tarul.cn

[U54] PHP：空安全调用
来源：http://hjh.yfazqb.com

$obj?->method()
来源：http://lwm.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://jxc.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zew.yvedp.cn

[U56] PHP：命名参数
来源：http://mml.xziqi.cn

f(a: 1, b: 2)
来源：http://rpt.jiagoushi.top

[U57] PHP：字符串插值
来源：http://kfk.jqgufenzy.top

"值: {$a}"
来源：http://rpb.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://dcm.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fxo.zhengqikj.top

[U59] PHP：自定义排序
来源：http://oxt.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kyg.havefunace.top

[U60] PHP：JSON 编解码
来源：http://hxx.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://quy.shzxlz.cn

[U61] PHP：正则
来源：http://bkv.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xdj.zhengqikj.top

[U62] PHP：日期对象
来源：http://dns.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://spi.jiagoushi.top

[U63] PHP：文件读写
来源：http://uxq.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qbr.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://vnq.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://oop.ctjpmb.com

[U65] PHP：会话
来源：http://wci.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://rqz.meibo888.top

[U66] PHP：设置 Cookie
来源：http://kgz.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lsc.zhiwuduotai.top

[U67] PHP：处理文件上传
来源：http://vrr.xziqi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zrk.zdqjudy.top

[U68] PHP：PDO 连接
来源：http://jdl.daria6918.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ezd.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://ijm.gotoacloud.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bsa.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://txs.yanxiufei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kmd.gzhubu.top

[U71] PHP：抛出异常
来源：http://dnl.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://iov.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://icg.birdmap.top

error_log("失败: " . $e->getMessage());
来源：http://dpa.sjlbkw.cn

[U73] PHP：读取 ini 配置
来源：http://yxe.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://ush.smart0.xyz

[U74] PHP：读取环境变量
来源：http://egv.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://mft.yuanzhike.top

[U75] PHP：依赖注入
来源：http://kjl.shanyushiyangtech.top

composer require psr/container
来源：http://fkr.chenzaomai.com

[U76] PHP：简单路由
来源：http://eid.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ulh.bjfxy.top

[U77] PHP：模板渲染
来源：http://nqz.redwolf501.top

composer require twig/twig
来源：http://bnu.gzhubu.top

[U78] PHP：单元测试
来源：http://ueo.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://qag.yangfankeji.com

[U79] PHP：静态分析
来源：http://jqc.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://nzd.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://jzd.aizwys.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ivr.shuidangran.top

[U81] JS：初始化项目
来源：http://ejs.dashuyun.cn

npm init -y;  npm i express
来源：http://mae.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://jty.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vsu.gaohongyu789.top

[U83] JS：ES Module 导入导出
来源：http://dhw.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://asa.cqqwz.cn

[U84] JS：CommonJS 写法
来源：http://blr.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wle.jlsjyb.cn

[U85] JS：可选链
来源：http://wkn.guannengcc.top

a?.b?.c
来源：http://cnv.jqgfzy.top

[U86] JS：空值合并
来源：http://pei.vehdjk.com

a ?? b
来源：http://wxd.tianlin.xyz

[U87] JS：解构默认值
来源：http://jlq.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://vuc.zhoulong.xyz

[U88] JS：对象展开合并
来源：http://emx.chenjidiqi.icu

{ ...a, ...b }
来源：http://oxn.nanxuanxn.top

[U89] JS：数组去重
来源：http://tcq.uphjek.com

[...new Set(arr)]
来源：http://unx.ivvv.top

[U90] JS：数字数组排序
来源：http://pmn.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://bwo.jlsjyb.cn

[U91] JS：对象键值遍历
来源：http://yxf.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://czo.tianlin.xyz

[U92] JS：深拷贝
来源：http://uyq.zhiwuduotai.top

structuredClone(obj)
来源：http://beo.tanke756.top

[U93] JS：模板字符串
来源：http://etk.kuanghao11.cn

`共 ${n} 条`
来源：http://wrx.zdqjudy.top

[U94] JS：箭头函数
来源：http://vrx.hammf.cn

const double = x => x * 2;
来源：http://amq.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://mkk.zdqjudy.top

new Promise((resolve, reject) => {})
来源：http://jxa.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://wjp.jinyuanbaomall.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rmf.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://hbp.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ida.gzhubu.top

[U98] JS：fetch 带 JSON
来源：http://uyv.andypj.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gxz.hysaishi.cn

[U99] JS：事件监听
来源：http://hnf.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://ewd.smart0.xyz

[U100] JS：DOM 查询
来源：http://yhx.shanyushiyangtech.top

document.querySelector(".item")
来源：http://esi.hnxiangtu.top

[U101] JS：classList 操作
来源：http://hdm.havefunace.top

el.classList.toggle("active")
来源：http://jxa.vqdsnc.cn

[U102] JS：本地存储
来源：http://uyj.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ujp.fktsv.cn

[U103] JS：定时器
来源：http://vnz.hnqzz.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wdx.cashguo.top

[U104] JS：防抖
来源：http://axj.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ycy.yueranfly.top

[U105] JS：节流
来源：http://dca.bbcook.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oup.daria6918.cn

[U106] JS：日期格式化
来源：http://awq.xingfuxueyuan.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://std.9152youxi.cn

[U107] JS：数字千分位
来源：http://jrj.hywenlv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pfq.xziqi.cn

[U108] JS：随机整数
来源：http://fnj.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hvf.sufxvd.cn

[U109] JS：数组分组
来源：http://orl.cashguo.top

Object.groupBy(arr, x => x.type)
来源：http://vwl.iojbl.cn

[U110] JS：数组分块
来源：http://gxp.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wnz.ppjwa.cn

[U111] JS：对象转 Map
来源：http://pzt.chenlongwang.top

new Map(Object.entries(obj))
来源：http://sis.jinghuilouyu.cn

[U112] JS：字符串补位
来源：http://rcz.shuidangran.top

"7".padStart(3, "0")
来源：http://poa.smart0.xyz

[U113] JS：正则替换全部
来源：http://qum.guowangkeji.top

s.replaceAll("a", "b")
来源：http://urv.hongshengwenyu.top

[U114] JS：JSON 深比较
来源：http://wzw.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ikn.gzhubu.top

[U115] JS：生成 UUID
来源：http://est.fengsongda.top

crypto.randomUUID()
来源：http://jvp.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://qpo.zhoulong.xyz

/** @param {string} name */ function f(name) {}
来源：http://vdy.zhongyouzk.top

[U117] JS：单元测试
来源：http://ylf.bjfxy.top

npm i -D vitest;  npx vitest
来源：http://lpb.daria6918.cn

[U118] JS：开发服务器
来源：http://iai.jqgfzy.top

npm i -D vite;  npx vite
来源：http://cfx.iojbl.cn

[U119] JS：生产构建
来源：http://dlf.fktsv.cn

npx vite build
来源：http://vbu.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://fat.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://hou.wangshuangyany.cn

================================================================================
来源：http://qen.guowangkeji.top

统计汇总
来源：http://wbz.xinyue.icu

================================================================================
来源：http://evy.jiagoushi.top

按语言统计（条）：
来源：http://bsa.ctjpmb.com

Python ......... 252
来源：http://wwk.hcnkem.com

PHP ............ 252
来源：http://gfx.ivvv.top

JavaScript ..... 252
来源：http://wug.zdbjq.cn

TypeScript ..... 212
来源：http://ito.mhx1999.top

Java ........... 212
来源：http://jym.yanxiufei.cn

Go ............. 212
来源：http://hss.fzhhl.top

Ruby ........... 212
来源：http://ddk.chenjidiqi.icu

C# ............. 212
来源：http://lvg.daxiang520.top

C .............. 30
来源：http://zgl.zhaomingkeji.xyz

C++ ............ 30
来源：http://xuk.gogol.net.cn

SQL ............ 90
来源：http://axk.zycfv.cn

Bash ........... 80
来源：http://ual.fehbvm.com

Kotlin ......... 15
来源：http://eet.cashguo.top

Swift .......... 15
来源：http://law.vehdjk.com

Lua ............ 10
来源：http://rxd.cheryme.top

Perl ........... 10
来源：http://gsw.hywenlv.cn

Scala .......... 10
来源：http://qxd.zhixingplan.top

------------------------------------
来源：http://ika.smart0.xyz

合计 ........... 2106 条
来源：http://oln.cheryme.top

按章节统计：
来源：http://nmr.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://otl.ybcxt.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://byn.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ins.fengsongda.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nxh.yueranfly.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://spd.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rjx.hammf.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qtk.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lyo.316326.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nit.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nrp.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mll.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kcx.wangdashe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qdg.daria6918.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://peo.meibo888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ykq.sxryk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wed.uphjek.com

Q SQL 专题                              90
来源：http://pui.tianlin.xyz

R Bash 专题                             80
来源：http://spi.xuetiantiany.cn

S C / C++ 专题                          60
来源：http://dny.xingfuxueyuan.xyz

T 其他语言补充                          60
来源：http://gid.chenjidiqi.icu

U 高频实用片段                         120
来源：http://vhx.havefunace.top

------------------------------------
来源：http://nys.ydzc1.top

合计                                  2106 条
来源：http://iok.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://fbv.zhijiandao.cn

使用提醒
来源：http://xks.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://tjh.guowangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ext.jyoumei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dnb.jinqigfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jmo.chenzaomai.com

在旧版本上使用前请先确认语法支持情况。
来源：http://geb.pycfn.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://irg.tian-w.cn

—— 文件结束 ——
来源：http://lkk.guowangkeji.top

================================================================================
来源：http://ywx.dianchejie.cn

程序语言常见例子速查手册（2024 版）
来源：http://xsz.tanke756.top

Common Programming Examples Cheat Book
来源：http://ttm.gogol.net.cn

================================================================================
来源：http://vqx.guannengcc.top

【收录内容】
来源：http://jdr.yvedp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ssc.jinqigfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fkn.haohaochexian.top

SQL · Bash · C · C++
来源：http://lju.sxryk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hfv.svipenyu.cn

【使用说明】
来源：http://uhk.yueranfly.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kwx.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ult.yj20258888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tro.aizwys.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://syv.yuanzhike.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qqh.shangyingyoupin.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rwl.jianghu66.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zbv.jinghuilouyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cpa.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yeu.ppjwa.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ubj.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jyc.shangyingyoupin.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dst.hywenlv.cn

【文件统计】
来源：http://ztq.daxiang520.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nyb.daria6918.cn

--------------------------------------------------------------------------------
来源：http://gxq.cheryme.top

目  录
来源：http://ebx.yj20258.top

--------------------------------------------------------------------------------
来源：http://fut.chenjidiqi.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xbl.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iza.9152youxi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cea.gotoacloud.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qjx.9152youxi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ike.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oif.hywenlv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uix.zhongyouzk.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wjq.shuidangran.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://egg.nwbrower.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://efg.xylfe.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vwm.gogol.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rxw.yvedp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fcy.hammf.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cdz.andypj.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zwu.sxryk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uwp.ctjpmb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mcf.52xcode.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cam.bbcook.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kcf.shuidangran.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://adl.feifeiyinyue.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://trs.wangshuangyany.cn

================================================================================
来源：http://awi.chenjidiqi.icu

A. 基础语法与类型
来源：http://kij.zhixingplan.top

================================================================================
来源：http://jhj.fzhhl.top

[A01] Hello World
来源：http://wps.aibaodan.cn

Py:   print("Hello, World!")
来源：http://phj.zhoulong.xyz

PHP:  echo "Hello, World!";
来源：http://jbj.kuanghao11.cn

JS:   console.log("Hello, World!");
来源：http://qgi.yanxiufei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mko.meibo888.top

Java: System.out.println("Hello, World!");
来源：http://teh.zhongyouzk.top

Go:   fmt.Println("Hello, World!")
来源：http://wou.ydjk.org.cn

Ruby: puts "Hello, World!"
来源：http://ija.zdbjq.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cxf.nanxinkj.top

[A02] 变量声明与赋值
来源：http://oll.fzhhl.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nrj.nwbrower.top

PHP:  $name = "Alex"; $age = 20;
来源：http://srr.fzhhl.top

JS:   let name = "Alex"; const age = 20;
来源：http://nih.yueranfly.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://snm.daria6918.cn

Java: String name = "Alex"; int age = 20;
来源：http://ano.pengpengdd.cyou

Go:   name := "Alex"; age := 20
来源：http://fhu.gogol.net.cn

Ruby: name = "Alex"; age = 20
来源：http://bvq.cashguo.top

C#:   string name = "Alex"; int age = 20;
来源：http://iku.nwbrower.top

[A03] 常量定义
来源：http://osj.gaohongyu789.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tyc.cqqwz.cn

PHP:  const PI = 3.14159;
来源：http://lok.jlsjyb.cn


<!-- 参考信息 -->