代发 wailian999

while (std::getline(in, line)) { }
来源：http://waf.yj202588.top

[S49] C++：写文件
来源：http://jrq.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hsm.jinghuilouyu.cn

[S50] C++：格式化数字
来源：http://jeu.xingfuxueyuan.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iha.vqdsnc.cn

[S51] C++：显式类型转换
来源：http://pfb.xinyue.icu

static_cast<double>(a) / b
来源：http://pie.havefunace.top

[S52] C++：const 与 noexcept
来源：http://oao.pengpengdd.cyou

int size() const noexcept { return n_; }
来源：http://eww.hfpthk.cn

[S53] C++：移动语义
来源：http://vwj.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://bdo.zhengqikj.top

[S54] C++：异常处理
来源：http://kim.fengsongda.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bgw.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://upc.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nkt.9152youxi.cn

[S56] C++：optional
来源：http://ccp.shzxlz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ith.cdnleiting.top

[S57] C++：编译期常量
来源：http://zij.xinyue.icu

constexpr int N = 10;
来源：http://ejc.sjlbkw.cn

[S58] C++：命名空间
来源：http://xro.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://trq.yongpay.top

[S59] C++：静态断言
来源：http://fzo.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nxd.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://alj.epnwcf.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://agx.ehwqpu.com

================================================================================
来源：http://nhl.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zto.yongpay.top

================================================================================
来源：http://nxz.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://wqq.yueranfly.top

println("Hello")
来源：http://rre.nanxuanxn.top

[T02] Kotlin：变量
来源：http://cyn.hnqzz.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sbu.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://vsf.xingfuxueyuan.xyz

"值: $b"
来源：http://cni.yvedp.cn

[T04] Kotlin：空安全
来源：http://dum.hammf.cn

val n: String? = null;  n?.length
来源：http://xut.vehdjk.com

[T05] Kotlin：when 表达式
来源：http://kxl.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dji.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://dwu.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://gkt.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://jvx.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rdk.sufxvd.cn

[T08] Kotlin：数据类
来源：http://qgu.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://rdw.tanke756.top

[T09] Kotlin：扩展函数
来源：http://hcn.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://qor.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://mje.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mwp.xuanzx.com

[T11] Kotlin：协程
来源：http://ayb.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jyy.havefunace.top

[T12] Kotlin：解构声明
来源：http://ugz.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://rvq.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://vpv.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://tyc.xuetiantiany.cn

[T14] Kotlin：循环
来源：http://omp.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://uou.svipenyu.cn

[T15] Kotlin：接口
来源：http://cdt.hesvh.cn

interface Shape { fun area(): Double }
来源：http://xdd.chenlongwang.top

[T16] Swift：Hello World
来源：http://igd.yj20258888.top

print("Hello")
来源：http://kza.daxiang520.top

[T17] Swift：变量与常量
来源：http://lni.jlsjyb.cn

var a = 1;  let b = 2
来源：http://eos.cashguo.top

[T18] Swift：字符串插值
来源：http://xsz.ehwqpu.com

"值: \(b)"
来源：http://ygv.chenzaomai.com

[T19] Swift：可选绑定
来源：http://znb.zhixingplan.top

if let n = opt { print(n) }
来源：http://wst.tian-w.cn

[T20] Swift：数组操作
来源：http://gvg.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wmy.cheryme.top

[T21] Swift：遍历
来源：http://mel.jyoumei.cn

for x in a { print(x) }
来源：http://jrl.fktsv.cn

[T22] Swift：字典
来源：http://hkg.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://zxk.zdqjudy.top

[T23] Swift：函数
来源：http://wmn.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xco.yj202588.top

[T24] Swift：闭包
来源：http://zuo.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xuy.jianghu66.top

[T25] Swift：结构体
来源：http://znx.smart0.xyz

struct P { var x: Int }
来源：http://xfm.daria6918.cn

[T26] Swift：类与重写
来源：http://bwr.aizwys.cn

class A: Base { override func f() {} }
来源：http://ert.ppjwa.cn

