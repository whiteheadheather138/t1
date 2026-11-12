代发 wailian999

[U19] Py：正则替换带回调
来源：http://bqa.dianchejie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://owv.gotoacloud.top

[U20] Py：缓存函数结果
来源：http://nng.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://nnu.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://tkc.xuetiantiany.cn

@contextlib.contextmanager
来源：http://xjn.cucudq.cn

[U22] Py：矩阵转置
来源：http://xhs.nanxuanxn.top

list(zip(*m))
来源：http://yid.52xcode.cn

[U23] Py：分块读取大文件
来源：http://cce.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jyu.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://jav.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tvm.fktsv.cn

[U25] Py：CSV 按字典读
来源：http://yux.yj20258888.top

csv.DictReader(f)
来源：http://fkz.andypj.xyz

[U26] Py：并发下载
来源：http://jlm.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qfw.uphjek.com

[U27] Py：异步 HTTP
来源：http://jug.cqqwz.cn

aiohttp.ClientSession() 配合 async with
来源：http://cah.hesvh.cn

[U28] Py：类型别名
来源：http://ldz.jqgfzy.top

UserId = int
来源：http://tzg.c1oappe.top

[U29] Py：属性校验
来源：http://blw.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://dug.zhengqikj.top

[U30] Py：数据类
来源：http://tjo.guannengcc.top

@dataclass(slots=True)
来源：http://suc.ctjpmb.com

[U31] Py：单测
来源：http://kfk.guowangkeji.top

python -m pytest -q
来源：http://fsb.gogol.net.cn

[U32] Py：代码格式化
来源：http://vei.hongshengwenyu.top

ruff format . && ruff check --fix .
来源：http://voy.chenjidiqi.icu

[U33] Py：打包发布
来源：http://nwm.jqgufenzy.top

python -m build  （依赖 pyproject.toml）
来源：http://ytw.zdqjudy.top

[U34] Py：判断编码
来源：http://sjy.cdnleiting.top

chardet.detect(raw)
来源：http://nik.havefunace.top

[U35] Py：发送邮件
来源：http://bxt.sxryk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oin.mhx1999.top

[U36] Py：定时任务
来源：http://kem.cucudq.cn

schedule.every(10).minutes.do(job)
来源：http://ufp.hesvh.cn

[U37] Py：读写 Excel
来源：http://fjt.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://koe.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://uaz.iojbl.cn

Path(__file__).resolve().parent
来源：http://qiq.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://wif.ydjk.org.cn

sys.stdout.isatty()
来源：http://zbd.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://dvs.sweek.top

print("err", file=sys.stderr)
来源：http://fsa.gzhubu.top

[U41] PHP：初始化 Composer 项目
来源：http://pcz.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gjh.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://jea.jyoumei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://trc.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://xkn.ydjk.org.cn

namespace App\Http;
来源：http://oys.fzhhl.top

[U44] PHP：开启严格类型
来源：http://rsl.zycfv.cn

declare(strict_types=1);
来源：http://daw.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://fdv.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nuv.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://isy.jiagoushi.top

?string $name = null
来源：http://mlh.zhijiandao.cn

[U47] PHP：联合类型
来源：http://opl.iojbl.cn

int|string $id
来源：http://erc.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://egm.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ywf.hongshengwenyu.top

[U49] PHP：只读属性
来源：http://dal.cashguo.top

public readonly string $name
来源：http://vhr.jlsjyb.cn

[U50] PHP：构造器属性提升
来源：http://vjo.uphjek.com

public function __construct(private int $id) {}
来源：http://wvh.ydzc1.top

[U51] PHP：数组解构
来源：http://xiy.52xcode.cn

[$a, $b] = $arr;
来源：http://ugu.chenzaomai.com

[U52] PHP：箭头函数
来源：http://unp.316326.xyz

$double = fn($x) => $x * 2;
来源：http://iub.sweek.top

