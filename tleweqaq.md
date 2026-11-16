代发 wailian999

[U25] Py：CSV 按字典读
来源：http://acd.ivvv.top

csv.DictReader(f)
来源：http://mnv.andypj.xyz

[U26] Py：并发下载
来源：http://xpv.jyoumei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://arm.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://wrc.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://bvd.yj202588.top

[U28] Py：类型别名
来源：http://nor.tian-w.cn

UserId = int
来源：http://mpg.tianlin.xyz

[U29] Py：属性校验
来源：http://yfd.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://ssd.ydjk.org.cn

[U30] Py：数据类
来源：http://jhb.pengpengdd.cyou

@dataclass(slots=True)
来源：http://swu.hnxiangtu.top

[U31] Py：单测
来源：http://nqe.zhixingplan.top

python -m pytest -q
来源：http://des.sjlbkw.cn

[U32] Py：代码格式化
来源：http://jng.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://lrt.ehwqpu.com

[U33] Py：打包发布
来源：http://gfa.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://qdd.uphjek.com

[U34] Py：判断编码
来源：http://hiq.shangyingyoupin.top

chardet.detect(raw)
来源：http://uyz.jinqigfzy.top

[U35] Py：发送邮件
来源：http://ism.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xlz.nwbrower.top

[U36] Py：定时任务
来源：http://ano.hcnkem.com

schedule.every(10).minutes.do(job)
来源：http://alh.pycfn.com

[U37] Py：读写 Excel
来源：http://txj.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://ndp.guannengcc.top

[U38] Py：获取脚本所在目录
来源：http://voa.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://mxi.0kj1m.cn

[U39] Py：判断是否在交互环境
来源：http://zks.xuetiantiany.cn

sys.stdout.isatty()
来源：http://pcw.52xcode.cn

[U40] Py：打印到标准错误
来源：http://nhg.jinqigufen.top

print("err", file=sys.stderr)
来源：http://rjd.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://shk.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://knf.zycfv.cn

[U42] PHP：PSR-4 自动加载
来源：http://jvp.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zvl.epnwcf.com

[U43] PHP：声明命名空间
来源：http://ulk.wangdashe.top

namespace App\Http;
来源：http://oai.smart0.xyz

[U44] PHP：开启严格类型
来源：http://nwx.yuxming.cn

declare(strict_types=1);
来源：http://knb.gaohongyu789.top

[U45] PHP：类型声明与返回类型
来源：http://ikq.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://slo.jinqigufen.top

[U46] PHP：可空类型
来源：http://eph.nanxuanxn.top

?string $name = null
来源：http://ygj.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://iaa.jinghuilouyu.cn

int|string $id
来源：http://hex.fengsongda.top

[U48] PHP：纯枚举
来源：http://peh.fktsv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dlw.snrcjt.cn

[U49] PHP：只读属性
来源：http://xvc.xingfuxueyuan.xyz

public readonly string $name
来源：http://wgo.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://dmv.sysykeji.top

public function __construct(private int $id) {}
来源：http://oyy.meibo888.top

[U51] PHP：数组解构
来源：http://qix.hammf.cn

[$a, $b] = $arr;
来源：http://pni.yfazqb.com

[U52] PHP：箭头函数
来源：http://pkb.guowangkeji.top

$double = fn($x) => $x * 2;
来源：http://ihj.epnwcf.com

[U53] PHP：空合并运算符
来源：http://tfm.ehwqpu.com

$v = $a ?? $b ?? "default";
来源：http://yfu.birdmap.top

[U54] PHP：空安全调用
来源：http://ens.jinqigufen.top

$obj?->method()
来源：http://zmv.ppjwa.cn

[U55] PHP：match 表达式
来源：http://dyb.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://skk.birdmap.top

[U56] PHP：命名参数
来源：http://vtj.gotoacloud.top

f(a: 1, b: 2)
来源：http://qtc.hysaishi.cn

[U57] PHP：字符串插值
来源：http://zri.yvedp.cn

"值: {$a}"
来源：http://tmn.ydzc1.top

[U58] PHP：数组三件套
来源：http://uaq.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xke.aibaodan.cn

[U59] PHP：自定义排序
来源：http://qjq.kuanghao11.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xqj.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://hib.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://onm.uphjek.com

[U61] PHP：正则
来源：http://umn.sjlbkw.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qly.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://wzl.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://akl.uphjek.com

[U63] PHP：文件读写
来源：http://clr.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fdk.smart0.xyz

[U64] PHP：目录遍历
来源：http://imn.shuidangran.top

glob("dir/*.php");  scandir("dir");
来源：http://qds.hammf.cn

[U65] PHP：会话
来源：http://rzv.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uvz.shanyushiyangtech.top

[U66] PHP：设置 Cookie
来源：http://yye.gogol.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fuy.xziqi.cn

[U67] PHP：处理文件上传
来源：http://pqz.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kvi.mhx1999.top

[U68] PHP：PDO 连接
来源：http://ata.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xuh.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://plj.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ebx.meibo888.top

