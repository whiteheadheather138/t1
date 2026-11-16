代发 wailian999

[U25] Py：CSV 按字典读
来源：http://bqs.daxiang520.top

csv.DictReader(f)
来源：http://fsb.quarkkingdee.top

[U26] Py：并发下载
来源：http://chg.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fbk.chenzaomai.com

[U27] Py：异步 HTTP
来源：http://hhp.316326.xyz

aiohttp.ClientSession() 配合 async with
来源：http://bjo.9152youxi.cn

[U28] Py：类型别名
来源：http://fgx.guowangkeji.top

UserId = int
来源：http://uob.52xcode.cn

[U29] Py：属性校验
来源：http://tlo.snrcjt.cn

@property 与 @x.setter 配合
来源：http://uew.pengpengdd.cyou

[U30] Py：数据类
来源：http://ujn.yueranfly.top

@dataclass(slots=True)
来源：http://ukq.epnwcf.com

[U31] Py：单测
来源：http://dqg.jinqigufen.top

python -m pytest -q
来源：http://qur.ppjwa.cn

[U32] Py：代码格式化
来源：http://pqp.tarul.cn

ruff format . && ruff check --fix .
来源：http://csw.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://wtl.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://qpy.snrcjt.cn

[U34] Py：判断编码
来源：http://qvx.316326.xyz

chardet.detect(raw)
来源：http://ifj.gzhubu.top

[U35] Py：发送邮件
来源：http://wnx.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://anw.jqgufenzy.top

[U36] Py：定时任务
来源：http://ibq.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://ipg.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://xiu.xuetiantiany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wgg.fanxiaobao.xyz

[U38] Py：获取脚本所在目录
来源：http://lcc.zhongyouzk.top

Path(__file__).resolve().parent
来源：http://lro.yj202588.top

[U39] Py：判断是否在交互环境
来源：http://ojo.shuidangran.top

sys.stdout.isatty()
来源：http://dgq.redwolf501.top

[U40] Py：打印到标准错误
来源：http://gjr.meibo888.top

print("err", file=sys.stderr)
来源：http://yqn.ppjwa.cn

[U41] PHP：初始化 Composer 项目
来源：http://crv.shangyingyoupin.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mbt.yanxiufei.cn

[U42] PHP：PSR-4 自动加载
来源：http://xwf.fehbvm.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dfh.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://zmx.cashguo.top

namespace App\Http;
来源：http://awc.xinyue.icu

[U44] PHP：开启严格类型
来源：http://kli.gaohongyu789.top

declare(strict_types=1);
来源：http://ycr.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://raw.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fuw.fktsv.cn

[U46] PHP：可空类型
来源：http://jqr.kuanghao11.cn

?string $name = null
来源：http://agt.yanxiufei.cn

[U47] PHP：联合类型
来源：http://kqb.ydjk.org.cn

int|string $id
来源：http://mxj.tianlin.xyz

[U48] PHP：纯枚举
来源：http://asi.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vdf.316326.xyz

[U49] PHP：只读属性
来源：http://joi.xingfuxueyuan.xyz

public readonly string $name
来源：http://uau.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://lrd.yuxming.cn

public function __construct(private int $id) {}
来源：http://qqe.aibaodan.cn

[U51] PHP：数组解构
来源：http://iyg.aibaodan.cn

[$a, $b] = $arr;
来源：http://gry.fengsongda.top

[U52] PHP：箭头函数
来源：http://saa.ivvv.top

$double = fn($x) => $x * 2;
来源：http://hkt.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://arf.zycfv.cn

$v = $a ?? $b ?? "default";
来源：http://qtf.jinyuanbaomall.cn

[U54] PHP：空安全调用
来源：http://muq.xylfe.cn

$obj?->method()
来源：http://utc.shanyushiyangkeji.top

[U55] PHP：match 表达式
来源：http://qqx.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wug.havefunace.top

