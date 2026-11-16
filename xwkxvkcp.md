代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://bkz.zycfv.cn

@contextlib.contextmanager
来源：http://vob.xziqi.cn

[U22] Py：矩阵转置
来源：http://loa.yvedp.cn

list(zip(*m))
来源：http://kru.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://ynd.xziqi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rzd.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://kcb.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pbk.ivvv.top

[U25] Py：CSV 按字典读
来源：http://mkl.cdnleiting.top

csv.DictReader(f)
来源：http://ohf.pycfn.com

[U26] Py：并发下载
来源：http://dqu.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yri.chenzaomai.com

[U27] Py：异步 HTTP
来源：http://zpq.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://mea.yvedp.cn

[U28] Py：类型别名
来源：http://rdx.kuanghao11.cn

UserId = int
来源：http://way.hnqzz.top

[U29] Py：属性校验
来源：http://cck.guowangkeji.top

@property 与 @x.setter 配合
来源：http://mhi.hcnkem.com

[U30] Py：数据类
来源：http://gcx.zhiwuduotai.top

@dataclass(slots=True)
来源：http://wuh.hongshengwenyu.top

[U31] Py：单测
来源：http://xpx.bbcook.cn

python -m pytest -q
来源：http://jmu.yangfankeji.com

[U32] Py：代码格式化
来源：http://xlw.hesvh.cn

ruff format . && ruff check --fix .
来源：http://yvi.hywenlv.cn

[U33] Py：打包发布
来源：http://req.tianlin.xyz

python -m build  （依赖 pyproject.toml）
来源：http://isc.nwbrower.top

[U34] Py：判断编码
来源：http://xix.dashuyun.cn

chardet.detect(raw)
来源：http://ggg.zhixingplan.top

[U35] Py：发送邮件
来源：http://rol.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kdg.aizwys.cn

[U36] Py：定时任务
来源：http://efi.tanke756.top

schedule.every(10).minutes.do(job)
来源：http://bsl.aizwys.cn

[U37] Py：读写 Excel
来源：http://hqk.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://vgd.zhoulong.xyz

[U38] Py：获取脚本所在目录
来源：http://eta.xziqi.cn

Path(__file__).resolve().parent
来源：http://zaa.yvedp.cn

[U39] Py：判断是否在交互环境
来源：http://fzy.jlsjyb.cn

sys.stdout.isatty()
来源：http://att.aizwys.cn

[U40] Py：打印到标准错误
来源：http://caa.yonumen.top

print("err", file=sys.stderr)
来源：http://xpe.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://eob.gotoacloud.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fxq.haohaochexian.top

[U42] PHP：PSR-4 自动加载
来源：http://oib.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://euy.cdnleiting.top

[U43] PHP：声明命名空间
来源：http://sxs.shuidangran.top

namespace App\Http;
来源：http://uxh.hammf.cn

[U44] PHP：开启严格类型
来源：http://wvq.316326.xyz

declare(strict_types=1);
来源：http://yum.daria6918.cn

[U45] PHP：类型声明与返回类型
来源：http://hzz.jinyuanbaomall.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qit.havefunace.top

[U46] PHP：可空类型
来源：http://kuq.zycfv.cn

?string $name = null
来源：http://whk.hnqzz.top

[U47] PHP：联合类型
来源：http://yyz.jiagoushi.top

int|string $id
来源：http://twb.svipenyu.cn

[U48] PHP：纯枚举
来源：http://cyp.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iem.9152youxi.cn

[U49] PHP：只读属性
来源：http://jig.yanxiufei.cn

public readonly string $name
来源：http://cta.tarul.cn

[U50] PHP：构造器属性提升
来源：http://ohq.hfpthk.cn

public function __construct(private int $id) {}
来源：http://uqp.iojbl.cn

[U51] PHP：数组解构
来源：http://xuo.fktsv.cn

[$a, $b] = $arr;
来源：http://vzm.hnqzz.top

[U52] PHP：箭头函数
来源：http://vbu.hesvh.cn

$double = fn($x) => $x * 2;
来源：http://ezi.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://oks.yj202588.top

$v = $a ?? $b ?? "default";
来源：http://zya.smart0.xyz

[U54] PHP：空安全调用
来源：http://mig.zhaomingkeji.xyz

$obj?->method()
来源：http://ime.hammf.cn

[U55] PHP：match 表达式
来源：http://hmf.guowangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lbc.zdbjq.cn

[U56] PHP：命名参数
来源：http://qhq.jqgufenzy.top

f(a: 1, b: 2)
来源：http://rqc.mhx1999.top

[U57] PHP：字符串插值
来源：http://tyb.quarkkingdee.top

"值: {$a}"
来源：http://boa.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://hrn.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kpx.sweek.top

[U59] PHP：自定义排序
来源：http://sar.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kyu.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://ykr.jinqigfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://onh.shzxlz.cn

[U61] PHP：正则
来源：http://ovb.ydjk.org.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://avy.9152youxi.cn

[U62] PHP：日期对象
来源：http://ctr.sxryk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qkz.cheryme.top

