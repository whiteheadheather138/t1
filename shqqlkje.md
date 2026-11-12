代发 wailian999

int size() const noexcept { return n_; }
来源：http://rkk.jinqigufen.top

[S53] C++：移动语义
来源：http://jvu.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://tvb.chenjidiqi.icu

[S54] C++：异常处理
来源：http://ntz.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ueu.ehwqpu.com

[S55] C++：结构化绑定
来源：http://pbs.birdmap.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ptx.jinqigfzy.top

[S56] C++：optional
来源：http://gux.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dac.52xcode.cn

[S57] C++：编译期常量
来源：http://pcc.cdnleiting.top

constexpr int N = 10;
来源：http://onx.jyoumei.cn

[S58] C++：命名空间
来源：http://bnt.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://hrb.jyoumei.cn

[S59] C++：静态断言
来源：http://uum.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vbk.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://xha.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mxc.vqdsnc.cn

================================================================================
来源：http://cqk.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lru.sysykeji.top

================================================================================
来源：http://pyh.fengsongda.top

[T01] Kotlin：Hello World
来源：http://nan.jinqigufen.top

println("Hello")
来源：http://nip.tian-w.cn

[T02] Kotlin：变量
来源：http://gju.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yuw.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://ayj.fengsongda.top

"值: $b"
来源：http://fas.zhengqikj.top

[T04] Kotlin：空安全
来源：http://ffp.zhengqikj.top

val n: String? = null;  n?.length
来源：http://yha.havefunace.top

[T05] Kotlin：when 表达式
来源：http://art.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vvx.birdmap.top

[T06] Kotlin：集合映射
来源：http://hzp.gogol.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tfp.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://obk.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uoh.fzhhl.top

[T08] Kotlin：数据类
来源：http://tlf.tanke756.top

data class User(val name: String, val age: Int)
来源：http://oep.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://kqi.tarul.cn

fun String.exclaim() = this + "!"
来源：http://myg.hammf.cn

[T10] Kotlin：默认参数
来源：http://zin.jiagoushi.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ied.nanxuanxn.top

[T11] Kotlin：协程
来源：http://hzf.fengsongda.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wmw.kuanghao11.cn

[T12] Kotlin：解构声明
来源：http://tbf.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://ypz.yongpay.top

[T13] Kotlin：只读 Map
来源：http://thw.316326.xyz

val m = mapOf("a" to 1)
来源：http://ivz.xuetiantiany.cn

[T14] Kotlin：循环
来源：http://jxf.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://jsu.ydzc1.top

[T15] Kotlin：接口
来源：http://pnw.yuxming.cn

interface Shape { fun area(): Double }
来源：http://wbn.aibaodan.cn

[T16] Swift：Hello World
来源：http://fdm.pycfn.com

print("Hello")
来源：http://ypp.ybcxt.top

[T17] Swift：变量与常量
来源：http://oed.hcnkem.com

var a = 1;  let b = 2
来源：http://gci.yj20258888.top

[T18] Swift：字符串插值
来源：http://div.mhx1999.top

"值: \(b)"
来源：http://uwt.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://yxo.zhixingplan.top

if let n = opt { print(n) }
来源：http://pwz.sufxvd.cn

[T20] Swift：数组操作
来源：http://olg.yj202588.top

var a = [1, 2, 3];  a.append(4)
来源：http://hyf.zdbjq.cn

[T21] Swift：遍历
来源：http://ger.hesvh.cn

for x in a { print(x) }
来源：http://hyh.zycfv.cn

[T22] Swift：字典
来源：http://ffn.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://qpz.hnxiangtu.top

[T23] Swift：函数
来源：http://ipv.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nmq.mhx1999.top

[T24] Swift：闭包
来源：http://rqc.yfazqb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://xgu.hesvh.cn

[T25] Swift：结构体
来源：http://qtk.hfpthk.cn

struct P { var x: Int }
来源：http://rhb.sufxvd.cn

[T26] Swift：类与重写
来源：http://uef.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://gam.yuanzhike.top

[T27] Swift：错误处理
来源：http://qrk.vehdjk.com

