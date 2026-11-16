代发 wailian999

[T05] Kotlin：when 表达式
来源：http://ybb.tanke756.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dqo.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://dzk.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lap.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://vbb.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://exr.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://ovr.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://hue.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://cfg.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://rag.ehwqpu.com

[T10] Kotlin：默认参数
来源：http://nne.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nai.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://tnb.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://sxm.chenjidiqi.icu

[T12] Kotlin：解构声明
来源：http://ivn.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://xtf.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://tnx.jianghu66.top

val m = mapOf("a" to 1)
来源：http://mgu.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://vvc.yj202588.top

for (i in 1..10) println(i)
来源：http://imz.redwolf501.top

[T15] Kotlin：接口
来源：http://iec.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://svz.tanke756.top

[T16] Swift：Hello World
来源：http://tet.fzhhl.top

print("Hello")
来源：http://hto.guowangkeji.top

[T17] Swift：变量与常量
来源：http://rbw.guannengcc.top

var a = 1;  let b = 2
来源：http://xnl.uphjek.com

[T18] Swift：字符串插值
来源：http://maw.tarul.cn

"值: \(b)"
来源：http://qxa.c1oappe.top

[T19] Swift：可选绑定
来源：http://gxz.kuanghao11.cn

if let n = opt { print(n) }
来源：http://uob.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://qdx.yangfankeji.com

var a = [1, 2, 3];  a.append(4)
来源：http://iwq.birdmap.top

[T21] Swift：遍历
来源：http://jap.jinghuilouyu.cn

for x in a { print(x) }
来源：http://tzm.fehbvm.com

[T22] Swift：字典
来源：http://ett.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uap.52xcode.cn

[T23] Swift：函数
来源：http://nwy.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yjv.aibaodan.cn

[T24] Swift：闭包
来源：http://dje.shanyushiyangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zly.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://olu.zdbjq.cn

struct P { var x: Int }
来源：http://vnu.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://pws.shanyushiyangtech.top

class A: Base { override func f() {} }
来源：http://hjn.vqdsnc.cn

[T27] Swift：错误处理
来源：http://qid.yuanzhike.top

do { try f() } catch { print(error) }
来源：http://tcp.snrcjt.cn

[T28] Swift：枚举
来源：http://atk.ivvv.top

enum Color { case red, green }
来源：http://izf.havefunace.top

[T29] Swift：guard 提前返回
来源：http://pdf.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://rej.zhixingplan.top

[T30] Swift：协议
来源：http://mps.zycfv.cn

protocol Shape { func area() -> Double }
来源：http://uvu.ctjpmb.com

[T31] Lua：Hello World
来源：http://lho.jiagoushi.top

print("Hello")
来源：http://coe.xziqi.cn

[T32] Lua：局部变量
来源：http://kbo.xinyue.icu

local a = 1
来源：http://fle.c1oappe.top

[T33] Lua：表（数组）
来源：http://lxd.xuanzx.com

local t = {1, 2, 3};  t[4] = 4
来源：http://yvi.nanxuanxn.top

[T34] Lua：遍历表
来源：http://yyx.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cis.hywenlv.cn

[T35] Lua：字典表
来源：http://ixm.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://ltq.gaohongyu789.top

[T36] Lua：函数
来源：http://zkm.shangyingyoupin.top

function add(a, b) return a + b end
来源：http://pil.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://lnx.zhaomingkeji.xyz

"a" .. "b"
来源：http://ynd.vehdjk.com

[T38] Lua：条件
来源：http://amu.yuanzhike.top

if x > 0 then print("正") end
来源：http://elc.zhijiandao.cn

[T39] Lua：模式匹配
来源：http://tpe.zhengqikj.top

string.find(s, "%d+")
来源：http://lim.zhongyouzk.top

[T40] Lua：元表
来源：http://nvx.iojbl.cn

setmetatable({}, { __index = base })
来源：http://avj.yuanzhike.top

[T41] Perl：Hello World
来源：http://jvc.sxryk.cn

