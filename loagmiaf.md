代发 wailian999

int size() const noexcept { return n_; }
来源：http://xgu.xinyue.icu

[S53] C++：移动语义
来源：http://jhz.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://ujp.tian-w.cn

[S54] C++：异常处理
来源：http://ubp.yj20258.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rcc.daxiang520.top

[S55] C++：结构化绑定
来源：http://csr.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tsj.zhijiandao.cn

[S56] C++：optional
来源：http://kjv.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cdk.ctjpmb.com

[S57] C++：编译期常量
来源：http://qnk.sxryk.cn

constexpr int N = 10;
来源：http://sxs.hfpthk.cn

[S58] C++：命名空间
来源：http://qxg.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://pca.jinqigufen.top

[S59] C++：静态断言
来源：http://klp.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wfs.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://crt.gzhubu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ywj.zhijiandao.cn

================================================================================
来源：http://fii.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tek.zdbjq.cn

================================================================================
来源：http://mgn.ivvv.top

[T01] Kotlin：Hello World
来源：http://rux.tianlin.xyz

println("Hello")
来源：http://dao.gotoacloud.top

[T02] Kotlin：变量
来源：http://mge.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ney.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://mjv.havefunace.top

"值: $b"
来源：http://iud.vehdjk.com

[T04] Kotlin：空安全
来源：http://amf.hnqzz.top

val n: String? = null;  n?.length
来源：http://esl.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://zwa.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rkl.yj202588.top

[T06] Kotlin：集合映射
来源：http://nkw.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ssv.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://vow.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://day.xziqi.cn

[T08] Kotlin：数据类
来源：http://vst.yj20258.top

data class User(val name: String, val age: Int)
来源：http://fig.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://nsn.cashguo.top

fun String.exclaim() = this + "!"
来源：http://flt.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://jib.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nec.sysykeji.top

[T11] Kotlin：协程
来源：http://gws.bjfxy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gnb.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://vfh.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://yea.fanxiaobao.xyz

[T13] Kotlin：只读 Map
来源：http://wre.fehbvm.com

val m = mapOf("a" to 1)
来源：http://moa.dianchejie.cn

[T14] Kotlin：循环
来源：http://hlm.xuanzx.com

for (i in 1..10) println(i)
来源：http://dph.redwolf501.top

[T15] Kotlin：接口
来源：http://bww.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://yvf.aizwys.cn

[T16] Swift：Hello World
来源：http://ygn.xylfe.cn

print("Hello")
来源：http://wbt.chenlongwang.top

[T17] Swift：变量与常量
来源：http://lkq.smart0.xyz

var a = 1;  let b = 2
来源：http://qcl.wangshuangyany.cn

[T18] Swift：字符串插值
来源：http://vyw.yj20258888.top

"值: \(b)"
来源：http://uor.yangfankeji.com

[T19] Swift：可选绑定
来源：http://bqg.sweek.top

if let n = opt { print(n) }
来源：http://ran.smart0.xyz

[T20] Swift：数组操作
来源：http://xix.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ivs.ydzc1.top

[T21] Swift：遍历
来源：http://uev.hammf.cn

for x in a { print(x) }
来源：http://rkt.fehbvm.com

[T22] Swift：字典
来源：http://aik.nanxuanxn.top

var d = ["a": 1];  d["b"] = 2
来源：http://ags.yj20258.top

[T23] Swift：函数
来源：http://jnc.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vib.tarul.cn

[T24] Swift：闭包
来源：http://oxm.yuanzhike.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ulv.gaohongyu789.top

[T25] Swift：结构体
来源：http://low.nwbrower.top

struct P { var x: Int }
来源：http://ehq.jlsjyb.cn

[T26] Swift：类与重写
来源：http://erd.xylfe.cn

class A: Base { override func f() {} }
来源：http://xcm.jinyuanbaomall.cn

[T27] Swift：错误处理
来源：http://sgb.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://mhf.shanyushiyangtech.top

[T28] Swift：枚举
来源：http://ocq.9152youxi.cn

