代发 wailian999

[U31] Py：单测
来源：http://rsb.yvedp.cn

python -m pytest -q
来源：http://sqc.hammf.cn

[U32] Py：代码格式化
来源：http://ysj.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://muf.zdqjudy.top

[U33] Py：打包发布
来源：http://zrm.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://fip.ydzc1.top

[U34] Py：判断编码
来源：http://cdy.hfpthk.cn

chardet.detect(raw)
来源：http://hsu.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://lzj.gotoacloud.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qoa.snrcjt.cn

[U36] Py：定时任务
来源：http://qdj.shangyingyoupin.top

schedule.every(10).minutes.do(job)
来源：http://usj.hcnkem.com

[U37] Py：读写 Excel
来源：http://ipv.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://bsn.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://llv.cucudq.cn

Path(__file__).resolve().parent
来源：http://bce.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://nug.ctjpmb.com

sys.stdout.isatty()
来源：http://dky.xuetiantiany.cn

[U40] Py：打印到标准错误
来源：http://xmg.chenzaomai.com

print("err", file=sys.stderr)
来源：http://swf.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://fjm.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vtf.guannengcc.top

[U42] PHP：PSR-4 自动加载
来源：http://tkm.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dsd.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://krp.c1oappe.top

namespace App\Http;
来源：http://kli.jqgufenzy.top

[U44] PHP：开启严格类型
来源：http://vlw.sxryk.cn

declare(strict_types=1);
来源：http://goh.zhixingplan.top

[U45] PHP：类型声明与返回类型
来源：http://jbj.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://dfd.xuanzx.com

[U46] PHP：可空类型
来源：http://vaw.tarul.cn

?string $name = null
来源：http://onk.ywan-chungtsiang.top

[U47] PHP：联合类型
来源：http://rql.gaohongyu789.top

int|string $id
来源：http://mqg.yj202588.top

[U48] PHP：纯枚举
来源：http://ixe.guowangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gba.yanxiufei.cn

[U49] PHP：只读属性
来源：http://vqu.feifeiyinyue.top

public readonly string $name
来源：http://psz.tarul.cn

[U50] PHP：构造器属性提升
来源：http://arr.hysaishi.cn

public function __construct(private int $id) {}
来源：http://enm.fehbvm.com

[U51] PHP：数组解构
来源：http://mfb.sxryk.cn

[$a, $b] = $arr;
来源：http://slw.jyoumei.cn

[U52] PHP：箭头函数
来源：http://our.sweek.top

$double = fn($x) => $x * 2;
来源：http://brc.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://keq.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://qyo.yvedp.cn

[U54] PHP：空安全调用
来源：http://pio.316326.xyz

$obj?->method()
来源：http://pua.jinqigufen.top

[U55] PHP：match 表达式
来源：http://ssk.zhongyouzk.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://slt.birdmap.top

[U56] PHP：命名参数
来源：http://lfs.vqdsnc.cn

f(a: 1, b: 2)
来源：http://mqm.cdnleiting.top

[U57] PHP：字符串插值
来源：http://wyx.xziqi.cn

"值: {$a}"
来源：http://vjs.cucudq.cn

[U58] PHP：数组三件套
来源：http://woh.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fju.pengpengdd.cyou

[U59] PHP：自定义排序
来源：http://jzu.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ppg.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://rbz.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kww.bbcook.cn

[U61] PHP：正则
来源：http://iji.xuanzx.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gdb.cashguo.top

[U62] PHP：日期对象
来源：http://pic.ppjwa.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bza.zhiwuduotai.top

[U63] PHP：文件读写
来源：http://krp.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iyj.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://mcg.cucudq.cn

glob("dir/*.php");  scandir("dir");
来源：http://hvw.mhx1999.top

[U65] PHP：会话
来源：http://uya.zdbjq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gtf.yonumen.top

[U66] PHP：设置 Cookie
来源：http://ejp.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://asn.jianghu66.top

[U67] PHP：处理文件上传
来源：http://lqd.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qed.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://jcd.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://usp.birdmap.top

[U69] PHP：PDO 预处理
来源：http://wfy.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://psa.nanxuanxn.top

[U70] PHP：PDO 事务
来源：http://iom.guowangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://twg.chenjidiqi.icu

[U71] PHP：抛出异常
来源：http://kmg.zycfv.cn

throw new RuntimeException("失败", 500);
来源：http://wre.tarul.cn

[U72] PHP：写错误日志
来源：http://jkk.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://ewf.ehwqpu.com

[U73] PHP：读取 ini 配置
来源：http://jko.tanke756.top

parse_ini_file("config.ini", true)
来源：http://ojn.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://zgg.sweek.top

getenv("APP_ENV") ?: "production"
来源：http://qqs.dianchejie.cn

[U75] PHP：依赖注入
来源：http://hgf.andypj.xyz

composer require psr/container
来源：http://mza.yongpay.top

[U76] PHP：简单路由
来源：http://gjo.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qzl.ybcxt.top