do { try f() } catch { print(error) }
来源：http://vpz.dashuyun.cn

[T28] Swift：枚举
来源：http://dvm.zdqjudy.top

enum Color { case red, green }
来源：http://oca.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://ngv.gotoacloud.top

guard let x = opt else { return }
来源：http://cbj.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://ksc.cashguo.top

protocol Shape { func area() -> Double }
来源：http://wng.fehbvm.com

[T31] Lua：Hello World
来源：http://lhg.hcnkem.com

print("Hello")
来源：http://tqe.yuanzhike.top

[T32] Lua：局部变量
来源：http://ayj.pycfn.com

local a = 1
来源：http://fvm.yfazqb.com

[T33] Lua：表（数组）
来源：http://lyg.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lpy.fanxiaobao.xyz

[T34] Lua：遍历表
来源：http://ssl.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mkj.redwolf501.top

[T35] Lua：字典表
来源：http://nrv.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://uuj.tianlin.xyz

[T36] Lua：函数
来源：http://tlf.zhongyouzk.top

function add(a, b) return a + b end
来源：http://kwj.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://wyt.iojbl.cn

"a" .. "b"
来源：http://qlt.jyoumei.cn

[T38] Lua：条件
来源：http://vsf.yj202588.top

if x > 0 then print("正") end
来源：http://hkq.hesvh.cn

[T39] Lua：模式匹配
来源：http://onr.xuetiantiany.cn

string.find(s, "%d+")
来源：http://eqc.kuanghao11.cn

[T40] Lua：元表
来源：http://pdq.hongshengwenyu.top

setmetatable({}, { __index = base })
来源：http://eez.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://apk.tian-w.cn

print "Hello\n";
来源：http://hyn.nanxinkj.top

[T42] Perl：变量类型
来源：http://egj.ppjwa.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pwi.hesvh.cn

[T43] Perl：字符串插值
来源：http://bva.ppjwa.cn

"值: $a"
来源：http://yyv.smart0.xyz

[T44] Perl：条件
来源：http://jkp.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://wnv.9152youxi.cn

[T45] Perl：数组遍历
来源：http://wxd.yj20258.top

for my $x (@arr) { print $x; }
来源：http://qjj.316326.xyz

[T46] Perl：哈希操作
来源：http://wmi.mhx1999.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://onp.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://ynd.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://cec.9152youxi.cn

[T48] Perl：正则替换
来源：http://odg.xziqi.cn

$s =~ s/old/new/g;
来源：http://pax.gogol.net.cn

[T49] Perl：函数
来源：http://xnh.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tpz.chenjidiqi.icu

[T50] Perl：逐行读文件
来源：http://hfs.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hbc.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://bqu.shuidangran.top

[T51] Scala：Hello World
来源：http://xcj.dianchejie.cn

println("Hello")
来源：http://ojl.smart0.xyz

[T52] Scala：变量
来源：http://tqu.iojbl.cn

val a = 1;  var b = 2
来源：http://rfc.ybcxt.top

[T53] Scala：字符串插值
来源：http://igq.zhijiandao.cn

s"值: $b"
来源：http://tgt.dianchejie.cn

[T54] Scala：集合映射
来源：http://edq.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://vpp.xylfe.cn

[T55] Scala：集合过滤
来源：http://ojc.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://ntd.jqgufenzy.top

[T56] Scala：样例类
来源：http://xwf.aibaodan.cn

case class User(name: String, age: Int)
来源：http://ogf.ybcxt.top

[T57] Scala：模式匹配
来源：http://ecr.dashuyun.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jwi.zhongyouzk.top

[T58] Scala：函数定义
来源：http://jrd.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://tqt.cucudq.cn

[T59] Scala：循环
来源：http://nng.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://hlh.tian-w.cn

[T60] Scala：折叠
来源：http://sba.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bdo.mhx1999.top

================================================================================
来源：http://qdq.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eto.jqgufenzy.top

================================================================================
来源：http://npf.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://lws.nwbrower.top