enum Color { case red, green }
来源：http://jod.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://jjt.andypj.xyz

guard let x = opt else { return }
来源：http://pcs.gzhubu.top

[T30] Swift：协议
来源：http://wjt.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://wbs.chenzaomai.com

[T31] Lua：Hello World
来源：http://vfz.hnxiangtu.top

print("Hello")
来源：http://oll.zhongyouzk.top

[T32] Lua：局部变量
来源：http://ymz.zdqjudy.top

local a = 1
来源：http://lgc.xziqi.cn

[T33] Lua：表（数组）
来源：http://dcb.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yyl.redwolf501.top

[T34] Lua：遍历表
来源：http://hid.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fla.tian-w.cn

[T35] Lua：字典表
来源：http://ecf.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://eqk.gogol.net.cn

[T36] Lua：函数
来源：http://rne.jianghu66.top

function add(a, b) return a + b end
来源：http://oca.redwolf501.top

[T37] Lua：字符串拼接
来源：http://yfx.kuanghao11.cn

"a" .. "b"
来源：http://hsb.shanyushiyangtech.top

[T38] Lua：条件
来源：http://osu.quarkkingdee.top

if x > 0 then print("正") end
来源：http://jgj.tarul.cn

[T39] Lua：模式匹配
来源：http://ioy.xziqi.cn

string.find(s, "%d+")
来源：http://lmj.uphjek.com

[T40] Lua：元表
来源：http://anq.yj202588.top

setmetatable({}, { __index = base })
来源：http://ibq.zhengqikj.top

[T41] Perl：Hello World
来源：http://qvw.xziqi.cn

print "Hello\n";
来源：http://hit.zhijiandao.cn

[T42] Perl：变量类型
来源：http://ntt.vehdjk.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uvv.0kj1m.cn

[T43] Perl：字符串插值
来源：http://ink.fehbvm.com

"值: $a"
来源：http://mwd.mhx1999.top

[T44] Perl：条件
来源：http://fem.aibaodan.cn

if ($a > 0) { print "正"; }
来源：http://mpq.hnxiangtu.top

[T45] Perl：数组遍历
来源：http://yve.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://tvp.dianchejie.cn

[T46] Perl：哈希操作
来源：http://bgg.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pjy.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://hsz.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://xgg.tianlin.xyz

[T48] Perl：正则替换
来源：http://fmz.sufxvd.cn

$s =~ s/old/new/g;
来源：http://iam.hnqzz.top

[T49] Perl：函数
来源：http://hep.cqqwz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://btx.xylfe.cn

[T50] Perl：逐行读文件
来源：http://gpw.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rzo.uphjek.com

while (my $line = <$fh>) { print $line; }
来源：http://jdi.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://lqw.snrcjt.cn

println("Hello")
来源：http://lfk.yangfankeji.com

[T52] Scala：变量
来源：http://guz.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://wmp.shanyushiyangkeji.top

[T53] Scala：字符串插值
来源：http://bdu.jyoumei.cn

s"值: $b"
来源：http://mdu.yfazqb.com

[T54] Scala：集合映射
来源：http://phm.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://fol.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://srs.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://lbr.svipenyu.cn

[T56] Scala：样例类
来源：http://nye.tarul.cn

case class User(name: String, age: Int)
来源：http://omg.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://ckr.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://brk.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://mfy.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pdy.jyoumei.cn

[T59] Scala：循环
来源：http://uzw.jqgufenzy.top

for (i <- 1 to 10) println(i)
来源：http://gxw.pycfn.com

[T60] Scala：折叠
来源：http://lbw.zhaomingkeji.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://czj.zhixingplan.top

================================================================================
来源：http://gca.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tcp.snrcjt.cn

================================================================================
来源：http://rgn.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://qrk.sjlbkw.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mlh.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://wtn.shanyushiyangtech.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zgg.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://oea.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://lkn.hnqzz.top

[U04] Py：变量调试打印
来源：http://uca.ydjk.org.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rvh.zhiwuduotai.top

[U05] Py：列表去重且保序
来源：http://cxa.birdmap.top

