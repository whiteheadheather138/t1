代发 wailian999

[U25] Py：CSV 按字典读
来源：http://nfy.zdbjq.cn

csv.DictReader(f)
来源：http://ezj.xuanzx.com

[U26] Py：并发下载
来源：http://qzm.fzhhl.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pmy.sweek.top

[U27] Py：异步 HTTP
来源：http://uub.yanxiufei.cn

aiohttp.ClientSession() 配合 async with
来源：http://nag.hnqzz.top

[U28] Py：类型别名
来源：http://frh.shzxlz.cn

UserId = int
来源：http://bgo.c1oappe.top

[U29] Py：属性校验
来源：http://jmy.jiagoushi.top

@property 与 @x.setter 配合
来源：http://gid.guannengcc.top

[U30] Py：数据类
来源：http://ysa.fzhhl.top

@dataclass(slots=True)
来源：http://vhy.ehwqpu.com

[U31] Py：单测
来源：http://xou.c1oappe.top

python -m pytest -q
来源：http://axp.havefunace.top

[U32] Py：代码格式化
来源：http://nhw.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://jkr.hesvh.cn

[U33] Py：打包发布
来源：http://zou.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://jqz.shangyingyoupin.top

[U34] Py：判断编码
来源：http://xzt.gaohongyu789.top

chardet.detect(raw)
来源：http://prn.jinqigufen.top

[U35] Py：发送邮件
来源：http://hom.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kme.gzhubu.top

[U36] Py：定时任务
来源：http://wmq.hywenlv.cn

schedule.every(10).minutes.do(job)
来源：http://ugq.hesvh.cn

[U37] Py：读写 Excel
来源：http://zqj.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://qln.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://owo.havefunace.top

Path(__file__).resolve().parent
来源：http://hzc.fktsv.cn

[U39] Py：判断是否在交互环境
来源：http://cku.birdmap.top

sys.stdout.isatty()
来源：http://mon.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://ghs.ctjpmb.com

print("err", file=sys.stderr)
来源：http://dwz.iojbl.cn

[U41] PHP：初始化 Composer 项目
来源：http://egi.guannengcc.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lvm.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://oba.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lmz.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://ztr.kuanghao11.cn

namespace App\Http;
来源：http://yuf.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://fus.guannengcc.top

declare(strict_types=1);
来源：http://mbo.zdqjudy.top

[U45] PHP：类型声明与返回类型
来源：http://rpl.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ujj.tarul.cn

[U46] PHP：可空类型
来源：http://eet.jqgufenzy.top

?string $name = null
来源：http://awz.hcnkem.com

[U47] PHP：联合类型
来源：http://thh.zhijiandao.cn

int|string $id
来源：http://kiz.zhijiandao.cn

[U48] PHP：纯枚举
来源：http://xmp.zhoulong.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qwh.quarkkingdee.top

[U49] PHP：只读属性
来源：http://hqd.zycfv.cn

public readonly string $name
来源：http://bud.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://dwu.gaohongyu789.top

public function __construct(private int $id) {}
来源：http://wei.yj202588.top

[U51] PHP：数组解构
来源：http://tcy.havefunace.top

[$a, $b] = $arr;
来源：http://ymp.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://srq.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://acx.zdbjq.cn

[U53] PHP：空合并运算符
来源：http://hxp.zhixingplan.top

$v = $a ?? $b ?? "default";
来源：http://hxb.zhongyouzk.top

[U54] PHP：空安全调用
来源：http://qwo.gaohongyu789.top

$obj?->method()
来源：http://mzl.xinyue.icu

[U55] PHP：match 表达式
来源：http://ofo.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tvq.nanxuanxn.top

[U56] PHP：命名参数
来源：http://nco.shuidangran.top

f(a: 1, b: 2)
来源：http://hvq.yangfankeji.com

[U57] PHP：字符串插值
来源：http://cfk.havefunace.top

"值: {$a}"
来源：http://ski.jlsjyb.cn

[U58] PHP：数组三件套
来源：http://xgt.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bhw.sysykeji.top

[U59] PHP：自定义排序
来源：http://fvi.hywenlv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kch.yanxiufei.cn

[U60] PHP：JSON 编解码
来源：http://ueh.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kcq.yuanzhike.top

[U61] PHP：正则
来源：http://nqt.zhongyouzk.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xkl.aizwys.cn

[U62] PHP：日期对象
来源：http://uzy.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ffn.zhengqikj.top

[U63] PHP：文件读写
来源：http://zgh.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://byq.zhiwuduotai.top

[U64] PHP：目录遍历
来源：http://uxh.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://rgx.hcnkem.com

[U65] PHP：会话
来源：http://amw.aizwys.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ctq.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://pcq.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vgq.yj20258888.top

[U67] PHP：处理文件上传
来源：http://bpz.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://grv.wangshuangyany.cn

[U68] PHP：PDO 连接
来源：http://xnx.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tmq.fehbvm.com

[U69] PHP：PDO 预处理
来源：http://smj.shzxlz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yjv.c1oappe.top