python -m venv .venv && source .venv/bin/activate
来源：http://mfl.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://eml.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lud.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://pqf.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rvk.zhixingplan.top

[U04] Py：变量调试打印
来源：http://zln.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jas.cheryme.top

[U05] Py：列表去重且保序
来源：http://xyf.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://tiz.bbcook.cn

[U06] Py：合并两个字典
来源：http://zpb.cheryme.top

{**a, **b}
来源：http://iuk.daxiang520.top

[U07] Py：反转字典键值
来源：http://ymr.epnwcf.com

{v: k for k, v in d.items()}
来源：http://bwf.feifeiyinyue.top

[U08] Py：展平二维列表
来源：http://qmg.jinghuilouyu.cn

[y for x in nested for y in x]
来源：http://kki.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://lvy.cheryme.top

max(d, key=d.get)
来源：http://pqf.tarul.cn

[U10] Py：按值排序字典
来源：http://djs.bbcook.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eqk.feifeiyinyue.top

[U11] Py：生成器表达式
来源：http://mvq.aizwys.cn

(x * 2 for x in arr)
来源：http://ipv.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://umv.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://nxw.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://orn.yonumen.top

deque(maxlen=10)
来源：http://xlr.sufxvd.cn

[U14] Py：分组收集到列表
来源：http://kqu.gzhubu.top

defaultdict(list)
来源：http://gxq.meibo888.top

[U15] Py：高精度计时
来源：http://xeu.haohaochexian.top

t = time.perf_counter()
来源：http://nnf.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://zay.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jnj.sjlbkw.cn

[U17] Py：初始化日志
来源：http://mez.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://dqw.gotoacloud.top

[U18] Py：预编译正则
来源：http://lqt.yj20258888.top

pat = re.compile(r"\d+")
来源：http://omy.redwolf501.top

[U19] Py：正则替换带回调
来源：http://slz.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nbt.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://wja.shzxlz.cn

@functools.lru_cache(maxsize=None)
来源：http://uhk.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://apx.shangyingyoupin.top

@contextlib.contextmanager
来源：http://zcs.yj20258888.top

[U22] Py：矩阵转置
来源：http://kqj.c1oappe.top

list(zip(*m))
来源：http://xwc.ywan-chungtsiang.top

[U23] Py：分块读取大文件
来源：http://flp.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jdu.cucudq.cn

[U24] Py：路径操作
来源：http://tmx.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nih.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://jjp.hammf.cn

csv.DictReader(f)
来源：http://lej.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://nrk.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eln.fktsv.cn

[U27] Py：异步 HTTP
来源：http://pje.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://aqa.cdnleiting.top

[U28] Py：类型别名
来源：http://she.sxryk.cn

UserId = int
来源：http://gzd.yangfankeji.com

[U29] Py：属性校验
来源：http://ocr.sufxvd.cn

@property 与 @x.setter 配合
来源：http://cvf.sysykeji.top

[U30] Py：数据类
来源：http://mvj.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://dbx.chenzaomai.com

[U31] Py：单测
来源：http://rsq.haohaochexian.top

python -m pytest -q
来源：http://jcz.hcnkem.com

[U32] Py：代码格式化
来源：http://xzn.chenjidiqi.icu

ruff format . && ruff check --fix .
来源：http://zsn.jinqigufen.top

[U33] Py：打包发布
来源：http://nqb.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://saa.tian-w.cn

[U34] Py：判断编码
来源：http://hpr.fanxiaobao.xyz

chardet.detect(raw)
来源：http://twh.hywenlv.cn

[U35] Py：发送邮件
来源：http://cyw.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yar.aibaodan.cn

[U36] Py：定时任务
来源：http://tpv.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://crp.hywenlv.cn

[U37] Py：读写 Excel
来源：http://ghe.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yzq.cdnleiting.top

[U38] Py：获取脚本所在目录
来源：http://asa.ehwqpu.com

Path(__file__).resolve().parent
来源：http://mxh.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://jub.yueranfly.top

sys.stdout.isatty()
来源：http://dmm.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://try.nwbrower.top

print("err", file=sys.stderr)
来源：http://adu.xuanzx.com