[U53] PHP：空合并运算符
来源：http://rne.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://pts.haohaochexian.top

[U54] PHP：空安全调用
来源：http://cvq.tianlin.xyz

$obj?->method()
来源：http://guy.smart0.xyz

[U55] PHP：match 表达式
来源：http://tak.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nxf.jlsjyb.cn

[U56] PHP：命名参数
来源：http://xyv.snrcjt.cn

f(a: 1, b: 2)
来源：http://wrp.52xcode.cn

[U57] PHP：字符串插值
来源：http://kcw.shzxlz.cn

"值: {$a}"
来源：http://hrg.xinyue.icu

[U58] PHP：数组三件套
来源：http://eyh.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hyz.uphjek.com

[U59] PHP：自定义排序
来源：http://mkz.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ipa.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://cem.dashuyun.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zqn.yangfankeji.com

[U61] PHP：正则
来源：http://gcj.xziqi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mpd.nanxinkj.top

[U62] PHP：日期对象
来源：http://lcx.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bps.chenlongwang.top

[U63] PHP：文件读写
来源：http://qug.bjfxy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cap.ybcxt.top

[U64] PHP：目录遍历
来源：http://moc.sysykeji.top

glob("dir/*.php");  scandir("dir");
来源：http://eqw.9152youxi.cn

[U65] PHP：会话
来源：http://gxg.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yto.kuanghao11.cn

[U66] PHP：设置 Cookie
来源：http://gzv.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rvq.aizwys.cn

[U67] PHP：处理文件上传
来源：http://pjq.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wkf.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://byv.snrcjt.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nay.zhengqikj.top

[U69] PHP：PDO 预处理
来源：http://rvh.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gif.jyoumei.cn

[U70] PHP：PDO 事务
来源：http://qrz.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://umm.nwbrower.top

[U71] PHP：抛出异常
来源：http://onc.jqgufenzy.top

throw new RuntimeException("失败", 500);
来源：http://bgb.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://kss.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://psk.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://yrr.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://grl.kuanghao11.cn

[U74] PHP：读取环境变量
来源：http://hhy.smart0.xyz

getenv("APP_ENV") ?: "production"
来源：http://ewt.xylfe.cn

[U75] PHP：依赖注入
来源：http://jvx.9152youxi.cn

composer require psr/container
来源：http://xvo.9152youxi.cn

[U76] PHP：简单路由
来源：http://dfv.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vkx.hcnkem.com

[U77] PHP：模板渲染
来源：http://ceq.zhixingplan.top

composer require twig/twig
来源：http://ttk.zdbjq.cn

[U78] PHP：单元测试
来源：http://awv.jiagoushi.top

composer require --dev phpunit/phpunit
来源：http://xpl.nanxinkj.top

[U79] PHP：静态分析
来源：http://hfj.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://krw.zhengqikj.top

[U80] PHP：代码规范修复
来源：http://sfl.hesvh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dly.fzhhl.top

[U81] JS：初始化项目
来源：http://fsd.xylfe.cn

npm init -y;  npm i express
来源：http://ufp.nanxuanxn.top

[U82] JS：package.json 脚本
来源：http://ldw.yongpay.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ulm.dashuyun.cn

[U83] JS：ES Module 导入导出
来源：http://ruw.shuidangran.top

export const a = 1;  import { a } from "./m.js";
来源：http://blf.sysykeji.top

[U84] JS：CommonJS 写法
来源：http://khu.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://hms.hywenlv.cn

[U85] JS：可选链
来源：http://hvr.fengsongda.top

a?.b?.c
来源：http://cvt.shuidangran.top

[U86] JS：空值合并
来源：http://tgp.zycfv.cn

a ?? b
来源：http://lxy.jqgfzy.top

[U87] JS：解构默认值
来源：http://kyq.ppjwa.cn

const { a = 1, b = 2 } = obj;
来源：http://krq.cqqwz.cn

