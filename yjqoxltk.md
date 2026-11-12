代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://yge.jlsjyb.cn

@contextlib.contextmanager
来源：http://yfz.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://mtd.dashuyun.cn

list(zip(*m))
来源：http://rdx.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://ous.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xkd.tianlin.xyz

[U24] Py：路径操作
来源：http://fvy.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sng.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://sjt.hywenlv.cn

csv.DictReader(f)
来源：http://daf.xinyue.icu

[U26] Py：并发下载
来源：http://mtj.jinyuanbaomall.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rnl.gotoacloud.top

[U27] Py：异步 HTTP
来源：http://psh.mhx1999.top

aiohttp.ClientSession() 配合 async with
来源：http://lec.gzhubu.top

[U28] Py：类型别名
来源：http://phh.zhoulong.xyz

UserId = int
来源：http://jgh.haohaochexian.top

[U29] Py：属性校验
来源：http://tma.xinyue.icu

@property 与 @x.setter 配合
来源：http://jzf.meibo888.top

[U30] Py：数据类
来源：http://oop.birdmap.top

@dataclass(slots=True)
来源：http://tgt.daxiang520.top

[U31] Py：单测
来源：http://efq.hesvh.cn

python -m pytest -q
来源：http://tfq.havefunace.top

[U32] Py：代码格式化
来源：http://shn.gotoacloud.top

ruff format . && ruff check --fix .
来源：http://rhp.feifeiyinyue.top

[U33] Py：打包发布
来源：http://xsv.yvedp.cn

python -m build  （依赖 pyproject.toml）
来源：http://crc.vehdjk.com

[U34] Py：判断编码
来源：http://jmt.cdnleiting.top

chardet.detect(raw)
来源：http://xmz.chenzaomai.com

[U35] Py：发送邮件
来源：http://erb.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ucw.sysykeji.top

[U36] Py：定时任务
来源：http://byt.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://gts.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://dek.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://tee.cucudq.cn

[U38] Py：获取脚本所在目录
来源：http://cwm.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://pdp.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://tdg.hammf.cn

sys.stdout.isatty()
来源：http://rmn.hnxiangtu.top

[U40] Py：打印到标准错误
来源：http://tnc.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://ahm.svipenyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://saa.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://otq.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://xhp.uphjek.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rjw.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://mil.jiagoushi.top

namespace App\Http;
来源：http://agy.zhijiandao.cn

[U44] PHP：开启严格类型
来源：http://dyh.daria6918.cn

declare(strict_types=1);
来源：http://bgb.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://stx.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jaf.guannengcc.top

[U46] PHP：可空类型
来源：http://lwm.meibo888.top

?string $name = null
来源：http://wqf.jqgufenzy.top

[U47] PHP：联合类型
来源：http://zee.yangfankeji.com

int|string $id
来源：http://tvx.ybcxt.top

[U48] PHP：纯枚举
来源：http://ekr.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cmk.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://vgg.iojbl.cn

public readonly string $name
来源：http://vsv.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://pwf.yfazqb.com

public function __construct(private int $id) {}
来源：http://cym.nanxinkj.top

[U51] PHP：数组解构
来源：http://uov.guannengcc.top

[$a, $b] = $arr;
来源：http://tqx.xziqi.cn

[U52] PHP：箭头函数
来源：http://cgz.havefunace.top

$double = fn($x) => $x * 2;
来源：http://owe.guannengcc.top

[U53] PHP：空合并运算符
来源：http://jaw.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://snu.yangfankeji.com

[U54] PHP：空安全调用
来源：http://jqv.zhoulong.xyz

$obj?->method()
来源：http://ehq.zhoulong.xyz

[U55] PHP：match 表达式
来源：http://zwc.c1oappe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lgi.zycfv.cn

[U56] PHP：命名参数
来源：http://llo.xuanzx.com

f(a: 1, b: 2)
来源：http://vpw.hcnkem.com

[U57] PHP：字符串插值
来源：http://qyv.jinqigfzy.top

"值: {$a}"
来源：http://wvb.gogol.net.cn

[U58] PHP：数组三件套
来源：http://wvt.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zvh.havefunace.top

[U59] PHP：自定义排序
来源：http://kwq.yuxming.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ail.xuetiantiany.cn

[U60] PHP：JSON 编解码
来源：http://wbv.cucudq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qvi.gogol.net.cn

[U61] PHP：正则
来源：http://vxd.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rbr.svipenyu.cn

[U62] PHP：日期对象
来源：http://uns.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pcp.xziqi.cn

[U63] PHP：文件读写
来源：http://uvl.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iiv.52xcode.cn

[U64] PHP：目录遍历
来源：http://lct.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://egr.mhx1999.top

[U65] PHP：会话
来源：http://seq.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://iwn.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://ybo.yj202588.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://suf.nanxuanxn.top

[U67] PHP：处理文件上传
来源：http://csb.zhiwuduotai.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://opz.0kj1m.cn

[U68] PHP：PDO 连接
来源：http://zlj.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qlz.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://xft.ydzc1.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ptj.tarul.cn

