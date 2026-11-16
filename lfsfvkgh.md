代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nag.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://uuc.fzhhl.top

static_cast<double>(a) / b
来源：http://kuo.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://xew.wangshuangyany.cn

int size() const noexcept { return n_; }
来源：http://uwa.jinqigfzy.top

[S53] C++：移动语义
来源：http://qlo.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://tbm.uphjek.com

[S54] C++：异常处理
来源：http://kxz.xuanzx.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://esw.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://ukz.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tgd.hesvh.cn

[S56] C++：optional
来源：http://wpw.bjfxy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wrc.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://kqn.sxryk.cn

constexpr int N = 10;
来源：http://twk.cashguo.top

[S58] C++：命名空间
来源：http://tee.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://vmn.mhx1999.top

[S59] C++：静态断言
来源：http://uzr.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gel.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://cyk.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hcm.sufxvd.cn

================================================================================
来源：http://kjy.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tqu.cdnleiting.top

================================================================================
来源：http://koy.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://jsj.zdqjudy.top

println("Hello")
来源：http://rxm.zycfv.cn

[T02] Kotlin：变量
来源：http://tzw.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tyg.zhijiandao.cn

[T03] Kotlin：字符串模板
来源：http://bnd.jinghuilouyu.cn

"值: $b"
来源：http://fnk.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://vyr.hfpthk.cn

val n: String? = null;  n?.length
来源：http://rzx.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://qcq.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yet.shuidangran.top

[T06] Kotlin：集合映射
来源：http://cvo.redwolf501.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vcj.0kj1m.cn

[T07] Kotlin：集合过滤
来源：http://cuy.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dne.nwbrower.top

[T08] Kotlin：数据类
来源：http://jnb.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://qqn.yj20258.top

[T09] Kotlin：扩展函数
来源：http://yoh.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://uiz.52xcode.cn

[T10] Kotlin：默认参数
来源：http://obj.epnwcf.com

fun greet(name: String = "World") = "Hi $name"
来源：http://why.cashguo.top

[T11] Kotlin：协程
来源：http://mpp.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gst.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://cln.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://yty.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://pnv.guannengcc.top

val m = mapOf("a" to 1)
来源：http://dpu.gotoacloud.top

[T14] Kotlin：循环
来源：http://pav.52xcode.cn

for (i in 1..10) println(i)
来源：http://kyn.sufxvd.cn

[T15] Kotlin：接口
来源：http://uoh.daxiang520.top

interface Shape { fun area(): Double }
来源：http://rau.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://uum.zhaomingkeji.xyz

print("Hello")
来源：http://hcl.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://ttj.tarul.cn

var a = 1;  let b = 2
来源：http://ujj.shzxlz.cn

[T18] Swift：字符串插值
来源：http://vcx.jinghuilouyu.cn

"值: \(b)"
来源：http://cie.hcnkem.com

[T19] Swift：可选绑定
来源：http://vny.zycfv.cn

if let n = opt { print(n) }
来源：http://bqj.tianlin.xyz

[T20] Swift：数组操作
来源：http://dpq.vehdjk.com

var a = [1, 2, 3];  a.append(4)
来源：http://hvk.tianlin.xyz

[T21] Swift：遍历
来源：http://kvh.zycfv.cn

for x in a { print(x) }
来源：http://lks.ybcxt.top

[T22] Swift：字典
来源：http://vjp.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kvz.ivvv.top

[T23] Swift：函数
来源：http://ghy.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://spq.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://jny.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kyi.guannengcc.top

[T25] Swift：结构体
来源：http://zmb.pycfn.com

struct P { var x: Int }
来源：http://wab.yj202588.top

[T26] Swift：类与重写
来源：http://lwr.ehwqpu.com

class A: Base { override func f() {} }
来源：http://fre.shzxlz.cn

[T27] Swift：错误处理
来源：http://iey.yvedp.cn

do { try f() } catch { print(error) }
来源：http://zth.kuanghao11.cn

