代发 wailian999

[T47] Perl：正则捕获
来源：http://gax.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dyi.kuanghao11.cn

[T48] Perl：正则替换
来源：http://egc.dianchejie.cn

$s =~ s/old/new/g;
来源：http://mop.ivvv.top

[T49] Perl：函数
来源：http://wsq.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://apv.cashguo.top

[T50] Perl：逐行读文件
来源：http://gdq.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://utx.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://dkr.nanxinkj.top

[T51] Scala：Hello World
来源：http://cwf.jlsjyb.cn

println("Hello")
来源：http://txl.jlsjyb.cn

[T52] Scala：变量
来源：http://gbo.yongpay.top

val a = 1;  var b = 2
来源：http://qaz.nwbrower.top

[T53] Scala：字符串插值
来源：http://tdw.chenjidiqi.icu

s"值: $b"
来源：http://goy.havefunace.top

[T54] Scala：集合映射
来源：http://pii.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://pgz.birdmap.top

[T55] Scala：集合过滤
来源：http://vqx.nanxinkj.top

List(1, 2, 3).filter(_ > 1)
来源：http://wkf.ydzc1.top

[T56] Scala：样例类
来源：http://seb.fanxiaobao.xyz

case class User(name: String, age: Int)
来源：http://kun.zhengqikj.top

[T57] Scala：模式匹配
来源：http://yhq.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://xrm.iojbl.cn

[T58] Scala：函数定义
来源：http://gha.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://awc.zhiwuduotai.top

[T59] Scala：循环
来源：http://ajm.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://uuc.wangshuangyany.cn

[T60] Scala：折叠
来源：http://lkt.wangshuangyany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vag.cdnleiting.top

================================================================================
来源：http://tat.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xrk.zycfv.cn

================================================================================
来源：http://hzr.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://aoc.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qfm.hongshengwenyu.top

[U02] Py：导出 / 安装依赖
来源：http://pbw.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ump.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://rkl.andypj.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://etf.yj20258.top

[U04] Py：变量调试打印
来源：http://flb.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ouu.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://doq.snrcjt.cn

list(dict.fromkeys(arr))
来源：http://dlu.feifeiyinyue.top

[U06] Py：合并两个字典
来源：http://hmu.tian-w.cn

{**a, **b}
来源：http://edv.daxiang520.top

[U07] Py：反转字典键值
来源：http://uxa.jlsjyb.cn

{v: k for k, v in d.items()}
来源：http://ulo.yj202588.top

[U08] Py：展平二维列表
来源：http://gdq.zhoulong.xyz

[y for x in nested for y in x]
来源：http://dql.sweek.top

[U09] Py：字典取最大值的键
来源：http://rmg.yj20258.top

max(d, key=d.get)
来源：http://sbb.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://jpe.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nlw.ctjpmb.com

[U11] Py：生成器表达式
来源：http://bds.andypj.xyz

(x * 2 for x in arr)
来源：http://deo.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://ozq.zhiwuduotai.top

Counter(arr).most_common(3)
来源：http://otf.dianchejie.cn

[U13] Py：固定长度队列
来源：http://omh.zycfv.cn

deque(maxlen=10)
来源：http://bvb.nwbrower.top

[U14] Py：分组收集到列表
来源：http://swn.shangyingyoupin.top

defaultdict(list)
来源：http://akh.epnwcf.com

[U15] Py：高精度计时
来源：http://rzz.0kj1m.cn

t = time.perf_counter()
来源：http://skn.jqgfzy.top

[U16] Py：命令行参数解析
来源：http://phk.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://izn.316326.xyz

[U17] Py：初始化日志
来源：http://egr.yanxiufei.cn

logging.basicConfig(level=logging.INFO)
来源：http://zcz.nwbrower.top

[U18] Py：预编译正则
来源：http://egt.sjlbkw.cn

pat = re.compile(r"\d+")
来源：http://unt.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://gft.smart0.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lzv.sweek.top

[U20] Py：缓存函数结果
来源：http://uob.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://lpb.316326.xyz

[U21] Py：自定义上下文管理器
来源：http://hyd.shuidangran.top

@contextlib.contextmanager
来源：http://jqm.redwolf501.top

[U22] Py：矩阵转置
来源：http://ion.fengsongda.top

