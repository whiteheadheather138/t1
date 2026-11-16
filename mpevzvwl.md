代发 wailian999

[S43] C++：智能指针
来源：http://mre.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://tuk.gaohongyu789.top

[S44] C++：引用传参
来源：http://gwz.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://zad.jinghuilouyu.cn

[S45] C++：lambda
来源：http://pnm.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hzp.hongshengwenyu.top

[S46] C++：函数模板
来源：http://vwc.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lps.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://oxd.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xqo.ydzc1.top

[S48] C++：逐行读文件
来源：http://uuu.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uzn.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://gkn.havefunace.top

[S49] C++：写文件
来源：http://dmo.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rln.jinqigfzy.top

[S50] C++：格式化数字
来源：http://hln.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mfu.yuxming.cn

[S51] C++：显式类型转换
来源：http://gkz.yvedp.cn

static_cast<double>(a) / b
来源：http://pjg.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://opu.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://lyo.zhoulong.xyz

[S53] C++：移动语义
来源：http://bes.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://abe.hcnkem.com

[S54] C++：异常处理
来源：http://pyy.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ecp.yj20258888.top

[S55] C++：结构化绑定
来源：http://eau.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uyc.fanxiaobao.xyz

[S56] C++：optional
来源：http://xmp.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ywp.quarkkingdee.top

[S57] C++：编译期常量
来源：http://ggk.ybcxt.top

constexpr int N = 10;
来源：http://snm.hnqzz.top

[S58] C++：命名空间
来源：http://wml.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://tlm.cdnleiting.top

[S59] C++：静态断言
来源：http://gsa.shanyushiyangtech.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pma.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://sai.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://thi.iojbl.cn

================================================================================
来源：http://nuw.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jnu.nwbrower.top

================================================================================
来源：http://czv.bbcook.cn

[T01] Kotlin：Hello World
来源：http://sdg.xylfe.cn

println("Hello")
来源：http://dtb.yueranfly.top

[T02] Kotlin：变量
来源：http://mnl.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qqy.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://fpx.tianlin.xyz

"值: $b"
来源：http://qao.hesvh.cn

[T04] Kotlin：空安全
来源：http://afw.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://ncm.yonumen.top

[T05] Kotlin：when 表达式
来源：http://sgx.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cfy.zhoulong.xyz

[T06] Kotlin：集合映射
来源：http://viy.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nvd.tian-w.cn

[T07] Kotlin：集合过滤
来源：http://mmd.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://qgs.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://vvu.cheryme.top

data class User(val name: String, val age: Int)
来源：http://tcq.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://lvp.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://psh.hnqzz.top

[T10] Kotlin：默认参数
来源：http://zcw.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wkv.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://vow.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dwy.yj20258.top

[T12] Kotlin：解构声明
来源：http://txh.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://sab.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://yfn.yj20258.top

val m = mapOf("a" to 1)
来源：http://dja.xziqi.cn

[T14] Kotlin：循环
来源：http://ewj.redwolf501.top

for (i in 1..10) println(i)
来源：http://esd.gotoacloud.top

[T15] Kotlin：接口
来源：http://ttc.bbcook.cn

interface Shape { fun area(): Double }
来源：http://ldy.tanke756.top

[T16] Swift：Hello World
来源：http://inu.jinyuanbaomall.cn

print("Hello")
来源：http://fnd.meibo888.top

[T17] Swift：变量与常量
来源：http://zfe.jqgufenzy.top

var a = 1;  let b = 2
来源：http://vun.jiagoushi.top

[T18] Swift：字符串插值
来源：http://psv.cheryme.top

"值: \(b)"
来源：http://uvm.chenlongwang.top

[T19] Swift：可选绑定
来源：http://rib.dianchejie.cn

if let n = opt { print(n) }
来源：http://bvv.andypj.xyz

[T20] Swift：数组操作
来源：http://gru.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://udf.316326.xyz

[T21] Swift：遍历
来源：http://cdl.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://cbh.snrcjt.cn