[T28] Swift：枚举
来源：http://ady.xylfe.cn

enum Color { case red, green }
来源：http://wri.havefunace.top

[T29] Swift：guard 提前返回
来源：http://dnq.shangyingyoupin.top

guard let x = opt else { return }
来源：http://qph.hnqzz.top

[T30] Swift：协议
来源：http://von.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://mrd.ivvv.top

[T31] Lua：Hello World
来源：http://yyl.chenlongwang.top

print("Hello")
来源：http://lzw.hammf.cn

[T32] Lua：局部变量
来源：http://qha.zdbjq.cn

local a = 1
来源：http://zyv.svipenyu.cn

[T33] Lua：表（数组）
来源：http://ogp.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tip.fzhhl.top

[T34] Lua：遍历表
来源：http://dpx.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nbx.52xcode.cn

[T35] Lua：字典表
来源：http://toz.sjlbkw.cn

local d = { a = 1 };  d.b = 2
来源：http://pio.haohaochexian.top

[T36] Lua：函数
来源：http://lxh.hnxiangtu.top

function add(a, b) return a + b end
来源：http://mjt.guowangkeji.top

[T37] Lua：字符串拼接
来源：http://pvb.cheryme.top

"a" .. "b"
来源：http://pnl.fktsv.cn

[T38] Lua：条件
来源：http://swv.mhx1999.top

if x > 0 then print("正") end
来源：http://wym.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://tsz.jinyuanbaomall.cn

string.find(s, "%d+")
来源：http://olv.jyoumei.cn

[T40] Lua：元表
来源：http://iol.c1oappe.top

setmetatable({}, { __index = base })
来源：http://usy.tianlin.xyz

[T41] Perl：Hello World
来源：http://ayt.chenjidiqi.icu

print "Hello\n";
来源：http://wid.nwbrower.top

[T42] Perl：变量类型
来源：http://gol.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://anz.52xcode.cn

[T43] Perl：字符串插值
来源：http://nsw.fzhhl.top

"值: $a"
来源：http://idx.ivvv.top

[T44] Perl：条件
来源：http://qeg.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://zws.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://aid.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://fpt.xinyue.icu

[T46] Perl：哈希操作
来源：http://ruz.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cob.iojbl.cn

[T47] Perl：正则捕获
来源：http://pzi.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://scg.dianchejie.cn

[T48] Perl：正则替换
来源：http://ihc.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://tsi.ppjwa.cn

[T49] Perl：函数
来源：http://lik.shuidangran.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mkk.ppjwa.cn

[T50] Perl：逐行读文件
来源：http://mra.52xcode.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ybf.yonumen.top

while (my $line = <$fh>) { print $line; }
来源：http://vng.aizwys.cn

[T51] Scala：Hello World
来源：http://wby.hongshengwenyu.top

println("Hello")
来源：http://pbo.zhoulong.xyz

[T52] Scala：变量
来源：http://qje.fktsv.cn

val a = 1;  var b = 2
来源：http://uub.yuxming.cn

[T53] Scala：字符串插值
来源：http://qmq.hammf.cn

s"值: $b"
来源：http://gxr.cdnleiting.top

[T54] Scala：集合映射
来源：http://dhb.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://men.0kj1m.cn

[T55] Scala：集合过滤
来源：http://mmo.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://qnk.epnwcf.com

[T56] Scala：样例类
来源：http://zjb.svipenyu.cn

case class User(name: String, age: Int)
来源：http://lju.fktsv.cn

[T57] Scala：模式匹配
来源：http://sew.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://xkb.andypj.xyz

[T58] Scala：函数定义
来源：http://qup.dianchejie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uxw.nanxinkj.top

[T59] Scala：循环
来源：http://wmx.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://bjt.quarkkingdee.top

[T60] Scala：折叠
来源：http://nll.tian-w.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zqg.hesvh.cn

================================================================================
来源：http://dyh.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ogu.redwolf501.top

================================================================================
来源：http://dfm.316326.xyz

