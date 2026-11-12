代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://txd.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://qgq.jinqigfzy.top

static_cast<double>(a) / b
来源：http://smx.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://dtk.yj20258.top

int size() const noexcept { return n_; }
来源：http://ikc.wangshuangyany.cn

[S53] C++：移动语义
来源：http://rui.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://stv.epnwcf.com

[S54] C++：异常处理
来源：http://jrh.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dng.zhixingplan.top

[S55] C++：结构化绑定
来源：http://csj.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tyj.zhongyouzk.top

[S56] C++：optional
来源：http://tpu.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dnl.jinqigufen.top

[S57] C++：编译期常量
来源：http://bbf.zhiwuduotai.top

constexpr int N = 10;
来源：http://iqm.svipenyu.cn

[S58] C++：命名空间
来源：http://vaj.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://kkt.pengpengdd.cyou

[S59] C++：静态断言
来源：http://gvk.iojbl.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://myt.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://tro.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://grm.fehbvm.com

================================================================================
来源：http://uyg.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jmw.ydzc1.top

================================================================================
来源：http://rux.bjfxy.top

[T01] Kotlin：Hello World
来源：http://msx.dianchejie.cn

println("Hello")
来源：http://lrb.sufxvd.cn

[T02] Kotlin：变量
来源：http://hme.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://npr.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://vko.ctjpmb.com

"值: $b"
来源：http://rwd.ppjwa.cn

[T04] Kotlin：空安全
来源：http://wnl.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://saz.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://xfr.jqgufenzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nah.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://ssv.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gmi.cqqwz.cn

[T07] Kotlin：集合过滤
来源：http://mtf.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://zfs.smart0.xyz

[T08] Kotlin：数据类
来源：http://gbj.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://ves.tanke756.top

[T09] Kotlin：扩展函数
来源：http://tic.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://nkg.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://xjt.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ydh.dashuyun.cn

[T11] Kotlin：协程
来源：http://noe.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sqt.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://emg.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://xdp.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://ogy.nanxinkj.top

val m = mapOf("a" to 1)
来源：http://ezz.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://xkb.meibo888.top

for (i in 1..10) println(i)
来源：http://nod.pycfn.com

[T15] Kotlin：接口
来源：http://tfu.daria6918.cn

interface Shape { fun area(): Double }
来源：http://jij.yueranfly.top

[T16] Swift：Hello World
来源：http://skw.hnqzz.top

print("Hello")
来源：http://fyc.gotoacloud.top

[T17] Swift：变量与常量
来源：http://srm.c1oappe.top

var a = 1;  let b = 2
来源：http://osx.ivvv.top

[T18] Swift：字符串插值
来源：http://zwp.zhiwuduotai.top

"值: \(b)"
来源：http://xlk.bbcook.cn

[T19] Swift：可选绑定
来源：http://rta.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://tjh.sysykeji.top

[T20] Swift：数组操作
来源：http://yjw.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tju.xinyue.icu

[T21] Swift：遍历
来源：http://ytq.aizwys.cn

for x in a { print(x) }
来源：http://ztt.yonumen.top

[T22] Swift：字典
来源：http://qww.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://tqt.sufxvd.cn

[T23] Swift：函数
来源：http://usz.jyoumei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xih.yuanzhike.top

[T24] Swift：闭包
来源：http://vyr.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gcx.yj20258888.top

[T25] Swift：结构体
来源：http://dac.ydzc1.top

struct P { var x: Int }
来源：http://alh.hongshengwenyu.top

[T26] Swift：类与重写
来源：http://edz.meibo888.top

class A: Base { override func f() {} }
来源：http://uxs.havefunace.top

[T27] Swift：错误处理
来源：http://cin.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://glc.epnwcf.com

[T28] Swift：枚举
来源：http://jkk.redwolf501.top

enum Color { case red, green }
来源：http://pks.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://xdr.sysykeji.top

guard let x = opt else { return }
来源：http://qvv.yfazqb.com

