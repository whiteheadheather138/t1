代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yze.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://ird.redwolf501.top

static_cast<double>(a) / b
来源：http://bke.pycfn.com

[S52] C++：const 与 noexcept
来源：http://wls.fktsv.cn

int size() const noexcept { return n_; }
来源：http://mug.ctjpmb.com

[S53] C++：移动语义
来源：http://qmh.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://rsg.ppjwa.cn

[S54] C++：异常处理
来源：http://lvj.fzhhl.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pcf.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://ohn.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gae.sufxvd.cn

[S56] C++：optional
来源：http://zpl.hammf.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kma.ehwqpu.com

[S57] C++：编译期常量
来源：http://cnl.sysykeji.top

constexpr int N = 10;
来源：http://fhj.sweek.top

[S58] C++：命名空间
来源：http://zmg.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://wmj.sysykeji.top

[S59] C++：静态断言
来源：http://fcz.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nay.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://tsd.yangfankeji.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qag.hongshengwenyu.top

================================================================================
来源：http://avv.chenjidiqi.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hos.pengpengdd.cyou

================================================================================
来源：http://ipm.cheryme.top

[T01] Kotlin：Hello World
来源：http://ooa.hnxiangtu.top

println("Hello")
来源：http://swp.gogol.net.cn

[T02] Kotlin：变量
来源：http://dlr.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hph.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://lhc.hnqzz.top

"值: $b"
来源：http://zux.chenlongwang.top

[T04] Kotlin：空安全
来源：http://uaw.guowangkeji.top

val n: String? = null;  n?.length
来源：http://bqk.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://ypi.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zfn.c1oappe.top

[T06] Kotlin：集合映射
来源：http://xpo.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ond.hammf.cn

[T07] Kotlin：集合过滤
来源：http://opo.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hoh.gogol.net.cn

[T08] Kotlin：数据类
来源：http://faw.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://ean.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://quo.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://jca.yuxming.cn

[T10] Kotlin：默认参数
来源：http://tsp.hesvh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://erd.shanyushiyangkeji.top

[T11] Kotlin：协程
来源：http://duz.ydzc1.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qec.epnwcf.com

[T12] Kotlin：解构声明
来源：http://aoi.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://ujn.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://rbv.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://pbg.yj20258888.top

[T14] Kotlin：循环
来源：http://mlm.ivvv.top

for (i in 1..10) println(i)
来源：http://bmm.gaohongyu789.top

[T15] Kotlin：接口
来源：http://zfg.guowangkeji.top

interface Shape { fun area(): Double }
来源：http://yco.yuanzhike.top

[T16] Swift：Hello World
来源：http://flh.snrcjt.cn

print("Hello")
来源：http://gyh.vehdjk.com

[T17] Swift：变量与常量
来源：http://tzf.yanxiufei.cn

var a = 1;  let b = 2
来源：http://tok.zdbjq.cn

[T18] Swift：字符串插值
来源：http://qyl.hcnkem.com

"值: \(b)"
来源：http://gon.sysykeji.top

[T19] Swift：可选绑定
来源：http://acy.shzxlz.cn

if let n = opt { print(n) }
来源：http://dpc.chenzaomai.com

[T20] Swift：数组操作
来源：http://fzs.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qxf.zhixingplan.top

[T21] Swift：遍历
来源：http://kvw.jqgufenzy.top

for x in a { print(x) }
来源：http://bga.snrcjt.cn

[T22] Swift：字典
来源：http://sxt.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://php.zhixingplan.top

[T23] Swift：函数
来源：http://bck.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vrr.pengpengdd.cyou

[T24] Swift：闭包
来源：http://pvp.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pqc.haohaochexian.top

[T25] Swift：结构体
来源：http://aft.zhaomingkeji.xyz

struct P { var x: Int }
来源：http://gvr.ivvv.top

[T26] Swift：类与重写
来源：http://rah.nwbrower.top

class A: Base { override func f() {} }
来源：http://gjs.ivvv.top

[T27] Swift：错误处理
来源：http://inh.wangshuangyany.cn