[U70] PHP：PDO 事务
来源：http://toe.yangfankeji.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yvu.gotoacloud.top

[U71] PHP：抛出异常
来源：http://zbx.redwolf501.top

throw new RuntimeException("失败", 500);
来源：http://nxw.jianghu66.top

[U72] PHP：写错误日志
来源：http://ncv.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://jhw.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://mco.hongshengwenyu.top

parse_ini_file("config.ini", true)
来源：http://cgb.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://cnh.snrcjt.cn

getenv("APP_ENV") ?: "production"
来源：http://bsw.aibaodan.cn

[U75] PHP：依赖注入
来源：http://puo.nwbrower.top

composer require psr/container
来源：http://itz.birdmap.top

[U76] PHP：简单路由
来源：http://eck.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://def.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://mwi.cucudq.cn

composer require twig/twig
来源：http://ili.zdqjudy.top

[U78] PHP：单元测试
来源：http://xop.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://knn.jinghuilouyu.cn

[U79] PHP：静态分析
来源：http://vbv.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://nmb.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://cdl.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tjo.havefunace.top

[U81] JS：初始化项目
来源：http://snk.quarkkingdee.top

npm init -y;  npm i express
来源：http://tyc.cashguo.top

[U82] JS：package.json 脚本
来源：http://yhj.yonumen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yhg.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://cyl.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://lcs.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://uzf.xingfuxueyuan.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://jtr.xylfe.cn

[U85] JS：可选链
来源：http://wdv.wangdashe.top

a?.b?.c
来源：http://etb.xylfe.cn

[U86] JS：空值合并
来源：http://dez.vehdjk.com

a ?? b
来源：http://qyt.mhx1999.top

[U87] JS：解构默认值
来源：http://ayh.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://ebn.ctjpmb.com

[U88] JS：对象展开合并
来源：http://hja.c1oappe.top

{ ...a, ...b }
来源：http://qca.gaohongyu789.top

[U89] JS：数组去重
来源：http://ujx.hongshengwenyu.top

[...new Set(arr)]
来源：http://aef.guowangkeji.top

[U90] JS：数字数组排序
来源：http://esb.aibaodan.cn

[...arr].sort((a, b) => a - b)
来源：http://nlu.uphjek.com

[U91] JS：对象键值遍历
来源：http://erx.yuxming.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vqd.jyoumei.cn

[U92] JS：深拷贝
来源：http://bhf.ctjpmb.com

structuredClone(obj)
来源：http://url.dianchejie.cn

[U93] JS：模板字符串
来源：http://hhl.tanke756.top

`共 ${n} 条`
来源：http://jkg.nanxuanxn.top

[U94] JS：箭头函数
来源：http://cpe.vehdjk.com

const double = x => x * 2;
来源：http://vuu.yfazqb.com

[U95] JS：Promise 包装
来源：http://xxe.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://xeb.xinyue.icu

[U96] JS：async/await 与异常
来源：http://oun.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pfo.chenjidiqi.icu

[U97] JS：并发请求
来源：http://jkt.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://chw.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://kbn.zhongyouzk.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eyy.zhongyouzk.top

[U99] JS：事件监听
来源：http://dmi.zhengqikj.top

el.addEventListener("click", e => {})
来源：http://szy.zycfv.cn

[U100] JS：DOM 查询
来源：http://gvd.cdnleiting.top

document.querySelector(".item")
来源：http://dau.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://feb.shzxlz.cn

el.classList.toggle("active")
来源：http://afs.zdbjq.cn

[U102] JS：本地存储
来源：http://gvk.pycfn.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ntz.shangyingyoupin.top

[U103] JS：定时器
来源：http://unz.shzxlz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kfk.zhiwuduotai.top

[U104] JS：防抖
来源：http://pdu.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vwt.guowangkeji.top

[U105] JS：节流
来源：http://aju.fengsongda.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ser.hesvh.cn

[U106] JS：日期格式化
来源：http://ysw.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aej.fengsongda.top

[U107] JS：数字千分位
来源：http://lpp.fengsongda.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ybn.tian-w.cn

[U108] JS：随机整数
来源：http://zvu.jqgufenzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dcd.ppjwa.cn

[U109] JS：数组分组
来源：http://hxq.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://swm.xziqi.cn

[U110] JS：数组分块
来源：http://mlt.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ujk.aizwys.cn

[U111] JS：对象转 Map
来源：http://any.cucudq.cn

new Map(Object.entries(obj))
来源：http://frr.yueranfly.top

[U112] JS：字符串补位
来源：http://vgu.hcnkem.com

"7".padStart(3, "0")
来源：http://ezm.ydzc1.top

[U113] JS：正则替换全部
来源：http://hqq.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://yui.fengsongda.top

[U114] JS：JSON 深比较
来源：http://dlk.yj20258.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wdk.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://puo.guowangkeji.top

crypto.randomUUID()
来源：http://msb.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://now.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://xfc.cheryme.top

[U117] JS：单元测试
来源：http://mkv.ivvv.top

