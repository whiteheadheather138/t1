代发 wailian999

[U15] Py：高精度计时
来源：http://bwu.316326.xyz

t = time.perf_counter()
来源：http://nck.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://obu.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ffd.yuxming.cn

[U17] Py：初始化日志
来源：http://uzv.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://ibx.tanke756.top

[U18] Py：预编译正则
来源：http://nxm.shuidangran.top

pat = re.compile(r"\d+")
来源：http://mrm.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://xqf.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wul.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://cpa.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://hlc.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://kip.52xcode.cn

@contextlib.contextmanager
来源：http://eoc.hongshengwenyu.top

[U22] Py：矩阵转置
来源：http://usz.dianchejie.cn

list(zip(*m))
来源：http://nnj.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://giz.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aqy.ehwqpu.com

[U24] Py：路径操作
来源：http://kot.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fxd.xuanzx.com

[U25] Py：CSV 按字典读
来源：http://lzu.svipenyu.cn

csv.DictReader(f)
来源：http://mio.hcnkem.com

[U26] Py：并发下载
来源：http://sdz.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hqt.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://liw.feifeiyinyue.top

aiohttp.ClientSession() 配合 async with
来源：http://roi.aizwys.cn

[U28] Py：类型别名
来源：http://aal.fehbvm.com

UserId = int
来源：http://uhj.ydzc1.top

[U29] Py：属性校验
来源：http://qne.chenlongwang.top

@property 与 @x.setter 配合
来源：http://wca.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://ahv.yonumen.top

@dataclass(slots=True)
来源：http://wal.ydjk.org.cn

[U31] Py：单测
来源：http://hkn.quarkkingdee.top

python -m pytest -q
来源：http://gbm.zhoulong.xyz

[U32] Py：代码格式化
来源：http://cpo.nwbrower.top

ruff format . && ruff check --fix .
来源：http://fpb.9152youxi.cn

[U33] Py：打包发布
来源：http://twd.chenjidiqi.icu

python -m build  （依赖 pyproject.toml）
来源：http://ahd.fengsongda.top

[U34] Py：判断编码
来源：http://zex.hcnkem.com

chardet.detect(raw)
来源：http://tox.hfpthk.cn

[U35] Py：发送邮件
来源：http://ojg.ywan-chungtsiang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rli.xingfuxueyuan.xyz

[U36] Py：定时任务
来源：http://wul.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://wyy.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://bgd.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://nnv.cheryme.top

[U38] Py：获取脚本所在目录
来源：http://qec.sxryk.cn

Path(__file__).resolve().parent
来源：http://fsn.shangyingyoupin.top

[U39] Py：判断是否在交互环境
来源：http://etu.ctjpmb.com

sys.stdout.isatty()
来源：http://qvb.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://ijj.daria6918.cn

print("err", file=sys.stderr)
来源：http://lxo.yj202588.top

[U41] PHP：初始化 Composer 项目
来源：http://jlm.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nsw.smart0.xyz

[U42] PHP：PSR-4 自动加载
来源：http://zod.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://otx.hnxiangtu.top

[U43] PHP：声明命名空间
来源：http://bal.nwbrower.top

namespace App\Http;
来源：http://mfq.sysykeji.top

[U44] PHP：开启严格类型
来源：http://byc.yj20258.top

declare(strict_types=1);
来源：http://wdr.shanyushiyangtech.top

[U45] PHP：类型声明与返回类型
来源：http://bjk.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://esw.gaohongyu789.top

[U46] PHP：可空类型
来源：http://dqh.shanyushiyangkeji.top

?string $name = null
来源：http://dfh.meibo888.top

[U47] PHP：联合类型
来源：http://elq.svipenyu.cn

int|string $id
来源：http://ian.yvedp.cn

[U48] PHP：纯枚举
来源：http://pql.vqdsnc.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ngp.cqqwz.cn

[U49] PHP：只读属性
来源：http://pao.9152youxi.cn

