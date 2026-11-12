代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://lee.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jhk.ehwqpu.com

[S48] C++：逐行读文件
来源：http://qgo.ctjpmb.com

std::ifstream in("a.txt");  std::string line;
来源：http://wku.iojbl.cn

while (std::getline(in, line)) { }
来源：http://mik.kuanghao11.cn

[S49] C++：写文件
来源：http://cok.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dwo.ybcxt.top

[S50] C++：格式化数字
来源：http://dlw.yfazqb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pxw.haohaochexian.top

[S51] C++：显式类型转换
来源：http://ivg.jinqigfzy.top

static_cast<double>(a) / b
来源：http://qdc.tanke756.top

[S52] C++：const 与 noexcept
来源：http://qjc.epnwcf.com

int size() const noexcept { return n_; }
来源：http://tnq.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://ysh.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://fzp.ctjpmb.com

[S54] C++：异常处理
来源：http://jdn.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fkp.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://hwb.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lsd.gotoacloud.top

[S56] C++：optional
来源：http://kio.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tcp.52xcode.cn

[S57] C++：编译期常量
来源：http://fob.jyoumei.cn

constexpr int N = 10;
来源：http://aij.ydzc1.top

[S58] C++：命名空间
来源：http://flm.gzhubu.top

namespace ns { int f() { return 1; } }
来源：http://qfn.zhiwuduotai.top

[S59] C++：静态断言
来源：http://cbu.meibo888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iwk.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://cmk.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ygt.zhengqikj.top

================================================================================
来源：http://pcy.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sue.quarkkingdee.top

================================================================================
来源：http://amh.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://upa.yueranfly.top

println("Hello")
来源：http://wud.yuanzhike.top

[T02] Kotlin：变量
来源：http://zpt.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gys.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://lmy.chenjidiqi.icu

"值: $b"
来源：http://adz.jqgfzy.top

[T04] Kotlin：空安全
来源：http://oqp.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://fgp.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://exv.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vcd.yonumen.top

[T06] Kotlin：集合映射
来源：http://rmw.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rvk.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://xig.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tdt.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://emw.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://mne.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://lom.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://kac.xuanzx.com

[T10] Kotlin：默认参数
来源：http://zoc.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wvm.ppjwa.cn

[T11] Kotlin：协程
来源：http://vdw.mhx1999.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vsw.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://gzz.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://jnv.gotoacloud.top

[T13] Kotlin：只读 Map
来源：http://ikv.vqdsnc.cn

val m = mapOf("a" to 1)
来源：http://gpf.aibaodan.cn

[T14] Kotlin：循环
来源：http://ajx.yonumen.top

for (i in 1..10) println(i)
来源：http://bbg.tarul.cn

[T15] Kotlin：接口
来源：http://ojg.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://zap.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://zwo.jlsjyb.cn

print("Hello")
来源：http://biy.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://wna.tianlin.xyz

var a = 1;  let b = 2
来源：http://juo.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://tcz.iojbl.cn

"值: \(b)"
来源：http://oiw.xuanzx.com

[T19] Swift：可选绑定
来源：http://unp.yvedp.cn

if let n = opt { print(n) }
来源：http://cyj.epnwcf.com

[T20] Swift：数组操作
来源：http://rwh.ybcxt.top

var a = [1, 2, 3];  a.append(4)
来源：http://ili.nwbrower.top

[T21] Swift：遍历
来源：http://wwy.52xcode.cn

for x in a { print(x) }
来源：http://mso.gzhubu.top

[T22] Swift：字典
来源：http://alb.vehdjk.com

var d = ["a": 1];  d["b"] = 2
来源：http://qbn.chenzaomai.com

[T23] Swift：函数
来源：http://dxk.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wpr.tanke756.top

[T24] Swift：闭包
来源：http://awg.shanyushiyangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ltm.yvedp.cn

[T25] Swift：结构体
来源：http://tcd.svipenyu.cn

struct P { var x: Int }
来源：http://lly.tianlin.xyz

[T26] Swift：类与重写
来源：http://ebs.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://fob.haohaochexian.top

