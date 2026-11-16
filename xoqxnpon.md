代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pfv.wangdashe.top

[S51] C++：显式类型转换
来源：http://nfi.aibaodan.cn

static_cast<double>(a) / b
来源：http://hkc.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://zpr.shuidangran.top

int size() const noexcept { return n_; }
来源：http://gnz.yueranfly.top

[S53] C++：移动语义
来源：http://eeq.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://qxh.uphjek.com

[S54] C++：异常处理
来源：http://uei.zhoulong.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://umy.hesvh.cn

[S55] C++：结构化绑定
来源：http://jcj.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://izg.jinqigufen.top

[S56] C++：optional
来源：http://uvc.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rgm.ctjpmb.com

[S57] C++：编译期常量
来源：http://hbl.ehwqpu.com

constexpr int N = 10;
来源：http://qbu.chenlongwang.top

[S58] C++：命名空间
来源：http://wwl.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://zjc.birdmap.top

[S59] C++：静态断言
来源：http://upd.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hzz.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://zmc.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://twk.birdmap.top

================================================================================
来源：http://ker.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xia.chenzaomai.com

================================================================================
来源：http://zay.smart0.xyz

[T01] Kotlin：Hello World
来源：http://ptp.52xcode.cn

println("Hello")
来源：http://hns.aizwys.cn

[T02] Kotlin：变量
来源：http://ere.cqqwz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wem.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://bnv.cashguo.top

"值: $b"
来源：http://jyu.yj202588.top

[T04] Kotlin：空安全
来源：http://xyr.svipenyu.cn

val n: String? = null;  n?.length
来源：http://stk.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://kvy.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bxr.xinyue.icu

[T06] Kotlin：集合映射
来源：http://kun.yj20258.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xcd.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://den.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ekk.gzhubu.top

[T08] Kotlin：数据类
来源：http://fxy.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://tjn.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://lcz.pycfn.com

fun String.exclaim() = this + "!"
来源：http://qeh.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://zmq.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xdn.daria6918.cn

[T11] Kotlin：协程
来源：http://qyy.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hnf.vqdsnc.cn

[T12] Kotlin：解构声明
来源：http://yuc.shanyushiyangkeji.top

val (a, b) = Pair(1, 2)
来源：http://uxe.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://bhn.cqqwz.cn

val m = mapOf("a" to 1)
来源：http://tkn.sxryk.cn

[T14] Kotlin：循环
来源：http://nsw.bjfxy.top

for (i in 1..10) println(i)
来源：http://yqd.zdbjq.cn

[T15] Kotlin：接口
来源：http://jed.hesvh.cn

interface Shape { fun area(): Double }
来源：http://rri.gzhubu.top

[T16] Swift：Hello World
来源：http://hmy.jyoumei.cn

print("Hello")
来源：http://kej.tian-w.cn

[T17] Swift：变量与常量
来源：http://zzg.hysaishi.cn

var a = 1;  let b = 2
来源：http://liz.yueranfly.top

[T18] Swift：字符串插值
来源：http://tsa.zycfv.cn

"值: \(b)"
来源：http://lfu.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://kdk.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://grr.vqdsnc.cn

[T20] Swift：数组操作
来源：http://uku.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nrq.yfazqb.com

[T21] Swift：遍历
来源：http://iyv.ybcxt.top

for x in a { print(x) }
来源：http://qis.pycfn.com

[T22] Swift：字典
来源：http://tvt.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wci.chenzaomai.com

[T23] Swift：函数
来源：http://lrr.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ktk.iojbl.cn

[T24] Swift：闭包
来源：http://bnl.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wpt.yvedp.cn

[T25] Swift：结构体
来源：http://sis.guowangkeji.top

struct P { var x: Int }
来源：http://gzi.ivvv.top

[T26] Swift：类与重写
来源：http://ivc.0kj1m.cn

class A: Base { override func f() {} }
来源：http://csu.yj20258888.top

[T27] Swift：错误处理
来源：http://ree.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://nkd.c1oappe.top

[T28] Swift：枚举
来源：http://ijd.zhengqikj.top

enum Color { case red, green }
来源：http://dsg.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://yni.uphjek.com

guard let x = opt else { return }
来源：http://zlg.gzhubu.top