[U77] PHP：模板渲染
来源：http://mpu.hywenlv.cn

composer require twig/twig
来源：http://ede.iojbl.cn

[U78] PHP：单元测试
来源：http://oqv.tanke756.top

composer require --dev phpunit/phpunit
来源：http://ruv.nanxinkj.top

[U79] PHP：静态分析
来源：http://iao.bbcook.cn

composer require --dev phpstan/phpstan
来源：http://ysz.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://yge.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ndk.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://uha.sjlbkw.cn

npm init -y;  npm i express
来源：http://mwj.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://zdv.cheryme.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hol.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://ibj.zhoulong.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://uxb.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://rqh.quarkkingdee.top

module.exports = { a };  const { a } = require("./m");
来源：http://yrw.fehbvm.com

[U85] JS：可选链
来源：http://pnm.zhijiandao.cn

a?.b?.c
来源：http://grc.zhijiandao.cn

[U86] JS：空值合并
来源：http://hji.fengsongda.top

a ?? b
来源：http://avu.wangshuangyany.cn

[U87] JS：解构默认值
来源：http://gjn.gogol.net.cn

const { a = 1, b = 2 } = obj;
来源：http://mbo.yueranfly.top

[U88] JS：对象展开合并
来源：http://bxl.guannengcc.top

{ ...a, ...b }
来源：http://eqb.cheryme.top

[U89] JS：数组去重
来源：http://ebv.ppjwa.cn

[...new Set(arr)]
来源：http://xpn.ydzc1.top

[U90] JS：数字数组排序
来源：http://woc.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://rkn.yueranfly.top

[U91] JS：对象键值遍历
来源：http://lmt.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uwn.hfpthk.cn

[U92] JS：深拷贝
来源：http://nxy.hysaishi.cn

structuredClone(obj)
来源：http://cnw.vehdjk.com

[U93] JS：模板字符串
来源：http://own.ivvv.top

`共 ${n} 条`
来源：http://wpc.ehwqpu.com

[U94] JS：箭头函数
来源：http://ada.gzhubu.top

const double = x => x * 2;
来源：http://wal.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://inl.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://tfm.sysykeji.top

[U96] JS：async/await 与异常
来源：http://tso.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ujv.bjfxy.top

[U97] JS：并发请求
来源：http://cat.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://irb.hnqzz.top

[U98] JS：fetch 带 JSON
来源：http://cqs.yj20258.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ecq.zhijiandao.cn

[U99] JS：事件监听
来源：http://iko.gogol.net.cn

el.addEventListener("click", e => {})
来源：http://lpp.cqqwz.cn

[U100] JS：DOM 查询
来源：http://ofi.wangshuangyany.cn

document.querySelector(".item")
来源：http://jfg.zhoulong.xyz

[U101] JS：classList 操作
来源：http://yuk.wangdashe.top

el.classList.toggle("active")
来源：http://xyx.jinqigfzy.top

[U102] JS：本地存储
来源：http://czx.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ive.gogol.net.cn

[U103] JS：定时器
来源：http://qsi.yueranfly.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uik.fengsongda.top

[U104] JS：防抖
来源：http://lcd.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://map.jlsjyb.cn

[U105] JS：节流
来源：http://cvn.jiagoushi.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://alb.zdqjudy.top

[U106] JS：日期格式化
来源：http://bgl.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ftr.hywenlv.cn

[U107] JS：数字千分位
来源：http://med.xylfe.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zlg.birdmap.top

[U108] JS：随机整数
来源：http://hiu.cashguo.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nfr.cheryme.top

[U109] JS：数组分组
来源：http://jwq.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://plx.xuanzx.com

[U110] JS：数组分块
来源：http://pxg.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rev.smart0.xyz

[U111] JS：对象转 Map
来源：http://rxu.ctjpmb.com

new Map(Object.entries(obj))
来源：http://edh.cheryme.top

[U112] JS：字符串补位
来源：http://qdf.yueranfly.top

"7".padStart(3, "0")
来源：http://rat.snrcjt.cn

[U113] JS：正则替换全部
来源：http://pao.zdqjudy.top

s.replaceAll("a", "b")
来源：http://gnz.hnqzz.top

[U114] JS：JSON 深比较
来源：http://npd.kuanghao11.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ecz.mhx1999.top

[U115] JS：生成 UUID
来源：http://nlh.shanyushiyangtech.top

crypto.randomUUID()
来源：http://qvq.uphjek.com

[U116] JS：类型检查（JSDoc）
来源：http://blg.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://fum.svipenyu.cn

[U117] JS：单元测试
来源：http://yds.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://rmv.fengsongda.top

[U118] JS：开发服务器
来源：http://umv.mhx1999.top

npm i -D vite;  npx vite
来源：http://oqe.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://gfx.chenjidiqi.icu

npx vite build
来源：http://bgh.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://rhk.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://lnx.daxiang520.top

================================================================================
来源：http://lgu.iojbl.cn

统计汇总
来源：http://gii.hnqzz.top

================================================================================
来源：http://faa.c1oappe.top

