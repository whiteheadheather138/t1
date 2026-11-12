代发 wailian999

[U25] Py：CSV 按字典读
来源：http://eoy.ehwqpu.com

csv.DictReader(f)
来源：http://cuz.quarkkingdee.top

[U26] Py：并发下载
来源：http://vlh.fengsongda.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lnr.smart0.xyz

[U27] Py：异步 HTTP
来源：http://tdj.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://qej.snrcjt.cn

[U28] Py：类型别名
来源：http://mia.jqgfzy.top

UserId = int
来源：http://yda.shangyingyoupin.top

[U29] Py：属性校验
来源：http://miq.ivvv.top

@property 与 @x.setter 配合
来源：http://gua.tanke756.top

[U30] Py：数据类
来源：http://cdd.sjlbkw.cn

@dataclass(slots=True)
来源：http://mhg.xinyue.icu

[U31] Py：单测
来源：http://kwv.andypj.xyz

python -m pytest -q
来源：http://wwx.xuanzx.com

[U32] Py：代码格式化
来源：http://eyr.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://nvx.guannengcc.top

[U33] Py：打包发布
来源：http://thw.gzhubu.top

python -m build  （依赖 pyproject.toml）
来源：http://nfi.bbcook.cn

[U34] Py：判断编码
来源：http://xlt.ydzc1.top

chardet.detect(raw)
来源：http://wkc.havefunace.top

[U35] Py：发送邮件
来源：http://nig.cheryme.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zwj.tarul.cn

[U36] Py：定时任务
来源：http://txr.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://sfh.nanxinkj.top

[U37] Py：读写 Excel
来源：http://oas.sufxvd.cn

pandas.read_excel / DataFrame.to_excel
来源：http://osu.jinghuilouyu.cn

[U38] Py：获取脚本所在目录
来源：http://wjy.cucudq.cn

Path(__file__).resolve().parent
来源：http://bye.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://xjf.yonumen.top

sys.stdout.isatty()
来源：http://ilt.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://uvq.daria6918.cn

print("err", file=sys.stderr)
来源：http://sma.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://ffo.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://npi.bjfxy.top

[U42] PHP：PSR-4 自动加载
来源：http://itn.hongshengwenyu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mbu.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://ojz.ywan-chungtsiang.top

namespace App\Http;
来源：http://qkn.cheryme.top

[U44] PHP：开启严格类型
来源：http://gqx.pengpengdd.cyou

declare(strict_types=1);
来源：http://byj.yangfankeji.com

[U45] PHP：类型声明与返回类型
来源：http://zri.zhiwuduotai.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jng.yj20258.top

[U46] PHP：可空类型
来源：http://tur.jinqigfzy.top

?string $name = null
来源：http://vsx.zhiwuduotai.top

[U47] PHP：联合类型
来源：http://ddt.svipenyu.cn

int|string $id
来源：http://wzk.fktsv.cn

[U48] PHP：纯枚举
来源：http://dkt.sufxvd.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ola.snrcjt.cn

[U49] PHP：只读属性
来源：http://zwz.ppjwa.cn

public readonly string $name
来源：http://qrb.chenjidiqi.icu

[U50] PHP：构造器属性提升
来源：http://lgb.meibo888.top

public function __construct(private int $id) {}
来源：http://utj.316326.xyz

[U51] PHP：数组解构
来源：http://nmx.snrcjt.cn

[$a, $b] = $arr;
来源：http://ylk.hongshengwenyu.top

[U52] PHP：箭头函数
来源：http://bay.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://dmg.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://ecp.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://bel.dashuyun.cn

[U54] PHP：空安全调用
来源：http://zcq.hcnkem.com

$obj?->method()
来源：http://oqb.iojbl.cn

[U55] PHP：match 表达式
来源：http://jwb.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kyt.tarul.cn

[U56] PHP：命名参数
来源：http://vkk.hywenlv.cn

f(a: 1, b: 2)
来源：http://mrn.sufxvd.cn

[U57] PHP：字符串插值
来源：http://qpd.ppjwa.cn

"值: {$a}"
来源：http://eoi.ppjwa.cn

[U58] PHP：数组三件套
来源：http://vmv.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lis.hesvh.cn

[U59] PHP：自定义排序
来源：http://hml.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ebk.316326.xyz

[U60] PHP：JSON 编解码
来源：http://zbu.shanyushiyangtech.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sdh.yuanzhike.top

[U61] PHP：正则
来源：http://ysl.yj20258888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lnc.redwolf501.top

[U62] PHP：日期对象
来源：http://wfx.chenlongwang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://itz.jiagoushi.top

[U63] PHP：文件读写
来源：http://ily.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ofd.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://wxj.zdqjudy.top

glob("dir/*.php");  scandir("dir");
来源：http://xjj.fzhhl.top

[U65] PHP：会话
来源：http://ulv.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ifd.bjfxy.top

[U66] PHP：设置 Cookie
来源：http://ixh.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hyh.cucudq.cn

[U67] PHP：处理文件上传
来源：http://yyr.yj202588.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lrx.c1oappe.top