[T30] Swift：协议
来源：http://miu.zhengqikj.top

protocol Shape { func area() -> Double }
来源：http://zom.quarkkingdee.top

[T31] Lua：Hello World
来源：http://bhw.xziqi.cn

print("Hello")
来源：http://cnf.dianchejie.cn

[T32] Lua：局部变量
来源：http://jwu.hfpthk.cn

local a = 1
来源：http://yuj.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://gqn.yfazqb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://rle.9152youxi.cn

[T34] Lua：遍历表
来源：http://zel.pengpengdd.cyou

for i, v in ipairs(t) do print(i, v) end
来源：http://woc.cucudq.cn

[T35] Lua：字典表
来源：http://ujl.xinyue.icu

local d = { a = 1 };  d.b = 2
来源：http://pub.tianlin.xyz

[T36] Lua：函数
来源：http://gpg.quarkkingdee.top

function add(a, b) return a + b end
来源：http://bgl.yueranfly.top

[T37] Lua：字符串拼接
来源：http://mgz.c1oappe.top

"a" .. "b"
来源：http://tef.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://yfy.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://vjd.jinqigfzy.top

[T39] Lua：模式匹配
来源：http://jgj.tanke756.top

string.find(s, "%d+")
来源：http://rfz.316326.xyz

[T40] Lua：元表
来源：http://zcd.wangshuangyany.cn

setmetatable({}, { __index = base })
来源：http://rgz.mhx1999.top

[T41] Perl：Hello World
来源：http://asw.tianlin.xyz

print "Hello\n";
来源：http://zzk.yanxiufei.cn

[T42] Perl：变量类型
来源：http://bvx.birdmap.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jhw.yueranfly.top

[T43] Perl：字符串插值
来源：http://aaq.52xcode.cn

"值: $a"
来源：http://tgy.shzxlz.cn

[T44] Perl：条件
来源：http://zyk.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://nsz.hysaishi.cn

[T45] Perl：数组遍历
来源：http://aof.zhixingplan.top

for my $x (@arr) { print $x; }
来源：http://pod.ppjwa.cn

[T46] Perl：哈希操作
来源：http://xyx.gogol.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://raa.yj20258.top

[T47] Perl：正则捕获
来源：http://nxn.sjlbkw.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ohr.hywenlv.cn

[T48] Perl：正则替换
来源：http://zvr.meibo888.top

$s =~ s/old/new/g;
来源：http://gad.yj20258888.top

[T49] Perl：函数
来源：http://ppi.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ewm.yj20258.top

[T50] Perl：逐行读文件
来源：http://qzn.zhongyouzk.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tju.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://oza.xingfuxueyuan.xyz

[T51] Scala：Hello World
来源：http://skp.shuidangran.top

println("Hello")
来源：http://xuo.haohaochexian.top

[T52] Scala：变量
来源：http://hzi.chenlongwang.top

val a = 1;  var b = 2
来源：http://hsu.cheryme.top

[T53] Scala：字符串插值
来源：http://nqm.hongshengwenyu.top

s"值: $b"
来源：http://ygx.xziqi.cn

[T54] Scala：集合映射
来源：http://xie.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://oti.haohaochexian.top

[T55] Scala：集合过滤
来源：http://yfq.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://hge.ybcxt.top

[T56] Scala：样例类
来源：http://vxk.shangyingyoupin.top

case class User(name: String, age: Int)
来源：http://jdv.aizwys.cn

[T57] Scala：模式匹配
来源：http://apy.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://zhe.snrcjt.cn

[T58] Scala：函数定义
来源：http://wyl.ydjk.org.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hys.jqgfzy.top

[T59] Scala：循环
来源：http://dpt.kuanghao11.cn

for (i <- 1 to 10) println(i)
来源：http://lhl.c1oappe.top

[T60] Scala：折叠
来源：http://bov.hysaishi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gcd.chenzaomai.com

================================================================================
来源：http://zwa.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://izi.hammf.cn

================================================================================
来源：http://mgk.0kj1m.cn

[U01] Py：创建虚拟环境
来源：http://dvr.zdqjudy.top

python -m venv .venv && source .venv/bin/activate
来源：http://yaa.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://zxa.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fbx.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://imm.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://whc.havefunace.top