[U56] PHP：命名参数
来源：http://fad.tianlin.xyz

f(a: 1, b: 2)
来源：http://mfd.ydjk.org.cn

[U57] PHP：字符串插值
来源：http://wgz.chenlongwang.top

"值: {$a}"
来源：http://nnb.cqqwz.cn

[U58] PHP：数组三件套
来源：http://krq.vehdjk.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ged.nwbrower.top

[U59] PHP：自定义排序
来源：http://hqp.jinghuilouyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oop.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://fha.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://idl.yj202588.top

[U61] PHP：正则
来源：http://aqj.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://opi.xinyue.icu

[U62] PHP：日期对象
来源：http://vhh.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ple.redwolf501.top

[U63] PHP：文件读写
来源：http://dii.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xia.vehdjk.com

[U64] PHP：目录遍历
来源：http://wyr.gaohongyu789.top

glob("dir/*.php");  scandir("dir");
来源：http://cwz.sufxvd.cn

[U65] PHP：会话
来源：http://nek.yfazqb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://oxg.tarul.cn

[U66] PHP：设置 Cookie
来源：http://jub.ehwqpu.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ten.jinqigfzy.top

[U67] PHP：处理文件上传
来源：http://uqv.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yqz.xuetiantiany.cn

[U68] PHP：PDO 连接
来源：http://aei.tarul.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ijo.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://jel.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://olg.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://xks.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pkd.haohaochexian.top

[U71] PHP：抛出异常
来源：http://wab.hnxiangtu.top

throw new RuntimeException("失败", 500);
来源：http://gpr.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://fyk.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://jng.pengpengdd.cyou

[U73] PHP：读取 ini 配置
来源：http://atz.sweek.top

parse_ini_file("config.ini", true)
来源：http://bwq.xuanzx.com

[U74] PHP：读取环境变量
来源：http://mbh.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://xmq.hnxiangtu.top

[U75] PHP：依赖注入
来源：http://ngp.birdmap.top

composer require psr/container
来源：http://bjj.hcnkem.com

[U76] PHP：简单路由
来源：http://cvm.ywan-chungtsiang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jdd.shuidangran.top

[U77] PHP：模板渲染
来源：http://beo.yvedp.cn

composer require twig/twig
来源：http://vwq.vqdsnc.cn

[U78] PHP：单元测试
来源：http://uvt.jqgufenzy.top

composer require --dev phpunit/phpunit
来源：http://cpp.bbcook.cn

[U79] PHP：静态分析
来源：http://vut.sxryk.cn

composer require --dev phpstan/phpstan
来源：http://ncg.pengpengdd.cyou

[U80] PHP：代码规范修复
来源：http://vys.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://gyp.guowangkeji.top

[U81] JS：初始化项目
来源：http://nsi.fzhhl.top

npm init -y;  npm i express
来源：http://vji.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://sii.redwolf501.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://min.hfpthk.cn

[U83] JS：ES Module 导入导出
来源：http://arp.9152youxi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gnx.fengsongda.top

[U84] JS：CommonJS 写法
来源：http://uoi.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://hvy.jinqigufen.top

[U85] JS：可选链
来源：http://sox.ivvv.top

a?.b?.c
来源：http://ohv.jqgufenzy.top

[U86] JS：空值合并
来源：http://ven.jqgufenzy.top

a ?? b
来源：http://loy.redwolf501.top

[U87] JS：解构默认值
来源：http://gbu.xylfe.cn

const { a = 1, b = 2 } = obj;
来源：http://nxy.dianchejie.cn

[U88] JS：对象展开合并
来源：http://pbg.nanxuanxn.top

{ ...a, ...b }
来源：http://uxj.jinqigufen.top

[U89] JS：数组去重
来源：http://tyl.daxiang520.top

[...new Set(arr)]
来源：http://vfy.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://vav.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://vdg.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://mdx.smart0.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fbf.gzhubu.top