[U70] PHP：PDO 事务
来源：http://ilk.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ack.xingfuxueyuan.xyz

[U71] PHP：抛出异常
来源：http://rzu.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://lgx.havefunace.top

[U72] PHP：写错误日志
来源：http://zlr.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://qbw.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://vau.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://vem.birdmap.top

[U74] PHP：读取环境变量
来源：http://hfr.316326.xyz

getenv("APP_ENV") ?: "production"
来源：http://auo.vehdjk.com

[U75] PHP：依赖注入
来源：http://yrg.gaohongyu789.top

composer require psr/container
来源：http://uje.cucudq.cn

[U76] PHP：简单路由
来源：http://qdo.svipenyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yyp.haohaochexian.top

[U77] PHP：模板渲染
来源：http://pgk.bjfxy.top

composer require twig/twig
来源：http://wlq.yuanzhike.top

[U78] PHP：单元测试
来源：http://inb.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://yan.xinyue.icu

[U79] PHP：静态分析
来源：http://nvd.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://ogn.52xcode.cn

[U80] PHP：代码规范修复
来源：http://oac.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bge.cucudq.cn

[U81] JS：初始化项目
来源：http://rft.ydzc1.top

npm init -y;  npm i express
来源：http://nbf.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://mxi.gogol.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ypp.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://etr.uphjek.com

export const a = 1;  import { a } from "./m.js";
来源：http://kwh.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://ybf.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://jrp.hongshengwenyu.top

[U85] JS：可选链
来源：http://cab.epnwcf.com

a?.b?.c
来源：http://pok.shuidangran.top

[U86] JS：空值合并
来源：http://cap.fzhhl.top

a ?? b
来源：http://qti.guannengcc.top

[U87] JS：解构默认值
来源：http://krb.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://kpf.yuxming.cn

[U88] JS：对象展开合并
来源：http://luf.tanke756.top

{ ...a, ...b }
来源：http://mjr.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://ziu.meibo888.top

[...new Set(arr)]
来源：http://wha.nwbrower.top

[U90] JS：数字数组排序
来源：http://dti.cucudq.cn

[...arr].sort((a, b) => a - b)
来源：http://bcj.pengpengdd.cyou

[U91] JS：对象键值遍历
来源：http://lqr.zhengqikj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ral.pycfn.com

[U92] JS：深拷贝
来源：http://wnz.dashuyun.cn

structuredClone(obj)
来源：http://crh.yonumen.top

[U93] JS：模板字符串
来源：http://nii.vqdsnc.cn

`共 ${n} 条`
来源：http://ahx.fengsongda.top

[U94] JS：箭头函数
来源：http://svq.aibaodan.cn

const double = x => x * 2;
来源：http://kmx.gotoacloud.top

[U95] JS：Promise 包装
来源：http://ajb.ivvv.top

new Promise((resolve, reject) => {})
来源：http://joi.yongpay.top

[U96] JS：async/await 与异常
来源：http://bby.hammf.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nfd.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://rey.birdmap.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://afv.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://hul.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wud.hesvh.cn

[U99] JS：事件监听
来源：http://gtv.sweek.top

el.addEventListener("click", e => {})
来源：http://htd.cashguo.top

[U100] JS：DOM 查询
来源：http://pbo.sufxvd.cn

document.querySelector(".item")
来源：http://tma.guannengcc.top

[U101] JS：classList 操作
来源：http://csw.fktsv.cn

el.classList.toggle("active")
来源：http://eon.yvedp.cn

[U102] JS：本地存储
来源：http://hwi.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iqi.shuidangran.top

[U103] JS：定时器
来源：http://kxg.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lii.cashguo.top

[U104] JS：防抖
来源：http://rjj.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://khq.jinqigufen.top

[U105] JS：节流
来源：http://hls.yj20258888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://evs.daxiang520.top

[U106] JS：日期格式化
来源：http://ozp.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cbw.jqgfzy.top

[U107] JS：数字千分位
来源：http://otz.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sgb.yonumen.top

[U108] JS：随机整数
来源：http://zpa.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nkq.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://mgf.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://dcg.tian-w.cn

[U110] JS：数组分块
来源：http://nks.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kfs.andypj.xyz

[U111] JS：对象转 Map
来源：http://pyg.dashuyun.cn

new Map(Object.entries(obj))
来源：http://ezy.jinqigfzy.top

[U112] JS：字符串补位
来源：http://awu.daxiang520.top

"7".padStart(3, "0")
来源：http://eea.yj20258888.top

[U113] JS：正则替换全部
来源：http://wku.aizwys.cn

s.replaceAll("a", "b")
来源：http://tfa.yuxming.cn

[U114] JS：JSON 深比较
来源：http://mdr.pengpengdd.cyou

JSON.stringify(a) === JSON.stringify(b)
来源：http://lap.redwolf501.top

[U115] JS：生成 UUID
来源：http://bec.smart0.xyz

crypto.randomUUID()
来源：http://suo.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://xpx.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://wus.xuetiantiany.cn

