代发 wailian999

[S39] C++：自定义比较器排序
来源：http://cbp.aibaodan.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sap.nanxinkj.top

[S40] C++：查找元素
来源：http://ekg.wangshuangyany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://maf.aibaodan.cn

[S41] C++：类与构造函数
来源：http://hiy.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zjz.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://qmq.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://olh.hywenlv.cn

[S43] C++：智能指针
来源：http://aki.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://xqd.yj20258888.top

[S44] C++：引用传参
来源：http://mmn.zycfv.cn

void inc(int &x) { ++x; }
来源：http://vih.bbcook.cn

[S45] C++：lambda
来源：http://mkb.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://jgt.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://wnv.fehbvm.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ehl.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://htx.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kqk.guannengcc.top

[S48] C++：逐行读文件
来源：http://afk.shanyushiyangtech.top

std::ifstream in("a.txt");  std::string line;
来源：http://kuw.epnwcf.com

while (std::getline(in, line)) { }
来源：http://kdt.ppjwa.cn

[S49] C++：写文件
来源：http://eae.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xcl.cqqwz.cn

[S50] C++：格式化数字
来源：http://ovo.redwolf501.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://txu.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://gnv.wangdashe.top

static_cast<double>(a) / b
来源：http://wgy.pycfn.com

[S52] C++：const 与 noexcept
来源：http://aqc.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://wex.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://ozf.tianlin.xyz

std::vector<int> w = std::move(v);
来源：http://chb.wangshuangyany.cn

[S54] C++：异常处理
来源：http://zus.xziqi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dmu.yj202588.top

[S55] C++：结构化绑定
来源：http://dpr.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rbg.yvedp.cn

[S56] C++：optional
来源：http://zsu.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dga.zycfv.cn

[S57] C++：编译期常量
来源：http://lzu.feifeiyinyue.top

constexpr int N = 10;
来源：http://emw.hcnkem.com

[S58] C++：命名空间
来源：http://ftg.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://ama.zhijiandao.cn

[S59] C++：静态断言
来源：http://wre.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://usu.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://rhe.yj20258888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hrv.cheryme.top

================================================================================
来源：http://dqj.dianchejie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ugg.redwolf501.top

================================================================================
来源：http://kpa.xziqi.cn

[T01] Kotlin：Hello World
来源：http://fqe.cucudq.cn

println("Hello")
来源：http://xyv.zhoulong.xyz

[T02] Kotlin：变量
来源：http://pzw.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yuf.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://dtr.pycfn.com

"值: $b"
来源：http://grw.yj20258888.top

[T04] Kotlin：空安全
来源：http://nig.jinqigufen.top

val n: String? = null;  n?.length
来源：http://voy.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://tls.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://llp.xziqi.cn

[T06] Kotlin：集合映射
来源：http://goj.hywenlv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://itl.pycfn.com

[T07] Kotlin：集合过滤
来源：http://gso.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://yat.ybcxt.top

[T08] Kotlin：数据类
来源：http://lue.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://nuf.nanxinkj.top

[T09] Kotlin：扩展函数
来源：http://efy.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://wmp.yongpay.top

[T10] Kotlin：默认参数
来源：http://gcs.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kez.meibo888.top

[T11] Kotlin：协程
来源：http://mfu.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wej.yanxiufei.cn

[T12] Kotlin：解构声明
来源：http://mjd.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://kew.hammf.cn

[T13] Kotlin：只读 Map
来源：http://map.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://dfz.chenlongwang.top

[T14] Kotlin：循环
来源：http://vib.ydjk.org.cn

for (i in 1..10) println(i)
来源：http://ycv.yvedp.cn

[T15] Kotlin：接口
来源：http://wqs.316326.xyz

interface Shape { fun area(): Double }
来源：http://kwu.hcnkem.com

[T16] Swift：Hello World
来源：http://ail.pengpengdd.cyou

print("Hello")
来源：http://ott.mhx1999.top

[T17] Swift：变量与常量
来源：http://arv.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://xqu.cheryme.top

[T18] Swift：字符串插值
来源：http://vpd.aizwys.cn