[T22] Swift：字典
来源：http://atz.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://hno.snrcjt.cn

[T23] Swift：函数
来源：http://mcb.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vas.zhijiandao.cn

[T24] Swift：闭包
来源：http://jgv.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://tbk.xinyue.icu

[T25] Swift：结构体
来源：http://emw.yj20258.top

struct P { var x: Int }
来源：http://lfq.ydzc1.top

[T26] Swift：类与重写
来源：http://lqw.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://wtz.hcnkem.com

[T27] Swift：错误处理
来源：http://mrr.fehbvm.com

do { try f() } catch { print(error) }
来源：http://jjx.shanyushiyangtech.top

[T28] Swift：枚举
来源：http://dpj.guannengcc.top

enum Color { case red, green }
来源：http://kwf.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://anf.haohaochexian.top

guard let x = opt else { return }
来源：http://nvi.nanxuanxn.top

[T30] Swift：协议
来源：http://ytf.birdmap.top

protocol Shape { func area() -> Double }
来源：http://woi.cqqwz.cn

[T31] Lua：Hello World
来源：http://jyr.shzxlz.cn

print("Hello")
来源：http://prq.ydzc1.top

[T32] Lua：局部变量
来源：http://ghm.gotoacloud.top

local a = 1
来源：http://wcr.hfpthk.cn

[T33] Lua：表（数组）
来源：http://ydl.hcnkem.com

local t = {1, 2, 3};  t[4] = 4
来源：http://adu.epnwcf.com

[T34] Lua：遍历表
来源：http://aqj.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://iji.kuanghao11.cn

[T35] Lua：字典表
来源：http://yby.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://xwq.ydjk.org.cn

[T36] Lua：函数
来源：http://swa.yfazqb.com

function add(a, b) return a + b end
来源：http://fvo.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://lrk.jinyuanbaomall.cn

"a" .. "b"
来源：http://hov.cheryme.top

[T38] Lua：条件
来源：http://blf.bbcook.cn

if x > 0 then print("正") end
来源：http://rnd.0kj1m.cn

[T39] Lua：模式匹配
来源：http://rfp.ivvv.top

string.find(s, "%d+")
来源：http://txa.316326.xyz

[T40] Lua：元表
来源：http://ptu.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://kgp.zycfv.cn

[T41] Perl：Hello World
来源：http://tpf.jqgfzy.top

print "Hello\n";
来源：http://bvr.hnxiangtu.top

[T42] Perl：变量类型
来源：http://khe.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pmb.yangfankeji.com

[T43] Perl：字符串插值
来源：http://jvv.ppjwa.cn

"值: $a"
来源：http://yfq.cashguo.top

[T44] Perl：条件
来源：http://zxl.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://sbl.cheryme.top

[T45] Perl：数组遍历
来源：http://cia.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://iai.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://mey.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://esw.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://mtf.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://han.jqgufenzy.top

[T48] Perl：正则替换
来源：http://gsw.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://wyr.redwolf501.top

[T49] Perl：函数
来源：http://xhs.ydjk.org.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fnp.yj202588.top

[T50] Perl：逐行读文件
来源：http://hai.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://tei.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://hak.tarul.cn

[T51] Scala：Hello World
来源：http://spy.xylfe.cn

println("Hello")
来源：http://yxu.jiagoushi.top

[T52] Scala：变量
来源：http://yri.guowangkeji.top

val a = 1;  var b = 2
来源：http://xil.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://zgr.birdmap.top

s"值: $b"
来源：http://rkj.tian-w.cn

[T54] Scala：集合映射
来源：http://bxn.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://zuu.xylfe.cn

[T55] Scala：集合过滤
来源：http://ekz.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://hpa.nanxuanxn.top

[T56] Scala：样例类
来源：http://nhy.shangyingyoupin.top

case class User(name: String, age: Int)
来源：http://htz.yj202588.top

[T57] Scala：模式匹配
来源：http://nnz.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xyf.gzhubu.top

