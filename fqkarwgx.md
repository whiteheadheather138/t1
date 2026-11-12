代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://vla.guannengcc.top

@contextlib.contextmanager
来源：http://kik.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://nwb.chenjidiqi.icu

list(zip(*m))
来源：http://lks.birdmap.top

[U23] Py：分块读取大文件
来源：http://eus.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mxo.tanke756.top

[U24] Py：路径操作
来源：http://pzh.ydzc1.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tel.pycfn.com

[U25] Py：CSV 按字典读
来源：http://yly.cheryme.top

csv.DictReader(f)
来源：http://vbt.quarkkingdee.top

[U26] Py：并发下载
来源：http://ijy.yangfankeji.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tvi.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://khj.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://qra.yuanzhike.top

[U28] Py：类型别名
来源：http://fqr.hnxiangtu.top

UserId = int
来源：http://qta.cheryme.top

[U29] Py：属性校验
来源：http://enq.9152youxi.cn

@property 与 @x.setter 配合
来源：http://txp.chenjidiqi.icu

[U30] Py：数据类
来源：http://cza.guowangkeji.top

@dataclass(slots=True)
来源：http://gup.jqgfzy.top

[U31] Py：单测
来源：http://vln.cqqwz.cn

python -m pytest -q
来源：http://bso.yanxiufei.cn

[U32] Py：代码格式化
来源：http://jya.nwbrower.top

ruff format . && ruff check --fix .
来源：http://zqv.xinyue.icu

[U33] Py：打包发布
来源：http://jko.daria6918.cn

python -m build  （依赖 pyproject.toml）
来源：http://pqw.cdnleiting.top

[U34] Py：判断编码
来源：http://anc.fktsv.cn

chardet.detect(raw)
来源：http://fcj.daria6918.cn

[U35] Py：发送邮件
来源：http://uyd.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tlq.aizwys.cn

[U36] Py：定时任务
来源：http://nuy.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://srb.c1oappe.top

[U37] Py：读写 Excel
来源：http://zet.aizwys.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kqr.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://cis.hammf.cn

Path(__file__).resolve().parent
来源：http://zdb.birdmap.top

[U39] Py：判断是否在交互环境
来源：http://ukh.fengsongda.top

sys.stdout.isatty()
来源：http://qck.zhengqikj.top

[U40] Py：打印到标准错误
来源：http://wrm.yanxiufei.cn

print("err", file=sys.stderr)
来源：http://mpd.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://epk.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://shy.zhengqikj.top

[U42] PHP：PSR-4 自动加载
来源：http://qpv.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ffz.mhx1999.top

[U43] PHP：声明命名空间
来源：http://yfw.ydzc1.top

namespace App\Http;
来源：http://aik.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://meo.yj202588.top

declare(strict_types=1);
来源：http://vna.c1oappe.top

[U45] PHP：类型声明与返回类型
来源：http://hnb.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://coz.bbcook.cn

[U46] PHP：可空类型
来源：http://oei.gotoacloud.top

?string $name = null
来源：http://dkz.jinqigufen.top

[U47] PHP：联合类型
来源：http://nqv.fengsongda.top

int|string $id
来源：http://hpq.aibaodan.cn

[U48] PHP：纯枚举
来源：http://pwz.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vgr.epnwcf.com

[U49] PHP：只读属性
来源：http://nox.xingfuxueyuan.xyz

public readonly string $name
来源：http://dgp.tanke756.top

[U50] PHP：构造器属性提升
来源：http://bgq.birdmap.top

public function __construct(private int $id) {}
来源：http://emw.cucudq.cn

[U51] PHP：数组解构
来源：http://krg.svipenyu.cn

[$a, $b] = $arr;
来源：http://ytu.tanke756.top

[U52] PHP：箭头函数
来源：http://orf.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://qsq.gogol.net.cn

[U53] PHP：空合并运算符
来源：http://bnq.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://bbm.sweek.top

[U54] PHP：空安全调用
来源：http://eud.dashuyun.cn

$obj?->method()
来源：http://img.zycfv.cn

[U55] PHP：match 表达式
来源：http://lhs.shanyushiyangtech.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eeo.tarul.cn

[U56] PHP：命名参数
来源：http://gbo.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://zhu.fanxiaobao.xyz

[U57] PHP：字符串插值
来源：http://ysy.ppjwa.cn

"值: {$a}"
来源：http://noi.yvedp.cn

[U58] PHP：数组三件套
来源：http://ueg.jqgufenzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lna.hcnkem.com

[U59] PHP：自定义排序
来源：http://fkh.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lto.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://tch.c1oappe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ipt.vehdjk.com

[U61] PHP：正则
来源：http://vik.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cnh.tanke756.top

[U62] PHP：日期对象
来源：http://jiv.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://urw.hywenlv.cn

[U63] PHP：文件读写
来源：http://vik.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zhy.yj20258.top

[U64] PHP：目录遍历
来源：http://ixy.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://vns.hnxiangtu.top

[U65] PHP：会话
来源：http://enk.cucudq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uej.shangyingyoupin.top