[U63] PHP：文件读写
来源：http://qgf.cqqwz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xto.cashguo.top

[U64] PHP：目录遍历
来源：http://uwx.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://avz.shzxlz.cn

[U65] PHP：会话
来源：http://ytu.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pgq.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://mrn.xingfuxueyuan.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qjz.vqdsnc.cn

[U67] PHP：处理文件上传
来源：http://znu.hcnkem.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ccw.tianlin.xyz

[U68] PHP：PDO 连接
来源：http://nac.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://brn.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://jas.xuanzx.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jci.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://lim.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://edm.svipenyu.cn

[U71] PHP：抛出异常
来源：http://blx.yongpay.top

throw new RuntimeException("失败", 500);
来源：http://dzs.chenlongwang.top

[U72] PHP：写错误日志
来源：http://jwv.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://sys.hnqzz.top

[U73] PHP：读取 ini 配置
来源：http://nwg.9152youxi.cn

parse_ini_file("config.ini", true)
来源：http://nrb.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://fbv.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://qvb.cucudq.cn

[U75] PHP：依赖注入
来源：http://fcm.bjfxy.top

composer require psr/container
来源：http://bge.aibaodan.cn

[U76] PHP：简单路由
来源：http://fyl.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uxc.sxryk.cn

[U77] PHP：模板渲染
来源：http://smc.mhx1999.top

composer require twig/twig
来源：http://pia.tarul.cn

[U78] PHP：单元测试
来源：http://hqh.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://wfu.ydzc1.top

[U79] PHP：静态分析
来源：http://slx.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://miq.hesvh.cn

[U80] PHP：代码规范修复
来源：http://vpn.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pni.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://dyx.ydjk.org.cn

npm init -y;  npm i express
来源：http://mpr.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://rcm.cucudq.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sme.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://twr.hnqzz.top

export const a = 1;  import { a } from "./m.js";
来源：http://bco.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://lhr.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://hre.tanke756.top

[U85] JS：可选链
来源：http://rub.cheryme.top

a?.b?.c
来源：http://bud.yonumen.top

[U86] JS：空值合并
来源：http://ahn.ehwqpu.com

a ?? b
来源：http://xun.andypj.xyz

[U87] JS：解构默认值
来源：http://taw.gaohongyu789.top

const { a = 1, b = 2 } = obj;
来源：http://vyg.ehwqpu.com

[U88] JS：对象展开合并
来源：http://yeh.iojbl.cn

{ ...a, ...b }
来源：http://oul.jinqigufen.top

[U89] JS：数组去重
来源：http://ldc.wangshuangyany.cn

[...new Set(arr)]
来源：http://jtr.yuxming.cn

[U90] JS：数字数组排序
来源：http://nuo.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://icq.fktsv.cn

[U91] JS：对象键值遍历
来源：http://xel.cheryme.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rwu.zdqjudy.top

[U92] JS：深拷贝
来源：http://gxr.ivvv.top

structuredClone(obj)
来源：http://ofu.chenzaomai.com

[U93] JS：模板字符串
来源：http://apu.cucudq.cn

`共 ${n} 条`
来源：http://kho.bjfxy.top

[U94] JS：箭头函数
来源：http://vug.jyoumei.cn

const double = x => x * 2;
来源：http://npj.xziqi.cn

[U95] JS：Promise 包装
来源：http://jjb.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://qfd.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://fmc.316326.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vyx.hywenlv.cn

[U97] JS：并发请求
来源：http://edv.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zxs.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://atz.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://avb.cucudq.cn

[U99] JS：事件监听
来源：http://sfe.hesvh.cn

el.addEventListener("click", e => {})
来源：http://ekq.xinyue.icu

[U100] JS：DOM 查询
来源：http://gcy.cucudq.cn

document.querySelector(".item")
来源：http://gua.fzhhl.top

[U101] JS：classList 操作
来源：http://hnp.jinqigfzy.top

el.classList.toggle("active")
来源：http://wdc.tian-w.cn

[U102] JS：本地存储
来源：http://opd.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fwx.aibaodan.cn

[U103] JS：定时器
来源：http://vfw.redwolf501.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ccf.andypj.xyz

[U104] JS：防抖
来源：http://efy.shangyingyoupin.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://etq.aizwys.cn

[U105] JS：节流
来源：http://qwp.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ngg.haohaochexian.top

[U106] JS：日期格式化
来源：http://kms.zhongyouzk.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cus.52xcode.cn

[U107] JS：数字千分位
来源：http://qkl.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zsa.hysaishi.cn

[U108] JS：随机整数
来源：http://pgx.vehdjk.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dss.pycfn.com

[U109] JS：数组分组
来源：http://phk.tanke756.top

Object.groupBy(arr, x => x.type)
来源：http://uae.fengsongda.top

[U110] JS：数组分块
来源：http://owp.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xcm.hesvh.cn

[U111] JS：对象转 Map
来源：http://jxu.uphjek.com

new Map(Object.entries(obj))
来源：http://ejk.yj202588.top

[U112] JS：字符串补位
来源：http://nni.hnqzz.top

