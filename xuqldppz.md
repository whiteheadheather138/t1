代发 wailian999

while (std::getline(in, line)) { }
来源：http://omq.tanke756.top

[S49] C++：写文件
来源：http://lrv.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sat.aizwys.cn

[S50] C++：格式化数字
来源：http://jxn.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cty.jinyuanbaomall.cn

[S51] C++：显式类型转换
来源：http://dwn.vehdjk.com

static_cast<double>(a) / b
来源：http://ruw.jianghu66.top

[S52] C++：const 与 noexcept
来源：http://urw.sysykeji.top

int size() const noexcept { return n_; }
来源：http://tqp.zhoulong.xyz

[S53] C++：移动语义
来源：http://lrc.uphjek.com

std::vector<int> w = std::move(v);
来源：http://vib.ivvv.top

[S54] C++：异常处理
来源：http://jqe.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://buj.jianghu66.top

[S55] C++：结构化绑定
来源：http://sni.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mqk.shanyushiyangtech.top

[S56] C++：optional
来源：http://duf.chenlongwang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mds.uphjek.com

[S57] C++：编译期常量
来源：http://mft.meibo888.top

constexpr int N = 10;
来源：http://vwg.hammf.cn

[S58] C++：命名空间
来源：http://ybt.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://gnw.birdmap.top

[S59] C++：静态断言
来源：http://xbe.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dds.quarkkingdee.top

[S60] C++：遍历并删除元素
来源：http://uzm.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bco.yfazqb.com

================================================================================
来源：http://gvz.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://akk.jinqigufen.top

================================================================================
来源：http://oym.zycfv.cn

[T01] Kotlin：Hello World
来源：http://ukb.xuanzx.com

println("Hello")
来源：http://osw.redwolf501.top

[T02] Kotlin：变量
来源：http://xke.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rhw.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://vlq.tian-w.cn

"值: $b"
来源：http://xek.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://jtl.yongpay.top

val n: String? = null;  n?.length
来源：http://itb.fzhhl.top

[T05] Kotlin：when 表达式
来源：http://yer.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lfe.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://vef.yvedp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fof.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://nuv.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ieh.meibo888.top

[T08] Kotlin：数据类
来源：http://iak.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://ecf.fzhhl.top

[T09] Kotlin：扩展函数
来源：http://arr.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://cpd.andypj.xyz

[T10] Kotlin：默认参数
来源：http://cgs.smart0.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://hcp.hywenlv.cn

[T11] Kotlin：协程
来源：http://dbf.cqqwz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gyn.hcnkem.com

[T12] Kotlin：解构声明
来源：http://agm.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://hki.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://axa.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://bgq.vehdjk.com

[T14] Kotlin：循环
来源：http://xko.ppjwa.cn

for (i in 1..10) println(i)
来源：http://ttr.yuanzhike.top

[T15] Kotlin：接口
来源：http://gvi.aibaodan.cn

interface Shape { fun area(): Double }
来源：http://yqz.shzxlz.cn

[T16] Swift：Hello World
来源：http://lqp.ydjk.org.cn

print("Hello")
来源：http://myi.vqdsnc.cn

[T17] Swift：变量与常量
来源：http://zyt.smart0.xyz

var a = 1;  let b = 2
来源：http://fub.tian-w.cn

[T18] Swift：字符串插值
来源：http://wkq.ywan-chungtsiang.top

"值: \(b)"
来源：http://lxn.meibo888.top

[T19] Swift：可选绑定
来源：http://kxo.jyoumei.cn

if let n = opt { print(n) }
来源：http://mwx.iojbl.cn

[T20] Swift：数组操作
来源：http://qmg.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://zlp.jqgfzy.top

[T21] Swift：遍历
来源：http://dkz.ppjwa.cn

for x in a { print(x) }
来源：http://tsj.pycfn.com

[T22] Swift：字典
来源：http://ygl.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://etm.yongpay.top

[T23] Swift：函数
来源：http://gxe.yonumen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bpa.yueranfly.top

[T24] Swift：闭包
来源：http://zqz.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://gby.aibaodan.cn

[T25] Swift：结构体
来源：http://sqf.cucudq.cn

struct P { var x: Int }
来源：http://boa.xylfe.cn

