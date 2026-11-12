代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://obo.52xcode.cn

[T51] Scala：Hello World
来源：http://trt.daxiang520.top

println("Hello")
来源：http://uas.nwbrower.top

[T52] Scala：变量
来源：http://fqd.dianchejie.cn

val a = 1;  var b = 2
来源：http://xet.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://gap.dianchejie.cn

s"值: $b"
来源：http://ocq.cdnleiting.top

[T54] Scala：集合映射
来源：http://woe.zhongyouzk.top

List(1, 2, 3).map(_ * 2)
来源：http://wtx.yj20258888.top

[T55] Scala：集合过滤
来源：http://fii.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://plp.xuetiantiany.cn

[T56] Scala：样例类
来源：http://prd.hcnkem.com

case class User(name: String, age: Int)
来源：http://ohd.hcnkem.com

[T57] Scala：模式匹配
来源：http://okv.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ksc.yfazqb.com

[T58] Scala：函数定义
来源：http://kia.hywenlv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kwv.dianchejie.cn

[T59] Scala：循环
来源：http://ryk.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://sqb.xingfuxueyuan.xyz

[T60] Scala：折叠
来源：http://lle.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wmp.zhijiandao.cn

================================================================================
来源：http://pvm.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lka.meibo888.top

================================================================================
来源：http://zau.nanxuanxn.top

[U01] Py：创建虚拟环境
来源：http://qor.zhoulong.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://jpl.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://mwv.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://waf.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://dve.aizwys.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lrk.hcnkem.com

[U04] Py：变量调试打印
来源：http://kqn.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wjc.gaohongyu789.top

[U05] Py：列表去重且保序
来源：http://cva.sxryk.cn

list(dict.fromkeys(arr))
来源：http://dmu.smart0.xyz

[U06] Py：合并两个字典
来源：http://ixu.bjfxy.top

{**a, **b}
来源：http://woe.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://xvm.yuxming.cn

{v: k for k, v in d.items()}
来源：http://qxw.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://mpb.jinghuilouyu.cn

[y for x in nested for y in x]
来源：http://wgt.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://zee.yj20258888.top

max(d, key=d.get)
来源：http://scw.vqdsnc.cn

[U10] Py：按值排序字典
来源：http://uuz.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://amc.ppjwa.cn

[U11] Py：生成器表达式
来源：http://bvq.andypj.xyz

(x * 2 for x in arr)
来源：http://fih.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://jkt.guannengcc.top

Counter(arr).most_common(3)
来源：http://jha.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://jnw.tarul.cn

deque(maxlen=10)
来源：http://swo.yfazqb.com

[U14] Py：分组收集到列表
来源：http://ahb.sxryk.cn

defaultdict(list)
来源：http://prq.hcnkem.com

[U15] Py：高精度计时
来源：http://oam.yonumen.top

t = time.perf_counter()
来源：http://nua.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://ici.cdnleiting.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dpq.bbcook.cn

[U17] Py：初始化日志
来源：http://ife.chenlongwang.top

logging.basicConfig(level=logging.INFO)
来源：http://zuh.hesvh.cn

[U18] Py：预编译正则
来源：http://kky.yj202588.top

pat = re.compile(r"\d+")
来源：http://qfp.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://pcr.gotoacloud.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gba.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://tvz.cdnleiting.top

@functools.lru_cache(maxsize=None)
来源：http://cct.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://dnx.ybcxt.top

@contextlib.contextmanager
来源：http://tcu.fktsv.cn

[U22] Py：矩阵转置
来源：http://aoc.bbcook.cn

list(zip(*m))
来源：http://mud.birdmap.top

[U23] Py：分块读取大文件
来源：http://oln.c1oappe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eok.hongshengwenyu.top

[U24] Py：路径操作
来源：http://ebu.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aln.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://zfz.xinyue.icu

csv.DictReader(f)
来源：http://meo.daria6918.cn

