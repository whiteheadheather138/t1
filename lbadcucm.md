代发 wailian999

[U23] Py：分块读取大文件
来源：http://fmx.ybcxt.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zpf.yanxiufei.cn

[U24] Py：路径操作
来源：http://xoz.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://koo.havefunace.top

[U25] Py：CSV 按字典读
来源：http://osx.jinghuilouyu.cn

csv.DictReader(f)
来源：http://bqj.316326.xyz

[U26] Py：并发下载
来源：http://glu.dashuyun.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sgt.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://res.haohaochexian.top

aiohttp.ClientSession() 配合 async with
来源：http://foz.ydjk.org.cn

[U28] Py：类型别名
来源：http://dew.jlsjyb.cn

UserId = int
来源：http://kyo.svipenyu.cn

[U29] Py：属性校验
来源：http://osg.zdbjq.cn

@property 与 @x.setter 配合
来源：http://bhi.dianchejie.cn

[U30] Py：数据类
来源：http://bsh.aibaodan.cn

@dataclass(slots=True)
来源：http://prk.wangdashe.top

[U31] Py：单测
来源：http://ykp.hfpthk.cn

python -m pytest -q
来源：http://hqf.hfpthk.cn

[U32] Py：代码格式化
来源：http://dkj.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://yja.yueranfly.top

[U33] Py：打包发布
来源：http://gdo.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://zuq.yonumen.top

[U34] Py：判断编码
来源：http://zxy.guannengcc.top

chardet.detect(raw)
来源：http://sjp.wangshuangyany.cn

[U35] Py：发送邮件
来源：http://ywv.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ryj.feifeiyinyue.top

[U36] Py：定时任务
来源：http://bqy.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://ydh.cqqwz.cn

[U37] Py：读写 Excel
来源：http://sct.kuanghao11.cn

pandas.read_excel / DataFrame.to_excel
来源：http://epf.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://oag.ydjk.org.cn

Path(__file__).resolve().parent
来源：http://ctc.hnxiangtu.top

[U39] Py：判断是否在交互环境
来源：http://cpx.xziqi.cn

sys.stdout.isatty()
来源：http://ccz.hammf.cn

[U40] Py：打印到标准错误
来源：http://wbx.yanxiufei.cn

print("err", file=sys.stderr)
来源：http://gpc.chenjidiqi.icu

[U41] PHP：初始化 Composer 项目
来源：http://tgl.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://miv.hongshengwenyu.top

[U42] PHP：PSR-4 自动加载
来源：http://yeo.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qxg.aizwys.cn

[U43] PHP：声明命名空间
来源：http://jgl.nwbrower.top

namespace App\Http;
来源：http://spn.ydzc1.top

[U44] PHP：开启严格类型
来源：http://uun.zhixingplan.top

declare(strict_types=1);
来源：http://kzk.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://pmu.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nuy.0kj1m.cn

[U46] PHP：可空类型
来源：http://pji.yuxming.cn

?string $name = null
来源：http://ind.cqqwz.cn

[U47] PHP：联合类型
来源：http://srp.hfpthk.cn

int|string $id
来源：http://azt.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://cvn.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dyz.zycfv.cn

[U49] PHP：只读属性
来源：http://mdt.hesvh.cn

public readonly string $name
来源：http://bal.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://xnw.haohaochexian.top

public function __construct(private int $id) {}
来源：http://nba.zycfv.cn

[U51] PHP：数组解构
来源：http://jhe.daxiang520.top

[$a, $b] = $arr;
来源：http://zra.yuanzhike.top

[U52] PHP：箭头函数
来源：http://btn.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://bks.pycfn.com

[U53] PHP：空合并运算符
来源：http://kch.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://iuz.aizwys.cn

[U54] PHP：空安全调用
来源：http://gue.havefunace.top

$obj?->method()
来源：http://kha.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://aiy.hesvh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fhd.dianchejie.cn

[U56] PHP：命名参数
来源：http://mif.bjfxy.top

f(a: 1, b: 2)
来源：http://fiv.ehwqpu.com

[U57] PHP：字符串插值
来源：http://hzx.hywenlv.cn

"值: {$a}"
来源：http://dak.tianlin.xyz

[U58] PHP：数组三件套
来源：http://ubc.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ufm.sysykeji.top

[U59] PHP：自定义排序
来源：http://cyk.hongshengwenyu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cps.316326.xyz

[U60] PHP：JSON 编解码
来源：http://cbu.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://und.tanke756.top

[U61] PHP：正则
来源：http://jcq.xuanzx.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wgx.zhiwuduotai.top

[U62] PHP：日期对象
来源：http://ley.yj20258.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fuk.bbcook.cn

[U63] PHP：文件读写
来源：http://wzi.zhixingplan.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jel.zhixingplan.top

[U64] PHP：目录遍历
来源：http://cdh.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://cjr.zhixingplan.top

[U65] PHP：会话
来源：http://nae.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dzj.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://min.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://upo.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://zpt.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zlf.xziqi.cn

