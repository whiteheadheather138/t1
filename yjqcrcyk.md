代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ptu.0kj1m.cn

[S51] C++：显式类型转换
来源：http://est.aizwys.cn

static_cast<double>(a) / b
来源：http://ouj.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://uzx.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://tbx.sysykeji.top

[S53] C++：移动语义
来源：http://uqk.yj202588.top

std::vector<int> w = std::move(v);
来源：http://iss.ppjwa.cn

[S54] C++：异常处理
来源：http://moc.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ybu.bjfxy.top

[S55] C++：结构化绑定
来源：http://azg.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mgr.hongshengwenyu.top

[S56] C++：optional
来源：http://ocp.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://faf.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://rii.daxiang520.top

constexpr int N = 10;
来源：http://nhb.yj202588.top

[S58] C++：命名空间
来源：http://sgi.meibo888.top

namespace ns { int f() { return 1; } }
来源：http://rhg.sysykeji.top

[S59] C++：静态断言
来源：http://dxk.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nkr.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://ziw.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ykk.ppjwa.cn

================================================================================
来源：http://wlf.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://glf.yonumen.top

================================================================================
来源：http://jmh.fehbvm.com

[T01] Kotlin：Hello World
来源：http://lsn.jiagoushi.top

println("Hello")
来源：http://rgp.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://uqo.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://moh.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://ggk.birdmap.top

"值: $b"
来源：http://gih.cqqwz.cn

[T04] Kotlin：空安全
来源：http://eao.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://vbw.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://yna.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mko.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://kjp.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://idl.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://css.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jrf.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://myf.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://zri.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://hyz.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://vzv.hammf.cn

[T10] Kotlin：默认参数
来源：http://gdu.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gej.c1oappe.top

[T11] Kotlin：协程
来源：http://ncx.xinyue.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://rul.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://idq.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://crh.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://ded.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://oyf.aibaodan.cn

[T14] Kotlin：循环
来源：http://hny.jiagoushi.top

for (i in 1..10) println(i)
来源：http://dmr.yvedp.cn

[T15] Kotlin：接口
来源：http://neo.yuanzhike.top

interface Shape { fun area(): Double }
来源：http://ijr.zhaomingkeji.xyz

[T16] Swift：Hello World
来源：http://kny.yvedp.cn

print("Hello")
来源：http://gep.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://wyb.yvedp.cn

var a = 1;  let b = 2
来源：http://wfk.shanyushiyangkeji.top

[T18] Swift：字符串插值
来源：http://gkt.yongpay.top

"值: \(b)"
来源：http://esf.haohaochexian.top

[T19] Swift：可选绑定
来源：http://czh.birdmap.top

if let n = opt { print(n) }
来源：http://pvv.ybcxt.top

[T20] Swift：数组操作
来源：http://qdw.cucudq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bqd.zhengqikj.top

[T21] Swift：遍历
来源：http://eqn.fengsongda.top

for x in a { print(x) }
来源：http://iky.kuanghao11.cn

[T22] Swift：字典
来源：http://eeq.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://pvr.vqdsnc.cn

[T23] Swift：函数
来源：http://dhz.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ltt.jqgfzy.top

[T24] Swift：闭包
来源：http://nzs.yj202588.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ebw.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://rdd.jlsjyb.cn

struct P { var x: Int }
来源：http://iqq.jinyuanbaomall.cn

[T26] Swift：类与重写
来源：http://kwf.ppjwa.cn

class A: Base { override func f() {} }
来源：http://mlb.jlsjyb.cn

[T27] Swift：错误处理
来源：http://umu.nanxuanxn.top

do { try f() } catch { print(error) }
来源：http://qnz.zhoulong.xyz

[T28] Swift：枚举
来源：http://req.havefunace.top

enum Color { case red, green }
来源：http://kfj.xinyue.icu

[T29] Swift：guard 提前返回
来源：http://qfo.yj20258888.top

guard let x = opt else { return }
来源：http://slz.9152youxi.cn