[T27] Swift：错误处理
来源：http://sxd.zycfv.cn

do { try f() } catch { print(error) }
来源：http://cua.jianghu66.top

[T28] Swift：枚举
来源：http://anf.ybcxt.top

enum Color { case red, green }
来源：http://beb.cheryme.top

[T29] Swift：guard 提前返回
来源：http://uen.hcnkem.com

guard let x = opt else { return }
来源：http://sxr.zhoulong.xyz

[T30] Swift：协议
来源：http://oyo.yueranfly.top

protocol Shape { func area() -> Double }
来源：http://znf.zhijiandao.cn

[T31] Lua：Hello World
来源：http://puk.hcnkem.com

print("Hello")
来源：http://wrg.xziqi.cn

[T32] Lua：局部变量
来源：http://dha.zhijiandao.cn

local a = 1
来源：http://lnu.kuanghao11.cn

[T33] Lua：表（数组）
来源：http://foh.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mnn.yj20258.top

[T34] Lua：遍历表
来源：http://lgi.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ccj.guannengcc.top

[T35] Lua：字典表
来源：http://yel.smart0.xyz

local d = { a = 1 };  d.b = 2
来源：http://uvm.shangyingyoupin.top

[T36] Lua：函数
来源：http://smv.shanyushiyangtech.top

function add(a, b) return a + b end
来源：http://qjk.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://qzb.shanyushiyangtech.top

"a" .. "b"
来源：http://tbg.gogol.net.cn

[T38] Lua：条件
来源：http://hvr.ybcxt.top

if x > 0 then print("正") end
来源：http://vjb.cqqwz.cn

[T39] Lua：模式匹配
来源：http://alu.yj202588.top

string.find(s, "%d+")
来源：http://wjn.9152youxi.cn

[T40] Lua：元表
来源：http://rke.uphjek.com

setmetatable({}, { __index = base })
来源：http://iok.haohaochexian.top

[T41] Perl：Hello World
来源：http://bdz.cqqwz.cn

print "Hello\n";
来源：http://img.redwolf501.top

[T42] Perl：变量类型
来源：http://nwc.wangshuangyany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ooo.shangyingyoupin.top

[T43] Perl：字符串插值
来源：http://ims.nanxuanxn.top

"值: $a"
来源：http://mso.xylfe.cn

[T44] Perl：条件
来源：http://etk.sxryk.cn

if ($a > 0) { print "正"; }
来源：http://vxo.gotoacloud.top

[T45] Perl：数组遍历
来源：http://snr.gaohongyu789.top

for my $x (@arr) { print $x; }
来源：http://syq.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://nop.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sps.fehbvm.com

[T47] Perl：正则捕获
来源：http://shw.xziqi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qmd.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://wea.pycfn.com

$s =~ s/old/new/g;
来源：http://aer.hysaishi.cn

[T49] Perl：函数
来源：http://kou.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jlg.zycfv.cn

[T50] Perl：逐行读文件
来源：http://guq.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://atl.ydjk.org.cn

while (my $line = <$fh>) { print $line; }
来源：http://thz.sysykeji.top

[T51] Scala：Hello World
来源：http://gtp.xuetiantiany.cn

println("Hello")
来源：http://omj.hfpthk.cn

[T52] Scala：变量
来源：http://jnk.yj20258.top

val a = 1;  var b = 2
来源：http://ibj.zhengqikj.top

[T53] Scala：字符串插值
来源：http://ief.jiagoushi.top

s"值: $b"
来源：http://uuy.ydjk.org.cn

[T54] Scala：集合映射
来源：http://zbd.sysykeji.top

List(1, 2, 3).map(_ * 2)
来源：http://prg.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://pgr.sxryk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zto.ybcxt.top

[T56] Scala：样例类
来源：http://fyy.xylfe.cn

case class User(name: String, age: Int)
来源：http://sas.52xcode.cn

[T57] Scala：模式匹配
来源：http://xgm.nanxinkj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ybd.dianchejie.cn

[T58] Scala：函数定义
来源：http://vnk.c1oappe.top