[U88] JS：对象展开合并
来源：http://aqd.shangyingyoupin.top

{ ...a, ...b }
来源：http://hhx.shanyushiyangtech.top

[U89] JS：数组去重
来源：http://xqa.tian-w.cn

[...new Set(arr)]
来源：http://uqp.nwbrower.top

[U90] JS：数字数组排序
来源：http://yvg.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://cnq.gzhubu.top

[U91] JS：对象键值遍历
来源：http://trm.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lno.daria6918.cn

[U92] JS：深拷贝
来源：http://zih.snrcjt.cn

structuredClone(obj)
来源：http://odd.epnwcf.com

[U93] JS：模板字符串
来源：http://ryv.hysaishi.cn

`共 ${n} 条`
来源：http://enm.sjlbkw.cn

[U94] JS：箭头函数
来源：http://dsf.cqqwz.cn

const double = x => x * 2;
来源：http://tpu.shanyushiyangkeji.top

[U95] JS：Promise 包装
来源：http://zjn.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://mrz.9152youxi.cn

[U96] JS：async/await 与异常
来源：http://rwp.tian-w.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cbh.jinyuanbaomall.cn

[U97] JS：并发请求
来源：http://ymq.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bhj.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://cgy.zhongyouzk.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://loa.gaohongyu789.top

[U99] JS：事件监听
来源：http://jeg.ivvv.top

el.addEventListener("click", e => {})
来源：http://gkn.guannengcc.top

[U100] JS：DOM 查询
来源：http://dip.smart0.xyz

document.querySelector(".item")
来源：http://sen.jyoumei.cn

[U101] JS：classList 操作
来源：http://lku.gogol.net.cn

el.classList.toggle("active")
来源：http://pzd.fengsongda.top

[U102] JS：本地存储
来源：http://mad.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vjk.wangdashe.top

[U103] JS：定时器
来源：http://rcs.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qmv.yvedp.cn

[U104] JS：防抖
来源：http://fko.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iuk.hcnkem.com

[U105] JS：节流
来源：http://dxj.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://efh.xingfuxueyuan.xyz

[U106] JS：日期格式化
来源：http://goo.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oui.ydjk.org.cn

[U107] JS：数字千分位
来源：http://obh.wangshuangyany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ads.zhaomingkeji.xyz

[U108] JS：随机整数
来源：http://ixf.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kgx.cheryme.top

[U109] JS：数组分组
来源：http://ilu.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://ylg.pycfn.com

[U110] JS：数组分块
来源：http://lqj.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aaw.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://uvj.meibo888.top

new Map(Object.entries(obj))
来源：http://ouh.sysykeji.top

[U112] JS：字符串补位
来源：http://jqw.sweek.top

"7".padStart(3, "0")
来源：http://rjz.hywenlv.cn

[U113] JS：正则替换全部
来源：http://phd.ydzc1.top

s.replaceAll("a", "b")
来源：http://wtq.xinyue.icu

[U114] JS：JSON 深比较
来源：http://vgo.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qiv.pengpengdd.cyou

[U115] JS：生成 UUID
来源：http://qqd.jinghuilouyu.cn

crypto.randomUUID()
来源：http://vbd.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://phs.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://tcp.fanxiaobao.xyz

[U117] JS：单元测试
来源：http://zrn.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://dcx.cdnleiting.top

[U118] JS：开发服务器
来源：http://zhd.dianchejie.cn

npm i -D vite;  npx vite
来源：http://kgj.hywenlv.cn

[U119] JS：生产构建
来源：http://lxc.xuanzx.com

npx vite build
来源：http://rxi.fehbvm.com

[U120] JS：读取环境变量（Vite）
来源：http://uof.xuetiantiany.cn

import.meta.env.VITE_API_URL
来源：http://nmx.fktsv.cn

================================================================================
来源：http://ibf.yuanzhike.top

统计汇总
来源：http://she.sjlbkw.cn

================================================================================
来源：http://lmu.zdbjq.cn