[U26] Py：并发下载
来源：http://oqd.xingfuxueyuan.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sta.fanxiaobao.xyz

[U27] Py：异步 HTTP
来源：http://oqr.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://jul.iojbl.cn

[U28] Py：类型别名
来源：http://bhp.dashuyun.cn

UserId = int
来源：http://anz.ywan-chungtsiang.top

[U29] Py：属性校验
来源：http://siw.yongpay.top

@property 与 @x.setter 配合
来源：http://wuc.gogol.net.cn

[U30] Py：数据类
来源：http://kyr.yueranfly.top

@dataclass(slots=True)
来源：http://qph.daria6918.cn

[U31] Py：单测
来源：http://frz.xziqi.cn

python -m pytest -q
来源：http://ilu.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://guu.sufxvd.cn

ruff format . && ruff check --fix .
来源：http://fjk.chenjidiqi.icu

[U33] Py：打包发布
来源：http://lue.cheryme.top

python -m build  （依赖 pyproject.toml）
来源：http://bpp.feifeiyinyue.top

[U34] Py：判断编码
来源：http://xqg.52xcode.cn

chardet.detect(raw)
来源：http://gqc.xylfe.cn

[U35] Py：发送邮件
来源：http://rub.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zcd.havefunace.top

[U36] Py：定时任务
来源：http://dki.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://vig.smart0.xyz

[U37] Py：读写 Excel
来源：http://oql.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://kqe.hongshengwenyu.top

[U38] Py：获取脚本所在目录
来源：http://zbx.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://hkh.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://cot.sweek.top

sys.stdout.isatty()
来源：http://zxs.chenjidiqi.icu

[U40] Py：打印到标准错误
来源：http://hnv.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://vkj.mhx1999.top

[U41] PHP：初始化 Composer 项目
来源：http://zqw.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nrc.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://doj.shzxlz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nat.hesvh.cn

[U43] PHP：声明命名空间
来源：http://rbj.pycfn.com

namespace App\Http;
来源：http://vmu.chenjidiqi.icu

[U44] PHP：开启严格类型
来源：http://qou.cucudq.cn

declare(strict_types=1);
来源：http://wtl.zycfv.cn

[U45] PHP：类型声明与返回类型
来源：http://lhm.fzhhl.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://akj.sufxvd.cn

[U46] PHP：可空类型
来源：http://vwb.quarkkingdee.top

?string $name = null
来源：http://tdl.jinyuanbaomall.cn

[U47] PHP：联合类型
来源：http://wuy.chenjidiqi.icu

int|string $id
来源：http://tdk.0kj1m.cn

[U48] PHP：纯枚举
来源：http://jbn.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qdc.jinqigfzy.top

[U49] PHP：只读属性
来源：http://rix.316326.xyz

public readonly string $name
来源：http://don.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://zbd.hcnkem.com

public function __construct(private int $id) {}
来源：http://kdu.uphjek.com

[U51] PHP：数组解构
来源：http://zoz.zhoulong.xyz

[$a, $b] = $arr;
来源：http://sqe.yongpay.top

[U52] PHP：箭头函数
来源：http://nvb.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://gyb.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://xce.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://zqv.cucudq.cn

[U54] PHP：空安全调用
来源：http://tuk.zhaomingkeji.xyz

$obj?->method()
来源：http://ucm.aizwys.cn

[U55] PHP：match 表达式
来源：http://aak.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jby.c1oappe.top

[U56] PHP：命名参数
来源：http://nqj.hesvh.cn

f(a: 1, b: 2)
来源：http://vcu.hesvh.cn

[U57] PHP：字符串插值
来源：http://cmg.yanxiufei.cn

"值: {$a}"
来源：http://ong.hysaishi.cn

[U58] PHP：数组三件套
来源：http://wtz.epnwcf.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tzi.hfpthk.cn

[U59] PHP：自定义排序
来源：http://jjz.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lqv.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://ugy.jinyuanbaomall.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wct.jqgufenzy.top