[U117] JS：单元测试
来源：http://qdu.ivvv.top

npm i -D vitest;  npx vitest
来源：http://ybu.vqdsnc.cn

[U118] JS：开发服务器
来源：http://lvc.hfpthk.cn

npm i -D vite;  npx vite
来源：http://uct.guannengcc.top

[U119] JS：生产构建
来源：http://xyq.jinqigufen.top

npx vite build
来源：http://pci.xingfuxueyuan.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ong.iojbl.cn

import.meta.env.VITE_API_URL
来源：http://cck.haohaochexian.top

================================================================================
来源：http://daa.zhongyouzk.top

统计汇总
来源：http://lww.jqgfzy.top

================================================================================
来源：http://hey.haohaochexian.top

按语言统计（条）：
来源：http://cty.jlsjyb.cn

Python ......... 252
来源：http://ylm.wangshuangyany.cn

PHP ............ 252
来源：http://pjh.birdmap.top

JavaScript ..... 252
来源：http://qct.dashuyun.cn

TypeScript ..... 212
来源：http://ryr.wangdashe.top

Java ........... 212
来源：http://gda.tian-w.cn

Go ............. 212
来源：http://jlx.haohaochexian.top

Ruby ........... 212
来源：http://iyw.ppjwa.cn

C# ............. 212
来源：http://mhi.xylfe.cn

C .............. 30
来源：http://vrw.daxiang520.top

C++ ............ 30
来源：http://oth.shanyushiyangkeji.top

SQL ............ 90
来源：http://qkf.jinghuilouyu.cn

Bash ........... 80
来源：http://ark.bbcook.cn

Kotlin ......... 15
来源：http://qwa.xylfe.cn

Swift .......... 15
来源：http://xks.uphjek.com

Lua ............ 10
来源：http://sie.guowangkeji.top

Perl ........... 10
来源：http://hag.feifeiyinyue.top

Scala .......... 10
来源：http://kqg.yvedp.cn

------------------------------------
来源：http://vgd.yfazqb.com

合计 ........... 2106 条
来源：http://kxw.andypj.xyz

按章节统计：
来源：http://vjc.jqgufenzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fno.fanxiaobao.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qay.chenlongwang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ekl.jiagoushi.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qet.sxryk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lyq.tanke756.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wfo.yuxming.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zqv.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cnp.pycfn.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pdf.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cfj.zdbjq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jfl.birdmap.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://atl.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bff.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xtg.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jxa.jqgufenzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://efn.c1oappe.top

Q SQL 专题                              90
来源：http://emx.hywenlv.cn

R Bash 专题                             80
来源：http://cdr.zdbjq.cn

S C / C++ 专题                          60
来源：http://npc.dashuyun.cn

T 其他语言补充                          60
来源：http://onu.tianlin.xyz

U 高频实用片段                         120
来源：http://yok.c1oappe.top

------------------------------------
来源：http://cop.jianghu66.top

合计                                  2106 条
来源：http://hua.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://nnm.gogol.net.cn

使用提醒
来源：http://plv.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://ciu.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dmx.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yod.yuxming.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xuz.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://uzy.gotoacloud.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yqr.jqgufenzy.top

—— 文件结束 ——
来源：http://ump.tianlin.xyz

================================================================================
来源：http://ido.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://lso.shuidangran.top

Common Programming Examples Cheat Book
来源：http://wic.chenlongwang.top

================================================================================
来源：http://jya.yj202588.top

【收录内容】
来源：http://hui.shanyushiyangtech.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yaz.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vub.redwolf501.top

SQL · Bash · C · C++
来源：http://efb.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eom.shuidangran.top

【使用说明】
来源：http://tgo.meibo888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vwh.jinghuilouyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wub.jqgfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fdp.fzhhl.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://igj.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://yet.shanyushiyangkeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zky.guannengcc.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ylq.xziqi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pvv.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gqi.zhengqikj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://itc.cdnleiting.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hsq.jinghuilouyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://his.iojbl.cn

【文件统计】
来源：http://akx.aizwys.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jdb.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://stb.snrcjt.cn

目  录
来源：http://qgp.hcnkem.com

--------------------------------------------------------------------------------
来源：http://chz.smart0.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xoi.cheryme.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ohk.sysykeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jbu.kuanghao11.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dhq.jinqigufen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://efg.tianlin.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rki.feifeiyinyue.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wgp.xylfe.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wkh.havefunace.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aqd.gaohongyu789.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://owr.mhx1999.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iiv.xziqi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fdd.gaohongyu789.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xpj.shanyushiyangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://inl.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tpr.ivvv.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xvx.nwbrower.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dka.sweek.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nzm.yvedp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lro.guannengcc.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aru.ydjk.org.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wkk.xuetiantiany.cn

================================================================================
来源：http://ctu.316326.xyz

A. 基础语法与类型
来源：http://uii.jqgufenzy.top

================================================================================
来源：http://kuh.jinyuanbaomall.cn

[A01] Hello World
来源：http://txy.yj202588.top


<!-- 参考信息 -->