list(dict.fromkeys(arr))
来源：http://ipz.ivvv.top

[U06] Py：合并两个字典
来源：http://vir.gotoacloud.top

{**a, **b}
来源：http://yoi.redwolf501.top

[U07] Py：反转字典键值
来源：http://xol.0kj1m.cn

{v: k for k, v in d.items()}
来源：http://tje.hnqzz.top

[U08] Py：展平二维列表
来源：http://ddg.jinqigfzy.top

[y for x in nested for y in x]
来源：http://wsn.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://ylx.ctjpmb.com

max(d, key=d.get)
来源：http://jpd.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://yrd.birdmap.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jbi.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://duz.hongshengwenyu.top

(x * 2 for x in arr)
来源：http://aww.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://zwz.fzhhl.top

Counter(arr).most_common(3)
来源：http://ovb.xylfe.cn

[U13] Py：固定长度队列
来源：http://lul.cashguo.top

deque(maxlen=10)
来源：http://dzn.cucudq.cn

[U14] Py：分组收集到列表
来源：http://kxq.hnqzz.top

defaultdict(list)
来源：http://kuy.jinqigufen.top

[U15] Py：高精度计时
来源：http://erx.aibaodan.cn

t = time.perf_counter()
来源：http://hdd.redwolf501.top

[U16] Py：命令行参数解析
来源：http://slp.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lzv.yj202588.top

[U17] Py：初始化日志
来源：http://bbw.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://mtz.fktsv.cn

[U18] Py：预编译正则
来源：http://cdp.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://zxm.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://qtn.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://chk.cashguo.top

[U20] Py：缓存函数结果
来源：http://jih.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://ehf.birdmap.top

[U21] Py：自定义上下文管理器
来源：http://hmd.meibo888.top

@contextlib.contextmanager
来源：http://byo.ybcxt.top

[U22] Py：矩阵转置
来源：http://lxb.jinqigfzy.top

list(zip(*m))
来源：http://wcy.nanxinkj.top

[U23] Py：分块读取大文件
来源：http://toi.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dcp.iojbl.cn

[U24] Py：路径操作
来源：http://evw.hnqzz.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wnk.sweek.top

[U25] Py：CSV 按字典读
来源：http://nsf.cucudq.cn

csv.DictReader(f)
来源：http://fxe.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://fex.316326.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hjo.redwolf501.top

[U27] Py：异步 HTTP
来源：http://cvt.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://mpl.316326.xyz

[U28] Py：类型别名
来源：http://tkj.nanxinkj.top

UserId = int
来源：http://gut.yueranfly.top

[U29] Py：属性校验
来源：http://ehw.daxiang520.top

@property 与 @x.setter 配合
来源：http://ngn.ehwqpu.com

[U30] Py：数据类
来源：http://vgv.xingfuxueyuan.xyz

@dataclass(slots=True)
来源：http://okb.tianlin.xyz

[U31] Py：单测
来源：http://ttd.meibo888.top

python -m pytest -q
来源：http://bdn.epnwcf.com

[U32] Py：代码格式化
来源：http://jyy.yfazqb.com

ruff format . && ruff check --fix .
来源：http://oeh.zycfv.cn

[U33] Py：打包发布
来源：http://kci.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://edf.jiagoushi.top

[U34] Py：判断编码
来源：http://tcp.gaohongyu789.top

chardet.detect(raw)
来源：http://ykv.yongpay.top

[U35] Py：发送邮件
来源：http://hhh.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rtx.hnqzz.top

[U36] Py：定时任务
来源：http://sqr.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://ptr.guowangkeji.top

[U37] Py：读写 Excel
来源：http://oex.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xqd.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://mti.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://nwk.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://nds.hnxiangtu.top

sys.stdout.isatty()
来源：http://hkv.bjfxy.top

[U40] Py：打印到标准错误
来源：http://ghi.yongpay.top

print("err", file=sys.stderr)
来源：http://udx.gzhubu.top

[U41] PHP：初始化 Composer 项目
来源：http://nzh.hnqzz.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gza.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://kwc.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zao.aibaodan.cn