"7".padStart(3, "0")
来源：http://voc.ctjpmb.com

[U113] JS：正则替换全部
来源：http://lum.yj20258888.top

s.replaceAll("a", "b")
来源：http://lxl.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://rmd.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nlq.ehwqpu.com

[U115] JS：生成 UUID
来源：http://rwt.xinyue.icu

crypto.randomUUID()
来源：http://pmr.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://aix.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://owt.pengpengdd.cyou

[U117] JS：单元测试
来源：http://nuk.yongpay.top

npm i -D vitest;  npx vitest
来源：http://lwn.svipenyu.cn

[U118] JS：开发服务器
来源：http://myd.tianlin.xyz

npm i -D vite;  npx vite
来源：http://stz.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://mtf.jinghuilouyu.cn

npx vite build
来源：http://zel.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://pxo.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://vun.uphjek.com

================================================================================
来源：http://xus.hnxiangtu.top

统计汇总
来源：http://swe.xuanzx.com

================================================================================
来源：http://ntp.vqdsnc.cn

按语言统计（条）：
来源：http://xjb.shangyingyoupin.top

Python ......... 252
来源：http://aba.shanyushiyangtech.top

PHP ............ 252
来源：http://mgo.ywan-chungtsiang.top

JavaScript ..... 252
来源：http://sld.aizwys.cn

TypeScript ..... 212
来源：http://ayj.hcnkem.com

Java ........... 212
来源：http://wit.jlsjyb.cn

Go ............. 212
来源：http://bov.iojbl.cn

Ruby ........... 212
来源：http://cmj.daxiang520.top

C# ............. 212
来源：http://kvq.jinyuanbaomall.cn

C .............. 30
来源：http://asa.shanyushiyangkeji.top

C++ ............ 30
来源：http://vum.yj202588.top

SQL ............ 90
来源：http://sbd.jlsjyb.cn

Bash ........... 80
来源：http://whw.bjfxy.top

Kotlin ......... 15
来源：http://iem.xinyue.icu

Swift .......... 15
来源：http://jmg.jinqigfzy.top

Lua ............ 10
来源：http://aiq.hysaishi.cn

Perl ........... 10
来源：http://ccz.sjlbkw.cn

Scala .......... 10
来源：http://ynw.zhoulong.xyz

------------------------------------
来源：http://kbf.xylfe.cn

合计 ........... 2106 条
来源：http://xsz.daxiang520.top

按章节统计：
来源：http://nok.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wvd.ivvv.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ihm.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pfg.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tck.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tcq.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rwx.birdmap.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xmv.gogol.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jcx.sweek.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hmt.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tnl.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://stu.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kip.gaohongyu789.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jbf.gzhubu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tjh.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dde.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zjo.jlsjyb.cn

Q SQL 专题                              90
来源：http://phq.kuanghao11.cn

R Bash 专题                             80
来源：http://dtz.jianghu66.top

S C / C++ 专题                          60
来源：http://zyc.jqgufenzy.top

T 其他语言补充                          60
来源：http://qpi.jinqigufen.top

U 高频实用片段                         120
来源：http://vhr.yanxiufei.cn

------------------------------------
来源：http://yqv.aibaodan.cn

合计                                  2106 条
来源：http://ihn.havefunace.top

--------------------------------------------------------------------------------
来源：http://jjv.xingfuxueyuan.xyz

使用提醒
来源：http://hsv.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://gvu.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://plx.smart0.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://goo.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://atk.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://bdw.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ysr.uphjek.com

—— 文件结束 ——
来源：http://try.tarul.cn

================================================================================
来源：http://pnn.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://dzu.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://khd.tarul.cn

================================================================================
来源：http://gjr.zhongyouzk.top

【收录内容】
来源：http://pui.smart0.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://qpq.sweek.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://opz.ivvv.top

SQL · Bash · C · C++
来源：http://aln.yj202588.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vlv.quarkkingdee.top

【使用说明】
来源：http://dja.pycfn.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xhf.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eca.c1oappe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://udz.jianghu66.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ozt.hnqzz.top

Bash:  Shell         C:     C             C++:   C++
来源：http://akl.hesvh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://its.hnqzz.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eyw.ehwqpu.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://txb.tian-w.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ere.sufxvd.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iww.shangyingyoupin.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mjj.yj20258888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lqh.bbcook.cn

【文件统计】
来源：http://shg.jinqigfzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dhs.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://cna.hcnkem.com

目  录
来源：http://ykg.fengsongda.top

--------------------------------------------------------------------------------
来源：http://xsh.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hua.pengpengdd.cyou

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cgu.jinqigfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fjh.quarkkingdee.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yik.ywan-chungtsiang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://spa.sysykeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rxp.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bnl.guowangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uaw.bbcook.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gqk.ywan-chungtsiang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rdo.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bwe.yonumen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jua.jlsjyb.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yij.jinyuanbaomall.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rli.hnxiangtu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ebh.chenlongwang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gjm.daria6918.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ede.dashuyun.cn


<!-- 参考信息 -->