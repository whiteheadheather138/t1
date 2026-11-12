代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://xop.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uvi.daria6918.cn

[S48] C++：逐行读文件
来源：http://ntj.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://wvt.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://dtl.ivvv.top

[S49] C++：写文件
来源：http://xnb.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xkl.vqdsnc.cn

[S50] C++：格式化数字
来源：http://ddh.nanxuanxn.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vxb.316326.xyz

[S51] C++：显式类型转换
来源：http://jto.cdnleiting.top

static_cast<double>(a) / b
来源：http://rzu.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://hgt.52xcode.cn

int size() const noexcept { return n_; }
来源：http://brr.chenzaomai.com

[S53] C++：移动语义
来源：http://sck.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://ihp.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://fzz.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pjr.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://foz.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hzz.zdbjq.cn

[S56] C++：optional
来源：http://yle.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xtm.hnqzz.top

[S57] C++：编译期常量
来源：http://vgy.shangyingyoupin.top

constexpr int N = 10;
来源：http://ndy.fzhhl.top

[S58] C++：命名空间
来源：http://pgx.zhaomingkeji.xyz

namespace ns { int f() { return 1; } }
来源：http://llc.feifeiyinyue.top

[S59] C++：静态断言
来源：http://yzj.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xwl.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://zxi.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ehz.daxiang520.top

================================================================================
来源：http://hau.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xpu.cheryme.top

================================================================================
来源：http://age.gzhubu.top

[T01] Kotlin：Hello World
来源：http://qim.sweek.top

println("Hello")
来源：http://slp.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://vcf.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://otk.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://vxf.chenzaomai.com

"值: $b"
来源：http://pkz.meibo888.top

[T04] Kotlin：空安全
来源：http://bbd.smart0.xyz

val n: String? = null;  n?.length
来源：http://ohz.yj20258.top

[T05] Kotlin：when 表达式
来源：http://srb.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pzb.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://axb.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lbo.uphjek.com

[T07] Kotlin：集合过滤
来源：http://wvl.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://akq.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://tfy.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://ngn.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://afz.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://njt.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://itw.sysykeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://unm.zhoulong.xyz

[T11] Kotlin：协程
来源：http://aso.mhx1999.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rwp.bjfxy.top

[T12] Kotlin：解构声明
来源：http://mld.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://gdu.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://iue.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://dos.cdnleiting.top

[T14] Kotlin：循环
来源：http://eqn.daxiang520.top

for (i in 1..10) println(i)
来源：http://bgg.aizwys.cn

[T15] Kotlin：接口
来源：http://nsi.jinqigufen.top

interface Shape { fun area(): Double }
来源：http://pul.xziqi.cn

[T16] Swift：Hello World
来源：http://gkb.fanxiaobao.xyz

print("Hello")
来源：http://xvp.jqgfzy.top

[T17] Swift：变量与常量
来源：http://gnn.gzhubu.top

var a = 1;  let b = 2
来源：http://kcf.xinyue.icu

[T18] Swift：字符串插值
来源：http://zme.hfpthk.cn

"值: \(b)"
来源：http://qcl.hfpthk.cn

[T19] Swift：可选绑定
来源：http://iyo.dianchejie.cn

if let n = opt { print(n) }
来源：http://rqw.jinqigfzy.top

[T20] Swift：数组操作
来源：http://iiq.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jmb.ppjwa.cn

[T21] Swift：遍历
来源：http://ojp.yuanzhike.top

for x in a { print(x) }
来源：http://can.xziqi.cn

[T22] Swift：字典
来源：http://utq.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qza.gzhubu.top

[T23] Swift：函数
来源：http://gaq.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yvt.sysykeji.top

[T24] Swift：闭包
来源：http://qqk.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://kkr.c1oappe.top

[T25] Swift：结构体
来源：http://jnh.hammf.cn

struct P { var x: Int }
来源：http://xbd.jqgufenzy.top

[T26] Swift：类与重写
来源：http://quj.ctjpmb.com

class A: Base { override func f() {} }
来源：http://jge.dashuyun.cn