按语言统计（条）：
来源：http://oox.yvedp.cn

Python ......... 252
来源：http://nbz.daria6918.cn

PHP ............ 252
来源：http://sym.daxiang520.top

JavaScript ..... 252
来源：http://dlc.tianlin.xyz

TypeScript ..... 212
来源：http://ojk.ivvv.top

Java ........... 212
来源：http://yba.yueranfly.top

Go ............. 212
来源：http://nqu.jlsjyb.cn

Ruby ........... 212
来源：http://fau.ctjpmb.com

C# ............. 212
来源：http://vey.vqdsnc.cn

C .............. 30
来源：http://rgt.jiagoushi.top

C++ ............ 30
来源：http://xkg.fzhhl.top

SQL ............ 90
来源：http://nka.snrcjt.cn

Bash ........... 80
来源：http://xfg.mhx1999.top

Kotlin ......... 15
来源：http://tsr.jinyuanbaomall.cn

Swift .......... 15
来源：http://exn.daxiang520.top

Lua ............ 10
来源：http://erj.xuetiantiany.cn

Perl ........... 10
来源：http://txr.quarkkingdee.top

Scala .......... 10
来源：http://oab.gotoacloud.top

------------------------------------
来源：http://sly.snrcjt.cn

合计 ........... 2106 条
来源：http://zam.cashguo.top

按章节统计：
来源：http://tzw.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vkk.ctjpmb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jqf.316326.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jtb.hnqzz.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nig.fzhhl.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rcg.xylfe.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uio.meibo888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://osv.yj20258888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rha.hfpthk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bpp.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dql.yj20258888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bfr.nwbrower.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://enm.hongshengwenyu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wgg.jinqigufen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tim.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lfd.shzxlz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hwa.jyoumei.cn

Q SQL 专题                              90
来源：http://xqw.yuxming.cn

R Bash 专题                             80
来源：http://ksm.kuanghao11.cn

S C / C++ 专题                          60
来源：http://nis.feifeiyinyue.top

T 其他语言补充                          60
来源：http://hvz.hammf.cn

U 高频实用片段                         120
来源：http://xzq.uphjek.com

------------------------------------
来源：http://bis.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://juv.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://bgy.cdnleiting.top

使用提醒
来源：http://wtj.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://bpe.yj202588.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rlp.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xgf.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ttb.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://epj.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cnz.cdnleiting.top

—— 文件结束 ——
来源：http://boh.ivvv.top

================================================================================
来源：http://ail.fzhhl.top

程序语言常见例子速查手册（2024 版）
来源：http://rbl.havefunace.top

Common Programming Examples Cheat Book
来源：http://ejs.wangshuangyany.cn

================================================================================
来源：http://zwz.gogol.net.cn

【收录内容】
来源：http://wpt.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vnj.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://olf.gzhubu.top

SQL · Bash · C · C++
来源：http://cgp.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tsv.ctjpmb.com

【使用说明】
来源：http://lxv.smart0.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dnv.meibo888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mfg.tianlin.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://erz.xingfuxueyuan.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://clh.sxryk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ksk.ivvv.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xji.bjfxy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iuk.sjlbkw.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://foy.kuanghao11.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ztg.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lit.yanxiufei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pvd.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ytc.vqdsnc.cn

【文件统计】
来源：http://fyi.xingfuxueyuan.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vwj.aizwys.cn

--------------------------------------------------------------------------------
来源：http://esz.jlsjyb.cn

目  录
来源：http://tlt.havefunace.top

--------------------------------------------------------------------------------
来源：http://ark.hammf.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vdg.hywenlv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ksa.hnqzz.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uas.ivvv.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dwf.ydjk.org.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uwe.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://anx.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ynu.smart0.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pqa.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://foy.fzhhl.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://txd.yueranfly.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cak.xziqi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bya.iojbl.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vzh.cqqwz.cn


<!-- 参考信息 -->