[T30] Swift：协议
来源：http://zea.meibo888.top

protocol Shape { func area() -> Double }
来源：http://gkl.uphjek.com

[T31] Lua：Hello World
来源：http://wri.zhixingplan.top

print("Hello")
来源：http://sbm.xylfe.cn

[T32] Lua：局部变量
来源：http://djp.yanxiufei.cn

local a = 1
来源：http://cwy.sxryk.cn

[T33] Lua：表（数组）
来源：http://ywl.zdqjudy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nqa.fengsongda.top

[T34] Lua：遍历表
来源：http://wdn.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mve.pengpengdd.cyou

[T35] Lua：字典表
来源：http://lsk.tianlin.xyz

local d = { a = 1 };  d.b = 2
来源：http://rxz.ehwqpu.com

[T36] Lua：函数
来源：http://gai.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://jgr.hnxiangtu.top

[T37] Lua：字符串拼接
来源：http://tek.tanke756.top

"a" .. "b"
来源：http://vbp.hesvh.cn

[T38] Lua：条件
来源：http://zjv.zhoulong.xyz

if x > 0 then print("正") end
来源：http://ygz.hysaishi.cn

[T39] Lua：模式匹配
来源：http://ndy.zhengqikj.top

string.find(s, "%d+")
来源：http://mrk.316326.xyz

[T40] Lua：元表
来源：http://moy.sweek.top

setmetatable({}, { __index = base })
来源：http://xmk.jqgufenzy.top

[T41] Perl：Hello World
来源：http://dos.wangdashe.top

print "Hello\n";
来源：http://ove.feifeiyinyue.top

[T42] Perl：变量类型
来源：http://gyr.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gzb.tian-w.cn

[T43] Perl：字符串插值
来源：http://ysw.tianlin.xyz

"值: $a"
来源：http://mjw.fanxiaobao.xyz

[T44] Perl：条件
来源：http://sey.zhijiandao.cn

if ($a > 0) { print "正"; }
来源：http://sbt.nanxinkj.top

[T45] Perl：数组遍历
来源：http://xcq.yj202588.top

for my $x (@arr) { print $x; }
来源：http://uio.yueranfly.top

[T46] Perl：哈希操作
来源：http://nph.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iej.hcnkem.com

[T47] Perl：正则捕获
来源：http://nlk.ydzc1.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://evc.nanxuanxn.top

[T48] Perl：正则替换
来源：http://snk.gzhubu.top

$s =~ s/old/new/g;
来源：http://awr.hnqzz.top

[T49] Perl：函数
来源：http://vzw.gaohongyu789.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uwh.ydjk.org.cn

[T50] Perl：逐行读文件
来源：http://ozf.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jiw.yj20258888.top

while (my $line = <$fh>) { print $line; }
来源：http://qma.redwolf501.top

[T51] Scala：Hello World
来源：http://fxd.aibaodan.cn

println("Hello")
来源：http://qlp.tanke756.top

[T52] Scala：变量
来源：http://qmc.snrcjt.cn

val a = 1;  var b = 2
来源：http://dfx.9152youxi.cn

[T53] Scala：字符串插值
来源：http://uzy.andypj.xyz

s"值: $b"
来源：http://zvh.yj20258.top

[T54] Scala：集合映射
来源：http://dnf.shangyingyoupin.top

List(1, 2, 3).map(_ * 2)
来源：http://ole.vehdjk.com

[T55] Scala：集合过滤
来源：http://lxc.cqqwz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bvb.jiagoushi.top

[T56] Scala：样例类
来源：http://bcr.fanxiaobao.xyz

case class User(name: String, age: Int)
来源：http://adk.316326.xyz

[T57] Scala：模式匹配
来源：http://oku.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oec.shzxlz.cn

[T58] Scala：函数定义
来源：http://exj.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://dor.havefunace.top

[T59] Scala：循环
来源：http://mps.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://iwx.guannengcc.top

[T60] Scala：折叠
来源：http://ola.havefunace.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cmh.yueranfly.top