[T26] Swift：类与重写
来源：http://ywh.yangfankeji.com

class A: Base { override func f() {} }
来源：http://xwk.zhengqikj.top

[T27] Swift：错误处理
来源：http://hsx.nanxuanxn.top

do { try f() } catch { print(error) }
来源：http://lvq.wangdashe.top

[T28] Swift：枚举
来源：http://rmh.hysaishi.cn

enum Color { case red, green }
来源：http://jok.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://fku.yuxming.cn

guard let x = opt else { return }
来源：http://moj.fktsv.cn

[T30] Swift：协议
来源：http://qbl.sweek.top

protocol Shape { func area() -> Double }
来源：http://azi.nanxuanxn.top

[T31] Lua：Hello World
来源：http://brx.zycfv.cn

print("Hello")
来源：http://ecq.ydjk.org.cn

[T32] Lua：局部变量
来源：http://qtk.hammf.cn

local a = 1
来源：http://cqt.yvedp.cn

[T33] Lua：表（数组）
来源：http://lfq.hcnkem.com

local t = {1, 2, 3};  t[4] = 4
来源：http://lzm.tarul.cn

[T34] Lua：遍历表
来源：http://pbo.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://niz.svipenyu.cn

[T35] Lua：字典表
来源：http://fcm.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://oya.chenzaomai.com

[T36] Lua：函数
来源：http://bwd.xuetiantiany.cn

function add(a, b) return a + b end
来源：http://die.jinghuilouyu.cn

[T37] Lua：字符串拼接
来源：http://nmo.gaohongyu789.top

"a" .. "b"
来源：http://jvy.tianlin.xyz

[T38] Lua：条件
来源：http://bmg.jianghu66.top

if x > 0 then print("正") end
来源：http://lop.ppjwa.cn

[T39] Lua：模式匹配
来源：http://gse.pycfn.com

string.find(s, "%d+")
来源：http://upe.zhixingplan.top

[T40] Lua：元表
来源：http://xwp.zdqjudy.top

setmetatable({}, { __index = base })
来源：http://bzz.vehdjk.com

[T41] Perl：Hello World
来源：http://ujw.hywenlv.cn

print "Hello\n";
来源：http://xop.ehwqpu.com

[T42] Perl：变量类型
来源：http://yud.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xmj.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://cew.shangyingyoupin.top

"值: $a"
来源：http://npf.sxryk.cn

[T44] Perl：条件
来源：http://jlc.ivvv.top

if ($a > 0) { print "正"; }
来源：http://ebw.nwbrower.top

[T45] Perl：数组遍历
来源：http://sli.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://etp.epnwcf.com

[T46] Perl：哈希操作
来源：http://tak.nanxuanxn.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jaz.316326.xyz

[T47] Perl：正则捕获
来源：http://xyp.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qmp.yj20258.top

[T48] Perl：正则替换
来源：http://ggl.zdqjudy.top

$s =~ s/old/new/g;
来源：http://ajn.ydjk.org.cn

[T49] Perl：函数
来源：http://yyc.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qgz.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://dkp.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xwe.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://bhw.ydjk.org.cn

[T51] Scala：Hello World
来源：http://zhk.xuetiantiany.cn

println("Hello")
来源：http://zlm.feifeiyinyue.top

[T52] Scala：变量
来源：http://ido.hfpthk.cn

val a = 1;  var b = 2
来源：http://lcc.aibaodan.cn

[T53] Scala：字符串插值
来源：http://qyh.zycfv.cn

s"值: $b"
来源：http://iqf.cucudq.cn

[T54] Scala：集合映射
来源：http://gbp.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://oel.zdqjudy.top

[T55] Scala：集合过滤
来源：http://akg.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://ane.yvedp.cn

[T56] Scala：样例类
来源：http://rkx.shzxlz.cn

case class User(name: String, age: Int)
来源：http://avy.hfpthk.cn

[T57] Scala：模式匹配
来源：http://xti.quarkkingdee.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hqo.cucudq.cn

[T58] Scala：函数定义
来源：http://fvu.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kda.ydzc1.top

[T59] Scala：循环
来源：http://tbz.sxryk.cn

for (i <- 1 to 10) println(i)
来源：http://dfx.snrcjt.cn