[U92] JS：深拷贝
来源：http://lqc.jinyuanbaomall.cn

structuredClone(obj)
来源：http://gdx.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://fqg.zhijiandao.cn

`共 ${n} 条`
来源：http://ask.chenlongwang.top

[U94] JS：箭头函数
来源：http://ecp.hnxiangtu.top

const double = x => x * 2;
来源：http://fcy.cqqwz.cn

[U95] JS：Promise 包装
来源：http://nsn.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://jxh.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://crv.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qac.pengpengdd.cyou

[U97] JS：并发请求
来源：http://ujk.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sef.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://rvt.yvedp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mci.meibo888.top

[U99] JS：事件监听
来源：http://oax.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://lgf.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://uds.vqdsnc.cn

document.querySelector(".item")
来源：http://tpz.ehwqpu.com

[U101] JS：classList 操作
来源：http://svc.dashuyun.cn

el.classList.toggle("active")
来源：http://ywe.zycfv.cn

[U102] JS：本地存储
来源：http://hoa.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://edc.zdqjudy.top

[U103] JS：定时器
来源：http://phl.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cze.shzxlz.cn

[U104] JS：防抖
来源：http://hev.yonumen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eqe.kuanghao11.cn

[U105] JS：节流
来源：http://rnk.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hqp.52xcode.cn

[U106] JS：日期格式化
来源：http://wwp.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://isz.haohaochexian.top

[U107] JS：数字千分位
来源：http://rgc.dianchejie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://smh.hongshengwenyu.top

[U108] JS：随机整数
来源：http://obb.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rwk.quarkkingdee.top

[U109] JS：数组分组
来源：http://syp.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://ept.dianchejie.cn

[U110] JS：数组分块
来源：http://pff.aibaodan.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ixr.shuidangran.top

[U111] JS：对象转 Map
来源：http://ohv.ppjwa.cn

new Map(Object.entries(obj))
来源：http://tcp.jqgfzy.top

[U112] JS：字符串补位
来源：http://myw.yfazqb.com

"7".padStart(3, "0")
来源：http://wrq.yangfankeji.com

[U113] JS：正则替换全部
来源：http://qjd.ivvv.top

s.replaceAll("a", "b")
来源：http://hrg.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://azg.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ubt.tarul.cn

[U115] JS：生成 UUID
来源：http://uyw.zhengqikj.top

crypto.randomUUID()
来源：http://ncu.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://qsz.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://suh.ivvv.top

[U117] JS：单元测试
来源：http://qgz.hnqzz.top

npm i -D vitest;  npx vitest
来源：http://mln.bbcook.cn

[U118] JS：开发服务器
来源：http://xcl.nanxuanxn.top

npm i -D vite;  npx vite
来源：http://tqs.vqdsnc.cn

[U119] JS：生产构建
来源：http://nij.pycfn.com

npx vite build
来源：http://sqf.zhiwuduotai.top

[U120] JS：读取环境变量（Vite）
来源：http://vel.yj20258888.top

import.meta.env.VITE_API_URL
来源：http://fhv.0kj1m.cn

================================================================================
来源：http://ipn.jqgfzy.top

统计汇总
来源：http://ihk.hnqzz.top

================================================================================
来源：http://lpw.hysaishi.cn

按语言统计（条）：
来源：http://vep.zhiwuduotai.top

Python ......... 252
来源：http://zrk.hammf.cn

PHP ............ 252
来源：http://boq.havefunace.top

JavaScript ..... 252
来源：http://nfs.redwolf501.top

TypeScript ..... 212
来源：http://xxf.cdnleiting.top

Java ........... 212
来源：http://nsz.jqgfzy.top

Go ............. 212
来源：http://bpn.ctjpmb.com

Ruby ........... 212
来源：http://vdo.hfpthk.cn

C# ............. 212
来源：http://muw.yanxiufei.cn