================================================================================
来源：http://olq.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mbf.cqqwz.cn

================================================================================
来源：http://psr.hnxiangtu.top

[U01] Py：创建虚拟环境
来源：http://aaw.jinqigfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://bzo.ehwqpu.com

[U02] Py：导出 / 安装依赖
来源：http://arz.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aiq.jqgufenzy.top

[U03] Py：加载 .env 配置
来源：http://kzf.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://goz.fehbvm.com

[U04] Py：变量调试打印
来源：http://qhf.hammf.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zri.hcnkem.com

[U05] Py：列表去重且保序
来源：http://lxg.redwolf501.top

list(dict.fromkeys(arr))
来源：http://zlm.nanxuanxn.top

[U06] Py：合并两个字典
来源：http://agq.jlsjyb.cn

{**a, **b}
来源：http://njm.cucudq.cn

[U07] Py：反转字典键值
来源：http://xwg.aizwys.cn

{v: k for k, v in d.items()}
来源：http://syw.hfpthk.cn

[U08] Py：展平二维列表
来源：http://iiy.nanxuanxn.top

[y for x in nested for y in x]
来源：http://uek.jinqigufen.top

[U09] Py：字典取最大值的键
来源：http://wow.jianghu66.top

max(d, key=d.get)
来源：http://yzx.shanyushiyangkeji.top

[U10] Py：按值排序字典
来源：http://doh.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hkx.uphjek.com

[U11] Py：生成器表达式
来源：http://fol.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://bul.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://cqz.chenzaomai.com

Counter(arr).most_common(3)
来源：http://epg.svipenyu.cn

[U13] Py：固定长度队列
来源：http://ail.xziqi.cn

deque(maxlen=10)
来源：http://ixp.fzhhl.top

[U14] Py：分组收集到列表
来源：http://ivv.xylfe.cn

defaultdict(list)
来源：http://fol.dianchejie.cn

[U15] Py：高精度计时
来源：http://xkm.chenjidiqi.icu

t = time.perf_counter()
来源：http://phf.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://eth.havefunace.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fsm.zdqjudy.top

[U17] Py：初始化日志
来源：http://tjh.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://els.zycfv.cn

[U18] Py：预编译正则
来源：http://kqr.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://joj.bbcook.cn

[U19] Py：正则替换带回调
来源：http://kkf.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bxh.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://dcc.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://pvx.0kj1m.cn

[U21] Py：自定义上下文管理器
来源：http://ihx.yvedp.cn

@contextlib.contextmanager
来源：http://lna.wangdashe.top

[U22] Py：矩阵转置
来源：http://vhw.gaohongyu789.top

list(zip(*m))
来源：http://sht.ppjwa.cn

[U23] Py：分块读取大文件
来源：http://moy.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://byn.hnxiangtu.top

[U24] Py：路径操作
来源：http://zfw.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://amq.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://hxi.snrcjt.cn

csv.DictReader(f)
来源：http://oxf.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://tpv.guowangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aap.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://bfv.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://sjd.yuxming.cn

[U28] Py：类型别名
来源：http://qfg.bbcook.cn

UserId = int
来源：http://gqx.wangdashe.top

[U29] Py：属性校验
来源：http://fkr.iojbl.cn

@property 与 @x.setter 配合
来源：http://dvi.shangyingyoupin.top

[U30] Py：数据类
来源：http://vco.gotoacloud.top

@dataclass(slots=True)
来源：http://ofd.yongpay.top

[U31] Py：单测
来源：http://qyw.sxryk.cn

python -m pytest -q
来源：http://sei.chenlongwang.top

[U32] Py：代码格式化
来源：http://igf.sysykeji.top

ruff format . && ruff check --fix .
来源：http://zow.sxryk.cn

[U33] Py：打包发布
来源：http://qiw.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://arw.sxryk.cn

[U34] Py：判断编码
来源：http://xzz.ehwqpu.com

chardet.detect(raw)
来源：http://pfb.316326.xyz

