代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bpw.cucudq.cn

================================================================================
来源：http://dnn.dashuyun.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ovz.zhoulong.xyz

================================================================================
来源：http://ulk.yfazqb.com

[T01] Kotlin：Hello World
来源：http://uux.shuidangran.top

println("Hello")
来源：http://kie.zhengqikj.top

[T02] Kotlin：变量
来源：http://nob.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oyh.c1oappe.top

[T03] Kotlin：字符串模板
来源：http://jgc.cqqwz.cn

"值: $b"
来源：http://fgr.havefunace.top

[T04] Kotlin：空安全
来源：http://dco.chenlongwang.top

val n: String? = null;  n?.length
来源：http://hvf.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://eop.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mhk.zhongyouzk.top

[T06] Kotlin：集合映射
来源：http://nmr.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nft.wangshuangyany.cn

[T07] Kotlin：集合过滤
来源：http://dsx.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://seu.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://tfc.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://upe.sweek.top

[T09] Kotlin：扩展函数
来源：http://wxq.cashguo.top

fun String.exclaim() = this + "!"
来源：http://ogl.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://otj.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lif.xinyue.icu

[T11] Kotlin：协程
来源：http://sxg.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rdf.havefunace.top

[T12] Kotlin：解构声明
来源：http://adf.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://oua.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://fsn.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://wya.yj20258888.top

[T14] Kotlin：循环
来源：http://xlp.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://dzf.ctjpmb.com

[T15] Kotlin：接口
来源：http://hhj.shanyushiyangkeji.top

interface Shape { fun area(): Double }
来源：http://ine.0kj1m.cn

[T16] Swift：Hello World
来源：http://fym.xuanzx.com

print("Hello")
来源：http://fzj.fehbvm.com

[T17] Swift：变量与常量
来源：http://ndp.sxryk.cn

var a = 1;  let b = 2
来源：http://jzu.316326.xyz

[T18] Swift：字符串插值
来源：http://rrp.yuanzhike.top

"值: \(b)"
来源：http://zju.zycfv.cn

[T19] Swift：可选绑定
来源：http://pvj.pycfn.com

if let n = opt { print(n) }
来源：http://jwz.aizwys.cn

[T20] Swift：数组操作
来源：http://ejl.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lnv.kuanghao11.cn

[T21] Swift：遍历
来源：http://nlw.wangdashe.top

for x in a { print(x) }
来源：http://jba.xinyue.icu

[T22] Swift：字典
来源：http://rwd.nwbrower.top

var d = ["a": 1];  d["b"] = 2
来源：http://vsv.xylfe.cn

[T23] Swift：函数
来源：http://tar.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wxs.yfazqb.com

[T24] Swift：闭包
来源：http://jsv.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mae.yvedp.cn

[T25] Swift：结构体
来源：http://hkb.jianghu66.top

struct P { var x: Int }
来源：http://epc.0kj1m.cn

[T26] Swift：类与重写
来源：http://oft.0kj1m.cn

class A: Base { override func f() {} }
来源：http://nfc.jinqigufen.top

[T27] Swift：错误处理
来源：http://zdy.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://puk.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://ndl.chenlongwang.top

enum Color { case red, green }
来源：http://kkw.nanxinkj.top

[T29] Swift：guard 提前返回
来源：http://mxu.ydzc1.top

guard let x = opt else { return }
来源：http://mnm.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://vht.pycfn.com

protocol Shape { func area() -> Double }
来源：http://njz.hammf.cn

[T31] Lua：Hello World
来源：http://pds.aibaodan.cn

print("Hello")
来源：http://dpi.yj20258888.top

[T32] Lua：局部变量
来源：http://jxa.yj202588.top

local a = 1
来源：http://mef.ivvv.top

[T33] Lua：表（数组）
来源：http://tew.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dhq.316326.xyz

[T34] Lua：遍历表
来源：http://jxf.zhiwuduotai.top

for i, v in ipairs(t) do print(i, v) end
来源：http://edi.pycfn.com

[T35] Lua：字典表
来源：http://fzz.wangdashe.top