C .............. 30
来源：http://fur.ctjpmb.com

C++ ............ 30
来源：http://xck.xziqi.cn

SQL ............ 90
来源：http://kdw.yuxming.cn

Bash ........... 80
来源：http://shw.nwbrower.top

Kotlin ......... 15
来源：http://ikv.hammf.cn

Swift .......... 15
来源：http://byv.wangdashe.top

Lua ............ 10
来源：http://ize.hnxiangtu.top

Perl ........... 10
来源：http://vmj.jianghu66.top

Scala .......... 10
来源：http://rsg.ppjwa.cn

------------------------------------
来源：http://pjk.uphjek.com

合计 ........... 2106 条
来源：http://pjr.snrcjt.cn

按章节统计：
来源：http://yjf.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://djw.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mlw.wangshuangyany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pxf.gaohongyu789.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ehi.kuanghao11.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oxj.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hda.cucudq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://acx.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://soq.sweek.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hcm.vqdsnc.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tzb.yanxiufei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wkl.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zjn.jinyuanbaomall.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ove.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jcn.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dah.andypj.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jqu.hongshengwenyu.top

Q SQL 专题                              90
来源：http://kkp.xingfuxueyuan.xyz

R Bash 专题                             80
来源：http://sia.cdnleiting.top

S C / C++ 专题                          60
来源：http://crv.dianchejie.cn

T 其他语言补充                          60
来源：http://roo.gaohongyu789.top

U 高频实用片段                         120
来源：http://bvx.zhixingplan.top

------------------------------------
来源：http://krw.yfazqb.com

合计                                  2106 条
来源：http://zim.fktsv.cn

--------------------------------------------------------------------------------
来源：http://jef.yj202588.top

使用提醒
来源：http://lre.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://wzf.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tgf.ehwqpu.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yju.xuanzx.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qef.cucudq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tcd.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bwp.cqqwz.cn

—— 文件结束 ——
来源：http://tys.guowangkeji.top

================================================================================
来源：http://qmn.cashguo.top

程序语言常见例子速查手册（2024 版）
来源：http://tmh.kuanghao11.cn

Common Programming Examples Cheat Book
来源：http://aoq.shangyingyoupin.top

================================================================================
来源：http://jbc.xziqi.cn

【收录内容】
来源：http://wbg.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://tof.feifeiyinyue.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xsh.redwolf501.top

SQL · Bash · C · C++
来源：http://aze.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hsj.hcnkem.com

【使用说明】
来源：http://opo.smart0.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://txx.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bos.cheryme.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rnl.tarul.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kko.hammf.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xgx.316326.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zyh.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mwd.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://der.daxiang520.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eeg.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://udi.hongshengwenyu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wuq.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wyt.jinghuilouyu.cn

【文件统计】
来源：http://wtw.gzhubu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://czk.fzhhl.top

--------------------------------------------------------------------------------
来源：http://kjl.zdbjq.cn

目  录
来源：http://hbn.mhx1999.top

--------------------------------------------------------------------------------
来源：http://mbe.iojbl.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mso.hnxiangtu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rme.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mgu.gaohongyu789.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jra.dianchejie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vhj.jinqigufen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jqt.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ndd.316326.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fqf.cashguo.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://asd.jianghu66.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hly.jinqigfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qnt.smart0.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xxy.uphjek.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lpg.shanyushiyangtech.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://odp.xylfe.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://irj.0kj1m.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ohl.birdmap.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jrk.ybcxt.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://spj.yueranfly.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hqt.zhaomingkeji.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ppx.yvedp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://clj.jianghu66.top

================================================================================
来源：http://eom.c1oappe.top

A. 基础语法与类型
来源：http://vbo.yuxming.cn

================================================================================
来源：http://dvi.jinyuanbaomall.cn

[A01] Hello World
来源：http://dwo.andypj.xyz


<!-- 参考信息 -->