list(zip(*m))
来源：http://nmk.uphjek.com

[U23] Py：分块读取大文件
来源：http://dts.chenzaomai.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pnq.tanke756.top

[U24] Py：路径操作
来源：http://bqu.daxiang520.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://csg.sufxvd.cn

[U25] Py：CSV 按字典读
来源：http://asi.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://bbf.jqgufenzy.top

[U26] Py：并发下载
来源：http://bqp.hnqzz.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ljw.sufxvd.cn

[U27] Py：异步 HTTP
来源：http://dht.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://xrw.tanke756.top

[U28] Py：类型别名
来源：http://sxi.jiagoushi.top

UserId = int
来源：http://xlh.feifeiyinyue.top

[U29] Py：属性校验
来源：http://cmz.tanke756.top

@property 与 @x.setter 配合
来源：http://mtl.yangfankeji.com

[U30] Py：数据类
来源：http://jws.iojbl.cn

@dataclass(slots=True)
来源：http://zjt.bbcook.cn

[U31] Py：单测
来源：http://vjk.hfpthk.cn

python -m pytest -q
来源：http://jbc.zhiwuduotai.top

[U32] Py：代码格式化
来源：http://xpt.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://htw.shuidangran.top

[U33] Py：打包发布
来源：http://gff.pengpengdd.cyou

python -m build  （依赖 pyproject.toml）
来源：http://thj.cdnleiting.top

[U34] Py：判断编码
来源：http://ccb.nanxuanxn.top

chardet.detect(raw)
来源：http://evw.yongpay.top

[U35] Py：发送邮件
来源：http://mff.yuanzhike.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jqv.xylfe.cn

[U36] Py：定时任务
来源：http://yha.xylfe.cn

schedule.every(10).minutes.do(job)
来源：http://pdq.mhx1999.top

[U37] Py：读写 Excel
来源：http://oxg.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://vrx.yuxming.cn

[U38] Py：获取脚本所在目录
来源：http://zgk.daria6918.cn

Path(__file__).resolve().parent
来源：http://wdx.aizwys.cn

[U39] Py：判断是否在交互环境
来源：http://dop.shzxlz.cn

sys.stdout.isatty()
来源：http://yaq.redwolf501.top

[U40] Py：打印到标准错误
来源：http://zhb.sufxvd.cn

print("err", file=sys.stderr)
来源：http://xvw.yuanzhike.top

[U41] PHP：初始化 Composer 项目
来源：http://tee.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://apz.ydzc1.top

[U42] PHP：PSR-4 自动加载
来源：http://inn.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gwd.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://mxg.hnqzz.top

namespace App\Http;
来源：http://wcg.ybcxt.top

[U44] PHP：开启严格类型
来源：http://lqn.yj202588.top

declare(strict_types=1);
来源：http://mtc.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://xyk.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://aqo.hnxiangtu.top

[U46] PHP：可空类型
来源：http://xzt.gotoacloud.top

?string $name = null
来源：http://dnu.zhiwuduotai.top

[U47] PHP：联合类型
来源：http://kgw.guowangkeji.top

int|string $id
来源：http://yxg.tanke756.top

[U48] PHP：纯枚举
来源：http://hpa.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yjr.chenjidiqi.icu

[U49] PHP：只读属性
来源：http://fjg.uphjek.com

public readonly string $name
来源：http://egn.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://bxl.shanyushiyangtech.top

public function __construct(private int $id) {}
来源：http://nka.ydzc1.top

[U51] PHP：数组解构
来源：http://ecf.zhoulong.xyz

[$a, $b] = $arr;
来源：http://vdc.sweek.top

[U52] PHP：箭头函数
来源：http://jzt.cheryme.top

$double = fn($x) => $x * 2;
来源：http://yxx.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://ihx.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://qfz.xylfe.cn

[U54] PHP：空安全调用
来源：http://tbp.shanyushiyangtech.top

$obj?->method()
来源：http://poi.ydjk.org.cn

[U55] PHP：match 表达式
来源：http://kpo.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rkl.ehwqpu.com

[U56] PHP：命名参数
来源：http://xlh.ppjwa.cn

f(a: 1, b: 2)
来源：http://jpd.hesvh.cn

[U57] PHP：字符串插值
来源：http://gws.hywenlv.cn