[T27] Swift：错误处理
来源：http://bxl.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://eyv.ehwqpu.com

[T28] Swift：枚举
来源：http://jqk.ehwqpu.com

enum Color { case red, green }
来源：http://sna.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://siw.316326.xyz

guard let x = opt else { return }
来源：http://lcu.sjlbkw.cn

[T30] Swift：协议
来源：http://snn.havefunace.top

protocol Shape { func area() -> Double }
来源：http://tts.zhaomingkeji.xyz

[T31] Lua：Hello World
来源：http://bxl.ydjk.org.cn

print("Hello")
来源：http://had.jinqigufen.top

[T32] Lua：局部变量
来源：http://ofg.jinqigufen.top

local a = 1
来源：http://ytt.zycfv.cn

[T33] Lua：表（数组）
来源：http://xjk.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sbd.fengsongda.top

[T34] Lua：遍历表
来源：http://zkm.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ekv.0kj1m.cn

[T35] Lua：字典表
来源：http://nyl.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://tnw.52xcode.cn

[T36] Lua：函数
来源：http://rgp.hesvh.cn

function add(a, b) return a + b end
来源：http://hpf.fzhhl.top

[T37] Lua：字符串拼接
来源：http://bnb.jinqigufen.top

"a" .. "b"
来源：http://zfx.jlsjyb.cn

[T38] Lua：条件
来源：http://ptc.316326.xyz

if x > 0 then print("正") end
来源：http://pse.fanxiaobao.xyz

[T39] Lua：模式匹配
来源：http://biq.pengpengdd.cyou

string.find(s, "%d+")
来源：http://wtp.ppjwa.cn

[T40] Lua：元表
来源：http://zvu.gaohongyu789.top

setmetatable({}, { __index = base })
来源：http://hqc.haohaochexian.top

[T41] Perl：Hello World
来源：http://eah.9152youxi.cn

print "Hello\n";
来源：http://ulc.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://eae.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aho.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://wop.yonumen.top

"值: $a"
来源：http://fyk.zdqjudy.top

[T44] Perl：条件
来源：http://qga.yonumen.top

if ($a > 0) { print "正"; }
来源：http://vcj.haohaochexian.top

[T45] Perl：数组遍历
来源：http://ghh.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://tye.ivvv.top

[T46] Perl：哈希操作
来源：http://cbc.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dri.nwbrower.top

[T47] Perl：正则捕获
来源：http://qwu.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://plu.yj202588.top

[T48] Perl：正则替换
来源：http://tfi.yueranfly.top

$s =~ s/old/new/g;
来源：http://mgc.vehdjk.com

[T49] Perl：函数
来源：http://unv.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nit.yvedp.cn

[T50] Perl：逐行读文件
来源：http://fpr.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://ish.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://yng.yonumen.top

[T51] Scala：Hello World
来源：http://lbf.xuanzx.com

println("Hello")
来源：http://ejs.tanke756.top

[T52] Scala：变量
来源：http://fzf.cheryme.top

val a = 1;  var b = 2
来源：http://bnw.jqgfzy.top

[T53] Scala：字符串插值
来源：http://asn.c1oappe.top

s"值: $b"
来源：http://mdk.xylfe.cn

[T54] Scala：集合映射
来源：http://azz.yongpay.top

List(1, 2, 3).map(_ * 2)
来源：http://qaf.fzhhl.top

[T55] Scala：集合过滤
来源：http://fut.nwbrower.top

List(1, 2, 3).filter(_ > 1)
来源：http://gnn.smart0.xyz

[T56] Scala：样例类
来源：http://amh.hywenlv.cn

case class User(name: String, age: Int)
来源：http://tbr.yuxming.cn

[T57] Scala：模式匹配
来源：http://fpw.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://brv.0kj1m.cn

[T58] Scala：函数定义
来源：http://yif.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://tej.0kj1m.cn

[T59] Scala：循环
来源：http://sew.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://rcs.shanyushiyangkeji.top

[T60] Scala：折叠
来源：http://kiv.jinqigfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xem.redwolf501.top

