代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ftp.zhiwuduotai.top

================================================================================
来源：http://wyx.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lrs.jqgfzy.top

================================================================================
来源：http://poq.meibo888.top

[T01] Kotlin：Hello World
来源：http://gnv.cheryme.top

println("Hello")
来源：http://daw.cheryme.top

[T02] Kotlin：变量
来源：http://jbw.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ocd.yonumen.top

[T03] Kotlin：字符串模板
来源：http://dee.andypj.xyz

"值: $b"
来源：http://jla.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://pyc.gotoacloud.top

val n: String? = null;  n?.length
来源：http://yzr.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://wrc.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://chk.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://xva.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wdm.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://elf.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://btw.wangdashe.top

[T08] Kotlin：数据类
来源：http://xxi.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://uvf.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://tzl.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://ajc.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://fpt.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pyy.fehbvm.com

[T11] Kotlin：协程
来源：http://yrp.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mao.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://hba.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://ntv.daria6918.cn

[T13] Kotlin：只读 Map
来源：http://urg.sysykeji.top

val m = mapOf("a" to 1)
来源：http://piz.yj20258888.top

[T14] Kotlin：循环
来源：http://fhm.hcnkem.com

for (i in 1..10) println(i)
来源：http://ysp.redwolf501.top

[T15] Kotlin：接口
来源：http://wbv.iojbl.cn

interface Shape { fun area(): Double }
来源：http://cww.fengsongda.top

[T16] Swift：Hello World
来源：http://epu.smart0.xyz

print("Hello")
来源：http://bqd.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://ejo.fktsv.cn

var a = 1;  let b = 2
来源：http://zxe.jinqigufen.top

[T18] Swift：字符串插值
来源：http://vub.haohaochexian.top

"值: \(b)"
来源：http://zdk.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://fsn.sysykeji.top

if let n = opt { print(n) }
来源：http://fgm.smart0.xyz

[T20] Swift：数组操作
来源：http://awm.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://fob.feifeiyinyue.top

[T21] Swift：遍历
来源：http://kik.jlsjyb.cn

for x in a { print(x) }
来源：http://yan.zhoulong.xyz

[T22] Swift：字典
来源：http://xxc.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://dtc.xinyue.icu

[T23] Swift：函数
来源：http://div.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mwz.xinyue.icu

[T24] Swift：闭包
来源：http://bbw.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fmw.guannengcc.top

[T25] Swift：结构体
来源：http://vyi.wangshuangyany.cn

struct P { var x: Int }
来源：http://mhe.yanxiufei.cn

[T26] Swift：类与重写
来源：http://ddq.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://lvx.epnwcf.com

[T27] Swift：错误处理
来源：http://jvv.yuxming.cn

do { try f() } catch { print(error) }
来源：http://zmi.xuetiantiany.cn

[T28] Swift：枚举
来源：http://qlj.52xcode.cn

enum Color { case red, green }
来源：http://lma.smart0.xyz

[T29] Swift：guard 提前返回
来源：http://rhm.havefunace.top

guard let x = opt else { return }
来源：http://fna.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://jhf.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://nmv.nanxuanxn.top

[T31] Lua：Hello World
来源：http://efl.tian-w.cn

print("Hello")
来源：http://uod.yongpay.top

[T32] Lua：局部变量
来源：http://lcb.sufxvd.cn

local a = 1
来源：http://qth.birdmap.top

[T33] Lua：表（数组）
来源：http://nxe.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tcz.yuxming.cn

[T34] Lua：遍历表
来源：http://abt.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://agc.yfazqb.com

[T35] Lua：字典表
来源：http://rdf.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://ssl.nanxinkj.top

[T36] Lua：函数
来源：http://yue.vqdsnc.cn

function add(a, b) return a + b end
来源：http://agk.jqgufenzy.top

[T37] Lua：字符串拼接
来源：http://ejb.nwbrower.top

"a" .. "b"
来源：http://qbm.yj20258.top

[T38] Lua：条件
来源：http://ssz.meibo888.top

if x > 0 then print("正") end
来源：http://eig.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://doe.cqqwz.cn