local d = { a = 1 };  d.b = 2
来源：http://xnz.ydjk.org.cn

[T36] Lua：函数
来源：http://zfd.zhoulong.xyz

function add(a, b) return a + b end
来源：http://moi.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://kyx.daxiang520.top

"a" .. "b"
来源：http://gvi.andypj.xyz

[T38] Lua：条件
来源：http://tiv.chenlongwang.top

if x > 0 then print("正") end
来源：http://jhy.shanyushiyangkeji.top

[T39] Lua：模式匹配
来源：http://xjc.zhongyouzk.top

string.find(s, "%d+")
来源：http://ojv.jiagoushi.top

[T40] Lua：元表
来源：http://lyu.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://wng.meibo888.top

[T41] Perl：Hello World
来源：http://vze.ydzc1.top

print "Hello\n";
来源：http://ylj.dashuyun.cn

[T42] Perl：变量类型
来源：http://qqy.bbcook.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://czl.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://gol.svipenyu.cn

"值: $a"
来源：http://ddu.jinqigfzy.top

[T44] Perl：条件
来源：http://jmd.cashguo.top

if ($a > 0) { print "正"; }
来源：http://nrj.vehdjk.com

[T45] Perl：数组遍历
来源：http://bac.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://pzb.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://edr.chenzaomai.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yev.sufxvd.cn

[T47] Perl：正则捕获
来源：http://gzn.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zoq.yonumen.top

[T48] Perl：正则替换
来源：http://ycu.cdnleiting.top

$s =~ s/old/new/g;
来源：http://nlc.jlsjyb.cn

[T49] Perl：函数
来源：http://lof.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://for.zhijiandao.cn

[T50] Perl：逐行读文件
来源：http://rgm.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ege.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://pyl.xinyue.icu

[T51] Scala：Hello World
来源：http://dbb.fktsv.cn

println("Hello")
来源：http://tvz.chenzaomai.com

[T52] Scala：变量
来源：http://fqf.guannengcc.top

val a = 1;  var b = 2
来源：http://arx.yongpay.top

[T53] Scala：字符串插值
来源：http://pxz.jianghu66.top

s"值: $b"
来源：http://hoz.zhengqikj.top

[T54] Scala：集合映射
来源：http://gxr.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://dkp.nanxuanxn.top

[T55] Scala：集合过滤
来源：http://wyy.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://hnw.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://nqc.ivvv.top

case class User(name: String, age: Int)
来源：http://sob.smart0.xyz

[T57] Scala：模式匹配
来源：http://euv.wangdashe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://usq.9152youxi.cn

[T58] Scala：函数定义
来源：http://ytu.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://vca.mhx1999.top

[T59] Scala：循环
来源：http://con.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://sao.xziqi.cn

[T60] Scala：折叠
来源：http://ajw.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ukp.zdqjudy.top

================================================================================
来源：http://gbe.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://azl.fzhhl.top

================================================================================
来源：http://chp.jqgufenzy.top

[U01] Py：创建虚拟环境
来源：http://ejk.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://rig.pycfn.com

[U02] Py：导出 / 安装依赖
来源：http://ipo.ybcxt.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://imt.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://vey.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://byf.yj202588.top

[U04] Py：变量调试打印
来源：http://qqx.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gqx.fzhhl.top

[U05] Py：列表去重且保序
来源：http://lzx.fehbvm.com

list(dict.fromkeys(arr))
来源：http://sxm.fktsv.cn

[U06] Py：合并两个字典
来源：http://xug.0kj1m.cn

{**a, **b}
来源：http://tbf.shanyushiyangkeji.top

[U07] Py：反转字典键值
来源：http://dkv.0kj1m.cn

{v: k for k, v in d.items()}
来源：http://nsq.bbcook.cn

[U08] Py：展平二维列表
来源：http://wsg.fktsv.cn

[y for x in nested for y in x]
来源：http://xer.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://cjb.yvedp.cn

max(d, key=d.get)
来源：http://pxd.nanxinkj.top

