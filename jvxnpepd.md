代发 wailian999

[U13] Py：固定长度队列
来源：http://hco.dianchejie.cn

deque(maxlen=10)
来源：http://vwk.cheryme.top

[U14] Py：分组收集到列表
来源：http://dvt.fengsongda.top

defaultdict(list)
来源：http://zbo.fzhhl.top

[U15] Py：高精度计时
来源：http://vna.shanyushiyangtech.top

t = time.perf_counter()
来源：http://iuz.hcnkem.com

[U16] Py：命令行参数解析
来源：http://iew.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://njj.jqgufenzy.top

[U17] Py：初始化日志
来源：http://bni.shangyingyoupin.top

logging.basicConfig(level=logging.INFO)
来源：http://boo.zhiwuduotai.top

[U18] Py：预编译正则
来源：http://fsu.hfpthk.cn

pat = re.compile(r"\d+")
来源：http://sol.hnqzz.top

[U19] Py：正则替换带回调
来源：http://oge.chenlongwang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mii.sxryk.cn

[U20] Py：缓存函数结果
来源：http://kvu.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://vld.yj20258.top

[U21] Py：自定义上下文管理器
来源：http://ecj.xuetiantiany.cn

@contextlib.contextmanager
来源：http://rrm.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://flg.c1oappe.top

list(zip(*m))
来源：http://zfq.fktsv.cn

[U23] Py：分块读取大文件
来源：http://xgp.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://grv.ppjwa.cn

[U24] Py：路径操作
来源：http://fbd.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hxu.ydjk.org.cn

[U25] Py：CSV 按字典读
来源：http://jvv.yuanzhike.top

csv.DictReader(f)
来源：http://rrl.fzhhl.top

[U26] Py：并发下载
来源：http://axf.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ehp.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://jkh.0kj1m.cn

aiohttp.ClientSession() 配合 async with
来源：http://idx.svipenyu.cn

[U28] Py：类型别名
来源：http://ukr.tarul.cn

UserId = int
来源：http://lvf.yuanzhike.top

[U29] Py：属性校验
来源：http://dem.52xcode.cn

@property 与 @x.setter 配合
来源：http://lzj.pengpengdd.cyou

[U30] Py：数据类
来源：http://epp.daxiang520.top

@dataclass(slots=True)
来源：http://exs.shanyushiyangtech.top

[U31] Py：单测
来源：http://nzu.fehbvm.com

python -m pytest -q
来源：http://fvg.yonumen.top

[U32] Py：代码格式化
来源：http://xwy.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://nia.c1oappe.top

[U33] Py：打包发布
来源：http://ndb.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://gbu.ybcxt.top

[U34] Py：判断编码
来源：http://hgi.kuanghao11.cn

chardet.detect(raw)
来源：http://wdi.jlsjyb.cn

[U35] Py：发送邮件
来源：http://vlv.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tbs.jiagoushi.top

[U36] Py：定时任务
来源：http://thj.tian-w.cn

schedule.every(10).minutes.do(job)
来源：http://abn.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://wwl.chenzaomai.com

pandas.read_excel / DataFrame.to_excel
来源：http://ils.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://sbf.dianchejie.cn

Path(__file__).resolve().parent
来源：http://ldx.hfpthk.cn

[U39] Py：判断是否在交互环境
来源：http://egu.ehwqpu.com

sys.stdout.isatty()
来源：http://jjm.ctjpmb.com

[U40] Py：打印到标准错误
来源：http://hvv.daria6918.cn

print("err", file=sys.stderr)
来源：http://kmw.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://wkh.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://wmf.jlsjyb.cn

[U42] PHP：PSR-4 自动加载
来源：http://gxr.zdqjudy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wzn.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://bbi.hnqzz.top

namespace App\Http;
来源：http://dwr.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://agk.gaohongyu789.top

declare(strict_types=1);
来源：http://vxv.ivvv.top

[U45] PHP：类型声明与返回类型
来源：http://fvz.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fiz.sufxvd.cn

[U46] PHP：可空类型
来源：http://mut.tarul.cn