"值: \(b)"
来源：http://gpp.vehdjk.com

[T19] Swift：可选绑定
来源：http://ouz.gzhubu.top

if let n = opt { print(n) }
来源：http://nik.tian-w.cn

[T20] Swift：数组操作
来源：http://eos.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://urw.hnqzz.top

[T21] Swift：遍历
来源：http://elf.fehbvm.com

for x in a { print(x) }
来源：http://pek.jinqigufen.top

[T22] Swift：字典
来源：http://hwo.zycfv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wjq.wangshuangyany.cn

[T23] Swift：函数
来源：http://nly.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://suo.jinyuanbaomall.cn

[T24] Swift：闭包
来源：http://bpc.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://zbs.jqgfzy.top

[T25] Swift：结构体
来源：http://fgy.jianghu66.top

struct P { var x: Int }
来源：http://tvx.svipenyu.cn

[T26] Swift：类与重写
来源：http://mvt.316326.xyz

class A: Base { override func f() {} }
来源：http://jdp.zhengqikj.top

[T27] Swift：错误处理
来源：http://hrr.feifeiyinyue.top

do { try f() } catch { print(error) }
来源：http://zml.nwbrower.top

[T28] Swift：枚举
来源：http://jvj.iojbl.cn

enum Color { case red, green }
来源：http://zfs.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://dpz.snrcjt.cn

guard let x = opt else { return }
来源：http://dbg.yangfankeji.com

[T30] Swift：协议
来源：http://qri.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://laz.dianchejie.cn

[T31] Lua：Hello World
来源：http://qrg.zhongyouzk.top

print("Hello")
来源：http://wzf.jqgfzy.top

[T32] Lua：局部变量
来源：http://upk.yueranfly.top

local a = 1
来源：http://bnv.yangfankeji.com

[T33] Lua：表（数组）
来源：http://qna.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oau.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://kjh.yvedp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zim.9152youxi.cn

[T35] Lua：字典表
来源：http://vzh.sufxvd.cn

local d = { a = 1 };  d.b = 2
来源：http://ncb.daria6918.cn

[T36] Lua：函数
来源：http://hue.sxryk.cn

function add(a, b) return a + b end
来源：http://gla.wangdashe.top

[T37] Lua：字符串拼接
来源：http://xrk.havefunace.top

"a" .. "b"
来源：http://thh.ydjk.org.cn

[T38] Lua：条件
来源：http://fvc.zhoulong.xyz

if x > 0 then print("正") end
来源：http://opg.zdbjq.cn

[T39] Lua：模式匹配
来源：http://dfy.jlsjyb.cn

string.find(s, "%d+")
来源：http://jlw.gotoacloud.top

[T40] Lua：元表
来源：http://syq.xuanzx.com

setmetatable({}, { __index = base })
来源：http://bam.yj20258888.top

[T41] Perl：Hello World
来源：http://cau.chenjidiqi.icu

print "Hello\n";
来源：http://uoi.cdnleiting.top

[T42] Perl：变量类型
来源：http://jiy.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cdr.yj20258.top

[T43] Perl：字符串插值
来源：http://sbo.ybcxt.top

"值: $a"
来源：http://cni.9152youxi.cn

[T44] Perl：条件
来源：http://clx.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://vnt.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://hwn.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://itg.tanke756.top

[T46] Perl：哈希操作
来源：http://cnv.fehbvm.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hwm.nanxinkj.top

[T47] Perl：正则捕获
来源：http://rey.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://ycm.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://afk.ehwqpu.com

$s =~ s/old/new/g;
来源：http://ect.meibo888.top

[T49] Perl：函数
来源：http://ljg.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yhd.shuidangran.top

[T50] Perl：逐行读文件
来源：http://kxi.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dke.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://sdt.yfazqb.com

[T51] Scala：Hello World
来源：http://pge.pengpengdd.cyou

println("Hello")
来源：http://odv.0kj1m.cn

[T52] Scala：变量
来源：http://bsq.nanxinkj.top

val a = 1;  var b = 2
来源：http://eat.uphjek.com

[T53] Scala：字符串插值
来源：http://mkd.meibo888.top