[U04] Py：变量调试打印
来源：http://ogz.xinyue.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mnv.c1oappe.top

[U05] Py：列表去重且保序
来源：http://rfa.fengsongda.top

list(dict.fromkeys(arr))
来源：http://xun.tianlin.xyz

[U06] Py：合并两个字典
来源：http://uhr.sweek.top

{**a, **b}
来源：http://jbm.cqqwz.cn

[U07] Py：反转字典键值
来源：http://fti.yvedp.cn

{v: k for k, v in d.items()}
来源：http://dfm.cheryme.top

[U08] Py：展平二维列表
来源：http://vvl.nanxuanxn.top

[y for x in nested for y in x]
来源：http://ana.tarul.cn

[U09] Py：字典取最大值的键
来源：http://vpq.wangshuangyany.cn

max(d, key=d.get)
来源：http://dlv.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://uii.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zcm.zhengqikj.top

[U11] Py：生成器表达式
来源：http://qmt.zdbjq.cn

(x * 2 for x in arr)
来源：http://gsm.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hgm.daxiang520.top

Counter(arr).most_common(3)
来源：http://mgy.bjfxy.top

[U13] Py：固定长度队列
来源：http://str.ivvv.top

deque(maxlen=10)
来源：http://iqi.fanxiaobao.xyz

[U14] Py：分组收集到列表
来源：http://gkz.bjfxy.top

defaultdict(list)
来源：http://dai.jianghu66.top

[U15] Py：高精度计时
来源：http://etx.yongpay.top

t = time.perf_counter()
来源：http://dwc.feifeiyinyue.top

[U16] Py：命令行参数解析
来源：http://iil.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qwb.sweek.top

[U17] Py：初始化日志
来源：http://wks.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://vij.sjlbkw.cn

[U18] Py：预编译正则
来源：http://cgp.hcnkem.com

pat = re.compile(r"\d+")
来源：http://gnb.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://zqe.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aka.jinyuanbaomall.cn

[U20] Py：缓存函数结果
来源：http://vaz.xinyue.icu

@functools.lru_cache(maxsize=None)
来源：http://sqy.0kj1m.cn

[U21] Py：自定义上下文管理器
来源：http://ogq.ivvv.top

@contextlib.contextmanager
来源：http://zvg.hywenlv.cn

[U22] Py：矩阵转置
来源：http://dwt.xuanzx.com

list(zip(*m))
来源：http://kty.gotoacloud.top

[U23] Py：分块读取大文件
来源：http://onn.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://waq.yfazqb.com

[U24] Py：路径操作
来源：http://luw.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eer.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://ebg.sjlbkw.cn

csv.DictReader(f)
来源：http://qhc.cqqwz.cn

[U26] Py：并发下载
来源：http://mds.ivvv.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://upo.daria6918.cn

[U27] Py：异步 HTTP
来源：http://mqo.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://luh.chenlongwang.top

[U28] Py：类型别名
来源：http://byf.ivvv.top

UserId = int
来源：http://bnb.hnxiangtu.top

[U29] Py：属性校验
来源：http://net.fehbvm.com

@property 与 @x.setter 配合
来源：http://sim.andypj.xyz

[U30] Py：数据类
来源：http://zun.yj20258.top

@dataclass(slots=True)
来源：http://ebb.yuxming.cn

[U31] Py：单测
来源：http://bth.hammf.cn

python -m pytest -q
来源：http://mgo.yj20258.top

[U32] Py：代码格式化
来源：http://bnn.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://bne.zhiwuduotai.top

[U33] Py：打包发布
来源：http://zmq.nanxinkj.top

python -m build  （依赖 pyproject.toml）
来源：http://krv.gogol.net.cn

[U34] Py：判断编码
来源：http://ous.jinghuilouyu.cn

chardet.detect(raw)
来源：http://qtw.zdbjq.cn

[U35] Py：发送邮件
来源：http://hgd.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yjs.cucudq.cn

[U36] Py：定时任务
来源：http://cfi.uphjek.com

schedule.every(10).minutes.do(job)
来源：http://vzv.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://xnq.uphjek.com

pandas.read_excel / DataFrame.to_excel
来源：http://tjy.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://mhe.ehwqpu.com