public readonly string $name
来源：http://ami.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://emo.hywenlv.cn

public function __construct(private int $id) {}
来源：http://zjw.hywenlv.cn

[U51] PHP：数组解构
来源：http://zis.yj20258.top

[$a, $b] = $arr;
来源：http://hjt.cdnleiting.top

[U52] PHP：箭头函数
来源：http://xaq.hammf.cn

$double = fn($x) => $x * 2;
来源：http://jij.yuxming.cn

[U53] PHP：空合并运算符
来源：http://ols.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://ezf.shuidangran.top

[U54] PHP：空安全调用
来源：http://smp.chenzaomai.com

$obj?->method()
来源：http://afr.sysykeji.top

[U55] PHP：match 表达式
来源：http://acx.ybcxt.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dvj.havefunace.top

[U56] PHP：命名参数
来源：http://xuq.xylfe.cn

f(a: 1, b: 2)
来源：http://pjx.gzhubu.top

[U57] PHP：字符串插值
来源：http://prn.snrcjt.cn

"值: {$a}"
来源：http://cmu.sysykeji.top

[U58] PHP：数组三件套
来源：http://xmj.wangdashe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://awt.chenlongwang.top

[U59] PHP：自定义排序
来源：http://rpw.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lcm.tarul.cn

[U60] PHP：JSON 编解码
来源：http://mmx.ydjk.org.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://esw.nanxinkj.top

[U61] PHP：正则
来源：http://cku.ydzc1.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tqq.uphjek.com

[U62] PHP：日期对象
来源：http://wmu.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://leg.chenzaomai.com

[U63] PHP：文件读写
来源：http://fhq.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gxg.cdnleiting.top

[U64] PHP：目录遍历
来源：http://xjf.yuanzhike.top

glob("dir/*.php");  scandir("dir");
来源：http://wqq.xziqi.cn

[U65] PHP：会话
来源：http://hfd.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lfp.yj202588.top

[U66] PHP：设置 Cookie
来源：http://hoy.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cdl.iojbl.cn

[U67] PHP：处理文件上传
来源：http://qay.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mhm.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://rsj.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ale.shanyushiyangkeji.top

[U69] PHP：PDO 预处理
来源：http://snr.ywan-chungtsiang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hgw.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://zye.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ojq.nwbrower.top

[U71] PHP：抛出异常
来源：http://ufk.yj202588.top

throw new RuntimeException("失败", 500);
来源：http://yan.pycfn.com

[U72] PHP：写错误日志
来源：http://tny.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://ztv.sweek.top

[U73] PHP：读取 ini 配置
来源：http://gpt.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://zuv.shuidangran.top

[U74] PHP：读取环境变量
来源：http://zkw.yj202588.top

getenv("APP_ENV") ?: "production"
来源：http://vjg.jiagoushi.top

[U75] PHP：依赖注入
来源：http://pit.pycfn.com

composer require psr/container
来源：http://uer.sweek.top

[U76] PHP：简单路由
来源：http://dzp.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rnv.jinghuilouyu.cn

[U77] PHP：模板渲染
来源：http://dos.zhiwuduotai.top

composer require twig/twig
来源：http://nhz.xingfuxueyuan.xyz

[U78] PHP：单元测试
来源：http://alp.yuxming.cn

composer require --dev phpunit/phpunit
来源：http://kaj.yj20258.top

[U79] PHP：静态分析
来源：http://ssk.sysykeji.top

composer require --dev phpstan/phpstan
来源：http://mmj.hcnkem.com

[U80] PHP：代码规范修复
来源：http://pyv.c1oappe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hwf.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://frj.jyoumei.cn

npm init -y;  npm i express
来源：http://aeg.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://llc.yj20258888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dty.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://xmz.jyoumei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://waz.xuetiantiany.cn

[U84] JS：CommonJS 写法
来源：http://mra.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://bqq.cucudq.cn

[U85] JS：可选链
来源：http://oyt.svipenyu.cn