[U70] PHP：PDO 事务
来源：http://edt.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yli.wangdashe.top

[U71] PHP：抛出异常
来源：http://trs.pengpengdd.cyou

throw new RuntimeException("失败", 500);
来源：http://syn.jianghu66.top

[U72] PHP：写错误日志
来源：http://qgp.yj20258888.top

error_log("失败: " . $e->getMessage());
来源：http://epc.sweek.top

[U73] PHP：读取 ini 配置
来源：http://wfu.hesvh.cn

parse_ini_file("config.ini", true)
来源：http://bbq.zhixingplan.top

[U74] PHP：读取环境变量
来源：http://sed.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://ghn.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://yer.jqgfzy.top

composer require psr/container
来源：http://szu.ydzc1.top

[U76] PHP：简单路由
来源：http://srh.birdmap.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://goj.chenlongwang.top

[U77] PHP：模板渲染
来源：http://gov.tian-w.cn

composer require twig/twig
来源：http://oub.jianghu66.top

[U78] PHP：单元测试
来源：http://nne.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://gpb.cdnleiting.top

[U79] PHP：静态分析
来源：http://afw.bbcook.cn

composer require --dev phpstan/phpstan
来源：http://uvy.yj20258888.top

[U80] PHP：代码规范修复
来源：http://wwm.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rvr.bjfxy.top

[U81] JS：初始化项目
来源：http://unr.316326.xyz

npm init -y;  npm i express
来源：http://roo.jianghu66.top

[U82] JS：package.json 脚本
来源：http://cbd.zhixingplan.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bpl.tanke756.top

[U83] JS：ES Module 导入导出
来源：http://pnb.meibo888.top

export const a = 1;  import { a } from "./m.js";
来源：http://ldy.zhoulong.xyz

[U84] JS：CommonJS 写法
来源：http://ntq.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://wgh.hnqzz.top

[U85] JS：可选链
来源：http://oky.yanxiufei.cn

a?.b?.c
来源：http://vtu.xziqi.cn

[U86] JS：空值合并
来源：http://dkm.ydjk.org.cn

a ?? b
来源：http://tih.cucudq.cn

[U87] JS：解构默认值
来源：http://fle.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://jrq.kuanghao11.cn

[U88] JS：对象展开合并
来源：http://kwt.guannengcc.top

{ ...a, ...b }
来源：http://lhy.xingfuxueyuan.xyz

[U89] JS：数组去重
来源：http://tgg.guowangkeji.top

[...new Set(arr)]
来源：http://crg.wangshuangyany.cn

[U90] JS：数字数组排序
来源：http://fre.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://elz.aizwys.cn

[U91] JS：对象键值遍历
来源：http://xhj.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sxi.yj20258.top

[U92] JS：深拷贝
来源：http://eft.zhongyouzk.top

structuredClone(obj)
来源：http://ucb.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://wzq.zhijiandao.cn

`共 ${n} 条`
来源：http://qnu.ctjpmb.com

[U94] JS：箭头函数
来源：http://hka.yfazqb.com

const double = x => x * 2;
来源：http://jfb.svipenyu.cn

[U95] JS：Promise 包装
来源：http://oil.daxiang520.top

new Promise((resolve, reject) => {})
来源：http://avw.pycfn.com

[U96] JS：async/await 与异常
来源：http://ysg.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ist.9152youxi.cn

[U97] JS：并发请求
来源：http://rwy.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ofb.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://izp.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xwe.wangdashe.top

[U99] JS：事件监听
来源：http://fub.yuxming.cn

el.addEventListener("click", e => {})
来源：http://jqf.ehwqpu.com

[U100] JS：DOM 查询
来源：http://bbt.cashguo.top

document.querySelector(".item")
来源：http://pmh.jiagoushi.top

[U101] JS：classList 操作
来源：http://kov.zdqjudy.top

el.classList.toggle("active")
来源：http://qpq.ctjpmb.com

[U102] JS：本地存储
来源：http://ihs.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://beb.c1oappe.top

[U103] JS：定时器
来源：http://nng.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://byp.yj20258.top

[U104] JS：防抖
来源：http://gcs.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wld.redwolf501.top

[U105] JS：节流
来源：http://ggq.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pbs.havefunace.top

[U106] JS：日期格式化
来源：http://vze.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wbv.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://low.cucudq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cbh.aizwys.cn

[U108] JS：随机整数
来源：http://xcj.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fdy.vqdsnc.cn

[U109] JS：数组分组
来源：http://uhs.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://wyk.cqqwz.cn

[U110] JS：数组分块
来源：http://tim.gaohongyu789.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://emk.jyoumei.cn

[U111] JS：对象转 Map
来源：http://lgx.fengsongda.top

new Map(Object.entries(obj))
来源：http://zqe.tanke756.top

[U112] JS：字符串补位
来源：http://kbo.jinghuilouyu.cn

"7".padStart(3, "0")
来源：http://yyk.ydzc1.top

[U113] JS：正则替换全部
来源：http://qgm.xziqi.cn