[U41] PHP：初始化 Composer 项目
来源：http://vib.svipenyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://len.yj202588.top

[U42] PHP：PSR-4 自动加载
来源：http://hhf.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ntg.aizwys.cn

[U43] PHP：声明命名空间
来源：http://xyu.zhaomingkeji.xyz

namespace App\Http;
来源：http://bze.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://prc.yuanzhike.top

declare(strict_types=1);
来源：http://bvb.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://yyh.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dwe.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://wqy.hongshengwenyu.top

?string $name = null
来源：http://vcs.zhixingplan.top

[U47] PHP：联合类型
来源：http://ttu.yueranfly.top

int|string $id
来源：http://ogt.tanke756.top

[U48] PHP：纯枚举
来源：http://mds.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lvo.shangyingyoupin.top

[U49] PHP：只读属性
来源：http://krn.fehbvm.com

public readonly string $name
来源：http://emx.hammf.cn

[U50] PHP：构造器属性提升
来源：http://vxu.0kj1m.cn

public function __construct(private int $id) {}
来源：http://kbk.aibaodan.cn

[U51] PHP：数组解构
来源：http://lor.cdnleiting.top

[$a, $b] = $arr;
来源：http://ntx.jlsjyb.cn

[U52] PHP：箭头函数
来源：http://nlg.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://rdd.nanxuanxn.top

[U53] PHP：空合并运算符
来源：http://hfm.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://lue.xinyue.icu

[U54] PHP：空安全调用
来源：http://tzz.dashuyun.cn

$obj?->method()
来源：http://wis.hesvh.cn

[U55] PHP：match 表达式
来源：http://eka.jlsjyb.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fzy.zdqjudy.top

[U56] PHP：命名参数
来源：http://fez.cucudq.cn

f(a: 1, b: 2)
来源：http://kyr.mhx1999.top

[U57] PHP：字符串插值
来源：http://buh.sxryk.cn

"值: {$a}"
来源：http://aar.daria6918.cn

[U58] PHP：数组三件套
来源：http://mzz.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mjh.nanxinkj.top

[U59] PHP：自定义排序
来源：http://ode.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ure.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://ruu.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qdf.pycfn.com

[U61] PHP：正则
来源：http://vze.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lmj.yongpay.top

[U62] PHP：日期对象
来源：http://tba.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jzw.zdbjq.cn

[U63] PHP：文件读写
来源：http://xud.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vjn.hcnkem.com

[U64] PHP：目录遍历
来源：http://ksd.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://ugr.yuxming.cn

[U65] PHP：会话
来源：http://xud.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gst.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://uvz.xingfuxueyuan.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wvl.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://brg.hysaishi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uvz.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://jsa.meibo888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sqa.shzxlz.cn

[U69] PHP：PDO 预处理
来源：http://dmf.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kvk.9152youxi.cn

[U70] PHP：PDO 事务
来源：http://ldj.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ztc.pycfn.com

[U71] PHP：抛出异常
来源：http://elj.guowangkeji.top

throw new RuntimeException("失败", 500);
来源：http://frq.yuanzhike.top

[U72] PHP：写错误日志
来源：http://yqc.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://fst.guowangkeji.top

[U73] PHP：读取 ini 配置
来源：http://ypf.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://kpp.yj202588.top

[U74] PHP：读取环境变量
来源：http://vxt.yfazqb.com

getenv("APP_ENV") ?: "production"
来源：http://zpe.chenlongwang.top

[U75] PHP：依赖注入
来源：http://fgr.xingfuxueyuan.xyz

composer require psr/container
来源：http://kds.jiagoushi.top

[U76] PHP：简单路由
来源：http://mjw.zdqjudy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ncn.havefunace.top

[U77] PHP：模板渲染
来源：http://diy.zdbjq.cn

composer require twig/twig
来源：http://xux.chenlongwang.top

[U78] PHP：单元测试
来源：http://avw.yongpay.top

composer require --dev phpunit/phpunit
来源：http://pvd.daria6918.cn


<!-- 参考信息 -->