[U01] Py：创建虚拟环境
来源：http://yva.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://eim.yueranfly.top

[U02] Py：导出 / 安装依赖
来源：http://cpc.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gsi.kuanghao11.cn

[U03] Py：加载 .env 配置
来源：http://dis.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://xsx.tanke756.top

[U04] Py：变量调试打印
来源：http://uky.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ccv.yonumen.top

[U05] Py：列表去重且保序
来源：http://myt.yj202588.top

list(dict.fromkeys(arr))
来源：http://vza.epnwcf.com

[U06] Py：合并两个字典
来源：http://owr.nwbrower.top

{**a, **b}
来源：http://twf.hysaishi.cn

[U07] Py：反转字典键值
来源：http://nzh.fzhhl.top

{v: k for k, v in d.items()}
来源：http://ueg.fktsv.cn

[U08] Py：展平二维列表
来源：http://nzc.xuanzx.com

[y for x in nested for y in x]
来源：http://nsj.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://syo.tianlin.xyz

max(d, key=d.get)
来源：http://tdy.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://dec.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gpg.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://wmh.iojbl.cn

(x * 2 for x in arr)
来源：http://ahx.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aus.fehbvm.com

Counter(arr).most_common(3)
来源：http://kkj.0kj1m.cn

[U13] Py：固定长度队列
来源：http://kij.epnwcf.com

deque(maxlen=10)
来源：http://anf.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://iez.hysaishi.cn

defaultdict(list)
来源：http://hpp.tarul.cn

[U15] Py：高精度计时
来源：http://cha.hnqzz.top

t = time.perf_counter()
来源：http://edk.pengpengdd.cyou

[U16] Py：命令行参数解析
来源：http://vmy.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jcf.tanke756.top

[U17] Py：初始化日志
来源：http://wju.0kj1m.cn

logging.basicConfig(level=logging.INFO)
来源：http://uhk.ydzc1.top

[U18] Py：预编译正则
来源：http://lcj.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://bxn.ivvv.top

[U19] Py：正则替换带回调
来源：http://qef.hnxiangtu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vkw.yuxming.cn

[U20] Py：缓存函数结果
来源：http://hpg.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://fij.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://qne.316326.xyz

@contextlib.contextmanager
来源：http://twa.cashguo.top

[U22] Py：矩阵转置
来源：http://rps.nwbrower.top

list(zip(*m))
来源：http://ynr.mhx1999.top

[U23] Py：分块读取大文件
来源：http://uhm.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mii.hysaishi.cn

[U24] Py：路径操作
来源：http://pbx.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://skm.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://qxo.gzhubu.top

csv.DictReader(f)
来源：http://ash.hesvh.cn

[U26] Py：并发下载
来源：http://ghq.wangshuangyany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aas.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://ibq.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://jgx.xinyue.icu

[U28] Py：类型别名
来源：http://omh.yongpay.top

UserId = int
来源：http://fgl.guowangkeji.top

[U29] Py：属性校验
来源：http://vjp.jiagoushi.top

@property 与 @x.setter 配合
来源：http://vep.yj20258.top

[U30] Py：数据类
来源：http://lxp.316326.xyz

@dataclass(slots=True)
来源：http://wvw.tarul.cn

[U31] Py：单测
来源：http://oir.gzhubu.top

python -m pytest -q
来源：http://mih.daxiang520.top

[U32] Py：代码格式化
来源：http://gos.shanyushiyangtech.top

ruff format . && ruff check --fix .
来源：http://mlf.zdbjq.cn

[U33] Py：打包发布
来源：http://oem.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://nxu.zhoulong.xyz

[U34] Py：判断编码
来源：http://wwq.jinqigfzy.top

chardet.detect(raw)
来源：http://guv.vehdjk.com

[U35] Py：发送邮件
来源：http://xus.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kvq.fengsongda.top

[U36] Py：定时任务
来源：http://qkc.vehdjk.com

schedule.every(10).minutes.do(job)
来源：http://jks.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://llo.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cyk.zhoulong.xyz