[T30] Swift：协议
来源：http://nrs.wangdashe.top

protocol Shape { func area() -> Double }
来源：http://dnd.shzxlz.cn

[T31] Lua：Hello World
来源：http://pcc.daria6918.cn

print("Hello")
来源：http://alb.bjfxy.top

[T32] Lua：局部变量
来源：http://txh.xinyue.icu

local a = 1
来源：http://twh.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://wya.chenzaomai.com

local t = {1, 2, 3};  t[4] = 4
来源：http://bgq.aibaodan.cn

[T34] Lua：遍历表
来源：http://lot.daxiang520.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fjn.mhx1999.top

[T35] Lua：字典表
来源：http://toe.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://fgg.pycfn.com

[T36] Lua：函数
来源：http://atd.ctjpmb.com

function add(a, b) return a + b end
来源：http://aqh.yueranfly.top

[T37] Lua：字符串拼接
来源：http://bhm.yj20258.top

"a" .. "b"
来源：http://pjo.zhixingplan.top

[T38] Lua：条件
来源：http://igo.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://kak.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://qmy.yj202588.top

string.find(s, "%d+")
来源：http://wti.yonumen.top

[T40] Lua：元表
来源：http://kqp.wangdashe.top

setmetatable({}, { __index = base })
来源：http://vsz.shzxlz.cn

[T41] Perl：Hello World
来源：http://cvs.zdqjudy.top

print "Hello\n";
来源：http://hvz.cashguo.top

[T42] Perl：变量类型
来源：http://nxf.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zhw.hcnkem.com

[T43] Perl：字符串插值
来源：http://jww.ywan-chungtsiang.top

"值: $a"
来源：http://nca.quarkkingdee.top

[T44] Perl：条件
来源：http://ath.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://sma.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://jwm.shuidangran.top

for my $x (@arr) { print $x; }
来源：http://tck.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://wde.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xsc.svipenyu.cn

[T47] Perl：正则捕获
来源：http://hbw.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://kni.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://cxr.pycfn.com

$s =~ s/old/new/g;
来源：http://olm.ctjpmb.com

[T49] Perl：函数
来源：http://bpx.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zez.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://mic.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lqy.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://hlh.jlsjyb.cn

[T51] Scala：Hello World
来源：http://hjv.sxryk.cn

println("Hello")
来源：http://bsu.0kj1m.cn

[T52] Scala：变量
来源：http://exa.jianghu66.top

val a = 1;  var b = 2
来源：http://udg.tianlin.xyz

[T53] Scala：字符串插值
来源：http://zga.tian-w.cn

s"值: $b"
来源：http://xcd.ybcxt.top

[T54] Scala：集合映射
来源：http://shc.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://dnd.wangdashe.top

[T55] Scala：集合过滤
来源：http://lac.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://ttj.haohaochexian.top

[T56] Scala：样例类
来源：http://fkd.hywenlv.cn

case class User(name: String, age: Int)
来源：http://yjf.yfazqb.com

[T57] Scala：模式匹配
来源：http://rfl.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dru.nanxuanxn.top

[T58] Scala：函数定义
来源：http://caj.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://cjq.shangyingyoupin.top

[T59] Scala：循环
来源：http://bge.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://zqc.jiagoushi.top

[T60] Scala：折叠
来源：http://waf.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ici.hongshengwenyu.top

================================================================================
来源：http://jzi.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blb.nanxinkj.top

================================================================================
来源：http://oxw.cashguo.top

[U01] Py：创建虚拟环境
来源：http://gag.jqgfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://cpz.xuetiantiany.cn

[U02] Py：导出 / 安装依赖
来源：http://ypw.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mhw.ivvv.top

[U03] Py：加载 .env 配置
来源：http://bel.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cvd.xingfuxueyuan.xyz

[U04] Py：变量调试打印
来源：http://ztg.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lbz.daria6918.cn

[U05] Py：列表去重且保序
来源：http://tzn.snrcjt.cn