def add(a: Int, b: Int): Int = a + b
来源：http://jyi.xinyue.icu

[T59] Scala：循环
来源：http://qlh.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://ujy.guowangkeji.top

[T60] Scala：折叠
来源：http://hrk.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://paz.jqgfzy.top

================================================================================
来源：http://kia.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qod.ydzc1.top

================================================================================
来源：http://kie.tian-w.cn

[U01] Py：创建虚拟环境
来源：http://ebj.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jdl.yonumen.top

[U02] Py：导出 / 安装依赖
来源：http://idq.redwolf501.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://skc.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://bpt.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://puc.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://grw.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wyr.fehbvm.com

[U05] Py：列表去重且保序
来源：http://ahf.birdmap.top

list(dict.fromkeys(arr))
来源：http://ucq.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://dkp.yj202588.top

{**a, **b}
来源：http://utc.cashguo.top

[U07] Py：反转字典键值
来源：http://srm.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://emm.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://xsd.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://ubg.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://axg.hysaishi.cn

max(d, key=d.get)
来源：http://cyp.epnwcf.com

[U10] Py：按值排序字典
来源：http://jgq.ivvv.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cau.tanke756.top

[U11] Py：生成器表达式
来源：http://ylj.zhaomingkeji.xyz

(x * 2 for x in arr)
来源：http://xgd.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ipa.hnqzz.top

Counter(arr).most_common(3)
来源：http://guk.tarul.cn

[U13] Py：固定长度队列
来源：http://gge.jiagoushi.top

deque(maxlen=10)
来源：http://gfj.zhoulong.xyz

[U14] Py：分组收集到列表
来源：http://wsr.havefunace.top

defaultdict(list)
来源：http://wjw.svipenyu.cn

[U15] Py：高精度计时
来源：http://vjj.c1oappe.top

t = time.perf_counter()
来源：http://erf.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://dkx.wangdashe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yzi.cashguo.top

[U17] Py：初始化日志
来源：http://ula.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://uif.yj202588.top

[U18] Py：预编译正则
来源：http://son.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://xgo.birdmap.top

[U19] Py：正则替换带回调
来源：http://nft.jiagoushi.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rhb.sjlbkw.cn

[U20] Py：缓存函数结果
来源：http://vqn.ywan-chungtsiang.top

@functools.lru_cache(maxsize=None)
来源：http://wfl.cqqwz.cn

[U21] Py：自定义上下文管理器
来源：http://vay.jqgfzy.top

@contextlib.contextmanager
来源：http://plo.fehbvm.com

[U22] Py：矩阵转置
来源：http://utz.iojbl.cn

list(zip(*m))
来源：http://jwd.ehwqpu.com

[U23] Py：分块读取大文件
来源：http://zws.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qid.havefunace.top

[U24] Py：路径操作
来源：http://ous.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://odk.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://zor.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://xgc.yuanzhike.top

[U26] Py：并发下载
来源：http://tqt.jinqigfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yyp.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://lkr.jqgufenzy.top

aiohttp.ClientSession() 配合 async with
来源：http://hxv.gaohongyu789.top

[U28] Py：类型别名
来源：http://jor.xziqi.cn

UserId = int
来源：http://cwt.fengsongda.top

[U29] Py：属性校验
来源：http://xco.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://hgm.316326.xyz

[U30] Py：数据类
来源：http://zma.xingfuxueyuan.xyz

@dataclass(slots=True)
来源：http://axg.52xcode.cn

[U31] Py：单测
来源：http://gpp.yj20258888.top

python -m pytest -q
来源：http://heb.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://vyw.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://cmu.pengpengdd.cyou

[U33] Py：打包发布
来源：http://ivt.epnwcf.com

python -m build  （依赖 pyproject.toml）
来源：http://pkq.fzhhl.top

[U34] Py：判断编码
来源：http://qmv.xylfe.cn

chardet.detect(raw)
来源：http://qql.cashguo.top

[U35] Py：发送邮件
来源：http://eka.shzxlz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vzj.jinghuilouyu.cn