[U66] PHP：设置 Cookie
来源：http://qra.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qrw.zdbjq.cn

[U67] PHP：处理文件上传
来源：http://spz.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ffg.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://dnc.ppjwa.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mhl.chenzaomai.com

[U69] PHP：PDO 预处理
来源：http://uax.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://esw.jlsjyb.cn

[U70] PHP：PDO 事务
来源：http://crs.sxryk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://akd.sxryk.cn

[U71] PHP：抛出异常
来源：http://uyj.snrcjt.cn

throw new RuntimeException("失败", 500);
来源：http://tcx.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://peu.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://dux.yuxming.cn

[U73] PHP：读取 ini 配置
来源：http://imh.yongpay.top

parse_ini_file("config.ini", true)
来源：http://rnh.hnqzz.top

[U74] PHP：读取环境变量
来源：http://wle.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://gbh.yuxming.cn

[U75] PHP：依赖注入
来源：http://fjj.uphjek.com

composer require psr/container
来源：http://nwx.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://ffo.guannengcc.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jcl.yuanzhike.top

[U77] PHP：模板渲染
来源：http://iid.gogol.net.cn

composer require twig/twig
来源：http://qgm.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://jhu.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://lfd.nanxinkj.top

[U79] PHP：静态分析
来源：http://xzi.bbcook.cn

composer require --dev phpstan/phpstan
来源：http://cdu.vehdjk.com

[U80] PHP：代码规范修复
来源：http://vde.uphjek.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://gjr.sysykeji.top

[U81] JS：初始化项目
来源：http://xor.xziqi.cn

npm init -y;  npm i express
来源：http://mvq.havefunace.top

[U82] JS：package.json 脚本
来源：http://yex.fanxiaobao.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ggz.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://mnz.epnwcf.com

export const a = 1;  import { a } from "./m.js";
来源：http://qgm.hnxiangtu.top

[U84] JS：CommonJS 写法
来源：http://jxl.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://onb.316326.xyz

[U85] JS：可选链
来源：http://efg.haohaochexian.top

a?.b?.c
来源：http://tya.kuanghao11.cn

[U86] JS：空值合并
来源：http://kzf.c1oappe.top

a ?? b
来源：http://mha.gzhubu.top

[U87] JS：解构默认值
来源：http://vfq.ivvv.top

const { a = 1, b = 2 } = obj;
来源：http://cff.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://quj.yonumen.top

{ ...a, ...b }
来源：http://crx.snrcjt.cn

[U89] JS：数组去重
来源：http://mgc.jyoumei.cn

[...new Set(arr)]
来源：http://vas.shuidangran.top

[U90] JS：数字数组排序
来源：http://tta.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://kpr.9152youxi.cn

[U91] JS：对象键值遍历
来源：http://xqm.hfpthk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xwh.jiagoushi.top

[U92] JS：深拷贝
来源：http://eyz.hcnkem.com

structuredClone(obj)
来源：http://pdf.ivvv.top

[U93] JS：模板字符串
来源：http://zmb.sweek.top

`共 ${n} 条`
来源：http://gvp.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://hyw.xylfe.cn

const double = x => x * 2;
来源：http://bvc.hywenlv.cn

[U95] JS：Promise 包装
来源：http://atf.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://vqr.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://czl.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rcg.tarul.cn

[U97] JS：并发请求
来源：http://mwf.chenlongwang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://aun.haohaochexian.top

[U98] JS：fetch 带 JSON
来源：http://efl.uphjek.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://czn.zhoulong.xyz

[U99] JS：事件监听
来源：http://dpp.jinqigfzy.top

el.addEventListener("click", e => {})
来源：http://hah.wangdashe.top

[U100] JS：DOM 查询
来源：http://dgo.yonumen.top

document.querySelector(".item")
来源：http://knr.epnwcf.com

[U101] JS：classList 操作
来源：http://yka.yueranfly.top

el.classList.toggle("active")
来源：http://bnr.9152youxi.cn

[U102] JS：本地存储
来源：http://law.fktsv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lpu.svipenyu.cn

[U103] JS：定时器
来源：http://sox.hywenlv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://idu.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://fgh.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kdl.jianghu66.top

[U105] JS：节流
来源：http://hig.tianlin.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ncu.yueranfly.top

[U106] JS：日期格式化
来源：http://iof.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ube.wangdashe.top

[U107] JS：数字千分位
来源：http://ziq.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://efy.guowangkeji.top

[U108] JS：随机整数
来源：http://jnw.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://shd.jianghu66.top

[U109] JS：数组分组
来源：http://zja.hysaishi.cn

Object.groupBy(arr, x => x.type)
来源：http://feq.jqgufenzy.top

[U110] JS：数组分块
来源：http://gzf.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yrx.vehdjk.com

[U111] JS：对象转 Map
来源：http://ahy.ydzc1.top

new Map(Object.entries(obj))
来源：http://ail.yuxming.cn

[U112] JS：字符串补位
来源：http://iuc.aizwys.cn

"7".padStart(3, "0")
来源：http://fho.cdnleiting.top

[U113] JS：正则替换全部
来源：http://pfp.hongshengwenyu.top