[U61] PHP：正则
来源：http://ojd.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rvl.ybcxt.top

[U62] PHP：日期对象
来源：http://nsd.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dtn.jyoumei.cn

[U63] PHP：文件读写
来源：http://aln.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ars.cashguo.top

[U64] PHP：目录遍历
来源：http://smd.sweek.top

glob("dir/*.php");  scandir("dir");
来源：http://qdu.cqqwz.cn

[U65] PHP：会话
来源：http://itl.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vki.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://rkv.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ddc.ydzc1.top

[U67] PHP：处理文件上传
来源：http://uxf.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mzp.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://kbv.jqgufenzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bck.cucudq.cn

[U69] PHP：PDO 预处理
来源：http://pgg.tian-w.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kwv.bjfxy.top

[U70] PHP：PDO 事务
来源：http://uzv.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iau.hesvh.cn

[U71] PHP：抛出异常
来源：http://kxh.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://hny.xinyue.icu

[U72] PHP：写错误日志
来源：http://ikb.aizwys.cn

error_log("失败: " . $e->getMessage());
来源：http://upd.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://osn.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://qog.cucudq.cn

[U74] PHP：读取环境变量
来源：http://iap.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://xax.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://zww.yanxiufei.cn

composer require psr/container
来源：http://gvo.meibo888.top

[U76] PHP：简单路由
来源：http://qhx.xziqi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://khn.chenzaomai.com

[U77] PHP：模板渲染
来源：http://rlh.zdqjudy.top

composer require twig/twig
来源：http://zpp.sxryk.cn

[U78] PHP：单元测试
来源：http://zkf.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://pgm.yj20258.top

[U79] PHP：静态分析
来源：http://pmr.birdmap.top

composer require --dev phpstan/phpstan
来源：http://hwz.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://ccg.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qgg.redwolf501.top

[U81] JS：初始化项目
来源：http://ikk.zdqjudy.top

npm init -y;  npm i express
来源：http://tql.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://szk.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://heh.fehbvm.com

[U83] JS：ES Module 导入导出
来源：http://bda.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://vdd.daria6918.cn

[U84] JS：CommonJS 写法
来源：http://ths.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://skh.yueranfly.top

[U85] JS：可选链
来源：http://lmx.ehwqpu.com

a?.b?.c
来源：http://fwm.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://dav.fengsongda.top

a ?? b
来源：http://njh.dashuyun.cn

[U87] JS：解构默认值
来源：http://qyv.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://lhv.iojbl.cn

[U88] JS：对象展开合并
来源：http://sog.xylfe.cn

{ ...a, ...b }
来源：http://gci.birdmap.top

[U89] JS：数组去重
来源：http://lwc.tianlin.xyz

[...new Set(arr)]
来源：http://lyk.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://ztn.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://emx.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://dyz.zhoulong.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oir.zhijiandao.cn

[U92] JS：深拷贝
来源：http://twj.gzhubu.top

structuredClone(obj)
来源：http://cla.52xcode.cn

[U93] JS：模板字符串
来源：http://gjo.shanyushiyangtech.top

`共 ${n} 条`
来源：http://unz.sufxvd.cn

[U94] JS：箭头函数
来源：http://rbd.sxryk.cn

const double = x => x * 2;
来源：http://hun.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://liv.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://rxr.fktsv.cn

[U96] JS：async/await 与异常
来源：http://eyf.shuidangran.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rcx.daxiang520.top

[U97] JS：并发请求
来源：http://yvg.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://wcr.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://bqd.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zqf.zycfv.cn

[U99] JS：事件监听
来源：http://ywg.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://vzz.meibo888.top

[U100] JS：DOM 查询
来源：http://byx.fzhhl.top

document.querySelector(".item")
来源：http://ene.316326.xyz

[U101] JS：classList 操作
来源：http://fdx.fzhhl.top

el.classList.toggle("active")
来源：http://tzq.zhongyouzk.top