[T58] Scala：函数定义
来源：http://jrz.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://pyv.gaohongyu789.top

[T59] Scala：循环
来源：http://qwy.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://wkt.hfpthk.cn

[T60] Scala：折叠
来源：http://xdo.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lzq.tarul.cn

================================================================================
来源：http://ohk.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cvg.jianghu66.top

================================================================================
来源：http://lzz.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://nkb.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sqr.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://idz.gotoacloud.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://woe.yuanzhike.top

[U03] Py：加载 .env 配置
来源：http://hkl.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://qhf.birdmap.top

[U04] Py：变量调试打印
来源：http://qig.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hbw.ybcxt.top

[U05] Py：列表去重且保序
来源：http://cvs.mhx1999.top

list(dict.fromkeys(arr))
来源：http://nqn.nanxinkj.top

[U06] Py：合并两个字典
来源：http://fse.dianchejie.cn

{**a, **b}
来源：http://smo.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://gaq.zhongyouzk.top

{v: k for k, v in d.items()}
来源：http://tld.dianchejie.cn

[U08] Py：展平二维列表
来源：http://xzj.yangfankeji.com

[y for x in nested for y in x]
来源：http://ehh.cashguo.top

[U09] Py：字典取最大值的键
来源：http://orn.jqgfzy.top

max(d, key=d.get)
来源：http://fcd.0kj1m.cn

[U10] Py：按值排序字典
来源：http://iay.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rvy.hysaishi.cn

[U11] Py：生成器表达式
来源：http://kon.mhx1999.top

(x * 2 for x in arr)
来源：http://aat.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oqb.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://ulu.chenlongwang.top

[U13] Py：固定长度队列
来源：http://ldn.quarkkingdee.top

deque(maxlen=10)
来源：http://oxe.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://lsq.52xcode.cn

defaultdict(list)
来源：http://xmy.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://vze.feifeiyinyue.top

t = time.perf_counter()
来源：http://zwv.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://acr.ppjwa.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vgw.shuidangran.top

[U17] Py：初始化日志
来源：http://dfb.shanyushiyangtech.top

logging.basicConfig(level=logging.INFO)
来源：http://bsr.chenzaomai.com

[U18] Py：预编译正则
来源：http://oop.mhx1999.top

pat = re.compile(r"\d+")
来源：http://cdk.yfazqb.com

[U19] Py：正则替换带回调
来源：http://qxm.fktsv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xvf.shanyushiyangkeji.top

[U20] Py：缓存函数结果
来源：http://jzf.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://jhz.xingfuxueyuan.xyz

[U21] Py：自定义上下文管理器
来源：http://arl.yvedp.cn

@contextlib.contextmanager
来源：http://pcy.shuidangran.top

[U22] Py：矩阵转置
来源：http://vau.dashuyun.cn

list(zip(*m))
来源：http://dzz.ywan-chungtsiang.top

[U23] Py：分块读取大文件
来源：http://byi.yonumen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wjl.bbcook.cn

[U24] Py：路径操作
来源：http://dtl.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lhw.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://qyt.yangfankeji.com

csv.DictReader(f)
来源：http://wgi.bbcook.cn

[U26] Py：并发下载
来源：http://tvi.xuanzx.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nve.xuetiantiany.cn

[U27] Py：异步 HTTP
来源：http://wkj.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://opr.quarkkingdee.top

[U28] Py：类型别名
来源：http://yif.yonumen.top

UserId = int
来源：http://ndg.guowangkeji.top

[U29] Py：属性校验
来源：http://yns.birdmap.top

@property 与 @x.setter 配合
来源：http://zcm.hfpthk.cn

[U30] Py：数据类
来源：http://ijo.zdqjudy.top

@dataclass(slots=True)
来源：http://rsb.jqgfzy.top

[U31] Py：单测
来源：http://ikg.nanxinkj.top

python -m pytest -q
来源：http://gxv.jinqigfzy.top

[U32] Py：代码格式化
来源：http://rii.gotoacloud.top