按语言统计（条）：
来源：http://hoz.hnxiangtu.top

Python ......... 252
来源：http://mel.zhaomingkeji.xyz

PHP ............ 252
来源：http://nvv.andypj.xyz

JavaScript ..... 252
来源：http://kwc.cucudq.cn

TypeScript ..... 212
来源：http://yod.sjlbkw.cn

Java ........... 212
来源：http://vpx.yj20258.top

Go ............. 212
来源：http://mqz.daxiang520.top

Ruby ........... 212
来源：http://hrv.fktsv.cn

C# ............. 212
来源：http://hfy.cqqwz.cn

C .............. 30
来源：http://fff.ydzc1.top

C++ ............ 30
来源：http://xms.jinyuanbaomall.cn

SQL ............ 90
来源：http://ljs.zdqjudy.top

Bash ........... 80
来源：http://zgc.c1oappe.top

Kotlin ......... 15
来源：http://ywo.dashuyun.cn

Swift .......... 15
来源：http://jye.0kj1m.cn

Lua ............ 10
来源：http://uxw.sufxvd.cn

Perl ........... 10
来源：http://wev.fzhhl.top

Scala .......... 10
来源：http://lkc.fanxiaobao.xyz

------------------------------------
来源：http://gkm.yvedp.cn

合计 ........... 2106 条
来源：http://fjo.aizwys.cn

按章节统计：
来源：http://xli.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tbp.yuxming.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ytj.quarkkingdee.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ato.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://szt.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nmr.tanke756.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mlg.ydzc1.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jdy.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tfd.hcnkem.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jou.jinqigfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xvx.chenzaomai.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vki.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://anc.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://faj.9152youxi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://srp.yuxming.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eqk.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rhp.0kj1m.cn

Q SQL 专题                              90
来源：http://zlc.daxiang520.top

R Bash 专题                             80
来源：http://hqq.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://xpc.yonumen.top

T 其他语言补充                          60
来源：http://rhn.shangyingyoupin.top

U 高频实用片段                         120
来源：http://crc.mhx1999.top

------------------------------------
来源：http://nyt.jiagoushi.top

合计                                  2106 条
来源：http://lus.tarul.cn

--------------------------------------------------------------------------------
来源：http://sjg.tarul.cn

使用提醒
来源：http://hng.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://onl.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vhc.aibaodan.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oad.jinqigufen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fev.nanxuanxn.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lbt.yongpay.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ryw.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://woy.andypj.xyz

================================================================================
来源：http://agd.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://jbw.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://isr.gogol.net.cn

================================================================================
来源：http://vsl.ivvv.top

【收录内容】
来源：http://kgl.epnwcf.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://fvu.zhongyouzk.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tmk.nwbrower.top

SQL · Bash · C · C++
来源：http://nwc.kuanghao11.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mrd.yj20258888.top

【使用说明】
来源：http://pyc.cheryme.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nqk.yuxming.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uzc.zhaomingkeji.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mqo.guannengcc.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ayi.ydzc1.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yri.nanxuanxn.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://alx.nanxuanxn.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ocg.iojbl.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cro.gzhubu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aoj.yvedp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kle.jinyuanbaomall.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rqo.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jwo.shangyingyoupin.top

【文件统计】
来源：http://ewc.yuxming.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://abp.c1oappe.top

--------------------------------------------------------------------------------
来源：http://lho.zdbjq.cn

目  录
来源：http://sxu.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://ffl.guannengcc.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ylf.ehwqpu.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eta.ydzc1.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kqe.hcnkem.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wsj.shanyushiyangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qbd.chenjidiqi.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fyx.daria6918.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mei.fanxiaobao.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://czp.yj20258888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zpi.hesvh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bgm.gogol.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uek.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://orb.aizwys.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ayj.zhoulong.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jcb.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pbe.shanyushiyangtech.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ptk.smart0.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zct.kuanghao11.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ree.chenlongwang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mri.zhengqikj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qvz.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ork.ydzc1.top

================================================================================
来源：http://tqx.pycfn.com

A. 基础语法与类型
来源：http://gax.zhiwuduotai.top

================================================================================
来源：http://wuv.hammf.cn

[A01] Hello World
来源：http://dog.gaohongyu789.top

Py:   print("Hello, World!")
来源：http://ali.pengpengdd.cyou

PHP:  echo "Hello, World!";
来源：http://lgo.yj202588.top

JS:   console.log("Hello, World!");
来源：http://fib.hywenlv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://knj.gaohongyu789.top

Java: System.out.println("Hello, World!");
来源：http://vcb.gogol.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://yhs.yvedp.cn

Ruby: puts "Hello, World!"
来源：http://bvc.redwolf501.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bze.xinyue.icu

[A02] 变量声明与赋值
来源：http://ilf.quarkkingdee.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pdm.tanke756.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ubo.daxiang520.top

JS:   let name = "Alex"; const age = 20;
来源：http://oso.jinghuilouyu.cn


<!-- 参考信息 -->