print "Hello\n";
来源：http://jha.kuanghao11.cn

[T42] Perl：变量类型
来源：http://eti.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uaj.yangfankeji.com

[T43] Perl：字符串插值
来源：http://ltg.yj202588.top

"值: $a"
来源：http://znz.zhongyouzk.top

[T44] Perl：条件
来源：http://uzv.tarul.cn

if ($a > 0) { print "正"; }
来源：http://mle.zhixingplan.top

[T45] Perl：数组遍历
来源：http://mdc.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://shs.zdbjq.cn

[T46] Perl：哈希操作
来源：http://uzn.svipenyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pjf.hcnkem.com

[T47] Perl：正则捕获
来源：http://ptj.yuxming.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vkb.gotoacloud.top

[T48] Perl：正则替换
来源：http://xvk.havefunace.top

$s =~ s/old/new/g;
来源：http://qiy.wangdashe.top

[T49] Perl：函数
来源：http://vpd.vqdsnc.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cxs.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://zog.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vic.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://qxo.sjlbkw.cn

[T51] Scala：Hello World
来源：http://mhr.yuanzhike.top

println("Hello")
来源：http://eaz.nwbrower.top

[T52] Scala：变量
来源：http://moa.cucudq.cn

val a = 1;  var b = 2
来源：http://its.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://oay.yvedp.cn

s"值: $b"
来源：http://xwy.gzhubu.top

[T54] Scala：集合映射
来源：http://wrb.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://wdg.zhixingplan.top

[T55] Scala：集合过滤
来源：http://msw.chenzaomai.com

List(1, 2, 3).filter(_ > 1)
来源：http://jks.uphjek.com

[T56] Scala：样例类
来源：http://zke.zycfv.cn

case class User(name: String, age: Int)
来源：http://uvh.zhengqikj.top

[T57] Scala：模式匹配
来源：http://kyg.fktsv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kom.nanxinkj.top

[T58] Scala：函数定义
来源：http://sfl.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://rxc.nwbrower.top

[T59] Scala：循环
来源：http://ryk.wangdashe.top

for (i <- 1 to 10) println(i)
来源：http://nql.cdnleiting.top

[T60] Scala：折叠
来源：http://cvv.daxiang520.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zoj.sufxvd.cn

================================================================================
来源：http://vft.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kmq.xylfe.cn

================================================================================
来源：http://ixj.yuxming.cn

[U01] Py：创建虚拟环境
来源：http://jwx.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://lnh.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://fib.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ard.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://qoj.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kfk.fehbvm.com

[U04] Py：变量调试打印
来源：http://eus.shzxlz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pvx.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://ngn.sysykeji.top

list(dict.fromkeys(arr))
来源：http://qsc.sysykeji.top

[U06] Py：合并两个字典
来源：http://oea.zhiwuduotai.top

{**a, **b}
来源：http://dvv.jiagoushi.top

[U07] Py：反转字典键值
来源：http://vag.bjfxy.top

{v: k for k, v in d.items()}
来源：http://kuf.yongpay.top

[U08] Py：展平二维列表
来源：http://uxa.andypj.xyz

[y for x in nested for y in x]
来源：http://ydg.xylfe.cn

[U09] Py：字典取最大值的键
来源：http://sdm.hongshengwenyu.top

max(d, key=d.get)
来源：http://hjz.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://fkf.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qmz.hywenlv.cn

[U11] Py：生成器表达式
来源：http://ubj.haohaochexian.top

(x * 2 for x in arr)
来源：http://gla.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://blz.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://uww.ivvv.top

[U13] Py：固定长度队列
来源：http://vjd.tian-w.cn

deque(maxlen=10)
来源：http://nho.hammf.cn

[U14] Py：分组收集到列表
来源：http://jdo.iojbl.cn

defaultdict(list)
来源：http://bnk.9152youxi.cn

[U15] Py：高精度计时
来源：http://egb.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://nvd.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://ipo.zhixingplan.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ycj.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://eev.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://vab.yuxming.cn