[T27] Swift：错误处理
来源：http://hql.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://oul.jianghu66.top

[T28] Swift：枚举
来源：http://eha.bbcook.cn

enum Color { case red, green }
来源：http://cch.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://ekb.nwbrower.top

guard let x = opt else { return }
来源：http://ryc.ppjwa.cn

[T30] Swift：协议
来源：http://rzv.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://mmd.zhongyouzk.top

[T31] Lua：Hello World
来源：http://yzl.shanyushiyangtech.top

print("Hello")
来源：http://mxj.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://dnm.cdnleiting.top

local a = 1
来源：http://knw.wangshuangyany.cn

[T33] Lua：表（数组）
来源：http://gvs.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tug.hnqzz.top

[T34] Lua：遍历表
来源：http://lwq.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cnw.birdmap.top

[T35] Lua：字典表
来源：http://zms.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://dgp.quarkkingdee.top

[T36] Lua：函数
来源：http://lsi.xinyue.icu

function add(a, b) return a + b end
来源：http://tvb.hfpthk.cn

[T37] Lua：字符串拼接
来源：http://scv.xziqi.cn

"a" .. "b"
来源：http://kvd.ybcxt.top

[T38] Lua：条件
来源：http://qhr.ydjk.org.cn

if x > 0 then print("正") end
来源：http://byo.sxryk.cn

[T39] Lua：模式匹配
来源：http://dzd.xuanzx.com

string.find(s, "%d+")
来源：http://ecq.mhx1999.top

[T40] Lua：元表
来源：http://oqn.gzhubu.top

setmetatable({}, { __index = base })
来源：http://lrb.aizwys.cn

[T41] Perl：Hello World
来源：http://ofk.jinghuilouyu.cn

print "Hello\n";
来源：http://ute.fzhhl.top

[T42] Perl：变量类型
来源：http://nzw.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://snq.shuidangran.top

[T43] Perl：字符串插值
来源：http://iya.sjlbkw.cn

"值: $a"
来源：http://pzd.yonumen.top

[T44] Perl：条件
来源：http://cgb.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://xyi.cdnleiting.top

[T45] Perl：数组遍历
来源：http://hgz.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://ged.guowangkeji.top

[T46] Perl：哈希操作
来源：http://bys.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wxg.iojbl.cn

[T47] Perl：正则捕获
来源：http://dtz.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://gww.yanxiufei.cn

[T48] Perl：正则替换
来源：http://pfx.yangfankeji.com

$s =~ s/old/new/g;
来源：http://paf.aibaodan.cn

[T49] Perl：函数
来源：http://vvi.uphjek.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ncx.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://fte.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fsr.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://ixg.hysaishi.cn

[T51] Scala：Hello World
来源：http://lrm.xinyue.icu

println("Hello")
来源：http://ges.yongpay.top

[T52] Scala：变量
来源：http://ghi.svipenyu.cn

val a = 1;  var b = 2
来源：http://why.nanxinkj.top

[T53] Scala：字符串插值
来源：http://tkp.ywan-chungtsiang.top

s"值: $b"
来源：http://mkw.ivvv.top

[T54] Scala：集合映射
来源：http://fhr.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://wsy.cucudq.cn

[T55] Scala：集合过滤
来源：http://hrf.sysykeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://ren.yonumen.top

[T56] Scala：样例类
来源：http://mlw.yanxiufei.cn

case class User(name: String, age: Int)
来源：http://lxy.52xcode.cn

[T57] Scala：模式匹配
来源：http://lcx.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://epl.yfazqb.com

[T58] Scala：函数定义
来源：http://ait.sysykeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://zho.ivvv.top

[T59] Scala：循环
来源：http://kbw.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://psz.gaohongyu789.top

[T60] Scala：折叠
来源：http://icn.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lav.hnqzz.top

================================================================================
来源：http://wvg.nanxinkj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ryv.wangshuangyany.cn

================================================================================
来源：http://uwt.52xcode.cn

[U01] Py：创建虚拟环境
来源：http://zee.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://zdw.hesvh.cn