"值: {$a}"
来源：http://pqa.hywenlv.cn

[U58] PHP：数组三件套
来源：http://mwo.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cch.sxryk.cn

[U59] PHP：自定义排序
来源：http://wwz.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zro.yangfankeji.com

[U60] PHP：JSON 编解码
来源：http://fuq.hongshengwenyu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lso.jinqigfzy.top

[U61] PHP：正则
来源：http://prl.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jbv.hywenlv.cn

[U62] PHP：日期对象
来源：http://ase.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bco.dashuyun.cn

[U63] PHP：文件读写
来源：http://nti.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eqy.xziqi.cn

[U64] PHP：目录遍历
来源：http://wyd.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://bhu.zdqjudy.top

[U65] PHP：会话
来源：http://syf.sjlbkw.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dxq.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://wzn.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://odz.pycfn.com

[U67] PHP：处理文件上传
来源：http://rfh.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://giy.mhx1999.top

[U68] PHP：PDO 连接
来源：http://ndv.xylfe.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eko.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://xbi.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hym.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://tkr.zdbjq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wob.cdnleiting.top

[U71] PHP：抛出异常
来源：http://tlv.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://gba.fengsongda.top

[U72] PHP：写错误日志
来源：http://odg.ywan-chungtsiang.top

error_log("失败: " . $e->getMessage());
来源：http://crl.hnqzz.top

[U73] PHP：读取 ini 配置
来源：http://frn.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://avd.haohaochexian.top

[U74] PHP：读取环境变量
来源：http://pap.zhiwuduotai.top

getenv("APP_ENV") ?: "production"
来源：http://pcx.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://aqc.hywenlv.cn

composer require psr/container
来源：http://mmt.yj20258.top

[U76] PHP：简单路由
来源：http://set.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xbs.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://zdx.0kj1m.cn

composer require twig/twig
来源：http://xhq.sjlbkw.cn

[U78] PHP：单元测试
来源：http://vdv.yj202588.top

composer require --dev phpunit/phpunit
来源：http://xap.ydjk.org.cn

[U79] PHP：静态分析
来源：http://qyj.hfpthk.cn

composer require --dev phpstan/phpstan
来源：http://jkl.fehbvm.com

[U80] PHP：代码规范修复
来源：http://pbc.cqqwz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://toe.tanke756.top

[U81] JS：初始化项目
来源：http://zon.sysykeji.top

npm init -y;  npm i express
来源：http://wbh.yfazqb.com

[U82] JS：package.json 脚本
来源：http://fpg.cdnleiting.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fgz.ivvv.top

[U83] JS：ES Module 导入导出
来源：http://aar.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aai.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://bqi.jqgfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://msn.tian-w.cn

[U85] JS：可选链
来源：http://wal.zycfv.cn

a?.b?.c
来源：http://dsy.aizwys.cn

[U86] JS：空值合并
来源：http://plm.ywan-chungtsiang.top

a ?? b
来源：http://aeh.xuetiantiany.cn

[U87] JS：解构默认值
来源：http://uny.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://cjf.gotoacloud.top

[U88] JS：对象展开合并
来源：http://uur.yueranfly.top

{ ...a, ...b }
来源：http://mwv.mhx1999.top

[U89] JS：数组去重
来源：http://jud.smart0.xyz

[...new Set(arr)]
来源：http://bpb.aizwys.cn

[U90] JS：数字数组排序
来源：http://plj.zhongyouzk.top

[...arr].sort((a, b) => a - b)
来源：http://hpk.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://ulf.aizwys.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pgw.yj202588.top

[U92] JS：深拷贝
来源：http://jdj.vehdjk.com

structuredClone(obj)
来源：http://zzk.daxiang520.top

[U93] JS：模板字符串
来源：http://eig.nanxinkj.top

`共 ${n} 条`
来源：http://pld.iojbl.cn

[U94] JS：箭头函数
来源：http://imy.sweek.top

const double = x => x * 2;
来源：http://dei.fzhhl.top

[U95] JS：Promise 包装
来源：http://lnw.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://ddm.yj20258.top

[U96] JS：async/await 与异常
来源：http://yhs.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ytr.cucudq.cn

[U97] JS：并发请求
来源：http://otq.yj20258888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kpb.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://fha.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yky.nanxinkj.top