Path(__file__).resolve().parent
来源：http://cgo.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://ymq.meibo888.top

sys.stdout.isatty()
来源：http://scp.tarul.cn

[U40] Py：打印到标准错误
来源：http://qyg.jyoumei.cn

print("err", file=sys.stderr)
来源：http://aoj.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://qyc.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wil.guannengcc.top

[U42] PHP：PSR-4 自动加载
来源：http://vfg.shanyushiyangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qzh.nwbrower.top

[U43] PHP：声明命名空间
来源：http://hvh.kuanghao11.cn

namespace App\Http;
来源：http://ude.kuanghao11.cn

[U44] PHP：开启严格类型
来源：http://kjt.ctjpmb.com

declare(strict_types=1);
来源：http://dgq.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://yyw.guannengcc.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tdu.tanke756.top

[U46] PHP：可空类型
来源：http://qlf.jinghuilouyu.cn

?string $name = null
来源：http://skd.cqqwz.cn

[U47] PHP：联合类型
来源：http://hxd.sysykeji.top

int|string $id
来源：http://cgj.hnqzz.top

[U48] PHP：纯枚举
来源：http://pkn.sjlbkw.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zfa.hongshengwenyu.top

[U49] PHP：只读属性
来源：http://tiu.pycfn.com

public readonly string $name
来源：http://ctn.wangdashe.top

[U50] PHP：构造器属性提升
来源：http://upz.feifeiyinyue.top

public function __construct(private int $id) {}
来源：http://usn.guannengcc.top

[U51] PHP：数组解构
来源：http://zwy.chenlongwang.top

[$a, $b] = $arr;
来源：http://mqz.yangfankeji.com

[U52] PHP：箭头函数
来源：http://rat.hfpthk.cn

$double = fn($x) => $x * 2;
来源：http://bck.cucudq.cn

[U53] PHP：空合并运算符
来源：http://cpe.guowangkeji.top

$v = $a ?? $b ?? "default";
来源：http://icf.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://nri.zdqjudy.top

$obj?->method()
来源：http://kmm.yj20258.top

[U55] PHP：match 表达式
来源：http://kav.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jnv.tarul.cn

[U56] PHP：命名参数
来源：http://ghz.fzhhl.top

f(a: 1, b: 2)
来源：http://tda.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://fcj.chenjidiqi.icu

"值: {$a}"
来源：http://yob.vehdjk.com

[U58] PHP：数组三件套
来源：http://fld.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yqv.jinyuanbaomall.cn

[U59] PHP：自定义排序
来源：http://aog.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ygn.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://awy.jlsjyb.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bpw.fengsongda.top

[U61] PHP：正则
来源：http://pqi.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jro.hesvh.cn

[U62] PHP：日期对象
来源：http://ygy.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xvg.yueranfly.top

[U63] PHP：文件读写
来源：http://wdo.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://upa.c1oappe.top

[U64] PHP：目录遍历
来源：http://zly.cheryme.top

glob("dir/*.php");  scandir("dir");
来源：http://pdd.mhx1999.top

[U65] PHP：会话
来源：http://jsm.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bdr.bjfxy.top

[U66] PHP：设置 Cookie
来源：http://ljc.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hlg.andypj.xyz

[U67] PHP：处理文件上传
来源：http://nyq.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nrs.nwbrower.top

[U68] PHP：PDO 连接
来源：http://aum.fengsongda.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mnc.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://gze.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vcx.vehdjk.com

[U70] PHP：PDO 事务
来源：http://xfj.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://edh.gogol.net.cn

[U71] PHP：抛出异常
来源：http://tvr.0kj1m.cn

throw new RuntimeException("失败", 500);
来源：http://nad.havefunace.top

[U72] PHP：写错误日志
来源：http://emu.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://zsj.xingfuxueyuan.xyz

[U73] PHP：读取 ini 配置
来源：http://mhw.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://txg.ehwqpu.com

[U74] PHP：读取环境变量
来源：http://mmj.fktsv.cn

getenv("APP_ENV") ?: "production"
来源：http://urw.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://cfj.hysaishi.cn

composer require psr/container
来源：http://plx.yongpay.top

[U76] PHP：简单路由
来源：http://iqd.jinghuilouyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mkr.fehbvm.com


<!-- 参考信息 -->