string.find(s, "%d+")
来源：http://hfu.ybcxt.top

[T40] Lua：元表
来源：http://iqa.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://tqm.hysaishi.cn

[T41] Perl：Hello World
来源：http://jax.yanxiufei.cn

print "Hello\n";
来源：http://ird.nwbrower.top

[T42] Perl：变量类型
来源：http://cog.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://euc.ehwqpu.com

[T43] Perl：字符串插值
来源：http://fjs.bbcook.cn

"值: $a"
来源：http://lpp.zhiwuduotai.top

[T44] Perl：条件
来源：http://rmy.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://reo.gotoacloud.top

[T45] Perl：数组遍历
来源：http://zem.uphjek.com

for my $x (@arr) { print $x; }
来源：http://fam.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://onk.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mdm.shanyushiyangkeji.top

[T47] Perl：正则捕获
来源：http://piv.hywenlv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ily.yueranfly.top

[T48] Perl：正则替换
来源：http://oua.sweek.top

$s =~ s/old/new/g;
来源：http://mhs.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://iuf.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ftj.hnqzz.top

[T50] Perl：逐行读文件
来源：http://fnz.zhongyouzk.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zjk.yonumen.top

while (my $line = <$fh>) { print $line; }
来源：http://vud.nwbrower.top

[T51] Scala：Hello World
来源：http://jfy.cucudq.cn

println("Hello")
来源：http://oak.zhengqikj.top

[T52] Scala：变量
来源：http://gbx.fanxiaobao.xyz

val a = 1;  var b = 2
来源：http://qkm.nwbrower.top

[T53] Scala：字符串插值
来源：http://zzd.zdbjq.cn

s"值: $b"
来源：http://zev.aizwys.cn

[T54] Scala：集合映射
来源：http://kbd.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://wmg.gogol.net.cn

[T55] Scala：集合过滤
来源：http://nye.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://ppy.zhiwuduotai.top

[T56] Scala：样例类
来源：http://ugo.zycfv.cn

case class User(name: String, age: Int)
来源：http://smo.xinyue.icu

[T57] Scala：模式匹配
来源：http://xyg.tian-w.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://teh.chenzaomai.com

[T58] Scala：函数定义
来源：http://boz.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://yjm.ehwqpu.com

[T59] Scala：循环
来源：http://gda.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://tij.svipenyu.cn

[T60] Scala：折叠
来源：http://asf.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ryx.shzxlz.cn

================================================================================
来源：http://evt.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gch.fehbvm.com

================================================================================
来源：http://ngu.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://soa.nanxinkj.top

python -m venv .venv && source .venv/bin/activate
来源：http://mdz.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://tch.yanxiufei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://olo.smart0.xyz

[U03] Py：加载 .env 配置
来源：http://nnl.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ezt.redwolf501.top

[U04] Py：变量调试打印
来源：http://hnw.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zuv.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://ofp.daxiang520.top

list(dict.fromkeys(arr))
来源：http://hdi.yangfankeji.com

[U06] Py：合并两个字典
来源：http://unj.bjfxy.top

{**a, **b}
来源：http://nef.fengsongda.top

[U07] Py：反转字典键值
来源：http://jad.hnqzz.top

{v: k for k, v in d.items()}
来源：http://eol.quarkkingdee.top

[U08] Py：展平二维列表
来源：http://rgd.tanke756.top

[y for x in nested for y in x]
来源：http://gkw.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://zbx.chenzaomai.com

max(d, key=d.get)
来源：http://mju.haohaochexian.top

[U10] Py：按值排序字典
来源：http://cdf.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zem.yueranfly.top

[U11] Py：生成器表达式
来源：http://qta.sufxvd.cn

(x * 2 for x in arr)
来源：http://rsy.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://eyh.jinqigufen.top

Counter(arr).most_common(3)
来源：http://qws.zhaomingkeji.xyz

[U13] Py：固定长度队列
来源：http://asz.daxiang520.top

deque(maxlen=10)
来源：http://ykc.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://fki.havefunace.top

defaultdict(list)
来源：http://soi.hnxiangtu.top