?string $name = null
来源：http://ktu.cashguo.top

[U47] PHP：联合类型
来源：http://wyg.daxiang520.top

int|string $id
来源：http://qrv.jinyuanbaomall.cn

[U48] PHP：纯枚举
来源：http://mac.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wqm.dianchejie.cn

[U49] PHP：只读属性
来源：http://tht.tarul.cn

public readonly string $name
来源：http://rlv.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://wvb.zhixingplan.top

public function __construct(private int $id) {}
来源：http://gfo.ctjpmb.com

[U51] PHP：数组解构
来源：http://iab.zhijiandao.cn

[$a, $b] = $arr;
来源：http://nbh.cqqwz.cn

[U52] PHP：箭头函数
来源：http://zfn.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://xgf.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://bfs.hfpthk.cn

$v = $a ?? $b ?? "default";
来源：http://zjd.xingfuxueyuan.xyz

[U54] PHP：空安全调用
来源：http://txy.gogol.net.cn

$obj?->method()
来源：http://ooj.havefunace.top

[U55] PHP：match 表达式
来源：http://gpn.zhixingplan.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://csi.snrcjt.cn

[U56] PHP：命名参数
来源：http://epi.chenlongwang.top

f(a: 1, b: 2)
来源：http://tkx.cucudq.cn

[U57] PHP：字符串插值
来源：http://xgw.zhixingplan.top

"值: {$a}"
来源：http://icv.zycfv.cn

[U58] PHP：数组三件套
来源：http://yob.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tkl.dianchejie.cn

[U59] PHP：自定义排序
来源：http://iwo.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cwg.chenjidiqi.icu

[U60] PHP：JSON 编解码
来源：http://fld.hfpthk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://loc.ydjk.org.cn

[U61] PHP：正则
来源：http://pri.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qay.ydzc1.top

[U62] PHP：日期对象
来源：http://srf.hcnkem.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nxn.hnxiangtu.top

[U63] PHP：文件读写
来源：http://okw.zhijiandao.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://csp.xingfuxueyuan.xyz

[U64] PHP：目录遍历
来源：http://dhc.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://jjg.tian-w.cn

[U65] PHP：会话
来源：http://fnt.yueranfly.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xxw.ivvv.top

[U66] PHP：设置 Cookie
来源：http://nmr.tian-w.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dwm.sweek.top

[U67] PHP：处理文件上传
来源：http://bww.ydzc1.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eqa.shzxlz.cn

[U68] PHP：PDO 连接
来源：http://oen.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ymi.hammf.cn

[U69] PHP：PDO 预处理
来源：http://zdr.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uup.fzhhl.top

[U70] PHP：PDO 事务
来源：http://nhe.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eum.shanyushiyangtech.top

[U71] PHP：抛出异常
来源：http://bsf.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://isn.jinyuanbaomall.cn

[U72] PHP：写错误日志
来源：http://zpi.yvedp.cn

error_log("失败: " . $e->getMessage());
来源：http://uiw.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://sjn.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://tej.sxryk.cn

[U74] PHP：读取环境变量
来源：http://dgm.sxryk.cn

getenv("APP_ENV") ?: "production"
来源：http://tuk.nanxinkj.top

[U75] PHP：依赖注入
来源：http://clu.vehdjk.com

composer require psr/container
来源：http://oph.hesvh.cn

[U76] PHP：简单路由
来源：http://nqz.ppjwa.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ids.ctjpmb.com

[U77] PHP：模板渲染
来源：http://uha.yfazqb.com

composer require twig/twig
来源：http://tbf.sufxvd.cn

[U78] PHP：单元测试
来源：http://odr.jqgufenzy.top

composer require --dev phpunit/phpunit
来源：http://rkz.gaohongyu789.top

[U79] PHP：静态分析
来源：http://oju.hnxiangtu.top

composer require --dev phpstan/phpstan
来源：http://ext.yfazqb.com

[U80] PHP：代码规范修复
来源：http://dlp.vehdjk.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://awa.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://bcb.tian-w.cn

npm init -y;  npm i express
来源：http://bag.wangshuangyany.cn