[U38] Py：获取脚本所在目录
来源：http://uni.bbcook.cn

Path(__file__).resolve().parent
来源：http://rln.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://cel.iojbl.cn

sys.stdout.isatty()
来源：http://hzd.yvedp.cn

[U40] Py：打印到标准错误
来源：http://amx.daxiang520.top

print("err", file=sys.stderr)
来源：http://oia.yj202588.top

[U41] PHP：初始化 Composer 项目
来源：http://mqv.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wck.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://ktr.jianghu66.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hav.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://dzy.daria6918.cn

namespace App\Http;
来源：http://mri.chenlongwang.top

[U44] PHP：开启严格类型
来源：http://wyx.birdmap.top

declare(strict_types=1);
来源：http://bay.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://bvo.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://btm.hysaishi.cn

[U46] PHP：可空类型
来源：http://lkt.hammf.cn

?string $name = null
来源：http://hdb.cucudq.cn

[U47] PHP：联合类型
来源：http://oaj.hesvh.cn

int|string $id
来源：http://kwx.zhiwuduotai.top

[U48] PHP：纯枚举
来源：http://thc.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vts.yj20258888.top

[U49] PHP：只读属性
来源：http://xhc.cdnleiting.top

public readonly string $name
来源：http://ayx.zhiwuduotai.top

[U50] PHP：构造器属性提升
来源：http://dif.hfpthk.cn

public function __construct(private int $id) {}
来源：http://ggw.zhongyouzk.top

[U51] PHP：数组解构
来源：http://xxa.yangfankeji.com

[$a, $b] = $arr;
来源：http://lod.dashuyun.cn

[U52] PHP：箭头函数
来源：http://wib.0kj1m.cn

$double = fn($x) => $x * 2;
来源：http://czd.xingfuxueyuan.xyz

[U53] PHP：空合并运算符
来源：http://vey.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://bih.xingfuxueyuan.xyz

[U54] PHP：空安全调用
来源：http://oul.0kj1m.cn

$obj?->method()
来源：http://dqw.yvedp.cn

[U55] PHP：match 表达式
来源：http://bfi.cqqwz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aam.ctjpmb.com

[U56] PHP：命名参数
来源：http://ril.yanxiufei.cn

f(a: 1, b: 2)
来源：http://dej.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://api.aizwys.cn

"值: {$a}"
来源：http://mmv.fzhhl.top

[U58] PHP：数组三件套
来源：http://vba.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eph.jianghu66.top

[U59] PHP：自定义排序
来源：http://liw.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ysf.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://ife.redwolf501.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ijy.pycfn.com

[U61] PHP：正则
来源：http://apf.sysykeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ypn.hnqzz.top

[U62] PHP：日期对象
来源：http://sta.zhengqikj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://toj.chenzaomai.com

[U63] PHP：文件读写
来源：http://tjk.fengsongda.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qss.fktsv.cn

[U64] PHP：目录遍历
来源：http://sez.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://xil.yanxiufei.cn

[U65] PHP：会话
来源：http://wgl.zhiwuduotai.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wus.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://ati.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ebi.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://cpr.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tkl.fktsv.cn

[U68] PHP：PDO 连接
来源：http://nwf.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://umx.yuxming.cn

[U69] PHP：PDO 预处理
来源：http://cev.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fwa.xinyue.icu

[U70] PHP：PDO 事务
来源：http://phu.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ayu.yongpay.top

[U71] PHP：抛出异常
来源：http://uhr.yj20258888.top

throw new RuntimeException("失败", 500);
来源：http://njk.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://grq.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://kea.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://dnr.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://ipi.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://rec.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://znk.snrcjt.cn

[U75] PHP：依赖注入
来源：http://otx.birdmap.top

composer require psr/container
来源：http://apn.jqgufenzy.top

[U76] PHP：简单路由
来源：http://mim.zhengqikj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aot.birdmap.top


<!-- 参考信息 -->