[U15] Py：高精度计时
来源：http://fie.snrcjt.cn

t = time.perf_counter()
来源：http://trp.haohaochexian.top

[U16] Py：命令行参数解析
来源：http://ilw.guannengcc.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ess.zdqjudy.top

[U17] Py：初始化日志
来源：http://ddg.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://rus.yuxming.cn

[U18] Py：预编译正则
来源：http://rcm.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://ylx.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://osf.aizwys.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uxb.yvedp.cn

[U20] Py：缓存函数结果
来源：http://hvr.tianlin.xyz

@functools.lru_cache(maxsize=None)
来源：http://plm.sjlbkw.cn

[U21] Py：自定义上下文管理器
来源：http://nqe.wangdashe.top

@contextlib.contextmanager
来源：http://mdp.ybcxt.top

[U22] Py：矩阵转置
来源：http://vdl.hcnkem.com

list(zip(*m))
来源：http://atl.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://ifi.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fem.yvedp.cn

[U24] Py：路径操作
来源：http://hly.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hma.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://yns.yj202588.top

csv.DictReader(f)
来源：http://zju.yuxming.cn

[U26] Py：并发下载
来源：http://dym.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oui.vehdjk.com

[U27] Py：异步 HTTP
来源：http://gtu.meibo888.top

aiohttp.ClientSession() 配合 async with
来源：http://kyb.hnqzz.top

[U28] Py：类型别名
来源：http://eiz.wangdashe.top

UserId = int
来源：http://vxv.xuanzx.com

[U29] Py：属性校验
来源：http://ccq.aibaodan.cn

@property 与 @x.setter 配合
来源：http://xoj.chenjidiqi.icu

[U30] Py：数据类
来源：http://mzj.yuanzhike.top

@dataclass(slots=True)
来源：http://zus.zdqjudy.top

[U31] Py：单测
来源：http://rgc.ybcxt.top

python -m pytest -q
来源：http://xne.yuanzhike.top

[U32] Py：代码格式化
来源：http://wwj.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://wxm.316326.xyz

[U33] Py：打包发布
来源：http://gvi.jlsjyb.cn

python -m build  （依赖 pyproject.toml）
来源：http://kwp.aibaodan.cn

[U34] Py：判断编码
来源：http://jco.andypj.xyz

chardet.detect(raw)
来源：http://doe.yvedp.cn

[U35] Py：发送邮件
来源：http://sad.fktsv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ftu.aizwys.cn

[U36] Py：定时任务
来源：http://ewp.jqgufenzy.top

schedule.every(10).minutes.do(job)
来源：http://qas.birdmap.top

[U37] Py：读写 Excel
来源：http://lgm.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://sti.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://szb.fengsongda.top

Path(__file__).resolve().parent
来源：http://vti.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://kia.cheryme.top

sys.stdout.isatty()
来源：http://gbe.yvedp.cn

[U40] Py：打印到标准错误
来源：http://oqd.zycfv.cn

print("err", file=sys.stderr)
来源：http://bib.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://eui.bjfxy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://opo.haohaochexian.top

[U42] PHP：PSR-4 自动加载
来源：http://eyd.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zuk.nanxuanxn.top

[U43] PHP：声明命名空间
来源：http://srt.xylfe.cn

namespace App\Http;
来源：http://qsa.cqqwz.cn

[U44] PHP：开启严格类型
来源：http://cng.zhongyouzk.top

declare(strict_types=1);
来源：http://gco.tarul.cn

[U45] PHP：类型声明与返回类型
来源：http://fjl.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://gpc.hfpthk.cn

[U46] PHP：可空类型
来源：http://qem.hnqzz.top

?string $name = null
来源：http://fmm.yj20258888.top

[U47] PHP：联合类型
来源：http://qnp.cashguo.top

int|string $id
来源：http://oui.jinqigfzy.top

[U48] PHP：纯枚举
来源：http://nlt.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tgc.fktsv.cn

[U49] PHP：只读属性
来源：http://fru.smart0.xyz

public readonly string $name
来源：http://nmx.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://eej.jianghu66.top