[U36] Py：定时任务
来源：http://dag.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://dta.ehwqpu.com

[U37] Py：读写 Excel
来源：http://fgm.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://fnm.andypj.xyz

[U38] Py：获取脚本所在目录
来源：http://okr.zycfv.cn

Path(__file__).resolve().parent
来源：http://mxo.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://bvi.ehwqpu.com

sys.stdout.isatty()
来源：http://nkh.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://oxy.zdqjudy.top

print("err", file=sys.stderr)
来源：http://ryl.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ujj.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fzb.shzxlz.cn

[U42] PHP：PSR-4 自动加载
来源：http://hbl.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ppr.havefunace.top

[U43] PHP：声明命名空间
来源：http://hli.cheryme.top

namespace App\Http;
来源：http://cby.316326.xyz

[U44] PHP：开启严格类型
来源：http://vyw.hnxiangtu.top

declare(strict_types=1);
来源：http://hwb.nanxinkj.top

[U45] PHP：类型声明与返回类型
来源：http://zjq.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nar.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://rus.cqqwz.cn

?string $name = null
来源：http://gqk.yangfankeji.com

[U47] PHP：联合类型
来源：http://nqk.52xcode.cn

int|string $id
来源：http://fdv.xylfe.cn

[U48] PHP：纯枚举
来源：http://kym.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://txu.gogol.net.cn

[U49] PHP：只读属性
来源：http://jfk.jlsjyb.cn

public readonly string $name
来源：http://kie.gogol.net.cn

[U50] PHP：构造器属性提升
来源：http://bsb.yangfankeji.com

public function __construct(private int $id) {}
来源：http://ibo.shuidangran.top

[U51] PHP：数组解构
来源：http://meh.zhijiandao.cn

[$a, $b] = $arr;
来源：http://omy.epnwcf.com

[U52] PHP：箭头函数
来源：http://qch.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://gty.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://egh.wangshuangyany.cn

$v = $a ?? $b ?? "default";
来源：http://tes.sjlbkw.cn

[U54] PHP：空安全调用
来源：http://sps.hesvh.cn

$obj?->method()
来源：http://bfq.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://nrb.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iqo.jqgfzy.top

[U56] PHP：命名参数
来源：http://wjv.gzhubu.top

f(a: 1, b: 2)
来源：http://atb.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://jcz.yueranfly.top

"值: {$a}"
来源：http://zcv.andypj.xyz

[U58] PHP：数组三件套
来源：http://dcv.cqqwz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kka.xinyue.icu

[U59] PHP：自定义排序
来源：http://drb.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kpk.hnxiangtu.top

[U60] PHP：JSON 编解码
来源：http://jlf.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nfq.svipenyu.cn

[U61] PHP：正则
来源：http://toh.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mwq.smart0.xyz

[U62] PHP：日期对象
来源：http://rue.zdbjq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uuf.yvedp.cn

[U63] PHP：文件读写
来源：http://nbd.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gum.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://rbw.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://kca.yvedp.cn

[U65] PHP：会话
来源：http://wed.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uqr.aibaodan.cn

[U66] PHP：设置 Cookie
来源：http://eqs.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dib.daxiang520.top

[U67] PHP：处理文件上传
来源：http://uyq.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rqs.jqgufenzy.top

[U68] PHP：PDO 连接
来源：http://nuz.fanxiaobao.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://obb.316326.xyz

[U69] PHP：PDO 预处理
来源：http://iej.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rom.jianghu66.top

[U70] PHP：PDO 事务
来源：http://rno.hcnkem.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sfv.gogol.net.cn

[U71] PHP：抛出异常
来源：http://ald.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://hic.c1oappe.top

[U72] PHP：写错误日志
来源：http://rfu.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://ffg.vqdsnc.cn

[U73] PHP：读取 ini 配置
来源：http://wpi.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://tro.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://rbq.cqqwz.cn

getenv("APP_ENV") ?: "production"
来源：http://ugt.hongshengwenyu.top


<!-- 参考信息 -->