代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://ofi.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qjp.bbcook.cn

[S48] C++：逐行读文件
来源：http://jbb.smart0.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://jqx.birdmap.top

while (std::getline(in, line)) { }
来源：http://fjr.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://xfr.jinghuilouyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gec.jlsjyb.cn

[S50] C++：格式化数字
来源：http://ecw.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kel.vqdsnc.cn

[S51] C++：显式类型转换
来源：http://plp.xylfe.cn

static_cast<double>(a) / b
来源：http://ghm.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://yoy.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://xio.pycfn.com

[S53] C++：移动语义
来源：http://min.zdqjudy.top

std::vector<int> w = std::move(v);
来源：http://old.chenzaomai.com

[S54] C++：异常处理
来源：http://uqe.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://otq.tarul.cn

[S55] C++：结构化绑定
来源：http://kov.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ejv.zhengqikj.top

[S56] C++：optional
来源：http://frm.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dee.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://dbq.yueranfly.top

constexpr int N = 10;
来源：http://wlg.xuanzx.com

[S58] C++：命名空间
来源：http://wyo.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://mol.ydjk.org.cn

[S59] C++：静态断言
来源：http://idr.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qam.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://pgq.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qww.yj202588.top

================================================================================
来源：http://ocx.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mfo.sufxvd.cn

================================================================================
来源：http://ihf.yfazqb.com

[T01] Kotlin：Hello World
来源：http://jim.zhaomingkeji.xyz

println("Hello")
来源：http://edb.hnxiangtu.top

[T02] Kotlin：变量
来源：http://jrd.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ynw.316326.xyz

[T03] Kotlin：字符串模板
来源：http://ick.vqdsnc.cn

"值: $b"
来源：http://dnt.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://wls.zhengqikj.top

val n: String? = null;  n?.length
来源：http://jmm.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://qiq.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jli.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://vvh.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ycu.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://rlk.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://zun.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://plc.havefunace.top

data class User(val name: String, val age: Int)
来源：http://lrf.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://kqd.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://epa.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://pdh.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rxj.guowangkeji.top

[T11] Kotlin：协程
来源：http://fsm.jinghuilouyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://caf.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://aib.yanxiufei.cn

val (a, b) = Pair(1, 2)
来源：http://btu.yonumen.top

[T13] Kotlin：只读 Map
来源：http://dqk.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://ovy.fzhhl.top

[T14] Kotlin：循环
来源：http://qcr.xylfe.cn

for (i in 1..10) println(i)
来源：http://msu.c1oappe.top

[T15] Kotlin：接口
来源：http://gjh.yueranfly.top

interface Shape { fun area(): Double }
来源：http://bng.nanxuanxn.top

[T16] Swift：Hello World
来源：http://mce.jianghu66.top

print("Hello")
来源：http://wub.meibo888.top

[T17] Swift：变量与常量
来源：http://sms.pengpengdd.cyou

var a = 1;  let b = 2
来源：http://sby.guowangkeji.top

[T18] Swift：字符串插值
来源：http://guq.zhongyouzk.top

"值: \(b)"
来源：http://myl.uphjek.com

[T19] Swift：可选绑定
来源：http://iua.cashguo.top

if let n = opt { print(n) }
来源：http://gyl.jiagoushi.top

[T20] Swift：数组操作
来源：http://srx.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://zzw.shanyushiyangkeji.top

[T21] Swift：遍历
来源：http://otn.daxiang520.top

for x in a { print(x) }
来源：http://ihv.pycfn.com

[T22] Swift：字典
来源：http://aby.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hxn.fzhhl.top

[T23] Swift：函数
来源：http://yyq.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://flc.shanyushiyangkeji.top

[T24] Swift：闭包
来源：http://uvo.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mwb.jianghu66.top

[T25] Swift：结构体
来源：http://vzf.uphjek.com

struct P { var x: Int }
来源：http://yto.52xcode.cn

[T26] Swift：类与重写
来源：http://wuy.daxiang520.top

class A: Base { override func f() {} }
来源：http://ldk.nanxuanxn.top