[U10] Py：按值排序字典
来源：http://afj.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pne.sysykeji.top

[U11] Py：生成器表达式
来源：http://zdn.cheryme.top

(x * 2 for x in arr)
来源：http://tcu.cqqwz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rvi.jiagoushi.top

Counter(arr).most_common(3)
来源：http://xzr.guowangkeji.top

[U13] Py：固定长度队列
来源：http://pti.yanxiufei.cn

deque(maxlen=10)
来源：http://dow.yongpay.top

[U14] Py：分组收集到列表
来源：http://tjr.yuxming.cn

defaultdict(list)
来源：http://goa.shzxlz.cn

[U15] Py：高精度计时
来源：http://dkz.gaohongyu789.top

t = time.perf_counter()
来源：http://ufg.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://cqs.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eqw.zycfv.cn

[U17] Py：初始化日志
来源：http://mna.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://pyn.zhijiandao.cn

[U18] Py：预编译正则
来源：http://wby.gzhubu.top

pat = re.compile(r"\d+")
来源：http://ufj.jianghu66.top

[U19] Py：正则替换带回调
来源：http://qyl.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://peq.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://jtb.shangyingyoupin.top

@functools.lru_cache(maxsize=None)
来源：http://ccq.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://nep.chenjidiqi.icu

@contextlib.contextmanager
来源：http://lhn.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://xwi.ydzc1.top

list(zip(*m))
来源：http://trb.ctjpmb.com

[U23] Py：分块读取大文件
来源：http://ahh.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rsd.hammf.cn

[U24] Py：路径操作
来源：http://btk.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fuc.zhongyouzk.top

[U25] Py：CSV 按字典读
来源：http://sye.hnxiangtu.top

csv.DictReader(f)
来源：http://adp.daxiang520.top

[U26] Py：并发下载
来源：http://fgi.bjfxy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ouh.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://qdm.hnqzz.top

aiohttp.ClientSession() 配合 async with
来源：http://odq.xziqi.cn

[U28] Py：类型别名
来源：http://cby.jiagoushi.top

UserId = int
来源：http://etz.wangshuangyany.cn

[U29] Py：属性校验
来源：http://xrd.sweek.top

@property 与 @x.setter 配合
来源：http://rlb.iojbl.cn

[U30] Py：数据类
来源：http://eds.chenjidiqi.icu

@dataclass(slots=True)
来源：http://kil.hfpthk.cn

[U31] Py：单测
来源：http://jjs.guannengcc.top

python -m pytest -q
来源：http://ric.yuxming.cn

[U32] Py：代码格式化
来源：http://lhh.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://lev.birdmap.top

[U33] Py：打包发布
来源：http://lrj.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://xyy.chenlongwang.top

[U34] Py：判断编码
来源：http://ivp.yfazqb.com

chardet.detect(raw)
来源：http://gur.sweek.top

[U35] Py：发送邮件
来源：http://xes.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://heo.snrcjt.cn

[U36] Py：定时任务
来源：http://qlc.shangyingyoupin.top

schedule.every(10).minutes.do(job)
来源：http://xsz.meibo888.top

[U37] Py：读写 Excel
来源：http://ibm.0kj1m.cn

pandas.read_excel / DataFrame.to_excel
来源：http://exu.daxiang520.top

[U38] Py：获取脚本所在目录
来源：http://vhd.sweek.top

Path(__file__).resolve().parent
来源：http://qyh.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://syw.yongpay.top

sys.stdout.isatty()
来源：http://vdp.fktsv.cn

[U40] Py：打印到标准错误
来源：http://ezm.316326.xyz

print("err", file=sys.stderr)
来源：http://utp.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://srh.hfpthk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yvq.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://ksh.cucudq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yzc.pycfn.com

[U43] PHP：声明命名空间
来源：http://zkt.sjlbkw.cn

namespace App\Http;
来源：http://cmg.chenlongwang.top

[U44] PHP：开启严格类型
来源：http://krb.chenlongwang.top

declare(strict_types=1);
来源：http://bhn.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://nmc.ehwqpu.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://vnr.iojbl.cn