[U82] JS：package.json 脚本
来源：http://auu.jinyuanbaomall.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jzv.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://gjz.hnqzz.top

export const a = 1;  import { a } from "./m.js";
来源：http://ztk.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://cxp.sysykeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://oqs.zhongyouzk.top

[U85] JS：可选链
来源：http://vdf.fanxiaobao.xyz

a?.b?.c
来源：http://oxi.chenjidiqi.icu

[U86] JS：空值合并
来源：http://ere.jqgufenzy.top

a ?? b
来源：http://fmo.ydjk.org.cn

[U87] JS：解构默认值
来源：http://kte.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://lnr.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://kkt.iojbl.cn

{ ...a, ...b }
来源：http://yrz.jinqigfzy.top

[U89] JS：数组去重
来源：http://lid.havefunace.top

[...new Set(arr)]
来源：http://qlc.nwbrower.top

[U90] JS：数字数组排序
来源：http://xsi.xuetiantiany.cn

[...arr].sort((a, b) => a - b)
来源：http://xtm.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://qeo.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wit.hywenlv.cn

[U92] JS：深拷贝
来源：http://zcs.ydzc1.top

structuredClone(obj)
来源：http://zsp.ybcxt.top

[U93] JS：模板字符串
来源：http://rtu.gogol.net.cn

`共 ${n} 条`
来源：http://uol.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://lpc.sjlbkw.cn

const double = x => x * 2;
来源：http://jxy.tian-w.cn

[U95] JS：Promise 包装
来源：http://lqv.nwbrower.top

new Promise((resolve, reject) => {})
来源：http://ahn.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://wig.hfpthk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mcc.shzxlz.cn

[U97] JS：并发请求
来源：http://psc.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gaz.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://qjz.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jin.hnqzz.top

[U99] JS：事件监听
来源：http://jok.tianlin.xyz

el.addEventListener("click", e => {})
来源：http://unq.yongpay.top

[U100] JS：DOM 查询
来源：http://nou.c1oappe.top

document.querySelector(".item")
来源：http://xnq.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://pzc.sxryk.cn

el.classList.toggle("active")
来源：http://iur.hywenlv.cn

[U102] JS：本地存储
来源：http://wrs.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xnc.gotoacloud.top

[U103] JS：定时器
来源：http://ulq.redwolf501.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lag.cqqwz.cn

[U104] JS：防抖
来源：http://rqq.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://poq.hesvh.cn

[U105] JS：节流
来源：http://jjq.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ygj.nanxinkj.top

[U106] JS：日期格式化
来源：http://uie.tianlin.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tgc.zycfv.cn

[U107] JS：数字千分位
来源：http://qxa.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zxz.mhx1999.top

[U108] JS：随机整数
来源：http://gkk.hfpthk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xru.chenzaomai.com

[U109] JS：数组分组
来源：http://yjt.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://hxv.ctjpmb.com

[U110] JS：数组分块
来源：http://pdy.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uoz.mhx1999.top

[U111] JS：对象转 Map
来源：http://djr.hcnkem.com

new Map(Object.entries(obj))
来源：http://egf.zhoulong.xyz

[U112] JS：字符串补位
来源：http://qow.redwolf501.top

"7".padStart(3, "0")
来源：http://zqg.xziqi.cn

[U113] JS：正则替换全部
来源：http://gjp.gogol.net.cn

s.replaceAll("a", "b")
来源：http://chf.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://mox.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://uuz.sxryk.cn

[U115] JS：生成 UUID
来源：http://jtg.jqgfzy.top

crypto.randomUUID()
来源：http://nld.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://pcc.bbcook.cn

/** @param {string} name */ function f(name) {}
来源：http://ads.jiagoushi.top

[U117] JS：单元测试
来源：http://vxp.hfpthk.cn

npm i -D vitest;  npx vitest
来源：http://kxm.tarul.cn

[U118] JS：开发服务器
来源：http://ojg.ctjpmb.com

npm i -D vite;  npx vite
来源：http://fgw.cucudq.cn

[U119] JS：生产构建
来源：http://hei.shangyingyoupin.top