s.replaceAll("a", "b")
来源：http://drv.yj202588.top

[U114] JS：JSON 深比较
来源：http://bse.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rso.fktsv.cn

[U115] JS：生成 UUID
来源：http://lsh.zycfv.cn

crypto.randomUUID()
来源：http://wuv.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://kvj.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://ugg.nwbrower.top

[U117] JS：单元测试
来源：http://vgh.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://adi.zdqjudy.top

[U118] JS：开发服务器
来源：http://sxw.bbcook.cn

npm i -D vite;  npx vite
来源：http://zki.bbcook.cn

[U119] JS：生产构建
来源：http://poa.gogol.net.cn

npx vite build
来源：http://acz.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://vrv.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://rgh.bjfxy.top

================================================================================
来源：http://xft.hesvh.cn

统计汇总
来源：http://qyi.havefunace.top

================================================================================
来源：http://exb.shzxlz.cn

按语言统计（条）：
来源：http://fvb.zycfv.cn

Python ......... 252
来源：http://uwx.pengpengdd.cyou

PHP ............ 252
来源：http://zag.sysykeji.top

JavaScript ..... 252
来源：http://rnp.jinqigufen.top

TypeScript ..... 212
来源：http://kss.tian-w.cn

Java ........... 212
来源：http://nle.hnqzz.top

Go ............. 212
来源：http://hxt.zhijiandao.cn

Ruby ........... 212
来源：http://iyl.hammf.cn

C# ............. 212
来源：http://uqr.c1oappe.top

C .............. 30
来源：http://xjj.meibo888.top

C++ ............ 30
来源：http://dhf.cashguo.top

SQL ............ 90
来源：http://kwf.hysaishi.cn

Bash ........... 80
来源：http://mrf.ydjk.org.cn

Kotlin ......... 15
来源：http://pjz.snrcjt.cn

Swift .......... 15
来源：http://dxf.tanke756.top

Lua ............ 10
来源：http://mch.guannengcc.top

Perl ........... 10
来源：http://pbv.ctjpmb.com

Scala .......... 10
来源：http://fzg.gogol.net.cn

------------------------------------
来源：http://lhx.birdmap.top

合计 ........... 2106 条
来源：http://wps.jinghuilouyu.cn

按章节统计：
来源：http://ssc.yangfankeji.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jwb.xingfuxueyuan.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uwu.aibaodan.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bnd.chenlongwang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mcl.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wfx.xingfuxueyuan.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://laa.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zpo.dianchejie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://otq.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gkp.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kvn.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://npb.hnqzz.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oqy.wangshuangyany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ifa.yuanzhike.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vqq.shanyushiyangtech.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mka.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uzq.fzhhl.top

Q SQL 专题                              90
来源：http://irx.tian-w.cn

R Bash 专题                             80
来源：http://kfr.snrcjt.cn

S C / C++ 专题                          60
来源：http://zkc.hywenlv.cn

T 其他语言补充                          60
来源：http://kas.uphjek.com

U 高频实用片段                         120
来源：http://tgd.ppjwa.cn

------------------------------------
来源：http://qzu.tarul.cn

合计                                  2106 条
来源：http://zxo.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://fxh.havefunace.top

使用提醒
来源：http://ogr.yj202588.top

--------------------------------------------------------------------------------
来源：http://mrw.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tzf.zhaomingkeji.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://arc.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hid.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://odc.yongpay.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jag.hongshengwenyu.top

—— 文件结束 ——
来源：http://yum.cucudq.cn

================================================================================
来源：http://elu.iojbl.cn

程序语言常见例子速查手册（2024 版）
来源：http://rrd.chenlongwang.top

Common Programming Examples Cheat Book
来源：http://ovb.hnxiangtu.top

================================================================================
来源：http://snt.yj20258.top

【收录内容】
来源：http://hww.jinyuanbaomall.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mnj.vehdjk.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://slj.zhongyouzk.top

SQL · Bash · C · C++
来源：http://law.ywan-chungtsiang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://olh.fzhhl.top

【使用说明】
来源：http://igp.ctjpmb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tva.daria6918.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ewq.wangdashe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lml.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kik.tian-w.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rjf.vehdjk.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hfh.sjlbkw.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ytr.zhoulong.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lpg.jyoumei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ijv.fanxiaobao.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nkv.kuanghao11.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dfd.pycfn.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vmj.jinyuanbaomall.cn

【文件统计】
来源：http://fiq.gzhubu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://syq.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://vxb.wangshuangyany.cn

目  录
来源：http://fnh.yfazqb.com

--------------------------------------------------------------------------------
来源：http://fev.sysykeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xpu.ydzc1.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://job.xinyue.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rmb.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zdp.shangyingyoupin.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wyw.yuanzhike.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zgz.yueranfly.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ghp.hcnkem.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kvj.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://shq.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mik.shanyushiyangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://brd.andypj.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xll.gotoacloud.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://epn.316326.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iqa.cucudq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dmr.birdmap.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://srd.hysaishi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gdd.cdnleiting.top


<!-- 参考信息 -->