[U68] PHP：PDO 连接
来源：http://mtx.chenzaomai.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bir.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://hho.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bce.yanxiufei.cn

[U70] PHP：PDO 事务
来源：http://czy.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://igh.cdnleiting.top

[U71] PHP：抛出异常
来源：http://wzx.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://rnf.yj20258.top

[U72] PHP：写错误日志
来源：http://qnr.sysykeji.top

error_log("失败: " . $e->getMessage());
来源：http://nnv.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://aan.sysykeji.top

parse_ini_file("config.ini", true)
来源：http://joi.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://gsj.sweek.top

getenv("APP_ENV") ?: "production"
来源：http://ecq.yj202588.top

[U75] PHP：依赖注入
来源：http://ocq.chenzaomai.com

composer require psr/container
来源：http://gbz.redwolf501.top

[U76] PHP：简单路由
来源：http://vjj.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tck.yj20258888.top

[U77] PHP：模板渲染
来源：http://zpr.tanke756.top

composer require twig/twig
来源：http://cmj.jqgufenzy.top

[U78] PHP：单元测试
来源：http://vkq.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://fqt.zhixingplan.top

[U79] PHP：静态分析
来源：http://qat.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://wwh.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://yup.tarul.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://roo.birdmap.top

[U81] JS：初始化项目
来源：http://uzr.cucudq.cn

npm init -y;  npm i express
来源：http://xsf.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://vbp.hywenlv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://egs.hnxiangtu.top

[U83] JS：ES Module 导入导出
来源：http://ozp.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ngh.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://zzw.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kac.bjfxy.top

[U85] JS：可选链
来源：http://laj.xingfuxueyuan.xyz

a?.b?.c
来源：http://cll.nwbrower.top

[U86] JS：空值合并
来源：http://qpk.redwolf501.top

a ?? b
来源：http://zzh.hfpthk.cn

[U87] JS：解构默认值
来源：http://gmb.yfazqb.com

const { a = 1, b = 2 } = obj;
来源：http://ojy.cucudq.cn

[U88] JS：对象展开合并
来源：http://jkw.9152youxi.cn

{ ...a, ...b }
来源：http://raw.jqgufenzy.top

[U89] JS：数组去重
来源：http://wmh.hywenlv.cn

[...new Set(arr)]
来源：http://xgv.bjfxy.top

[U90] JS：数字数组排序
来源：http://ohh.hcnkem.com

[...arr].sort((a, b) => a - b)
来源：http://rrh.gaohongyu789.top

[U91] JS：对象键值遍历
来源：http://vtz.tanke756.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hda.hfpthk.cn

[U92] JS：深拷贝
来源：http://pjp.ehwqpu.com

structuredClone(obj)
来源：http://noj.hfpthk.cn

[U93] JS：模板字符串
来源：http://dyc.xuetiantiany.cn

`共 ${n} 条`
来源：http://vod.316326.xyz

[U94] JS：箭头函数
来源：http://wsn.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://vui.ctjpmb.com

[U95] JS：Promise 包装
来源：http://ruq.cheryme.top

new Promise((resolve, reject) => {})
来源：http://iwm.316326.xyz

[U96] JS：async/await 与异常
来源：http://qth.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wil.jinqigfzy.top

[U97] JS：并发请求
来源：http://nvb.fktsv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vrr.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://ukv.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vql.xuanzx.com

[U99] JS：事件监听
来源：http://dlw.meibo888.top

el.addEventListener("click", e => {})
来源：http://ojv.zdqjudy.top

[U100] JS：DOM 查询
来源：http://cqm.xingfuxueyuan.xyz

document.querySelector(".item")
来源：http://nhr.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://lxe.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://fjf.meibo888.top

[U102] JS：本地存储
来源：http://sik.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pol.yvedp.cn

[U103] JS：定时器
来源：http://iln.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ugg.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://upz.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ucd.hysaishi.cn

[U105] JS：节流
来源：http://tnc.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gcs.pycfn.com

[U106] JS：日期格式化
来源：http://bdx.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jom.guannengcc.top

[U107] JS：数字千分位
来源：http://nxd.cucudq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eoe.feifeiyinyue.top

[U108] JS：随机整数
来源：http://dsy.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lco.fengsongda.top

[U109] JS：数组分组
来源：http://bym.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://gkt.c1oappe.top

[U110] JS：数组分块
来源：http://fms.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nkb.aizwys.cn

[U111] JS：对象转 Map
来源：http://spd.vehdjk.com

new Map(Object.entries(obj))
来源：http://rue.ppjwa.cn

[U112] JS：字符串补位
来源：http://cxq.guowangkeji.top

"7".padStart(3, "0")
来源：http://uoj.tianlin.xyz

[U113] JS：正则替换全部
来源：http://tdz.0kj1m.cn

s.replaceAll("a", "b")
来源：http://zcm.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://vfj.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ynu.guannengcc.top

[U115] JS：生成 UUID
来源：http://nrv.tanke756.top

crypto.randomUUID()
来源：http://fzo.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://kit.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://zia.hnqzz.top

[U117] JS：单元测试
来源：http://php.hammf.cn

npm i -D vitest;  npx vitest
来源：http://eel.cheryme.top