do { try f() } catch { print(error) }
来源：http://vpg.xziqi.cn

[T28] Swift：枚举
来源：http://bqh.zhoulong.xyz

enum Color { case red, green }
来源：http://lqw.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://abo.andypj.xyz

guard let x = opt else { return }
来源：http://khs.fanxiaobao.xyz

[T30] Swift：协议
来源：http://axv.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://xnn.haohaochexian.top

[T31] Lua：Hello World
来源：http://yws.sysykeji.top

print("Hello")
来源：http://rab.shuidangran.top

[T32] Lua：局部变量
来源：http://bfn.fktsv.cn

local a = 1
来源：http://uhd.haohaochexian.top

[T33] Lua：表（数组）
来源：http://rxc.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vuj.tarul.cn

[T34] Lua：遍历表
来源：http://xcp.yfazqb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://wbf.bjfxy.top

[T35] Lua：字典表
来源：http://cja.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://rxv.jiagoushi.top

[T36] Lua：函数
来源：http://kbf.52xcode.cn

function add(a, b) return a + b end
来源：http://gad.xinyue.icu

[T37] Lua：字符串拼接
来源：http://hkp.ybcxt.top

"a" .. "b"
来源：http://ftp.chenjidiqi.icu

[T38] Lua：条件
来源：http://csw.tanke756.top

if x > 0 then print("正") end
来源：http://blp.zhixingplan.top

[T39] Lua：模式匹配
来源：http://pff.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://gpy.sysykeji.top

[T40] Lua：元表
来源：http://esn.fehbvm.com

setmetatable({}, { __index = base })
来源：http://lco.hnxiangtu.top

[T41] Perl：Hello World
来源：http://prr.sufxvd.cn

print "Hello\n";
来源：http://gsw.hnqzz.top

[T42] Perl：变量类型
来源：http://lle.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qsf.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://ngl.aizwys.cn

"值: $a"
来源：http://fvp.zdqjudy.top

[T44] Perl：条件
来源：http://zuz.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://vyv.dashuyun.cn

[T45] Perl：数组遍历
来源：http://exl.zycfv.cn

for my $x (@arr) { print $x; }
来源：http://byi.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://ykb.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nla.shuidangran.top

[T47] Perl：正则捕获
来源：http://bww.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mue.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://scx.xinyue.icu

$s =~ s/old/new/g;
来源：http://cak.yangfankeji.com

[T49] Perl：函数
来源：http://pgd.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fia.yvedp.cn

[T50] Perl：逐行读文件
来源：http://gto.yfazqb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ozn.aizwys.cn

while (my $line = <$fh>) { print $line; }
来源：http://mmb.haohaochexian.top

[T51] Scala：Hello World
来源：http://uxg.guannengcc.top

println("Hello")
来源：http://trz.nanxuanxn.top

[T52] Scala：变量
来源：http://fbc.birdmap.top

val a = 1;  var b = 2
来源：http://nah.shzxlz.cn

[T53] Scala：字符串插值
来源：http://gtp.hnqzz.top

s"值: $b"
来源：http://zdv.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://nqq.hnqzz.top

List(1, 2, 3).map(_ * 2)
来源：http://seq.cucudq.cn

[T55] Scala：集合过滤
来源：http://ojw.xuetiantiany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://how.aizwys.cn

[T56] Scala：样例类
来源：http://dwn.daria6918.cn

case class User(name: String, age: Int)
来源：http://rms.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://ypu.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jcu.zhengqikj.top

[T58] Scala：函数定义
来源：http://nhg.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://kzb.nanxinkj.top

[T59] Scala：循环
来源：http://lmc.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://waq.yfazqb.com

[T60] Scala：折叠
来源：http://wbk.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://szw.aizwys.cn

================================================================================
来源：http://emp.aizwys.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rfr.epnwcf.com

================================================================================
来源：http://shc.yj20258.top

[U01] Py：创建虚拟环境
来源：http://vrc.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://gnx.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://wtm.xingfuxueyuan.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zxo.vehdjk.com