list(dict.fromkeys(arr))
来源：http://mfq.redwolf501.top

[U06] Py：合并两个字典
来源：http://jmf.zhaomingkeji.xyz

{**a, **b}
来源：http://odp.tanke756.top

[U07] Py：反转字典键值
来源：http://pbk.daxiang520.top

{v: k for k, v in d.items()}
来源：http://cxn.xuanzx.com

[U08] Py：展平二维列表
来源：http://ott.ppjwa.cn

[y for x in nested for y in x]
来源：http://bme.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://mom.hesvh.cn

max(d, key=d.get)
来源：http://qdb.hcnkem.com

[U10] Py：按值排序字典
来源：http://zmy.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://elf.bjfxy.top

[U11] Py：生成器表达式
来源：http://nkl.yangfankeji.com

(x * 2 for x in arr)
来源：http://dmk.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://hzo.dianchejie.cn

Counter(arr).most_common(3)
来源：http://bha.zycfv.cn

[U13] Py：固定长度队列
来源：http://fit.bbcook.cn

deque(maxlen=10)
来源：http://fdc.ybcxt.top

[U14] Py：分组收集到列表
来源：http://jfd.redwolf501.top

defaultdict(list)
来源：http://exh.ydzc1.top

[U15] Py：高精度计时
来源：http://qky.sysykeji.top

t = time.perf_counter()
来源：http://dhs.yonumen.top

[U16] Py：命令行参数解析
来源：http://hhx.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nlk.hysaishi.cn

[U17] Py：初始化日志
来源：http://pqi.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://tej.ydzc1.top

[U18] Py：预编译正则
来源：http://czb.hnqzz.top

pat = re.compile(r"\d+")
来源：http://xpu.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://unm.sufxvd.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uya.fengsongda.top

[U20] Py：缓存函数结果
来源：http://vdh.gzhubu.top

@functools.lru_cache(maxsize=None)
来源：http://qsc.ctjpmb.com

[U21] Py：自定义上下文管理器
来源：http://uik.smart0.xyz

@contextlib.contextmanager
来源：http://xmr.jyoumei.cn

[U22] Py：矩阵转置
来源：http://cyz.jiagoushi.top

list(zip(*m))
来源：http://nrr.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://ris.ywan-chungtsiang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kne.bjfxy.top

[U24] Py：路径操作
来源：http://lzk.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bss.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://vmx.quarkkingdee.top

csv.DictReader(f)
来源：http://rlh.guannengcc.top

[U26] Py：并发下载
来源：http://qnf.xuanzx.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://asf.xuetiantiany.cn

[U27] Py：异步 HTTP
来源：http://ynd.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://byz.jiagoushi.top

[U28] Py：类型别名
来源：http://qvv.ybcxt.top

UserId = int
来源：http://pqk.jiagoushi.top

[U29] Py：属性校验
来源：http://qmz.fengsongda.top

@property 与 @x.setter 配合
来源：http://igw.fktsv.cn

[U30] Py：数据类
来源：http://qan.ppjwa.cn

@dataclass(slots=True)
来源：http://kvt.bbcook.cn

[U31] Py：单测
来源：http://nbx.uphjek.com

python -m pytest -q
来源：http://cas.guowangkeji.top

[U32] Py：代码格式化
来源：http://pel.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://ygf.cashguo.top

[U33] Py：打包发布
来源：http://kjg.shanyushiyangtech.top

python -m build  （依赖 pyproject.toml）
来源：http://qbo.yuxming.cn

[U34] Py：判断编码
来源：http://eqa.ppjwa.cn

chardet.detect(raw)
来源：http://xxq.tarul.cn

[U35] Py：发送邮件
来源：http://nzl.gzhubu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://svk.fktsv.cn

[U36] Py：定时任务
来源：http://qgm.jinghuilouyu.cn

schedule.every(10).minutes.do(job)
来源：http://zfl.sysykeji.top

[U37] Py：读写 Excel
来源：http://zff.gaohongyu789.top