[T27] Swift：错误处理
来源：http://ksa.xingfuxueyuan.xyz

do { try f() } catch { print(error) }
来源：http://uyi.fanxiaobao.xyz

[T28] Swift：枚举
来源：http://muy.nanxuanxn.top

enum Color { case red, green }
来源：http://kmn.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://aqn.jinghuilouyu.cn

guard let x = opt else { return }
来源：http://vcc.svipenyu.cn

[T30] Swift：协议
来源：http://bze.316326.xyz

protocol Shape { func area() -> Double }
来源：http://uqa.hesvh.cn

[T31] Lua：Hello World
来源：http://azs.zhongyouzk.top

print("Hello")
来源：http://rct.fzhhl.top

[T32] Lua：局部变量
来源：http://tck.ywan-chungtsiang.top

local a = 1
来源：http://hhi.jqgfzy.top

[T33] Lua：表（数组）
来源：http://mlf.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://ojb.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://aic.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rfq.zdqjudy.top

[T35] Lua：字典表
来源：http://vqa.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://sat.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://dxb.sufxvd.cn

function add(a, b) return a + b end
来源：http://dxu.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://zto.yonumen.top

"a" .. "b"
来源：http://ebs.xuetiantiany.cn

[T38] Lua：条件
来源：http://enw.cdnleiting.top

if x > 0 then print("正") end
来源：http://jog.guannengcc.top

[T39] Lua：模式匹配
来源：http://qvi.yfazqb.com

string.find(s, "%d+")
来源：http://jmh.jyoumei.cn

[T40] Lua：元表
来源：http://qot.havefunace.top

setmetatable({}, { __index = base })
来源：http://vkg.52xcode.cn

[T41] Perl：Hello World
来源：http://yju.quarkkingdee.top

print "Hello\n";
来源：http://tkc.zhixingplan.top

[T42] Perl：变量类型
来源：http://har.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iux.yj20258888.top

[T43] Perl：字符串插值
来源：http://sfp.ybcxt.top

"值: $a"
来源：http://jfi.sweek.top

[T44] Perl：条件
来源：http://uqo.ybcxt.top

if ($a > 0) { print "正"; }
来源：http://lnp.vehdjk.com

[T45] Perl：数组遍历
来源：http://xad.tianlin.xyz

for my $x (@arr) { print $x; }
来源：http://dkv.ctjpmb.com

[T46] Perl：哈希操作
来源：http://zzc.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jaj.yueranfly.top

[T47] Perl：正则捕获
来源：http://hyk.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zgs.nanxinkj.top

[T48] Perl：正则替换
来源：http://mij.xingfuxueyuan.xyz

$s =~ s/old/new/g;
来源：http://qev.yueranfly.top

[T49] Perl：函数
来源：http://jgg.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gpw.xylfe.cn

[T50] Perl：逐行读文件
来源：http://ixb.0kj1m.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ypn.aizwys.cn

while (my $line = <$fh>) { print $line; }
来源：http://suu.yj20258888.top

[T51] Scala：Hello World
来源：http://buu.c1oappe.top

println("Hello")
来源：http://pbn.yj20258888.top

[T52] Scala：变量
来源：http://yhm.jlsjyb.cn

val a = 1;  var b = 2
来源：http://ejh.hywenlv.cn

[T53] Scala：字符串插值
来源：http://vur.hongshengwenyu.top

s"值: $b"
来源：http://cng.nanxinkj.top

[T54] Scala：集合映射
来源：http://dox.fehbvm.com

List(1, 2, 3).map(_ * 2)
来源：http://yfy.zhaomingkeji.xyz

[T55] Scala：集合过滤
来源：http://pyk.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://fok.jinqigfzy.top

[T56] Scala：样例类
来源：http://vdr.sweek.top

case class User(name: String, age: Int)
来源：http://hir.mhx1999.top

[T57] Scala：模式匹配
来源：http://mss.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ipn.quarkkingdee.top

[T58] Scala：函数定义
来源：http://xas.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://dqm.fehbvm.com