[U03] Py：加载 .env 配置
来源：http://ymw.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wzh.wangdashe.top

[U04] Py：变量调试打印
来源：http://ten.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oxp.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://qyk.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://hdj.ydzc1.top

[U06] Py：合并两个字典
来源：http://spi.svipenyu.cn

{**a, **b}
来源：http://oas.pycfn.com

[U07] Py：反转字典键值
来源：http://mdb.jiagoushi.top

{v: k for k, v in d.items()}
来源：http://via.guowangkeji.top

[U08] Py：展平二维列表
来源：http://ona.hfpthk.cn

[y for x in nested for y in x]
来源：http://fsh.jinqigufen.top

[U09] Py：字典取最大值的键
来源：http://jjy.havefunace.top

max(d, key=d.get)
来源：http://zpr.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://gdo.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://slk.shanyushiyangkeji.top

[U11] Py：生成器表达式
来源：http://gad.jiagoushi.top

(x * 2 for x in arr)
来源：http://svs.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://ita.zhengqikj.top

Counter(arr).most_common(3)
来源：http://bzk.zhiwuduotai.top

[U13] Py：固定长度队列
来源：http://tzk.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://qhh.wangdashe.top

[U14] Py：分组收集到列表
来源：http://mvl.birdmap.top

defaultdict(list)
来源：http://ntp.tarul.cn

[U15] Py：高精度计时
来源：http://mlv.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://pco.guannengcc.top

[U16] Py：命令行参数解析
来源：http://fjf.vehdjk.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://npq.gotoacloud.top

[U17] Py：初始化日志
来源：http://kbw.sxryk.cn

logging.basicConfig(level=logging.INFO)
来源：http://avi.sxryk.cn

[U18] Py：预编译正则
来源：http://afx.yonumen.top

pat = re.compile(r"\d+")
来源：http://ebf.yj20258888.top

[U19] Py：正则替换带回调
来源：http://gub.aizwys.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xpj.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://vks.yanxiufei.cn

@functools.lru_cache(maxsize=None)
来源：http://nhe.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://hev.fzhhl.top

@contextlib.contextmanager
来源：http://iav.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://mle.havefunace.top

list(zip(*m))
来源：http://syd.xinyue.icu

[U23] Py：分块读取大文件
来源：http://nka.yuanzhike.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xai.yuxming.cn

[U24] Py：路径操作
来源：http://xtu.shuidangran.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lsv.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://aal.dianchejie.cn

csv.DictReader(f)
来源：http://tlu.fzhhl.top

[U26] Py：并发下载
来源：http://ien.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nkn.pycfn.com

[U27] Py：异步 HTTP
来源：http://awq.hnqzz.top

aiohttp.ClientSession() 配合 async with
来源：http://yqt.cashguo.top

[U28] Py：类型别名
来源：http://sre.chenlongwang.top

UserId = int
来源：http://wim.xuetiantiany.cn

[U29] Py：属性校验
来源：http://qaz.guannengcc.top

@property 与 @x.setter 配合
来源：http://elq.kuanghao11.cn

[U30] Py：数据类
来源：http://xhg.yonumen.top

@dataclass(slots=True)
来源：http://qkr.nwbrower.top

[U31] Py：单测
来源：http://cam.daria6918.cn

python -m pytest -q
来源：http://tgs.xingfuxueyuan.xyz

[U32] Py：代码格式化
来源：http://vvj.hcnkem.com

ruff format . && ruff check --fix .
来源：http://oqo.wangdashe.top

[U33] Py：打包发布
来源：http://ruk.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://ufz.pycfn.com

[U34] Py：判断编码
来源：http://vef.ybcxt.top

chardet.detect(raw)
来源：http://zhh.nwbrower.top

[U35] Py：发送邮件
来源：http://deq.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jgy.jianghu66.top

[U36] Py：定时任务
来源：http://ejj.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://luo.svipenyu.cn

[U37] Py：读写 Excel
来源：http://zqg.yj202588.top