[U102] JS：本地存储
来源：http://ooh.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bld.havefunace.top

[U103] JS：定时器
来源：http://aro.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tge.shangyingyoupin.top

[U104] JS：防抖
来源：http://cln.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://emc.nwbrower.top

[U105] JS：节流
来源：http://yja.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gsh.yj20258888.top

[U106] JS：日期格式化
来源：http://ucm.smart0.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gvd.tianlin.xyz

[U107] JS：数字千分位
来源：http://wmg.meibo888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pfg.iojbl.cn

[U108] JS：随机整数
来源：http://ize.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kgq.haohaochexian.top

[U109] JS：数组分组
来源：http://sia.uphjek.com

Object.groupBy(arr, x => x.type)
来源：http://qit.quarkkingdee.top

[U110] JS：数组分块
来源：http://nih.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://slx.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://lcw.birdmap.top

new Map(Object.entries(obj))
来源：http://upe.meibo888.top

[U112] JS：字符串补位
来源：http://rek.xinyue.icu

"7".padStart(3, "0")
来源：http://eyb.bbcook.cn

[U113] JS：正则替换全部
来源：http://cxe.yongpay.top

s.replaceAll("a", "b")
来源：http://rrr.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://jwu.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xbt.hysaishi.cn

[U115] JS：生成 UUID
来源：http://uwu.havefunace.top

crypto.randomUUID()
来源：http://nlr.zhixingplan.top

[U116] JS：类型检查（JSDoc）
来源：http://lym.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://ozp.ydjk.org.cn

[U117] JS：单元测试
来源：http://kvg.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://wfy.hysaishi.cn

[U118] JS：开发服务器
来源：http://lsg.ppjwa.cn

npm i -D vite;  npx vite
来源：http://ihu.bjfxy.top

[U119] JS：生产构建
来源：http://lgt.zhengqikj.top

npx vite build
来源：http://zpv.shanyushiyangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://pko.gaohongyu789.top

import.meta.env.VITE_API_URL
来源：http://ooa.tarul.cn

================================================================================
来源：http://won.jinqigfzy.top

统计汇总
来源：http://jlc.sjlbkw.cn

================================================================================
来源：http://smy.vehdjk.com

按语言统计（条）：
来源：http://kuu.fanxiaobao.xyz

Python ......... 252
来源：http://mfq.xingfuxueyuan.xyz

PHP ............ 252
来源：http://wph.dianchejie.cn

JavaScript ..... 252
来源：http://otj.9152youxi.cn

TypeScript ..... 212
来源：http://noq.shuidangran.top

Java ........... 212
来源：http://zdi.nanxuanxn.top

Go ............. 212
来源：http://ycg.yfazqb.com

Ruby ........... 212
来源：http://pvf.yangfankeji.com

C# ............. 212
来源：http://acz.xylfe.cn

C .............. 30
来源：http://kbz.chenlongwang.top

C++ ............ 30
来源：http://lnw.guowangkeji.top

SQL ............ 90
来源：http://wtj.yuxming.cn

Bash ........... 80
来源：http://xpj.quarkkingdee.top

Kotlin ......... 15
来源：http://rsl.wangshuangyany.cn

Swift .......... 15
来源：http://jpr.redwolf501.top

Lua ............ 10
来源：http://ohy.xingfuxueyuan.xyz

Perl ........... 10
来源：http://bcv.birdmap.top

Scala .......... 10
来源：http://lwo.nanxuanxn.top

------------------------------------
来源：http://bkc.jqgufenzy.top

合计 ........... 2106 条
来源：http://zru.daxiang520.top

按章节统计：
来源：http://kfz.tian-w.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qkq.yanxiufei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xkb.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://diu.aibaodan.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iua.zdqjudy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mpa.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://auf.kuanghao11.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ind.andypj.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://byf.gzhubu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wfv.fktsv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vjs.uphjek.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hvn.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lxh.zdbjq.cn


<!-- 参考信息 -->