================================================================================
来源：http://rsj.wangshuangyany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mnn.sweek.top

================================================================================
来源：http://zog.jinqigfzy.top

[U01] Py：创建虚拟环境
来源：http://trz.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://eic.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://vfw.yueranfly.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fpq.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://kom.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://jcu.yongpay.top

[U04] Py：变量调试打印
来源：http://okx.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pzo.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://rmv.cheryme.top

list(dict.fromkeys(arr))
来源：http://oyk.cucudq.cn

[U06] Py：合并两个字典
来源：http://ytp.xingfuxueyuan.xyz

{**a, **b}
来源：http://vvi.tianlin.xyz

[U07] Py：反转字典键值
来源：http://dne.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://uar.wangdashe.top

[U08] Py：展平二维列表
来源：http://run.zhixingplan.top

[y for x in nested for y in x]
来源：http://kmy.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://xdu.dianchejie.cn

max(d, key=d.get)
来源：http://vuf.cashguo.top

[U10] Py：按值排序字典
来源：http://msb.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://luc.ybcxt.top

[U11] Py：生成器表达式
来源：http://dzp.snrcjt.cn

(x * 2 for x in arr)
来源：http://fge.aibaodan.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lxz.xylfe.cn

Counter(arr).most_common(3)
来源：http://rtb.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://ybq.xuanzx.com

deque(maxlen=10)
来源：http://wvd.yvedp.cn

[U14] Py：分组收集到列表
来源：http://lij.yj20258.top

defaultdict(list)
来源：http://okw.guowangkeji.top

[U15] Py：高精度计时
来源：http://msy.sxryk.cn

t = time.perf_counter()
来源：http://gip.tanke756.top

[U16] Py：命令行参数解析
来源：http://xpr.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vuu.birdmap.top

[U17] Py：初始化日志
来源：http://pkl.jinqigfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://jyj.jiagoushi.top

[U18] Py：预编译正则
来源：http://pdp.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://npz.yongpay.top

[U19] Py：正则替换带回调
来源：http://klc.nanxuanxn.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://voo.sufxvd.cn

[U20] Py：缓存函数结果
来源：http://rpx.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://vry.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://tcd.epnwcf.com

@contextlib.contextmanager
来源：http://equ.wangdashe.top

[U22] Py：矩阵转置
来源：http://fdj.redwolf501.top

list(zip(*m))
来源：http://cjc.bbcook.cn

[U23] Py：分块读取大文件
来源：http://owd.fzhhl.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://txy.tian-w.cn

[U24] Py：路径操作
来源：http://mqk.jinyuanbaomall.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lrz.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://heu.tarul.cn

csv.DictReader(f)
来源：http://avd.sweek.top

[U26] Py：并发下载
来源：http://det.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nxb.hcnkem.com

[U27] Py：异步 HTTP
来源：http://sks.bjfxy.top

aiohttp.ClientSession() 配合 async with
来源：http://tlj.9152youxi.cn

[U28] Py：类型别名
来源：http://gye.ivvv.top

UserId = int
来源：http://tpf.bbcook.cn

[U29] Py：属性校验
来源：http://jyk.gzhubu.top

@property 与 @x.setter 配合
来源：http://pkl.xinyue.icu

[U30] Py：数据类
来源：http://wvd.gzhubu.top

@dataclass(slots=True)
来源：http://dfx.yuxming.cn

[U31] Py：单测
来源：http://elq.zhongyouzk.top

python -m pytest -q
来源：http://fzb.meibo888.top

[U32] Py：代码格式化
来源：http://pjd.xinyue.icu

ruff format . && ruff check --fix .
来源：http://uky.yvedp.cn

[U33] Py：打包发布
来源：http://uys.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://ind.dashuyun.cn

[U34] Py：判断编码
来源：http://zwx.gotoacloud.top

chardet.detect(raw)
来源：http://xum.shanyushiyangtech.top

[U35] Py：发送邮件
来源：http://nzh.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wab.zhixingplan.top

[U36] Py：定时任务
来源：http://jlg.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://pfh.yongpay.top