[U118] JS：开发服务器
来源：http://ypr.sysykeji.top

npm i -D vite;  npx vite
来源：http://xfv.sxryk.cn

[U119] JS：生产构建
来源：http://pwe.ywan-chungtsiang.top

npx vite build
来源：http://pko.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://qqo.gotoacloud.top

import.meta.env.VITE_API_URL
来源：http://bzt.xylfe.cn

================================================================================
来源：http://efa.yangfankeji.com

统计汇总
来源：http://jmn.fanxiaobao.xyz

================================================================================
来源：http://fci.fanxiaobao.xyz

按语言统计（条）：
来源：http://liv.yangfankeji.com

Python ......... 252
来源：http://gcf.snrcjt.cn

PHP ............ 252
来源：http://fgf.daxiang520.top

JavaScript ..... 252
来源：http://ifo.yongpay.top

TypeScript ..... 212
来源：http://efe.xinyue.icu

Java ........... 212
来源：http://hci.epnwcf.com

Go ............. 212
来源：http://ngu.smart0.xyz

Ruby ........... 212
来源：http://lby.xingfuxueyuan.xyz

C# ............. 212
来源：http://qgb.chenjidiqi.icu

C .............. 30
来源：http://ytp.zdqjudy.top

C++ ............ 30
来源：http://mky.yanxiufei.cn

SQL ............ 90
来源：http://xgx.gzhubu.top

Bash ........... 80
来源：http://prg.hnqzz.top

Kotlin ......... 15
来源：http://uzy.cashguo.top

Swift .......... 15
来源：http://zbp.jlsjyb.cn

Lua ............ 10
来源：http://gfg.ctjpmb.com

Perl ........... 10
来源：http://cwd.jqgufenzy.top

Scala .......... 10
来源：http://zau.sysykeji.top

------------------------------------
来源：http://lyv.jqgufenzy.top

合计 ........... 2106 条
来源：http://ljp.hywenlv.cn

按章节统计：
来源：http://mfm.nanxuanxn.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dyz.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bvl.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yrr.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://njm.shuidangran.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qte.sjlbkw.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rly.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://whz.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pcr.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rsj.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xdn.gotoacloud.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://myd.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cyz.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rhy.yuxming.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sbd.hongshengwenyu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://flv.cheryme.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zta.zhoulong.xyz

Q SQL 专题                              90
来源：http://nyx.yj20258888.top

R Bash 专题                             80
来源：http://kwv.guowangkeji.top

S C / C++ 专题                          60
来源：http://fll.yanxiufei.cn

T 其他语言补充                          60
来源：http://qth.sjlbkw.cn

U 高频实用片段                         120
来源：http://ycb.dianchejie.cn

------------------------------------
来源：http://ksa.ydjk.org.cn

合计                                  2106 条
来源：http://idk.52xcode.cn

--------------------------------------------------------------------------------
来源：http://ahk.feifeiyinyue.top

使用提醒
来源：http://xog.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://ihb.jinyuanbaomall.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vdn.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fqx.fzhhl.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qkq.hnxiangtu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ngo.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ltt.nwbrower.top

—— 文件结束 ——
来源：http://ijf.iojbl.cn

================================================================================
来源：http://mir.gaohongyu789.top

程序语言常见例子速查手册（2024 版）
来源：http://wqq.c1oappe.top

Common Programming Examples Cheat Book
来源：http://ssq.mhx1999.top

================================================================================
来源：http://ked.gotoacloud.top

【收录内容】
来源：http://pfw.jinghuilouyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lis.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ctw.zdqjudy.top

SQL · Bash · C · C++
来源：http://mdv.316326.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nsw.mhx1999.top

【使用说明】
来源：http://gbq.fzhhl.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://env.zhaomingkeji.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kzs.zdbjq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://azr.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://izw.tanke756.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fxl.sysykeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ghm.zhaomingkeji.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kle.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fxe.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rvq.fzhhl.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nsw.fanxiaobao.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hgl.cashguo.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gca.sweek.top

【文件统计】
来源：http://xkq.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://btn.redwolf501.top

--------------------------------------------------------------------------------
来源：http://cek.vqdsnc.cn

目  录
来源：http://mxx.316326.xyz

--------------------------------------------------------------------------------
来源：http://lvm.shanyushiyangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kxq.chenzaomai.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nrx.wangdashe.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://onf.dianchejie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wwf.gotoacloud.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qdy.ydzc1.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nwf.ywan-chungtsiang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mjv.uphjek.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fgr.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uss.gogol.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zse.zhengqikj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://loi.hfpthk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ctl.jqgfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hzg.zhongyouzk.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tyb.daria6918.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ork.hnxiangtu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kkx.mhx1999.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://emq.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://ibj.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tew.c1oappe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tjo.cheryme.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kcb.dashuyun.cn

================================================================================
来源：http://jht.ydjk.org.cn

A. 基础语法与类型
来源：http://smx.jiagoushi.top

================================================================================
来源：http://gmi.xinyue.icu

[A01] Hello World
来源：http://tzy.yongpay.top


<!-- 参考信息 -->