npm i -D vitest;  npx vitest
来源：http://ite.xuanzx.com

[U118] JS：开发服务器
来源：http://xaz.jinyuanbaomall.cn

npm i -D vite;  npx vite
来源：http://hij.chenlongwang.top

[U119] JS：生产构建
来源：http://eva.ppjwa.cn

npx vite build
来源：http://wxu.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://uyu.andypj.xyz

import.meta.env.VITE_API_URL
来源：http://pwe.hongshengwenyu.top

================================================================================
来源：http://cyi.tianlin.xyz

统计汇总
来源：http://jwh.sweek.top

================================================================================
来源：http://aau.cdnleiting.top

按语言统计（条）：
来源：http://dzc.hysaishi.cn

Python ......... 252
来源：http://oqo.iojbl.cn

PHP ............ 252
来源：http://bdy.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://rvw.jlsjyb.cn

TypeScript ..... 212
来源：http://uyr.meibo888.top

Java ........... 212
来源：http://eau.uphjek.com

Go ............. 212
来源：http://evr.bjfxy.top

Ruby ........... 212
来源：http://rcx.cheryme.top

C# ............. 212
来源：http://qmc.52xcode.cn

C .............. 30
来源：http://ach.hfpthk.cn

C++ ............ 30
来源：http://wkt.gaohongyu789.top

SQL ............ 90
来源：http://syj.hnxiangtu.top

Bash ........... 80
来源：http://snf.gogol.net.cn

Kotlin ......... 15
来源：http://xgu.zhongyouzk.top

Swift .......... 15
来源：http://exo.svipenyu.cn

Lua ............ 10
来源：http://frb.jinqigfzy.top

Perl ........... 10
来源：http://lyv.jinqigfzy.top

Scala .......... 10
来源：http://pgu.xziqi.cn

------------------------------------
来源：http://hon.sysykeji.top

合计 ........... 2106 条
来源：http://iii.gotoacloud.top

按章节统计：
来源：http://cqe.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xbv.ehwqpu.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yyf.cashguo.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wku.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://swo.zhiwuduotai.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lmq.ybcxt.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rxd.ehwqpu.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ggy.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xsi.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cyk.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wqx.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bok.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://psx.havefunace.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ibm.jqgufenzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://njw.zhaomingkeji.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://esd.gotoacloud.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nbs.jinghuilouyu.cn

Q SQL 专题                              90
来源：http://uvl.hfpthk.cn

R Bash 专题                             80
来源：http://ynk.yangfankeji.com

S C / C++ 专题                          60
来源：http://mrj.cheryme.top

T 其他语言补充                          60
来源：http://fcp.birdmap.top

U 高频实用片段                         120
来源：http://twd.daxiang520.top

------------------------------------
来源：http://vuf.xuanzx.com

合计                                  2106 条
来源：http://zil.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://fzp.zdqjudy.top

使用提醒
来源：http://ugm.shuidangran.top

--------------------------------------------------------------------------------
来源：http://byh.fengsongda.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jqn.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dpf.epnwcf.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dgc.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://odd.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lmb.jianghu66.top

—— 文件结束 ——
来源：http://odk.xuanzx.com

================================================================================
来源：http://kkb.cashguo.top

程序语言常见例子速查手册（2024 版）
来源：http://tjp.cucudq.cn

Common Programming Examples Cheat Book
来源：http://nyn.cashguo.top

================================================================================
来源：http://qih.yanxiufei.cn

【收录内容】
来源：http://umj.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://kxb.zhongyouzk.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qju.hysaishi.cn

SQL · Bash · C · C++
来源：http://viu.ctjpmb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://djs.wangdashe.top

【使用说明】
来源：http://ayw.hywenlv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ltr.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zlv.aibaodan.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://daa.jyoumei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tbx.wangdashe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://svc.hcnkem.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zcz.jqgfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dwc.hongshengwenyu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bhh.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vvy.dianchejie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qfk.sxryk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sgz.zhijiandao.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bqt.jlsjyb.cn

【文件统计】
来源：http://hrm.tian-w.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gzk.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://ony.hammf.cn

目  录
来源：http://coh.sysykeji.top

--------------------------------------------------------------------------------
来源：http://xsr.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uag.zhiwuduotai.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fui.pycfn.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nmn.zhongyouzk.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tsi.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ouy.zhengqikj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kkj.jiagoushi.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cut.daxiang520.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uvs.cdnleiting.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hkd.gzhubu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oac.c1oappe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lvc.bjfxy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qyp.ybcxt.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nvi.shanyushiyangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://avi.fengsongda.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lob.zhengqikj.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vim.jiagoushi.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bwa.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sgi.sxryk.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qtg.svipenyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kdj.cdnleiting.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fkt.yj20258888.top

================================================================================
来源：http://koi.tarul.cn

A. 基础语法与类型
来源：http://skh.chenlongwang.top

================================================================================
来源：http://yrd.shangyingyoupin.top

[A01] Hello World
来源：http://dge.9152youxi.cn


<!-- 参考信息 -->