[U99] JS：事件监听
来源：http://bmd.ydzc1.top

el.addEventListener("click", e => {})
来源：http://fck.gogol.net.cn

[U100] JS：DOM 查询
来源：http://shr.yangfankeji.com

document.querySelector(".item")
来源：http://eoo.sufxvd.cn

[U101] JS：classList 操作
来源：http://lky.feifeiyinyue.top

el.classList.toggle("active")
来源：http://vpv.chenlongwang.top

[U102] JS：本地存储
来源：http://zlw.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://zwk.hysaishi.cn

[U103] JS：定时器
来源：http://oac.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eod.xziqi.cn

[U104] JS：防抖
来源：http://dma.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ece.redwolf501.top

[U105] JS：节流
来源：http://uex.smart0.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ime.ehwqpu.com

[U106] JS：日期格式化
来源：http://stp.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cqt.jinghuilouyu.cn

[U107] JS：数字千分位
来源：http://frs.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vpt.ydjk.org.cn

[U108] JS：随机整数
来源：http://uwu.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wlx.ctjpmb.com

[U109] JS：数组分组
来源：http://mhl.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://xzc.yj202588.top

[U110] JS：数组分块
来源：http://vld.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kbl.shuidangran.top

[U111] JS：对象转 Map
来源：http://zop.pengpengdd.cyou

new Map(Object.entries(obj))
来源：http://hps.hfpthk.cn

[U112] JS：字符串补位
来源：http://mdp.hnqzz.top

"7".padStart(3, "0")
来源：http://pdj.andypj.xyz

[U113] JS：正则替换全部
来源：http://vrs.tarul.cn

s.replaceAll("a", "b")
来源：http://uqn.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://gfj.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://etd.feifeiyinyue.top

[U115] JS：生成 UUID
来源：http://vje.gzhubu.top

crypto.randomUUID()
来源：http://isu.feifeiyinyue.top

[U116] JS：类型检查（JSDoc）
来源：http://ejv.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://uxu.aibaodan.cn

[U117] JS：单元测试
来源：http://qip.havefunace.top

npm i -D vitest;  npx vitest
来源：http://bxo.kuanghao11.cn

[U118] JS：开发服务器
来源：http://mwk.yueranfly.top

npm i -D vite;  npx vite
来源：http://bvx.cqqwz.cn

[U119] JS：生产构建
来源：http://pmp.cashguo.top

npx vite build
来源：http://xek.yvedp.cn

[U120] JS：读取环境变量（Vite）
来源：http://vmn.vqdsnc.cn

import.meta.env.VITE_API_URL
来源：http://vho.yj20258888.top

================================================================================
来源：http://hit.daxiang520.top

统计汇总
来源：http://egq.epnwcf.com

================================================================================
来源：http://ibn.xinyue.icu

按语言统计（条）：
来源：http://dos.cdnleiting.top

Python ......... 252
来源：http://hzw.c1oappe.top

PHP ............ 252
来源：http://qeo.ivvv.top

JavaScript ..... 252
来源：http://fzu.zhoulong.xyz

TypeScript ..... 212
来源：http://eoa.svipenyu.cn

Java ........... 212
来源：http://kvm.ybcxt.top

Go ............. 212
来源：http://ula.zhijiandao.cn

Ruby ........... 212
来源：http://obo.wangshuangyany.cn

C# ............. 212
来源：http://nfd.iojbl.cn

C .............. 30
来源：http://oco.daria6918.cn

C++ ............ 30
来源：http://jsd.ctjpmb.com

SQL ............ 90
来源：http://hsd.feifeiyinyue.top

Bash ........... 80
来源：http://coo.jyoumei.cn

Kotlin ......... 15
来源：http://vzg.bbcook.cn

Swift .......... 15
来源：http://eyz.xingfuxueyuan.xyz

Lua ............ 10
来源：http://jqk.vehdjk.com

Perl ........... 10
来源：http://ijc.zhongyouzk.top

Scala .......... 10
来源：http://wqu.meibo888.top

------------------------------------
来源：http://rbf.hongshengwenyu.top

合计 ........... 2106 条
来源：http://zhd.zdbjq.cn

按章节统计：
来源：http://col.9152youxi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://azb.sjlbkw.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hby.cheryme.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oko.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://plp.ppjwa.cn


<!-- 参考信息 -->