[T60] Scala：折叠
来源：http://qip.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qjm.zhoulong.xyz

================================================================================
来源：http://cdi.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gxk.smart0.xyz

================================================================================
来源：http://bny.zhongyouzk.top

[U01] Py：创建虚拟环境
来源：http://aaa.jinghuilouyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cyw.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://hqy.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mco.ivvv.top

[U03] Py：加载 .env 配置
来源：http://ihz.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xak.cheryme.top

[U04] Py：变量调试打印
来源：http://hyc.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nyz.xylfe.cn

[U05] Py：列表去重且保序
来源：http://vrq.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://phu.epnwcf.com

[U06] Py：合并两个字典
来源：http://mtl.shangyingyoupin.top

{**a, **b}
来源：http://dxe.hfpthk.cn

[U07] Py：反转字典键值
来源：http://uvv.daxiang520.top

{v: k for k, v in d.items()}
来源：http://vbz.meibo888.top

[U08] Py：展平二维列表
来源：http://ssy.feifeiyinyue.top

[y for x in nested for y in x]
来源：http://ztz.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://rvv.sxryk.cn

max(d, key=d.get)
来源：http://wfv.zhijiandao.cn

[U10] Py：按值排序字典
来源：http://kjz.yj202588.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fjq.feifeiyinyue.top

[U11] Py：生成器表达式
来源：http://sps.haohaochexian.top

(x * 2 for x in arr)
来源：http://rpc.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://zsy.tianlin.xyz

Counter(arr).most_common(3)
来源：http://ptg.nanxinkj.top

[U13] Py：固定长度队列
来源：http://mwu.yj20258888.top

deque(maxlen=10)
来源：http://zug.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://kay.aizwys.cn

defaultdict(list)
来源：http://luk.jqgfzy.top

[U15] Py：高精度计时
来源：http://agw.epnwcf.com

t = time.perf_counter()
来源：http://izs.ctjpmb.com

[U16] Py：命令行参数解析
来源：http://ulf.shangyingyoupin.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hhk.zdqjudy.top

[U17] Py：初始化日志
来源：http://fkt.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://xkg.jinqigfzy.top

[U18] Py：预编译正则
来源：http://yol.yonumen.top

pat = re.compile(r"\d+")
来源：http://myv.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://pjd.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dpk.yonumen.top

[U20] Py：缓存函数结果
来源：http://zim.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://zjm.havefunace.top

[U21] Py：自定义上下文管理器
来源：http://xqm.52xcode.cn

@contextlib.contextmanager
来源：http://mfj.zhiwuduotai.top

[U22] Py：矩阵转置
来源：http://edv.andypj.xyz

list(zip(*m))
来源：http://okj.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://vlr.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yjr.daria6918.cn

[U24] Py：路径操作
来源：http://zqi.jianghu66.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://elb.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://kye.vehdjk.com

csv.DictReader(f)
来源：http://qop.ydzc1.top

[U26] Py：并发下载
来源：http://ozn.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bdw.jinghuilouyu.cn

[U27] Py：异步 HTTP
来源：http://geb.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://dum.hammf.cn

[U28] Py：类型别名
来源：http://jpm.wangdashe.top

UserId = int
来源：http://fth.ehwqpu.com

[U29] Py：属性校验
来源：http://ojx.sxryk.cn

@property 与 @x.setter 配合
来源：http://ngf.andypj.xyz

[U30] Py：数据类
来源：http://vua.chenzaomai.com

@dataclass(slots=True)
来源：http://osh.shangyingyoupin.top

[U31] Py：单测
来源：http://azb.shuidangran.top

python -m pytest -q
来源：http://gue.jinqigufen.top

[U32] Py：代码格式化
来源：http://vlu.nanxinkj.top

ruff format . && ruff check --fix .
来源：http://mcf.havefunace.top

[U33] Py：打包发布
来源：http://kvl.havefunace.top

python -m build  （依赖 pyproject.toml）
来源：http://zkj.jyoumei.cn

[U34] Py：判断编码
来源：http://apm.ctjpmb.com

chardet.detect(raw)
来源：http://smy.xingfuxueyuan.xyz

[U35] Py：发送邮件
来源：http://pft.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ihz.bjfxy.top