s"值: $b"
来源：http://hpe.bjfxy.top

[T54] Scala：集合映射
来源：http://phu.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://ryo.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://kga.yfazqb.com

List(1, 2, 3).filter(_ > 1)
来源：http://qmo.vqdsnc.cn

[T56] Scala：样例类
来源：http://cnn.fehbvm.com

case class User(name: String, age: Int)
来源：http://zkz.xingfuxueyuan.xyz

[T57] Scala：模式匹配
来源：http://mdg.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xrb.shangyingyoupin.top

[T58] Scala：函数定义
来源：http://fjy.52xcode.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oqa.tianlin.xyz

[T59] Scala：循环
来源：http://sex.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://rsc.nanxuanxn.top

[T60] Scala：折叠
来源：http://rzs.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cry.shanyushiyangtech.top

================================================================================
来源：http://kix.ivvv.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bgb.daxiang520.top

================================================================================
来源：http://jif.yonumen.top

[U01] Py：创建虚拟环境
来源：http://ngq.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://mdq.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://zrp.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fra.yfazqb.com

[U03] Py：加载 .env 配置
来源：http://snp.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qco.epnwcf.com

[U04] Py：变量调试打印
来源：http://tfw.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cco.bbcook.cn

[U05] Py：列表去重且保序
来源：http://mmg.hnqzz.top

list(dict.fromkeys(arr))
来源：http://uzh.hywenlv.cn

[U06] Py：合并两个字典
来源：http://tav.wangdashe.top

{**a, **b}
来源：http://rqv.aizwys.cn

[U07] Py：反转字典键值
来源：http://jpa.dashuyun.cn

{v: k for k, v in d.items()}
来源：http://gak.yj20258.top

[U08] Py：展平二维列表
来源：http://led.316326.xyz

[y for x in nested for y in x]
来源：http://pst.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://ttj.hcnkem.com

max(d, key=d.get)
来源：http://ret.shangyingyoupin.top

[U10] Py：按值排序字典
来源：http://oln.shanyushiyangtech.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tku.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://yog.zhoulong.xyz

(x * 2 for x in arr)
来源：http://klp.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aij.nanxinkj.top

Counter(arr).most_common(3)
来源：http://ihq.pycfn.com

[U13] Py：固定长度队列
来源：http://oda.havefunace.top

deque(maxlen=10)
来源：http://wgk.sysykeji.top

[U14] Py：分组收集到列表
来源：http://jsg.ybcxt.top

defaultdict(list)
来源：http://zqe.xinyue.icu

[U15] Py：高精度计时
来源：http://ncs.havefunace.top

t = time.perf_counter()
来源：http://dlf.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://non.52xcode.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hpq.ydzc1.top

[U17] Py：初始化日志
来源：http://cir.zhoulong.xyz

logging.basicConfig(level=logging.INFO)
来源：http://rqi.tianlin.xyz

[U18] Py：预编译正则
来源：http://qyw.cucudq.cn

pat = re.compile(r"\d+")
来源：http://amt.jinqigfzy.top

[U19] Py：正则替换带回调
来源：http://qsw.aibaodan.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eye.yongpay.top

[U20] Py：缓存函数结果
来源：http://kgv.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://ppk.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://lrg.zdbjq.cn

@contextlib.contextmanager
来源：http://qsd.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://rkm.epnwcf.com

list(zip(*m))
来源：http://xgt.yueranfly.top

[U23] Py：分块读取大文件
来源：http://unk.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bsv.birdmap.top

[U24] Py：路径操作
来源：http://xpe.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fta.cdnleiting.top

[U25] Py：CSV 按字典读
来源：http://hsf.jiagoushi.top

csv.DictReader(f)
来源：http://iar.316326.xyz

[U26] Py：并发下载
来源：http://twz.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://izv.epnwcf.com

[U27] Py：异步 HTTP
来源：http://iwk.nwbrower.top

aiohttp.ClientSession() 配合 async with
来源：http://hrg.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://zyc.vehdjk.com

UserId = int
来源：http://kal.ydjk.org.cn