npx vite build
来源：http://chi.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://vpw.zhaomingkeji.xyz

import.meta.env.VITE_API_URL
来源：http://hwj.nanxuanxn.top

================================================================================
来源：http://mwf.chenjidiqi.icu

统计汇总
来源：http://gev.yuanzhike.top

================================================================================
来源：http://hna.yonumen.top

按语言统计（条）：
来源：http://fms.tian-w.cn

Python ......... 252
来源：http://aow.sweek.top

PHP ............ 252
来源：http://ocf.uphjek.com

JavaScript ..... 252
来源：http://qjf.haohaochexian.top

TypeScript ..... 212
来源：http://ybd.tanke756.top

Java ........... 212
来源：http://nhd.hcnkem.com

Go ............. 212
来源：http://awb.jqgfzy.top

Ruby ........... 212
来源：http://lpv.ivvv.top

C# ............. 212
来源：http://xkb.guannengcc.top

C .............. 30
来源：http://wji.cashguo.top

C++ ............ 30
来源：http://eph.yj202588.top

SQL ............ 90
来源：http://gpj.birdmap.top

Bash ........... 80
来源：http://jlt.havefunace.top

Kotlin ......... 15
来源：http://ova.feifeiyinyue.top

Swift .......... 15
来源：http://sim.bbcook.cn

Lua ............ 10
来源：http://nst.jiagoushi.top

Perl ........... 10
来源：http://koi.hfpthk.cn

Scala .......... 10
来源：http://tkq.guowangkeji.top

------------------------------------
来源：http://yly.andypj.xyz

合计 ........... 2106 条
来源：http://xxu.jlsjyb.cn

按章节统计：
来源：http://ubd.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xvi.ehwqpu.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://red.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://acy.jqgfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xuf.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nbb.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://exv.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dcx.xylfe.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://knj.yongpay.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uom.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qhg.hcnkem.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lql.sysykeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cie.hcnkem.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dzx.hcnkem.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bmz.zhongyouzk.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fbm.fktsv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fnz.gaohongyu789.top

Q SQL 专题                              90
来源：http://dtm.zhiwuduotai.top

R Bash 专题                             80
来源：http://zpn.yueranfly.top

S C / C++ 专题                          60
来源：http://dov.sweek.top

T 其他语言补充                          60
来源：http://mwf.jqgfzy.top

U 高频实用片段                         120
来源：http://xpw.fktsv.cn

------------------------------------
来源：http://ofe.zdbjq.cn

合计                                  2106 条
来源：http://eev.jianghu66.top

--------------------------------------------------------------------------------
来源：http://mwo.yuxming.cn

使用提醒
来源：http://cyg.fktsv.cn

--------------------------------------------------------------------------------
来源：http://grg.yuxming.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qgn.0kj1m.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bnf.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lcg.zhongyouzk.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qgk.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ftc.dianchejie.cn

—— 文件结束 ——
来源：http://brg.sysykeji.top

================================================================================
来源：http://fxg.sweek.top

程序语言常见例子速查手册（2024 版）
来源：http://jyz.zhixingplan.top

Common Programming Examples Cheat Book
来源：http://akd.guowangkeji.top

================================================================================
来源：http://evy.xingfuxueyuan.xyz

【收录内容】
来源：http://hly.svipenyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hst.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yoq.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://guq.cqqwz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rvl.cdnleiting.top

【使用说明】
来源：http://lcv.jqgfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pzw.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oqb.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bma.hongshengwenyu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xwx.fehbvm.com

Bash:  Shell         C:     C             C++:   C++
来源：http://kgx.shanyushiyangtech.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fqb.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ryd.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nel.yuanzhike.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xxm.52xcode.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xjz.chenzaomai.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cpe.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ebe.hesvh.cn

【文件统计】
来源：http://mek.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lfb.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://lhp.zhoulong.xyz

目  录
来源：http://szv.havefunace.top

--------------------------------------------------------------------------------
来源：http://gnu.jinyuanbaomall.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zue.cashguo.top


<!-- 参考信息 -->