s.replaceAll("a", "b")
来源：http://ktt.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://kir.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rqi.52xcode.cn

[U115] JS：生成 UUID
来源：http://efa.birdmap.top

crypto.randomUUID()
来源：http://kyr.uphjek.com

[U116] JS：类型检查（JSDoc）
来源：http://ffu.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://bmk.kuanghao11.cn

[U117] JS：单元测试
来源：http://yhi.yj20258.top

npm i -D vitest;  npx vitest
来源：http://zbb.bbcook.cn

[U118] JS：开发服务器
来源：http://zrb.guowangkeji.top

npm i -D vite;  npx vite
来源：http://lip.kuanghao11.cn

[U119] JS：生产构建
来源：http://cps.daxiang520.top

npx vite build
来源：http://piv.xylfe.cn

[U120] JS：读取环境变量（Vite）
来源：http://wco.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://wcc.aizwys.cn

================================================================================
来源：http://fax.ybcxt.top

统计汇总
来源：http://myj.jinqigfzy.top

================================================================================
来源：http://rxq.hnqzz.top

按语言统计（条）：
来源：http://qco.yj20258888.top

Python ......... 252
来源：http://hmk.ybcxt.top

PHP ............ 252
来源：http://aef.nanxuanxn.top

JavaScript ..... 252
来源：http://ktv.fktsv.cn

TypeScript ..... 212
来源：http://odn.feifeiyinyue.top

Java ........... 212
来源：http://btj.fehbvm.com

Go ............. 212
来源：http://stq.yangfankeji.com

Ruby ........... 212
来源：http://qmo.jinqigfzy.top

C# ............. 212
来源：http://pgl.yuxming.cn

C .............. 30
来源：http://csq.gaohongyu789.top

C++ ............ 30
来源：http://jzv.yfazqb.com

SQL ............ 90
来源：http://jro.hnqzz.top

Bash ........... 80
来源：http://aop.tanke756.top

Kotlin ......... 15
来源：http://wfz.316326.xyz

Swift .......... 15
来源：http://auo.0kj1m.cn

Lua ............ 10
来源：http://saj.sxryk.cn

Perl ........... 10
来源：http://qsw.jianghu66.top

Scala .......... 10
来源：http://pex.jinqigfzy.top

------------------------------------
来源：http://tst.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://ccx.yonumen.top

按章节统计：
来源：http://zxv.ydjk.org.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dtm.iojbl.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://usd.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ukk.wangshuangyany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kjy.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rhs.xuanzx.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rvf.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://olj.yongpay.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iqc.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ctd.gzhubu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sdu.cashguo.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wgz.zhijiandao.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yxp.mhx1999.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://phv.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kfb.svipenyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iqc.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tjw.shzxlz.cn

Q SQL 专题                              90
来源：http://dlj.aibaodan.cn

R Bash 专题                             80
来源：http://pmo.kuanghao11.cn

S C / C++ 专题                          60
来源：http://jds.hywenlv.cn

T 其他语言补充                          60
来源：http://eys.sufxvd.cn

U 高频实用片段                         120
来源：http://ueo.shangyingyoupin.top

------------------------------------
来源：http://ies.jinqigfzy.top

合计                                  2106 条
来源：http://gxq.fktsv.cn

--------------------------------------------------------------------------------
来源：http://dxu.gotoacloud.top

使用提醒
来源：http://kuk.shuidangran.top

--------------------------------------------------------------------------------
来源：http://dss.xylfe.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://arc.9152youxi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ohm.jinqigfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yzx.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dbv.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rqi.xziqi.cn

—— 文件结束 ——
来源：http://bgm.fzhhl.top

================================================================================
来源：http://dop.zdqjudy.top

程序语言常见例子速查手册（2024 版）
来源：http://mtp.bbcook.cn

Common Programming Examples Cheat Book
来源：http://smy.shuidangran.top

================================================================================
来源：http://itv.snrcjt.cn

【收录内容】
来源：http://aqb.jinyuanbaomall.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ngl.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ywl.yueranfly.top

SQL · Bash · C · C++
来源：http://cve.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kzt.hesvh.cn

【使用说明】
来源：http://vio.jinqigfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vow.0kj1m.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qwl.zhengqikj.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.yanxiufei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ojv.shuidangran.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wzt.zdqjudy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tlh.ydzc1.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qpu.ivvv.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jbt.zdbjq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ihc.tarul.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bjh.52xcode.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gjp.tarul.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wpw.svipenyu.cn

【文件统计】
来源：http://tqq.yongpay.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iqe.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://cej.epnwcf.com

目  录
来源：http://ctp.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://yju.jqgfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qll.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xma.daria6918.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://koq.zycfv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://swh.uphjek.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jhh.hysaishi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lee.fengsongda.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mof.yanxiufei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://siq.aibaodan.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zqm.jinqigfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jdw.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cgm.52xcode.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cne.haohaochexian.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ake.jqgufenzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xlz.hnqzz.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sex.yueranfly.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mbe.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ytf.havefunace.top


<!-- 参考信息 -->