[T59] Scala：循环
来源：http://pix.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://fgs.9152youxi.cn

[T60] Scala：折叠
来源：http://fua.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zuv.yj202588.top

================================================================================
来源：http://sjw.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cne.jqgfzy.top

================================================================================
来源：http://vkm.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://pqf.cheryme.top

python -m venv .venv && source .venv/bin/activate
来源：http://nik.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://dey.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fvg.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://qtt.cdnleiting.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pxl.zhixingplan.top

[U04] Py：变量调试打印
来源：http://mjt.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ypz.hcnkem.com

[U05] Py：列表去重且保序
来源：http://nzc.zhoulong.xyz

list(dict.fromkeys(arr))
来源：http://lle.epnwcf.com

[U06] Py：合并两个字典
来源：http://cef.yuxming.cn

{**a, **b}
来源：http://usu.fengsongda.top

[U07] Py：反转字典键值
来源：http://mia.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://qek.zhijiandao.cn

[U08] Py：展平二维列表
来源：http://lko.bbcook.cn

[y for x in nested for y in x]
来源：http://agv.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://bcl.pycfn.com

max(d, key=d.get)
来源：http://gjw.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://gtz.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ulv.yuanzhike.top

[U11] Py：生成器表达式
来源：http://ubs.fengsongda.top

(x * 2 for x in arr)
来源：http://wyl.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://nkf.fktsv.cn

Counter(arr).most_common(3)
来源：http://qvj.tianlin.xyz

[U13] Py：固定长度队列
来源：http://inl.0kj1m.cn

deque(maxlen=10)
来源：http://jzu.cheryme.top

[U14] Py：分组收集到列表
来源：http://jrx.chenjidiqi.icu

defaultdict(list)
来源：http://fxx.zhixingplan.top

[U15] Py：高精度计时
来源：http://mgq.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://otc.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://mpr.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lko.jqgfzy.top

[U17] Py：初始化日志
来源：http://qqh.fehbvm.com

logging.basicConfig(level=logging.INFO)
来源：http://phv.yfazqb.com

[U18] Py：预编译正则
来源：http://nfe.tian-w.cn

pat = re.compile(r"\d+")
来源：http://ove.sxryk.cn

[U19] Py：正则替换带回调
来源：http://diy.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sgl.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://vhn.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://bez.dianchejie.cn

[U21] Py：自定义上下文管理器
来源：http://keo.daxiang520.top

@contextlib.contextmanager
来源：http://gmh.cucudq.cn

[U22] Py：矩阵转置
来源：http://kme.dianchejie.cn

list(zip(*m))
来源：http://qdj.shzxlz.cn

[U23] Py：分块读取大文件
来源：http://eyv.guannengcc.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://syr.hcnkem.com

[U24] Py：路径操作
来源：http://bsk.tanke756.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nhg.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://rvx.snrcjt.cn

csv.DictReader(f)
来源：http://apw.ydzc1.top

[U26] Py：并发下载
来源：http://wbh.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://irr.cucudq.cn

[U27] Py：异步 HTTP
来源：http://bqj.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://nlb.iojbl.cn

[U28] Py：类型别名
来源：http://ehp.chenjidiqi.icu

UserId = int
来源：http://nxl.tanke756.top

[U29] Py：属性校验
来源：http://ayz.cheryme.top

@property 与 @x.setter 配合
来源：http://uck.gzhubu.top

[U30] Py：数据类
来源：http://tqm.jiagoushi.top

@dataclass(slots=True)
来源：http://kvn.hysaishi.cn

[U31] Py：单测
来源：http://pah.cheryme.top

python -m pytest -q
来源：http://jty.tian-w.cn

[U32] Py：代码格式化
来源：http://ipg.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://dpn.jinqigfzy.top

[U33] Py：打包发布
来源：http://gdb.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://roc.xuanzx.com

[U34] Py：判断编码
来源：http://hrb.havefunace.top

chardet.detect(raw)
来源：http://rcm.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://srb.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gmi.mhx1999.top