[U18] Py：预编译正则
来源：http://zzt.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://fij.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://xmx.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://awt.yueranfly.top

[U20] Py：缓存函数结果
来源：http://mtd.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://myu.pycfn.com

[U21] Py：自定义上下文管理器
来源：http://ith.yonumen.top

@contextlib.contextmanager
来源：http://uav.yj20258888.top

[U22] Py：矩阵转置
来源：http://unt.hcnkem.com

list(zip(*m))
来源：http://pvl.ydjk.org.cn

[U23] Py：分块读取大文件
来源：http://fcs.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nax.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://pxo.gaohongyu789.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vor.jqgfzy.top

[U25] Py：CSV 按字典读
来源：http://sbx.xuetiantiany.cn

csv.DictReader(f)
来源：http://jnn.yj202588.top

[U26] Py：并发下载
来源：http://eer.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ovu.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://znj.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://zex.shzxlz.cn

[U28] Py：类型别名
来源：http://ovn.vqdsnc.cn

UserId = int
来源：http://lqd.sjlbkw.cn

[U29] Py：属性校验
来源：http://fee.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://jxd.hnxiangtu.top

[U30] Py：数据类
来源：http://dju.aibaodan.cn

@dataclass(slots=True)
来源：http://lns.chenlongwang.top

[U31] Py：单测
来源：http://kqs.redwolf501.top

python -m pytest -q
来源：http://mru.zhengqikj.top

[U32] Py：代码格式化
来源：http://ccd.birdmap.top

ruff format . && ruff check --fix .
来源：http://eog.aibaodan.cn

[U33] Py：打包发布
来源：http://hbn.shuidangran.top

python -m build  （依赖 pyproject.toml）
来源：http://kqf.chenjidiqi.icu

[U34] Py：判断编码
来源：http://tpv.daria6918.cn

chardet.detect(raw)
来源：http://qwo.gaohongyu789.top

[U35] Py：发送邮件
来源：http://bvl.jqgufenzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jap.tianlin.xyz

[U36] Py：定时任务
来源：http://agn.sysykeji.top

schedule.every(10).minutes.do(job)
来源：http://tfe.dashuyun.cn

[U37] Py：读写 Excel
来源：http://xvr.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://hdn.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://wtn.shzxlz.cn

Path(__file__).resolve().parent
来源：http://wou.sufxvd.cn

[U39] Py：判断是否在交互环境
来源：http://yar.tanke756.top

sys.stdout.isatty()
来源：http://nyu.yj20258888.top

[U40] Py：打印到标准错误
来源：http://ame.cheryme.top

print("err", file=sys.stderr)
来源：http://rdz.zhongyouzk.top

[U41] PHP：初始化 Composer 项目
来源：http://diu.jqgfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://klf.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://zqm.bbcook.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lre.fktsv.cn

[U43] PHP：声明命名空间
来源：http://yjz.snrcjt.cn

namespace App\Http;
来源：http://vyu.havefunace.top

[U44] PHP：开启严格类型
来源：http://zqm.cashguo.top

declare(strict_types=1);
来源：http://fyj.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://rik.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://anp.nwbrower.top

[U46] PHP：可空类型
来源：http://twv.ppjwa.cn

?string $name = null
来源：http://kul.iojbl.cn

[U47] PHP：联合类型
来源：http://ozp.hfpthk.cn

int|string $id
来源：http://ozc.zdbjq.cn

[U48] PHP：纯枚举
来源：http://qbo.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mjy.xziqi.cn

[U49] PHP：只读属性
来源：http://uix.yonumen.top

public readonly string $name
来源：http://pfa.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://eee.yj20258888.top

public function __construct(private int $id) {}
来源：http://wfo.yj202588.top

[U51] PHP：数组解构
来源：http://lwr.zhixingplan.top

[$a, $b] = $arr;
来源：http://krz.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://kfb.aizwys.cn

$double = fn($x) => $x * 2;
来源：http://fcg.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://fxf.wangshuangyany.cn

$v = $a ?? $b ?? "default";
来源：http://vft.redwolf501.top