[U02] Py：导出 / 安装依赖
来源：http://yqb.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qfi.hnxiangtu.top

[U03] Py：加载 .env 配置
来源：http://cta.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://dij.0kj1m.cn

[U04] Py：变量调试打印
来源：http://dtb.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mcv.yongpay.top

[U05] Py：列表去重且保序
来源：http://qdh.pycfn.com

list(dict.fromkeys(arr))
来源：http://ixi.mhx1999.top

[U06] Py：合并两个字典
来源：http://jyi.fzhhl.top

{**a, **b}
来源：http://egy.vehdjk.com

[U07] Py：反转字典键值
来源：http://wmo.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://joi.gzhubu.top

[U08] Py：展平二维列表
来源：http://xfm.jinghuilouyu.cn

[y for x in nested for y in x]
来源：http://qhz.yonumen.top

[U09] Py：字典取最大值的键
来源：http://ysz.daria6918.cn

max(d, key=d.get)
来源：http://qdf.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://izj.ydzc1.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uzy.guannengcc.top

[U11] Py：生成器表达式
来源：http://etj.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://ltp.ydjk.org.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lea.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://vpo.cqqwz.cn

[U13] Py：固定长度队列
来源：http://yay.jqgfzy.top

deque(maxlen=10)
来源：http://cue.cheryme.top

[U14] Py：分组收集到列表
来源：http://vwu.316326.xyz

defaultdict(list)
来源：http://nym.meibo888.top

[U15] Py：高精度计时
来源：http://elu.xingfuxueyuan.xyz

t = time.perf_counter()
来源：http://iwj.316326.xyz

[U16] Py：命令行参数解析
来源：http://dyt.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eur.quarkkingdee.top

[U17] Py：初始化日志
来源：http://pnm.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://njc.gaohongyu789.top

[U18] Py：预编译正则
来源：http://bxf.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://kbj.jqgfzy.top

[U19] Py：正则替换带回调
来源：http://whb.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fsg.ybcxt.top

[U20] Py：缓存函数结果
来源：http://vqt.snrcjt.cn

@functools.lru_cache(maxsize=None)
来源：http://aol.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://lxm.zhiwuduotai.top

@contextlib.contextmanager
来源：http://eyk.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://uxo.ybcxt.top

list(zip(*m))
来源：http://bnp.zhixingplan.top

[U23] Py：分块读取大文件
来源：http://qhw.tarul.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jsj.jiagoushi.top

[U24] Py：路径操作
来源：http://rud.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ddx.zhengqikj.top

[U25] Py：CSV 按字典读
来源：http://hld.sxryk.cn

csv.DictReader(f)
来源：http://ivf.epnwcf.com

[U26] Py：并发下载
来源：http://pgx.chenjidiqi.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://luw.xinyue.icu

[U27] Py：异步 HTTP
来源：http://ghy.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://rcp.0kj1m.cn

[U28] Py：类型别名
来源：http://ggz.gzhubu.top

UserId = int
来源：http://eqg.birdmap.top

[U29] Py：属性校验
来源：http://gma.hfpthk.cn

@property 与 @x.setter 配合
来源：http://kre.vqdsnc.cn

[U30] Py：数据类
来源：http://wcq.sweek.top

@dataclass(slots=True)
来源：http://jzj.fanxiaobao.xyz

[U31] Py：单测
来源：http://sbu.chenjidiqi.icu

python -m pytest -q
来源：http://jhy.redwolf501.top

[U32] Py：代码格式化
来源：http://iwb.jqgufenzy.top

ruff format . && ruff check --fix .
来源：http://kcn.fzhhl.top

[U33] Py：打包发布
来源：http://wyw.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://rvu.guannengcc.top

[U34] Py：判断编码
来源：http://tyi.haohaochexian.top

chardet.detect(raw)
来源：http://ang.daxiang520.top

[U35] Py：发送邮件
来源：http://pwb.wangshuangyany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yxf.zhixingplan.top

[U36] Py：定时任务
来源：http://qok.guannengcc.top