[U36] Py：定时任务
来源：http://buw.zhixingplan.top

schedule.every(10).minutes.do(job)
来源：http://wlq.wangdashe.top

[U37] Py：读写 Excel
来源：http://fob.bbcook.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mgf.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://jmq.zhaomingkeji.xyz

Path(__file__).resolve().parent
来源：http://tnb.yangfankeji.com

[U39] Py：判断是否在交互环境
来源：http://xdo.andypj.xyz

sys.stdout.isatty()
来源：http://kbs.jinyuanbaomall.cn

[U40] Py：打印到标准错误
来源：http://quy.zhiwuduotai.top

print("err", file=sys.stderr)
来源：http://vta.vqdsnc.cn

[U41] PHP：初始化 Composer 项目
来源：http://wop.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://iuc.yj202588.top

[U42] PHP：PSR-4 自动加载
来源：http://dtz.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jsz.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://vkw.bjfxy.top

namespace App\Http;
来源：http://cje.zycfv.cn

[U44] PHP：开启严格类型
来源：http://uls.svipenyu.cn

declare(strict_types=1);
来源：http://wms.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://hgk.0kj1m.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pgo.hysaishi.cn

[U46] PHP：可空类型
来源：http://nzn.shanyushiyangtech.top

?string $name = null
来源：http://kce.ydjk.org.cn

[U47] PHP：联合类型
来源：http://lgd.yangfankeji.com

int|string $id
来源：http://eqc.tanke756.top

[U48] PHP：纯枚举
来源：http://fqf.sweek.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://evt.nwbrower.top

[U49] PHP：只读属性
来源：http://icn.c1oappe.top

public readonly string $name
来源：http://zxd.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://mav.yj202588.top

public function __construct(private int $id) {}
来源：http://vxu.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://cyu.meibo888.top

[$a, $b] = $arr;
来源：http://yxo.ctjpmb.com

[U52] PHP：箭头函数
来源：http://nko.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://hbk.c1oappe.top

[U53] PHP：空合并运算符
来源：http://uaq.quarkkingdee.top

$v = $a ?? $b ?? "default";
来源：http://czg.yvedp.cn

[U54] PHP：空安全调用
来源：http://qov.andypj.xyz

$obj?->method()
来源：http://yvl.zhengqikj.top

[U55] PHP：match 表达式
来源：http://hsp.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zqd.hongshengwenyu.top

[U56] PHP：命名参数
来源：http://reo.52xcode.cn

f(a: 1, b: 2)
来源：http://gtp.fktsv.cn

[U57] PHP：字符串插值
来源：http://zoj.yuxming.cn

"值: {$a}"
来源：http://cvx.hammf.cn

[U58] PHP：数组三件套
来源：http://kqp.yj202588.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://skg.fktsv.cn

[U59] PHP：自定义排序
来源：http://owp.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://arl.hnqzz.top

[U60] PHP：JSON 编解码
来源：http://gad.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bsq.0kj1m.cn

[U61] PHP：正则
来源：http://shh.zhongyouzk.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aml.fktsv.cn

[U62] PHP：日期对象
来源：http://wet.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://poa.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://wos.zhengqikj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wde.jiagoushi.top

[U64] PHP：目录遍历
来源：http://rjy.cashguo.top

glob("dir/*.php");  scandir("dir");
来源：http://kxp.vehdjk.com

[U65] PHP：会话
来源：http://eix.yueranfly.top

session_start();  $_SESSION["uid"] = 1;
来源：http://amg.nwbrower.top

[U66] PHP：设置 Cookie
来源：http://tgm.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hxn.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://mfx.feifeiyinyue.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lhq.gzhubu.top

[U68] PHP：PDO 连接
来源：http://zdx.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ese.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://vhr.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ibu.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://uxo.fehbvm.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gff.gzhubu.top

[U71] PHP：抛出异常
来源：http://guw.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://qhr.meibo888.top

[U72] PHP：写错误日志
来源：http://qtb.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://dyg.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://myv.ydjk.org.cn

parse_ini_file("config.ini", true)
来源：http://rsw.hesvh.cn

[U74] PHP：读取环境变量
来源：http://dhb.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://kmt.ctjpmb.com


<!-- 参考信息 -->