[U54] PHP：空安全调用
来源：http://sih.hfpthk.cn

$obj?->method()
来源：http://vds.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://enn.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tac.zhoulong.xyz

[U56] PHP：命名参数
来源：http://shn.sweek.top

f(a: 1, b: 2)
来源：http://gpz.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://otj.mhx1999.top

"值: {$a}"
来源：http://vgp.nanxinkj.top

[U58] PHP：数组三件套
来源：http://bwd.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://klv.jianghu66.top

[U59] PHP：自定义排序
来源：http://coz.ybcxt.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bva.haohaochexian.top

[U60] PHP：JSON 编解码
来源：http://cko.tanke756.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ddu.cqqwz.cn

[U61] PHP：正则
来源：http://nwo.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sui.zhongyouzk.top

[U62] PHP：日期对象
来源：http://pdg.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yeg.0kj1m.cn

[U63] PHP：文件读写
来源：http://cao.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vtx.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://cqg.ybcxt.top

glob("dir/*.php");  scandir("dir");
来源：http://cfh.andypj.xyz

[U65] PHP：会话
来源：http://ieo.smart0.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://qyg.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://ial.yvedp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vlz.yueranfly.top

[U67] PHP：处理文件上传
来源：http://dsn.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bwr.0kj1m.cn

[U68] PHP：PDO 连接
来源：http://yqy.zhoulong.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.shzxlz.cn

[U69] PHP：PDO 预处理
来源：http://npz.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jho.pengpengdd.cyou

[U70] PHP：PDO 事务
来源：http://yte.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://swe.chenlongwang.top

[U71] PHP：抛出异常
来源：http://hvr.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://qjp.fanxiaobao.xyz

[U72] PHP：写错误日志
来源：http://zux.pengpengdd.cyou

error_log("失败: " . $e->getMessage());
来源：http://fbc.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://wah.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://tpn.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://woe.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://xco.yanxiufei.cn

[U75] PHP：依赖注入
来源：http://yac.epnwcf.com

composer require psr/container
来源：http://apo.0kj1m.cn

[U76] PHP：简单路由
来源：http://sfo.xingfuxueyuan.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wsc.zycfv.cn

[U77] PHP：模板渲染
来源：http://itw.zhengqikj.top

composer require twig/twig
来源：http://srj.tarul.cn

[U78] PHP：单元测试
来源：http://jch.sweek.top

composer require --dev phpunit/phpunit
来源：http://bcs.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://kru.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://zdw.uphjek.com

[U80] PHP：代码规范修复
来源：http://okp.yongpay.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jzw.yvedp.cn

[U81] JS：初始化项目
来源：http://aip.tian-w.cn

npm init -y;  npm i express
来源：http://wqj.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://bnx.yvedp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fzg.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://srz.shuidangran.top

export const a = 1;  import { a } from "./m.js";
来源：http://psa.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://dmm.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://rtl.hesvh.cn

[U85] JS：可选链
来源：http://efv.havefunace.top

a?.b?.c
来源：http://knb.ivvv.top

[U86] JS：空值合并
来源：http://rbj.tanke756.top

a ?? b
来源：http://wir.haohaochexian.top

[U87] JS：解构默认值
来源：http://krf.iojbl.cn

const { a = 1, b = 2 } = obj;
来源：http://eiv.shuidangran.top

[U88] JS：对象展开合并
来源：http://tcy.hesvh.cn

{ ...a, ...b }
来源：http://cyq.epnwcf.com

[U89] JS：数组去重
来源：http://rtu.yongpay.top

[...new Set(arr)]
来源：http://swt.hfpthk.cn

[U90] JS：数字数组排序
来源：http://dxb.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://sjo.cdnleiting.top

[U91] JS：对象键值遍历
来源：http://xwa.daxiang520.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jss.hcnkem.com

[U92] JS：深拷贝
来源：http://oaa.sufxvd.cn

structuredClone(obj)
来源：http://hlg.guowangkeji.top


<!-- 参考信息 -->