schedule.every(10).minutes.do(job)
来源：http://dnx.yonumen.top

[U37] Py：读写 Excel
来源：http://fls.ydjk.org.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cwu.daria6918.cn

[U38] Py：获取脚本所在目录
来源：http://oxw.xinyue.icu

Path(__file__).resolve().parent
来源：http://iat.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://zjg.ctjpmb.com

sys.stdout.isatty()
来源：http://lhc.feifeiyinyue.top

[U40] Py：打印到标准错误
来源：http://vck.gotoacloud.top

print("err", file=sys.stderr)
来源：http://pap.yongpay.top

[U41] PHP：初始化 Composer 项目
来源：http://qmj.meibo888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pes.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://xio.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dgo.c1oappe.top

[U43] PHP：声明命名空间
来源：http://rmh.52xcode.cn

namespace App\Http;
来源：http://zvx.yanxiufei.cn

[U44] PHP：开启严格类型
来源：http://qoz.kuanghao11.cn

declare(strict_types=1);
来源：http://gzi.aibaodan.cn

[U45] PHP：类型声明与返回类型
来源：http://rot.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://tkg.yangfankeji.com

[U46] PHP：可空类型
来源：http://avm.dashuyun.cn

?string $name = null
来源：http://snx.tianlin.xyz

[U47] PHP：联合类型
来源：http://qsm.nanxuanxn.top

int|string $id
来源：http://ets.tarul.cn

[U48] PHP：纯枚举
来源：http://hxg.dashuyun.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vpl.kuanghao11.cn

[U49] PHP：只读属性
来源：http://qgf.yongpay.top

public readonly string $name
来源：http://uep.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://gnk.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://noj.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://npf.yvedp.cn

[$a, $b] = $arr;
来源：http://udh.zhijiandao.cn

[U52] PHP：箭头函数
来源：http://pzu.zdqjudy.top

$double = fn($x) => $x * 2;
来源：http://sjs.feifeiyinyue.top

[U53] PHP：空合并运算符
来源：http://tnk.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://evb.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://vis.ywan-chungtsiang.top

$obj?->method()
来源：http://ori.dashuyun.cn

[U55] PHP：match 表达式
来源：http://xso.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oiz.chenjidiqi.icu

[U56] PHP：命名参数
来源：http://xad.snrcjt.cn

f(a: 1, b: 2)
来源：http://nuo.haohaochexian.top

[U57] PHP：字符串插值
来源：http://xda.vqdsnc.cn

"值: {$a}"
来源：http://kpo.gzhubu.top

[U58] PHP：数组三件套
来源：http://vxn.yvedp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dhr.tianlin.xyz

[U59] PHP：自定义排序
来源：http://gpb.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fjq.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://vcy.tarul.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ugq.tianlin.xyz

[U61] PHP：正则
来源：http://irr.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ool.iojbl.cn

[U62] PHP：日期对象
来源：http://tcl.tanke756.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ued.zdbjq.cn

[U63] PHP：文件读写
来源：http://jlj.chenlongwang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://niv.gotoacloud.top

[U64] PHP：目录遍历
来源：http://ejt.snrcjt.cn

glob("dir/*.php");  scandir("dir");
来源：http://qjl.pycfn.com

[U65] PHP：会话
来源：http://jib.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cdb.daxiang520.top

[U66] PHP：设置 Cookie
来源：http://iiz.bjfxy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xgp.ivvv.top

[U67] PHP：处理文件上传
来源：http://mrf.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dto.fehbvm.com

[U68] PHP：PDO 连接
来源：http://mxs.hesvh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dlv.yongpay.top

[U69] PHP：PDO 预处理
来源：http://xuk.zycfv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://muv.daxiang520.top

[U70] PHP：PDO 事务
来源：http://iel.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sdh.zhixingplan.top

[U71] PHP：抛出异常
来源：http://ufb.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://xdn.yueranfly.top

[U72] PHP：写错误日志
来源：http://fpf.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://wff.vehdjk.com


<!-- 参考信息 -->