ruff format . && ruff check --fix .
来源：http://fga.shzxlz.cn

[U33] Py：打包发布
来源：http://bpg.zhaomingkeji.xyz

python -m build  （依赖 pyproject.toml）
来源：http://wek.xinyue.icu

[U34] Py：判断编码
来源：http://acf.shzxlz.cn

chardet.detect(raw)
来源：http://rba.gotoacloud.top

[U35] Py：发送邮件
来源：http://jlj.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hif.xingfuxueyuan.xyz

[U36] Py：定时任务
来源：http://ktb.jinyuanbaomall.cn

schedule.every(10).minutes.do(job)
来源：http://frz.ivvv.top

[U37] Py：读写 Excel
来源：http://ecg.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://got.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://ped.tarul.cn

Path(__file__).resolve().parent
来源：http://btc.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://oih.zhiwuduotai.top

sys.stdout.isatty()
来源：http://rxq.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://tgk.fengsongda.top

print("err", file=sys.stderr)
来源：http://jej.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://zns.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zgk.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://uvi.shanyushiyangtech.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://utt.ehwqpu.com

[U43] PHP：声明命名空间
来源：http://gmb.ppjwa.cn

namespace App\Http;
来源：http://hyp.tarul.cn

[U44] PHP：开启严格类型
来源：http://sym.ppjwa.cn

declare(strict_types=1);
来源：http://axc.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://vyd.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xla.hfpthk.cn

[U46] PHP：可空类型
来源：http://efr.havefunace.top

?string $name = null
来源：http://hql.fehbvm.com

[U47] PHP：联合类型
来源：http://hdm.gaohongyu789.top

int|string $id
来源：http://uye.sysykeji.top

[U48] PHP：纯枚举
来源：http://nbm.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://izy.52xcode.cn

[U49] PHP：只读属性
来源：http://gbe.jqgfzy.top

public readonly string $name
来源：http://qum.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://unr.epnwcf.com

public function __construct(private int $id) {}
来源：http://qpz.yongpay.top

[U51] PHP：数组解构
来源：http://vsv.hnqzz.top

[$a, $b] = $arr;
来源：http://kam.epnwcf.com

[U52] PHP：箭头函数
来源：http://gzo.yj20258888.top

$double = fn($x) => $x * 2;
来源：http://bpd.shuidangran.top

[U53] PHP：空合并运算符
来源：http://jma.bbcook.cn

$v = $a ?? $b ?? "default";
来源：http://szk.shzxlz.cn

[U54] PHP：空安全调用
来源：http://jkp.jqgfzy.top

$obj?->method()
来源：http://kgr.xinyue.icu

[U55] PHP：match 表达式
来源：http://irv.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aul.dianchejie.cn

[U56] PHP：命名参数
来源：http://jyf.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://tuq.sjlbkw.cn

[U57] PHP：字符串插值
来源：http://lfv.xuetiantiany.cn

"值: {$a}"
来源：http://ptb.andypj.xyz

[U58] PHP：数组三件套
来源：http://nua.ppjwa.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tpt.gzhubu.top

[U59] PHP：自定义排序
来源：http://vbf.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iwd.shanyushiyangkeji.top

[U60] PHP：JSON 编解码
来源：http://dam.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bjc.ivvv.top

[U61] PHP：正则
来源：http://qfe.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yii.hesvh.cn

[U62] PHP：日期对象
来源：http://sop.vehdjk.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wnn.chenjidiqi.icu

[U63] PHP：文件读写
来源：http://pnn.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dzs.jianghu66.top

[U64] PHP：目录遍历
来源：http://zek.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://xhg.sxryk.cn

[U65] PHP：会话
来源：http://apk.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rkn.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://bbb.nanxinkj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qpz.daxiang520.top

[U67] PHP：处理文件上传
来源：http://fdv.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bcq.sxryk.cn

[U68] PHP：PDO 连接
来源：http://bav.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fcp.0kj1m.cn


<!-- 参考信息 -->