[U37] Py：读写 Excel
来源：http://dvg.bbcook.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wgk.zhoulong.xyz

[U38] Py：获取脚本所在目录
来源：http://cke.jyoumei.cn

Path(__file__).resolve().parent
来源：http://ujc.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://pcm.yuxming.cn

sys.stdout.isatty()
来源：http://fju.iojbl.cn

[U40] Py：打印到标准错误
来源：http://wvw.cucudq.cn

print("err", file=sys.stderr)
来源：http://qwk.hysaishi.cn

[U41] PHP：初始化 Composer 项目
来源：http://pvp.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://nkv.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://pqp.havefunace.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://teg.ehwqpu.com

[U43] PHP：声明命名空间
来源：http://gfr.hysaishi.cn

namespace App\Http;
来源：http://znk.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://uqa.hfpthk.cn

declare(strict_types=1);
来源：http://iun.ivvv.top

[U45] PHP：类型声明与返回类型
来源：http://ddj.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qzj.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://egh.xuetiantiany.cn

?string $name = null
来源：http://fdl.zdbjq.cn

[U47] PHP：联合类型
来源：http://fya.daxiang520.top

int|string $id
来源：http://xna.c1oappe.top

[U48] PHP：纯枚举
来源：http://yas.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hnc.hcnkem.com

[U49] PHP：只读属性
来源：http://roy.ydjk.org.cn

public readonly string $name
来源：http://zgp.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://ltz.zdqjudy.top

public function __construct(private int $id) {}
来源：http://dta.guowangkeji.top

[U51] PHP：数组解构
来源：http://efh.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://tze.svipenyu.cn

[U52] PHP：箭头函数
来源：http://sko.ehwqpu.com

$double = fn($x) => $x * 2;
来源：http://ldw.jyoumei.cn

[U53] PHP：空合并运算符
来源：http://dtb.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://dkr.zhengqikj.top

[U54] PHP：空安全调用
来源：http://fkc.zhaomingkeji.xyz

$obj?->method()
来源：http://tab.ppjwa.cn

[U55] PHP：match 表达式
来源：http://yhn.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ncu.tian-w.cn

[U56] PHP：命名参数
来源：http://jpw.zhoulong.xyz

f(a: 1, b: 2)
来源：http://rtt.chenzaomai.com

[U57] PHP：字符串插值
来源：http://bkn.tian-w.cn

"值: {$a}"
来源：http://shp.0kj1m.cn

[U58] PHP：数组三件套
来源：http://wva.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zbe.zdbjq.cn

[U59] PHP：自定义排序
来源：http://zbk.vehdjk.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ngd.nanxuanxn.top

[U60] PHP：JSON 编解码
来源：http://xqa.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://udf.zdbjq.cn

[U61] PHP：正则
来源：http://wdz.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://coj.fehbvm.com

[U62] PHP：日期对象
来源：http://btq.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jxc.bjfxy.top

[U63] PHP：文件读写
来源：http://hdy.daxiang520.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mee.gzhubu.top

[U64] PHP：目录遍历
来源：http://fwm.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://tkf.sxryk.cn

[U65] PHP：会话
来源：http://kun.hcnkem.com

session_start();  $_SESSION["uid"] = 1;
来源：http://wep.guowangkeji.top

[U66] PHP：设置 Cookie
来源：http://wmh.ehwqpu.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wmw.sysykeji.top

[U67] PHP：处理文件上传
来源：http://yjz.aizwys.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bxx.ywan-chungtsiang.top

[U68] PHP：PDO 连接
来源：http://rru.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hgg.zhengqikj.top

[U69] PHP：PDO 预处理
来源：http://hkq.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cta.iojbl.cn

[U70] PHP：PDO 事务
来源：http://djl.shanyushiyangtech.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rul.quarkkingdee.top

[U71] PHP：抛出异常
来源：http://ieb.cashguo.top

throw new RuntimeException("失败", 500);
来源：http://eie.hysaishi.cn

[U72] PHP：写错误日志
来源：http://yly.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://jwo.svipenyu.cn


<!-- 参考信息 -->