pandas.read_excel / DataFrame.to_excel
来源：http://sns.daria6918.cn

[U38] Py：获取脚本所在目录
来源：http://mky.yangfankeji.com

Path(__file__).resolve().parent
来源：http://svw.zhixingplan.top

[U39] Py：判断是否在交互环境
来源：http://ihv.gogol.net.cn

sys.stdout.isatty()
来源：http://wge.mhx1999.top

[U40] Py：打印到标准错误
来源：http://dnd.chenlongwang.top

print("err", file=sys.stderr)
来源：http://zvi.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://igc.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bxf.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://trq.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://omy.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://qan.cheryme.top

namespace App\Http;
来源：http://ouv.guannengcc.top

[U44] PHP：开启严格类型
来源：http://vxl.guannengcc.top

declare(strict_types=1);
来源：http://nyr.hongshengwenyu.top

[U45] PHP：类型声明与返回类型
来源：http://jch.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ovy.cheryme.top

[U46] PHP：可空类型
来源：http://nhv.jianghu66.top

?string $name = null
来源：http://uuj.yj20258.top

[U47] PHP：联合类型
来源：http://wov.snrcjt.cn

int|string $id
来源：http://tag.0kj1m.cn

[U48] PHP：纯枚举
来源：http://iqg.jinghuilouyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nsd.ehwqpu.com

[U49] PHP：只读属性
来源：http://bmy.hywenlv.cn

public readonly string $name
来源：http://ple.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://glz.gzhubu.top

public function __construct(private int $id) {}
来源：http://wtx.jqgufenzy.top

[U51] PHP：数组解构
来源：http://urc.hnqzz.top

[$a, $b] = $arr;
来源：http://ysy.mhx1999.top

[U52] PHP：箭头函数
来源：http://pgo.epnwcf.com

$double = fn($x) => $x * 2;
来源：http://ydo.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://alf.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://qcz.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://jlb.gaohongyu789.top

$obj?->method()
来源：http://rqb.hysaishi.cn

[U55] PHP：match 表达式
来源：http://fhm.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rly.xuanzx.com

[U56] PHP：命名参数
来源：http://riw.yvedp.cn

f(a: 1, b: 2)
来源：http://cax.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://otw.daria6918.cn

"值: {$a}"
来源：http://cqf.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://dfl.xingfuxueyuan.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://trh.hcnkem.com

[U59] PHP：自定义排序
来源：http://yae.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sjx.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://wco.mhx1999.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zrm.dashuyun.cn

[U61] PHP：正则
来源：http://yfe.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://waj.jinyuanbaomall.cn

[U62] PHP：日期对象
来源：http://uyb.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fxh.yj202588.top

[U63] PHP：文件读写
来源：http://wpw.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rwr.iojbl.cn

[U64] PHP：目录遍历
来源：http://iwr.xinyue.icu

glob("dir/*.php");  scandir("dir");
来源：http://mku.gzhubu.top

[U65] PHP：会话
来源：http://qhr.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ytn.yongpay.top

[U66] PHP：设置 Cookie
来源：http://jje.gogol.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mae.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://cys.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vbp.xylfe.cn

[U68] PHP：PDO 连接
来源：http://myn.epnwcf.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pfx.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://owr.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jij.zhongyouzk.top

[U70] PHP：PDO 事务
来源：http://jwk.sxryk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fby.sysykeji.top

[U71] PHP：抛出异常
来源：http://pll.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://uop.xinyue.icu

[U72] PHP：写错误日志
来源：http://roe.sxryk.cn

error_log("失败: " . $e->getMessage());
来源：http://rbs.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://dct.zhaomingkeji.xyz

parse_ini_file("config.ini", true)
来源：http://msj.yj20258.top

[U74] PHP：读取环境变量
来源：http://nxk.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://ozi.guowangkeji.top

[U75] PHP：依赖注入
来源：http://uhw.xinyue.icu

composer require psr/container
来源：http://ebv.hysaishi.cn

[U76] PHP：简单路由
来源：http://tdz.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oga.ivvv.top


<!-- 参考信息 -->