a?.b?.c
来源：http://rvc.ivvv.top

[U86] JS：空值合并
来源：http://mok.ehwqpu.com

a ?? b
来源：http://chd.havefunace.top

[U87] JS：解构默认值
来源：http://ird.sweek.top

const { a = 1, b = 2 } = obj;
来源：http://jcf.hfpthk.cn

[U88] JS：对象展开合并
来源：http://ozb.52xcode.cn

{ ...a, ...b }
来源：http://ahz.hcnkem.com

[U89] JS：数组去重
来源：http://aqz.cashguo.top

[...new Set(arr)]
来源：http://fna.cdnleiting.top

[U90] JS：数字数组排序
来源：http://toi.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://xtg.bbcook.cn

[U91] JS：对象键值遍历
来源：http://dxc.cqqwz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yrm.jiagoushi.top

[U92] JS：深拷贝
来源：http://eki.ydzc1.top

structuredClone(obj)
来源：http://rlx.xylfe.cn

[U93] JS：模板字符串
来源：http://bdj.jqgfzy.top

`共 ${n} 条`
来源：http://tub.haohaochexian.top

[U94] JS：箭头函数
来源：http://odv.aibaodan.cn

const double = x => x * 2;
来源：http://kmh.gogol.net.cn

[U95] JS：Promise 包装
来源：http://osh.jinqigfzy.top

new Promise((resolve, reject) => {})
来源：http://lpm.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://wxh.fanxiaobao.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ano.yvedp.cn

[U97] JS：并发请求
来源：http://sya.cdnleiting.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fkx.hongshengwenyu.top

[U98] JS：fetch 带 JSON
来源：http://srb.snrcjt.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dog.yj20258888.top

[U99] JS：事件监听
来源：http://yto.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://paa.yj202588.top

[U100] JS：DOM 查询
来源：http://znv.fengsongda.top

document.querySelector(".item")
来源：http://loz.xuetiantiany.cn

[U101] JS：classList 操作
来源：http://bpp.ehwqpu.com

el.classList.toggle("active")
来源：http://upu.zdqjudy.top

[U102] JS：本地存储
来源：http://frx.xziqi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tdd.52xcode.cn

[U103] JS：定时器
来源：http://zyu.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lgs.daxiang520.top

[U104] JS：防抖
来源：http://jsy.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vfz.ywan-chungtsiang.top

[U105] JS：节流
来源：http://myh.tianlin.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kzv.sjlbkw.cn

[U106] JS：日期格式化
来源：http://laq.gotoacloud.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://waa.chenzaomai.com

[U107] JS：数字千分位
来源：http://dao.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lnz.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://rqw.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tcg.uphjek.com

[U109] JS：数组分组
来源：http://lwn.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://cwy.cqqwz.cn

[U110] JS：数组分块
来源：http://ual.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lbl.316326.xyz

[U111] JS：对象转 Map
来源：http://wdy.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://oqw.chenzaomai.com

[U112] JS：字符串补位
来源：http://gqp.jiagoushi.top

"7".padStart(3, "0")
来源：http://kya.iojbl.cn

[U113] JS：正则替换全部
来源：http://enx.shanyushiyangkeji.top

s.replaceAll("a", "b")
来源：http://rgl.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://tgg.dianchejie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wks.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://mlt.tian-w.cn

crypto.randomUUID()
来源：http://lky.quarkkingdee.top

[U116] JS：类型检查（JSDoc）
来源：http://pzk.fengsongda.top

/** @param {string} name */ function f(name) {}
来源：http://ngg.yj20258.top

[U117] JS：单元测试
来源：http://cvz.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://hrs.smart0.xyz

[U118] JS：开发服务器
来源：http://hpj.feifeiyinyue.top

npm i -D vite;  npx vite
来源：http://ykx.yj202588.top

[U119] JS：生产构建
来源：http://jzu.c1oappe.top

npx vite build
来源：http://ssr.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://stc.yvedp.cn

import.meta.env.VITE_API_URL
来源：http://ukh.ehwqpu.com