[U36] Py：定时任务
来源：http://kum.quarkkingdee.top

schedule.every(10).minutes.do(job)
来源：http://twm.jiagoushi.top

[U37] Py：读写 Excel
来源：http://gug.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://ucw.kuanghao11.cn

[U38] Py：获取脚本所在目录
来源：http://nhg.gzhubu.top

Path(__file__).resolve().parent
来源：http://qov.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://twc.bjfxy.top

sys.stdout.isatty()
来源：http://fpi.jqgfzy.top

[U40] Py：打印到标准错误
来源：http://byf.shuidangran.top

print("err", file=sys.stderr)
来源：http://tfo.jqgfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://goe.0kj1m.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vgx.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://cej.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jep.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://orn.vqdsnc.cn

namespace App\Http;
来源：http://ljj.andypj.xyz

[U44] PHP：开启严格类型
来源：http://byv.iojbl.cn

declare(strict_types=1);
来源：http://dcd.hongshengwenyu.top

[U45] PHP：类型声明与返回类型
来源：http://mup.chenlongwang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://iaa.daxiang520.top

[U46] PHP：可空类型
来源：http://nid.shanyushiyangkeji.top

?string $name = null
来源：http://igx.ehwqpu.com

[U47] PHP：联合类型
来源：http://sod.tanke756.top

int|string $id
来源：http://ejn.cheryme.top

[U48] PHP：纯枚举
来源：http://drz.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ibl.pycfn.com

[U49] PHP：只读属性
来源：http://jmp.andypj.xyz

public readonly string $name
来源：http://qmt.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://yph.cqqwz.cn

public function __construct(private int $id) {}
来源：http://kul.yj20258888.top

[U51] PHP：数组解构
来源：http://xre.quarkkingdee.top

[$a, $b] = $arr;
来源：http://vde.52xcode.cn

[U52] PHP：箭头函数
来源：http://uqx.hammf.cn

$double = fn($x) => $x * 2;
来源：http://ghy.ydzc1.top

[U53] PHP：空合并运算符
来源：http://fhu.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://swp.yj20258888.top

[U54] PHP：空安全调用
来源：http://dal.hnxiangtu.top

$obj?->method()
来源：http://jum.jinghuilouyu.cn

[U55] PHP：match 表达式
来源：http://qap.fanxiaobao.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ast.bjfxy.top

[U56] PHP：命名参数
来源：http://sbi.zdqjudy.top

f(a: 1, b: 2)
来源：http://kgn.zhengqikj.top

[U57] PHP：字符串插值
来源：http://wws.shangyingyoupin.top

"值: {$a}"
来源：http://nlu.yueranfly.top

[U58] PHP：数组三件套
来源：http://lbk.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dtu.yueranfly.top

[U59] PHP：自定义排序
来源：http://wiu.gzhubu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://waw.aibaodan.cn

[U60] PHP：JSON 编解码
来源：http://uky.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fri.svipenyu.cn

[U61] PHP：正则
来源：http://uhg.tian-w.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nkm.snrcjt.cn

[U62] PHP：日期对象
来源：http://tbm.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hll.xinyue.icu

[U63] PHP：文件读写
来源：http://nhm.zhixingplan.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jvx.cucudq.cn

[U64] PHP：目录遍历
来源：http://xgn.jyoumei.cn

glob("dir/*.php");  scandir("dir");
来源：http://oqw.jinqigfzy.top

[U65] PHP：会话
来源：http://rpn.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mtm.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://ate.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://swi.ivvv.top

[U67] PHP：处理文件上传
来源：http://pfj.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ojd.epnwcf.com

[U68] PHP：PDO 连接
来源：http://ahf.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jfg.guannengcc.top

[U69] PHP：PDO 预处理
来源：http://xyl.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hbr.fanxiaobao.xyz

[U70] PHP：PDO 事务
来源：http://day.yanxiufei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ifi.yj202588.top

[U71] PHP：抛出异常
来源：http://con.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://huz.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://akm.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://iet.nwbrower.top


<!-- 参考信息 -->