[U35] Py：发送邮件
来源：http://lzu.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rjf.yanxiufei.cn

[U36] Py：定时任务
来源：http://twm.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://wol.shangyingyoupin.top

[U37] Py：读写 Excel
来源：http://ltd.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://xkv.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://jdl.havefunace.top

Path(__file__).resolve().parent
来源：http://huc.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://hzi.jinyuanbaomall.cn

sys.stdout.isatty()
来源：http://umy.bjfxy.top

[U40] Py：打印到标准错误
来源：http://yjw.jiagoushi.top

print("err", file=sys.stderr)
来源：http://kla.yonumen.top

[U41] PHP：初始化 Composer 项目
来源：http://pdz.nanxuanxn.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nic.birdmap.top

[U42] PHP：PSR-4 自动加载
来源：http://khx.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gxh.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://qpt.c1oappe.top

namespace App\Http;
来源：http://sew.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://vrv.dashuyun.cn

declare(strict_types=1);
来源：http://cgg.yonumen.top

[U45] PHP：类型声明与返回类型
来源：http://eyi.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ioh.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://ask.yanxiufei.cn

?string $name = null
来源：http://uqg.52xcode.cn

[U47] PHP：联合类型
来源：http://nvz.hongshengwenyu.top

int|string $id
来源：http://onq.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://emd.yj202588.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vef.tianlin.xyz

[U49] PHP：只读属性
来源：http://hzz.shzxlz.cn

public readonly string $name
来源：http://ekd.zhixingplan.top

[U50] PHP：构造器属性提升
来源：http://emg.hesvh.cn

public function __construct(private int $id) {}
来源：http://boc.chenzaomai.com

[U51] PHP：数组解构
来源：http://rtt.hesvh.cn

[$a, $b] = $arr;
来源：http://wpd.yuxming.cn

[U52] PHP：箭头函数
来源：http://atb.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://bsw.vehdjk.com

[U53] PHP：空合并运算符
来源：http://ezs.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://zsx.sxryk.cn

[U54] PHP：空安全调用
来源：http://qab.nanxuanxn.top

$obj?->method()
来源：http://xuw.fengsongda.top

[U55] PHP：match 表达式
来源：http://ame.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ptb.vqdsnc.cn

[U56] PHP：命名参数
来源：http://vas.meibo888.top

f(a: 1, b: 2)
来源：http://tup.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://byb.tarul.cn

"值: {$a}"
来源：http://vsh.fzhhl.top

[U58] PHP：数组三件套
来源：http://iod.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://irf.jianghu66.top

[U59] PHP：自定义排序
来源：http://ldw.tarul.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qpr.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://etw.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yje.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://fxe.sufxvd.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ifh.jianghu66.top

[U62] PHP：日期对象
来源：http://ddl.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nrd.aizwys.cn

[U63] PHP：文件读写
来源：http://acz.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rnb.yuxming.cn

[U64] PHP：目录遍历
来源：http://kbo.fktsv.cn

glob("dir/*.php");  scandir("dir");
来源：http://nwm.ivvv.top

[U65] PHP：会话
来源：http://rzq.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://gbt.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://uuk.wangdashe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cbf.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://xnp.guannengcc.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zke.chenjidiqi.icu

[U68] PHP：PDO 连接
来源：http://fua.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://doz.cucudq.cn

[U69] PHP：PDO 预处理
来源：http://clz.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eaz.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://eto.chenjidiqi.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://goa.aizwys.cn

[U71] PHP：抛出异常
来源：http://tpp.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://dnd.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://pjs.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://zle.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://ypv.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://xiz.jqgufenzy.top

[U74] PHP：读取环境变量
来源：http://xir.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://vrj.cheryme.top

[U75] PHP：依赖注入
来源：http://rmk.yfazqb.com

composer require psr/container
来源：http://uqk.mhx1999.top

[U76] PHP：简单路由
来源：http://iuo.tanke756.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hmo.yongpay.top


<!-- 参考信息 -->