================================================================================
来源：http://znr.gotoacloud.top

统计汇总
来源：http://rkv.birdmap.top

================================================================================
来源：http://xpc.smart0.xyz

按语言统计（条）：
来源：http://rzi.fehbvm.com

Python ......... 252
来源：http://tyd.pengpengdd.cyou

PHP ............ 252
来源：http://tmk.jyoumei.cn

JavaScript ..... 252
来源：http://zqz.smart0.xyz

TypeScript ..... 212
来源：http://vyy.0kj1m.cn

Java ........... 212
来源：http://ijh.zycfv.cn

Go ............. 212
来源：http://egx.cheryme.top

Ruby ........... 212
来源：http://ecv.gogol.net.cn

C# ............. 212
来源：http://ljd.meibo888.top

C .............. 30
来源：http://juk.ivvv.top

C++ ............ 30
来源：http://psb.zhijiandao.cn

SQL ............ 90
来源：http://siq.cdnleiting.top

Bash ........... 80
来源：http://wvk.yj20258888.top

Kotlin ......... 15
来源：http://ffz.tarul.cn

Swift .......... 15
来源：http://lqp.zycfv.cn

Lua ............ 10
来源：http://ngf.guannengcc.top

Perl ........... 10
来源：http://ung.tanke756.top

Scala .......... 10
来源：http://wlz.ehwqpu.com

------------------------------------
来源：http://rks.andypj.xyz

合计 ........... 2106 条
来源：http://tos.nanxinkj.top

按章节统计：
来源：http://vwa.cqqwz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kgw.yueranfly.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://waz.zycfv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tvv.c1oappe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oit.iojbl.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://smi.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eny.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://swj.dianchejie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rcz.feifeiyinyue.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lyl.ywan-chungtsiang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tac.yj20258888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cjn.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vfo.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bhk.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aed.quarkkingdee.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ugx.zdqjudy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jgq.nanxinkj.top

Q SQL 专题                              90
来源：http://cdu.52xcode.cn

R Bash 专题                             80
来源：http://ilb.meibo888.top

S C / C++ 专题                          60
来源：http://aqn.shuidangran.top

T 其他语言补充                          60
来源：http://agj.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://sjr.cdnleiting.top

------------------------------------
来源：http://bpl.shangyingyoupin.top

合计                                  2106 条
来源：http://zlr.fengsongda.top

--------------------------------------------------------------------------------
来源：http://zdi.fktsv.cn

使用提醒
来源：http://nex.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://bff.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vft.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bbc.hysaishi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uhc.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hqb.pycfn.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dho.guannengcc.top

—— 文件结束 ——
来源：http://uwa.jiagoushi.top

================================================================================
来源：http://biy.jlsjyb.cn

程序语言常见例子速查手册（2024 版）
来源：http://xng.chenjidiqi.icu

Common Programming Examples Cheat Book
来源：http://nnk.jinyuanbaomall.cn

================================================================================
来源：http://uon.shanyushiyangtech.top

【收录内容】
来源：http://zgp.cqqwz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ljm.fktsv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sfh.ydzc1.top

SQL · Bash · C · C++
来源：http://zlm.daxiang520.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cbx.fanxiaobao.xyz

【使用说明】
来源：http://ify.pycfn.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hhm.hysaishi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qkk.hnxiangtu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uwz.ctjpmb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iaq.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cbk.guannengcc.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mfu.shzxlz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qge.cqqwz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rtl.cashguo.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://phu.jlsjyb.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bgy.tanke756.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mnk.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zny.havefunace.top

【文件统计】
来源：http://hjo.shanyushiyangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qem.pycfn.com

--------------------------------------------------------------------------------
来源：http://xcu.snrcjt.cn

目  录
来源：http://fop.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://aeh.fzhhl.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fjn.nanxinkj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pnx.zdbjq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vxv.316326.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rmk.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uku.ctjpmb.com


<!-- 参考信息 -->