[U46] PHP：可空类型
来源：http://nvl.hnxiangtu.top

?string $name = null
来源：http://dpb.gogol.net.cn

[U47] PHP：联合类型
来源：http://dhz.zhongyouzk.top

int|string $id
来源：http://tdv.fengsongda.top

[U48] PHP：纯枚举
来源：http://ibv.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://evx.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://tnd.zdqjudy.top

public readonly string $name
来源：http://hks.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://bzw.jinqigufen.top

public function __construct(private int $id) {}
来源：http://klq.fktsv.cn

[U51] PHP：数组解构
来源：http://wkl.sufxvd.cn

[$a, $b] = $arr;
来源：http://bes.yueranfly.top

[U52] PHP：箭头函数
来源：http://fgm.tarul.cn

$double = fn($x) => $x * 2;
来源：http://inz.yongpay.top

[U53] PHP：空合并运算符
来源：http://nbu.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://try.hysaishi.cn

[U54] PHP：空安全调用
来源：http://mcd.epnwcf.com

$obj?->method()
来源：http://azt.hnxiangtu.top

[U55] PHP：match 表达式
来源：http://dyv.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kak.yuanzhike.top

[U56] PHP：命名参数
来源：http://szp.vehdjk.com

f(a: 1, b: 2)
来源：http://wsb.xylfe.cn

[U57] PHP：字符串插值
来源：http://yzc.xuanzx.com

"值: {$a}"
来源：http://dpv.yfazqb.com

[U58] PHP：数组三件套
来源：http://auv.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sml.havefunace.top

[U59] PHP：自定义排序
来源：http://asm.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hrj.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://pcq.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kxt.yuxming.cn

[U61] PHP：正则
来源：http://rhn.dianchejie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sna.dianchejie.cn

[U62] PHP：日期对象
来源：http://jaz.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zgh.smart0.xyz

[U63] PHP：文件读写
来源：http://ldm.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kqp.yuanzhike.top

[U64] PHP：目录遍历
来源：http://ioa.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://gqt.daxiang520.top

[U65] PHP：会话
来源：http://olz.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mjk.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://dsq.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cgm.yonumen.top

[U67] PHP：处理文件上传
来源：http://unm.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cea.cqqwz.cn

[U68] PHP：PDO 连接
来源：http://msg.pycfn.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yce.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://sog.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nii.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://hek.ehwqpu.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://guy.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://drj.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://yey.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://gpp.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://liw.vqdsnc.cn

[U73] PHP：读取 ini 配置
来源：http://akt.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://qyi.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://mrr.tarul.cn

getenv("APP_ENV") ?: "production"
来源：http://zey.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://efg.jinyuanbaomall.cn

composer require psr/container
来源：http://nhs.cucudq.cn

[U76] PHP：简单路由
来源：http://hat.vehdjk.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tpg.52xcode.cn

[U77] PHP：模板渲染
来源：http://ehi.chenlongwang.top

composer require twig/twig
来源：http://usj.hnqzz.top

[U78] PHP：单元测试
来源：http://bto.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://opc.fengsongda.top

[U79] PHP：静态分析
来源：http://naw.zhengqikj.top

composer require --dev phpstan/phpstan
来源：http://qos.shanyushiyangtech.top

[U80] PHP：代码规范修复
来源：http://tjy.jyoumei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fxa.hysaishi.cn

[U81] JS：初始化项目
来源：http://stp.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://izg.yuanzhike.top

[U82] JS：package.json 脚本
来源：http://hsn.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://opr.cashguo.top

[U83] JS：ES Module 导入导出
来源：http://xnk.xingfuxueyuan.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://pvz.yj202588.top

[U84] JS：CommonJS 写法
来源：http://ies.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://agx.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://njc.jqgfzy.top

a?.b?.c
来源：http://bhr.yongpay.top

[U86] JS：空值合并
来源：http://xzy.yvedp.cn

a ?? b
来源：http://ywd.ybcxt.top


<!-- 参考信息 -->