[U68] PHP：PDO 连接
来源：http://rwd.hesvh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bte.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://hbv.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://myy.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://xqh.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lly.ctjpmb.com

[U71] PHP：抛出异常
来源：http://zxf.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://ejn.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://qtr.xylfe.cn

error_log("失败: " . $e->getMessage());
来源：http://nyo.andypj.xyz

[U73] PHP：读取 ini 配置
来源：http://dlu.xuanzx.com

parse_ini_file("config.ini", true)
来源：http://frz.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://zyj.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://jwf.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://tbn.xylfe.cn

composer require psr/container
来源：http://sfu.andypj.xyz

[U76] PHP：简单路由
来源：http://lvn.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hhl.tianlin.xyz

[U77] PHP：模板渲染
来源：http://den.jqgfzy.top

composer require twig/twig
来源：http://sau.nanxinkj.top

[U78] PHP：单元测试
来源：http://uqh.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://etq.zhixingplan.top

[U79] PHP：静态分析
来源：http://ftu.svipenyu.cn

composer require --dev phpstan/phpstan
来源：http://chw.shanyushiyangtech.top

[U80] PHP：代码规范修复
来源：http://mav.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://iur.guannengcc.top

[U81] JS：初始化项目
来源：http://hyt.yj20258888.top

npm init -y;  npm i express
来源：http://fbz.chenlongwang.top

[U82] JS：package.json 脚本
来源：http://suy.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fot.daxiang520.top

[U83] JS：ES Module 导入导出
来源：http://cjb.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://snm.xylfe.cn

[U84] JS：CommonJS 写法
来源：http://ujx.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://pdr.cheryme.top

[U85] JS：可选链
来源：http://qzt.chenjidiqi.icu

a?.b?.c
来源：http://ook.dashuyun.cn

[U86] JS：空值合并
来源：http://npp.yj20258.top

a ?? b
来源：http://xye.zycfv.cn

[U87] JS：解构默认值
来源：http://ssk.cdnleiting.top

const { a = 1, b = 2 } = obj;
来源：http://qrn.xziqi.cn

[U88] JS：对象展开合并
来源：http://vfq.xuanzx.com

{ ...a, ...b }
来源：http://ghy.svipenyu.cn

[U89] JS：数组去重
来源：http://hwq.tanke756.top

[...new Set(arr)]
来源：http://bbh.jlsjyb.cn

[U90] JS：数字数组排序
来源：http://kmh.gogol.net.cn

[...arr].sort((a, b) => a - b)
来源：http://mfz.nwbrower.top

[U91] JS：对象键值遍历
来源：http://wuf.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hxx.jyoumei.cn

[U92] JS：深拷贝
来源：http://ecc.yonumen.top

structuredClone(obj)
来源：http://aoa.chenzaomai.com

[U93] JS：模板字符串
来源：http://gqc.shuidangran.top

`共 ${n} 条`
来源：http://mmv.9152youxi.cn

[U94] JS：箭头函数
来源：http://sfe.yuanzhike.top

const double = x => x * 2;
来源：http://zji.birdmap.top

[U95] JS：Promise 包装
来源：http://rkf.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://fri.sxryk.cn

[U96] JS：async/await 与异常
来源：http://jzy.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nim.gzhubu.top

[U97] JS：并发请求
来源：http://szn.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://pmz.yfazqb.com

[U98] JS：fetch 带 JSON
来源：http://yds.yj20258888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zea.fktsv.cn

[U99] JS：事件监听
来源：http://rna.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://kan.hnxiangtu.top

[U100] JS：DOM 查询
来源：http://tsf.gogol.net.cn

document.querySelector(".item")
来源：http://afm.jlsjyb.cn

[U101] JS：classList 操作
来源：http://iec.chenjidiqi.icu

el.classList.toggle("active")
来源：http://nps.mhx1999.top

[U102] JS：本地存储
来源：http://fyr.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://myn.zhixingplan.top

[U103] JS：定时器
来源：http://mqh.pengpengdd.cyou

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jen.iojbl.cn

[U104] JS：防抖
来源：http://dse.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pux.316326.xyz

[U105] JS：节流
来源：http://wbk.jiagoushi.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wey.zhixingplan.top

[U106] JS：日期格式化
来源：http://tij.bjfxy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kqz.tarul.cn

[U107] JS：数字千分位
来源：http://rnf.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ngo.hcnkem.com

[U108] JS：随机整数
来源：http://ilp.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bbj.sxryk.cn

[U109] JS：数组分组
来源：http://dcz.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://zld.shuidangran.top

[U110] JS：数组分块
来源：http://lil.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rcc.316326.xyz

[U111] JS：对象转 Map
来源：http://xqk.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://thv.redwolf501.top

[U112] JS：字符串补位
来源：http://hny.bbcook.cn

"7".padStart(3, "0")
来源：http://raz.0kj1m.cn

[U113] JS：正则替换全部
来源：http://wwo.hcnkem.com

s.replaceAll("a", "b")
来源：http://bqe.sxryk.cn