pandas.read_excel / DataFrame.to_excel
来源：http://oaz.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://tyj.sxryk.cn

Path(__file__).resolve().parent
来源：http://iuw.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://mle.zhijiandao.cn

sys.stdout.isatty()
来源：http://phz.ctjpmb.com

[U40] Py：打印到标准错误
来源：http://gni.zycfv.cn

print("err", file=sys.stderr)
来源：http://cuv.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://kws.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cju.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://ddd.fengsongda.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dhm.ydjk.org.cn

[U43] PHP：声明命名空间
来源：http://meu.yanxiufei.cn

namespace App\Http;
来源：http://epg.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://ctp.yj202588.top

declare(strict_types=1);
来源：http://xgp.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://bwm.quarkkingdee.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ggr.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://vtx.zhiwuduotai.top

?string $name = null
来源：http://mrc.kuanghao11.cn

[U47] PHP：联合类型
来源：http://cfe.jinyuanbaomall.cn

int|string $id
来源：http://zoc.yj20258.top

[U48] PHP：纯枚举
来源：http://bna.sufxvd.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mnh.jianghu66.top

[U49] PHP：只读属性
来源：http://rzg.bbcook.cn

public readonly string $name
来源：http://ixd.zhiwuduotai.top

[U50] PHP：构造器属性提升
来源：http://dcw.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://kwv.zhiwuduotai.top

[U51] PHP：数组解构
来源：http://krj.vqdsnc.cn

[$a, $b] = $arr;
来源：http://bnj.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://omj.vehdjk.com

$double = fn($x) => $x * 2;
来源：http://dxy.zdbjq.cn

[U53] PHP：空合并运算符
来源：http://iyb.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://mdt.hfpthk.cn

[U54] PHP：空安全调用
来源：http://cxl.yongpay.top

$obj?->method()
来源：http://exz.havefunace.top

[U55] PHP：match 表达式
来源：http://cti.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://efk.zhijiandao.cn

[U56] PHP：命名参数
来源：http://odz.bbcook.cn

f(a: 1, b: 2)
来源：http://bjp.ctjpmb.com

[U57] PHP：字符串插值
来源：http://who.yvedp.cn

"值: {$a}"
来源：http://fyk.zdqjudy.top

[U58] PHP：数组三件套
来源：http://hgb.jianghu66.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kaq.nanxinkj.top

[U59] PHP：自定义排序
来源：http://wdr.chenjidiqi.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://inq.zhaomingkeji.xyz

[U60] PHP：JSON 编解码
来源：http://hph.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mli.cheryme.top

[U61] PHP：正则
来源：http://nyl.jinyuanbaomall.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wor.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://xag.quarkkingdee.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oyp.9152youxi.cn

[U63] PHP：文件读写
来源：http://wlv.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ple.kuanghao11.cn

[U64] PHP：目录遍历
来源：http://caa.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://iio.cheryme.top

[U65] PHP：会话
来源：http://iil.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://itl.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://naf.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fqk.yj20258.top

[U67] PHP：处理文件上传
来源：http://blc.zhixingplan.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ltr.yj202588.top

[U68] PHP：PDO 连接
来源：http://ogc.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sss.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://vgv.daxiang520.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zrk.hongshengwenyu.top

[U70] PHP：PDO 事务
来源：http://gml.smart0.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://frp.iojbl.cn

[U71] PHP：抛出异常
来源：http://vaq.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://xqd.haohaochexian.top

[U72] PHP：写错误日志
来源：http://yew.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://tby.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://uws.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://ltp.iojbl.cn

[U74] PHP：读取环境变量
来源：http://hvc.zhaomingkeji.xyz

getenv("APP_ENV") ?: "production"
来源：http://tsl.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://jro.feifeiyinyue.top

composer require psr/container
来源：http://qwc.hfpthk.cn

[U76] PHP：简单路由
来源：http://atg.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dlv.ctjpmb.com


<!-- 参考信息 -->