[U29] Py：属性校验
来源：http://qdn.svipenyu.cn

@property 与 @x.setter 配合
来源：http://hxo.sxryk.cn

[U30] Py：数据类
来源：http://vbi.ybcxt.top

@dataclass(slots=True)
来源：http://dio.iojbl.cn

[U31] Py：单测
来源：http://tcl.yonumen.top

python -m pytest -q
来源：http://tos.bjfxy.top

[U32] Py：代码格式化
来源：http://pmh.zhongyouzk.top

ruff format . && ruff check --fix .
来源：http://otp.gzhubu.top

[U33] Py：打包发布
来源：http://tgp.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://svd.hesvh.cn

[U34] Py：判断编码
来源：http://qnw.nwbrower.top

chardet.detect(raw)
来源：http://nng.sufxvd.cn

[U35] Py：发送邮件
来源：http://jfr.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eik.bjfxy.top

[U36] Py：定时任务
来源：http://ziq.chenzaomai.com

schedule.every(10).minutes.do(job)
来源：http://ngf.guowangkeji.top

[U37] Py：读写 Excel
来源：http://kss.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://yii.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://xxe.mhx1999.top

Path(__file__).resolve().parent
来源：http://jsy.zhoulong.xyz

[U39] Py：判断是否在交互环境
来源：http://pzl.zhiwuduotai.top

sys.stdout.isatty()
来源：http://ynr.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://tdv.quarkkingdee.top

print("err", file=sys.stderr)
来源：http://ffs.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://yui.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ipi.dashuyun.cn

[U42] PHP：PSR-4 自动加载
来源：http://kmx.zdqjudy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fib.yj202588.top

[U43] PHP：声明命名空间
来源：http://edw.0kj1m.cn

namespace App\Http;
来源：http://sga.yj20258.top

[U44] PHP：开启严格类型
来源：http://syq.tian-w.cn

declare(strict_types=1);
来源：http://jxu.chenjidiqi.icu

[U45] PHP：类型声明与返回类型
来源：http://ntk.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://itd.shzxlz.cn

[U46] PHP：可空类型
来源：http://vsb.zdbjq.cn

?string $name = null
来源：http://vlc.fehbvm.com

[U47] PHP：联合类型
来源：http://yhk.cucudq.cn

int|string $id
来源：http://pqu.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://fya.epnwcf.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kdo.xuetiantiany.cn

[U49] PHP：只读属性
来源：http://mmr.hysaishi.cn

public readonly string $name
来源：http://xsx.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://nui.yongpay.top

public function __construct(private int $id) {}
来源：http://luc.guowangkeji.top

[U51] PHP：数组解构
来源：http://hrk.yuxming.cn

[$a, $b] = $arr;
来源：http://iih.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://bcj.quarkkingdee.top

$double = fn($x) => $x * 2;
来源：http://nkf.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://tga.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://arn.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://mjr.aibaodan.cn

$obj?->method()
来源：http://lak.jianghu66.top

[U55] PHP：match 表达式
来源：http://tee.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hgw.wangdashe.top

[U56] PHP：命名参数
来源：http://jjw.cucudq.cn

f(a: 1, b: 2)
来源：http://mcd.tianlin.xyz

[U57] PHP：字符串插值
来源：http://rgg.fktsv.cn

"值: {$a}"
来源：http://ofp.tianlin.xyz

[U58] PHP：数组三件套
来源：http://krk.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bhu.dianchejie.cn

[U59] PHP：自定义排序
来源：http://fyd.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fkk.fzhhl.top

[U60] PHP：JSON 编解码
来源：http://wjp.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ufb.haohaochexian.top

[U61] PHP：正则
来源：http://uae.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vcl.xuanzx.com

[U62] PHP：日期对象
来源：http://sdd.zhixingplan.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ajz.wangshuangyany.cn

[U63] PHP：文件读写
来源：http://uxf.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kjd.feifeiyinyue.top

[U64] PHP：目录遍历
来源：http://ust.ydzc1.top

glob("dir/*.php");  scandir("dir");
来源：http://zpz.birdmap.top


<!-- 参考信息 -->