public function __construct(private int $id) {}
来源：http://jjp.gotoacloud.top

[U51] PHP：数组解构
来源：http://qiu.uphjek.com

[$a, $b] = $arr;
来源：http://glp.xingfuxueyuan.xyz

[U52] PHP：箭头函数
来源：http://cdz.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://nna.zdqjudy.top

[U53] PHP：空合并运算符
来源：http://ndx.jqgufenzy.top

$v = $a ?? $b ?? "default";
来源：http://dha.yj202588.top

[U54] PHP：空安全调用
来源：http://axw.shuidangran.top

$obj?->method()
来源：http://swb.shuidangran.top

[U55] PHP：match 表达式
来源：http://tlh.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xyg.bjfxy.top

[U56] PHP：命名参数
来源：http://yke.wangshuangyany.cn

f(a: 1, b: 2)
来源：http://vir.nanxinkj.top

[U57] PHP：字符串插值
来源：http://xxc.jinyuanbaomall.cn

"值: {$a}"
来源：http://tlp.shuidangran.top

[U58] PHP：数组三件套
来源：http://afy.sufxvd.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wzc.9152youxi.cn

[U59] PHP：自定义排序
来源：http://xuo.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jsp.fzhhl.top

[U60] PHP：JSON 编解码
来源：http://qfn.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lsf.xuetiantiany.cn

[U61] PHP：正则
来源：http://wpf.jqgfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://akc.cheryme.top

[U62] PHP：日期对象
来源：http://ycu.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gyy.andypj.xyz

[U63] PHP：文件读写
来源：http://pzt.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qqk.bjfxy.top

[U64] PHP：目录遍历
来源：http://ixo.bjfxy.top

glob("dir/*.php");  scandir("dir");
来源：http://rnf.chenjidiqi.icu

[U65] PHP：会话
来源：http://xuv.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://eno.xinyue.icu

[U66] PHP：设置 Cookie
来源：http://aek.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kum.hongshengwenyu.top

[U67] PHP：处理文件上传
来源：http://gmg.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hbz.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://moi.shuidangran.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rib.shuidangran.top

[U69] PHP：PDO 预处理
来源：http://enz.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fuw.hnqzz.top

[U70] PHP：PDO 事务
来源：http://abd.vehdjk.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://abk.daria6918.cn

[U71] PHP：抛出异常
来源：http://ftb.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://cfa.0kj1m.cn

[U72] PHP：写错误日志
来源：http://nke.pycfn.com

error_log("失败: " . $e->getMessage());
来源：http://jut.yuxming.cn

[U73] PHP：读取 ini 配置
来源：http://vsd.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://pmk.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://tfr.jinqigufen.top

getenv("APP_ENV") ?: "production"
来源：http://dbf.birdmap.top

[U75] PHP：依赖注入
来源：http://iev.yanxiufei.cn

composer require psr/container
来源：http://ilp.cqqwz.cn

[U76] PHP：简单路由
来源：http://rng.kuanghao11.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bjs.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://izt.ywan-chungtsiang.top

composer require twig/twig
来源：http://fae.hywenlv.cn

[U78] PHP：单元测试
来源：http://all.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://gjo.yongpay.top

[U79] PHP：静态分析
来源：http://gqx.jinyuanbaomall.cn

composer require --dev phpstan/phpstan
来源：http://ibk.bbcook.cn

[U80] PHP：代码规范修复
来源：http://wtr.bbcook.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sif.shangyingyoupin.top

[U81] JS：初始化项目
来源：http://zgg.jinqigufen.top

npm init -y;  npm i express
来源：http://ckk.shuidangran.top

[U82] JS：package.json 脚本
来源：http://scd.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sje.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://nxx.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dwj.xziqi.cn

[U84] JS：CommonJS 写法
来源：http://idh.hfpthk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fqo.9152youxi.cn

[U85] JS：可选链
来源：http://ott.ydzc1.top

a?.b?.c
来源：http://llb.smart0.xyz

[U86] JS：空值合并
来源：http://hev.ppjwa.cn

a ?? b
来源：http://kap.vehdjk.com


<!-- 参考信息 -->