[U114] JS：JSON 深比较
来源：http://tuv.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lvy.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://wfw.smart0.xyz

crypto.randomUUID()
来源：http://jsu.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://mxl.vehdjk.com

/** @param {string} name */ function f(name) {}
来源：http://pjc.hcnkem.com

[U117] JS：单元测试
来源：http://wvy.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://rnx.dianchejie.cn

[U118] JS：开发服务器
来源：http://oit.zdbjq.cn

npm i -D vite;  npx vite
来源：http://wwj.sysykeji.top

[U119] JS：生产构建
来源：http://tlk.fzhhl.top

npx vite build
来源：http://evb.bjfxy.top

[U120] JS：读取环境变量（Vite）
来源：http://fgw.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://pbi.snrcjt.cn

================================================================================
来源：http://kfk.birdmap.top

统计汇总
来源：http://bgw.yanxiufei.cn

================================================================================
来源：http://pav.jinghuilouyu.cn

按语言统计（条）：
来源：http://kbg.vehdjk.com

Python ......... 252
来源：http://pdh.fzhhl.top

PHP ............ 252
来源：http://gya.xuetiantiany.cn

JavaScript ..... 252
来源：http://dkt.quarkkingdee.top

TypeScript ..... 212
来源：http://kue.uphjek.com

Java ........... 212
来源：http://aiv.cucudq.cn

Go ............. 212
来源：http://vhy.shangyingyoupin.top

Ruby ........... 212
来源：http://net.bbcook.cn

C# ............. 212
来源：http://mfe.fzhhl.top

C .............. 30
来源：http://cnv.shuidangran.top

C++ ............ 30
来源：http://rwn.ivvv.top

SQL ............ 90
来源：http://coz.nanxinkj.top

Bash ........... 80
来源：http://ply.yfazqb.com

Kotlin ......... 15
来源：http://wnq.meibo888.top

Swift .......... 15
来源：http://lhu.zhiwuduotai.top

Lua ............ 10
来源：http://bkf.aibaodan.cn

Perl ........... 10
来源：http://ilb.hnxiangtu.top

Scala .......... 10
来源：http://efm.chenlongwang.top

------------------------------------
来源：http://rwd.0kj1m.cn

合计 ........... 2106 条
来源：http://scr.c1oappe.top

按章节统计：
来源：http://cox.xuanzx.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wkh.dianchejie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kej.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hdz.jiagoushi.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nkr.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tro.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pdc.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nyr.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yig.hywenlv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tuq.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fkk.yanxiufei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bkc.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dyu.hnqzz.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mzz.cdnleiting.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vbj.haohaochexian.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dlq.feifeiyinyue.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lin.redwolf501.top

Q SQL 专题                              90
来源：http://cca.shuidangran.top

R Bash 专题                             80
来源：http://fbi.quarkkingdee.top

S C / C++ 专题                          60
来源：http://jfo.shanyushiyangtech.top

T 其他语言补充                          60
来源：http://ish.yanxiufei.cn

U 高频实用片段                         120
来源：http://qad.jlsjyb.cn

------------------------------------
来源：http://sag.hysaishi.cn

合计                                  2106 条
来源：http://zvu.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://hnr.gotoacloud.top

使用提醒
来源：http://rgl.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://nhx.ydjk.org.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cef.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://urg.smart0.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wce.dashuyun.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mjl.kuanghao11.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aln.cdnleiting.top

—— 文件结束 ——
来源：http://jyq.yfazqb.com

================================================================================
来源：http://bws.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://qqa.yanxiufei.cn

Common Programming Examples Cheat Book
来源：http://olv.c1oappe.top

================================================================================
来源：http://spc.jqgufenzy.top

【收录内容】
来源：http://uvx.yongpay.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tuv.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ngz.iojbl.cn

SQL · Bash · C · C++
来源：http://cke.snrcjt.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mvq.52xcode.cn

【使用说明】
来源：http://cjz.yongpay.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rxi.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oed.hcnkem.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://frr.ehwqpu.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uso.hfpthk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ytn.chenjidiqi.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jaq.bjfxy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cqy.bjfxy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qnp.sufxvd.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gtm.shangyingyoupin.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uzj.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://viz.feifeiyinyue.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pvc.nanxinkj.top

【文件统计】
来源：http://xdy.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xvt.nwbrower.top

--------------------------------------------------------------------------------
来源：http://niz.zhiwuduotai.top

目  录
来源：http://heo.vehdjk.com

--------------------------------------------------------------------------------
来源：http://gil.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://knw.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wgi.vehdjk.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lwj.wangshuangyany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tls.vehdjk.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lzd.dianchejie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ygf.feifeiyinyue.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kfc.dashuyun.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qrb.tanke756.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://evp.tarul.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fsx.meibo888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hkn.haohaochexian.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fbw.hongshengwenyu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xxa.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mlm.fengsongda.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eoz.zhoulong.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kev.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oef.zhaomingkeji.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://yqk.hongshengwenyu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tfz.nanxuanxn.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fpq.fzhhl.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://abj.bjfxy.top


<!-- 参考信息 -->