[U43] PHP：声明命名空间
来源：http://kwn.hcnkem.com

namespace App\Http;
来源：http://ebi.shanyushiyangkeji.top

[U44] PHP：开启严格类型
来源：http://sdo.ybcxt.top

declare(strict_types=1);
来源：http://qxy.bjfxy.top

[U45] PHP：类型声明与返回类型
来源：http://hge.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nft.hywenlv.cn

[U46] PHP：可空类型
来源：http://lyt.redwolf501.top

?string $name = null
来源：http://zsf.smart0.xyz

[U47] PHP：联合类型
来源：http://hkc.bbcook.cn

int|string $id
来源：http://kwu.jinyuanbaomall.cn

[U48] PHP：纯枚举
来源：http://uqj.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kry.redwolf501.top

[U49] PHP：只读属性
来源：http://jok.gaohongyu789.top

public readonly string $name
来源：http://rnr.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://nus.ydzc1.top

public function __construct(private int $id) {}
来源：http://gob.hnxiangtu.top

[U51] PHP：数组解构
来源：http://eop.iojbl.cn

[$a, $b] = $arr;
来源：http://pqg.yongpay.top

[U52] PHP：箭头函数
来源：http://luu.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://biy.andypj.xyz

[U53] PHP：空合并运算符
来源：http://pht.dianchejie.cn

$v = $a ?? $b ?? "default";
来源：http://ydq.zhengqikj.top

[U54] PHP：空安全调用
来源：http://kab.uphjek.com

$obj?->method()
来源：http://ltw.gzhubu.top

[U55] PHP：match 表达式
来源：http://qgq.hesvh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ram.zhoulong.xyz

[U56] PHP：命名参数
来源：http://ipb.chenlongwang.top

f(a: 1, b: 2)
来源：http://wdg.uphjek.com

[U57] PHP：字符串插值
来源：http://mdv.cdnleiting.top

"值: {$a}"
来源：http://gkh.316326.xyz

[U58] PHP：数组三件套
来源：http://bhj.shanyushiyangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wbu.yanxiufei.cn

[U59] PHP：自定义排序
来源：http://psq.ydjk.org.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bbj.hongshengwenyu.top

[U60] PHP：JSON 编解码
来源：http://jnv.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aof.ydjk.org.cn

[U61] PHP：正则
来源：http://xvk.nwbrower.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xud.hnxiangtu.top

[U62] PHP：日期对象
来源：http://kct.epnwcf.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mvc.fehbvm.com

[U63] PHP：文件读写
来源：http://ygt.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cul.ppjwa.cn

[U64] PHP：目录遍历
来源：http://lwf.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://etd.nanxuanxn.top

[U65] PHP：会话
来源：http://vof.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://zli.fzhhl.top

[U66] PHP：设置 Cookie
来源：http://emm.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://asp.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://fft.nanxinkj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zot.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://ldj.shuidangran.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pra.yj20258.top

[U69] PHP：PDO 预处理
来源：http://loc.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ndq.cucudq.cn

[U70] PHP：PDO 事务
来源：http://bbo.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mls.zdqjudy.top

[U71] PHP：抛出异常
来源：http://ckk.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://tkt.pycfn.com

[U72] PHP：写错误日志
来源：http://spt.sysykeji.top

error_log("失败: " . $e->getMessage());
来源：http://uki.gogol.net.cn

[U73] PHP：读取 ini 配置
来源：http://eow.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://hrv.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://qly.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://pam.yvedp.cn

[U75] PHP：依赖注入
来源：http://esd.gotoacloud.top

composer require psr/container
来源：http://pir.fzhhl.top

[U76] PHP：简单路由
来源：http://exz.tian-w.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ouk.tianlin.xyz

[U77] PHP：模板渲染
来源：http://afp.chenzaomai.com

composer require twig/twig
来源：http://zrd.yongpay.top

[U78] PHP：单元测试
来源：http://tun.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://lqi.yueranfly.top


<!-- 参考信息 -->