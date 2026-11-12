代发 wailian999

#include <iostream>
来源：http://scw.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://kdg.fktsv.cn

[S32] C++：字符串
来源：http://eno.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://tpo.ppjwa.cn

[S33] C++：vector 增删
来源：http://yga.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jvo.zdbjq.cn

[S34] C++：遍历 vector
来源：http://kxy.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://fgb.yj202588.top

[S35] C++：map
来源：http://vcf.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lkm.sufxvd.cn

[S36] C++：unordered_map
来源：http://fak.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fbc.zdqjudy.top

[S37] C++：set
来源：http://kmt.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fgw.yuanzhike.top

[S38] C++：排序
来源：http://lds.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://lya.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://pqn.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zbq.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://vay.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kwh.hnqzz.top

[S41] C++：类与构造函数
来源：http://xxc.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ypk.zycfv.cn

[S42] C++：继承与虚函数
来源：http://cdn.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://ctx.ydzc1.top

[S43] C++：智能指针
来源：http://bya.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://dth.fengsongda.top

[S44] C++：引用传参
来源：http://iqd.yfazqb.com

void inc(int &x) { ++x; }
来源：http://tjl.chenjidiqi.icu

[S45] C++：lambda
来源：http://dej.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pax.shuidangran.top

[S46] C++：函数模板
来源：http://rgo.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nxu.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://pmo.havefunace.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uqg.yuxming.cn

[S48] C++：逐行读文件
来源：http://zuz.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://sjb.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://kxv.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://dqi.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aep.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://rcn.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lep.ybcxt.top

[S51] C++：显式类型转换
来源：http://mac.hnqzz.top

static_cast<double>(a) / b
来源：http://dzc.meibo888.top

[S52] C++：const 与 noexcept
来源：http://lux.tarul.cn

int size() const noexcept { return n_; }
来源：http://gqr.shzxlz.cn

[S53] C++：移动语义
来源：http://qdv.zdqjudy.top

std::vector<int> w = std::move(v);
来源：http://rsz.zhijiandao.cn

[S54] C++：异常处理
来源：http://ljn.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qgj.yueranfly.top

[S55] C++：结构化绑定
来源：http://qsm.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://dtp.chenzaomai.com

[S56] C++：optional
来源：http://mow.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://puc.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://phk.vehdjk.com

constexpr int N = 10;
来源：http://idz.zdbjq.cn

[S58] C++：命名空间
来源：http://hsn.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://ikx.zhiwuduotai.top

[S59] C++：静态断言
来源：http://uut.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://eki.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wul.zhongyouzk.top

================================================================================
来源：http://swz.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mgq.aibaodan.cn

================================================================================
来源：http://uqa.nwbrower.top

[T01] Kotlin：Hello World
来源：http://azo.aibaodan.cn

println("Hello")
来源：http://uli.pycfn.com

[T02] Kotlin：变量
来源：http://cmg.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nkb.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://bov.jinyuanbaomall.cn

"值: $b"
来源：http://voo.yj20258888.top

[T04] Kotlin：空安全
来源：http://fnh.shuidangran.top

val n: String? = null;  n?.length
来源：http://yah.zdbjq.cn

[T05] Kotlin：when 表达式
来源：http://dmu.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bos.epnwcf.com

[T06] Kotlin：集合映射
来源：http://ale.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gjw.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://lsc.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://qia.52xcode.cn

[T08] Kotlin：数据类
来源：http://jcm.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://vnd.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://vqy.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://urc.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://bnn.svipenyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://foi.yanxiufei.cn

[T11] Kotlin：协程
来源：http://yhm.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://yuo.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://zmk.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://mkd.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://pmm.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://mpm.tianlin.xyz

[T14] Kotlin：循环
来源：http://mrz.hnqzz.top

for (i in 1..10) println(i)
来源：http://ayb.xinyue.icu

[T15] Kotlin：接口
来源：http://tni.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://qjl.yongpay.top

[T16] Swift：Hello World
来源：http://gxx.snrcjt.cn

print("Hello")
来源：http://sta.hammf.cn

[T17] Swift：变量与常量
来源：http://mgn.andypj.xyz

var a = 1;  let b = 2
来源：http://auc.yfazqb.com

[T18] Swift：字符串插值
来源：http://xrz.yvedp.cn

"值: \(b)"
来源：http://yni.zycfv.cn

[T19] Swift：可选绑定
来源：http://pbk.hammf.cn

if let n = opt { print(n) }
来源：http://ihs.fengsongda.top

[T20] Swift：数组操作
来源：http://wbv.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kmn.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://joo.hcnkem.com

for x in a { print(x) }
来源：http://orl.tianlin.xyz

[T22] Swift：字典
来源：http://qss.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://gaj.sufxvd.cn

[T23] Swift：函数
来源：http://gzi.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gvi.sysykeji.top

[T24] Swift：闭包
来源：http://iqk.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xwu.chenjidiqi.icu

[T25] Swift：结构体
来源：http://rbu.gzhubu.top

struct P { var x: Int }
来源：http://zmt.hesvh.cn

[T26] Swift：类与重写
来源：http://nxb.nwbrower.top

class A: Base { override func f() {} }
来源：http://iys.yj20258888.top

[T27] Swift：错误处理
来源：http://zfi.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://vkm.jianghu66.top

[T28] Swift：枚举
来源：http://byr.havefunace.top

enum Color { case red, green }
来源：http://uas.cqqwz.cn

[T29] Swift：guard 提前返回
来源：http://rme.bjfxy.top

guard let x = opt else { return }
来源：http://dms.jinqigfzy.top

[T30] Swift：协议
来源：http://sxl.dianchejie.cn

protocol Shape { func area() -> Double }
来源：http://ski.hcnkem.com

[T31] Lua：Hello World
来源：http://jou.sweek.top

print("Hello")
来源：http://yvf.snrcjt.cn

[T32] Lua：局部变量
来源：http://zth.tianlin.xyz

local a = 1
来源：http://dwk.hcnkem.com

[T33] Lua：表（数组）
来源：http://man.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://htf.nwbrower.top

[T34] Lua：遍历表
来源：http://rdu.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dfd.zhoulong.xyz

[T35] Lua：字典表
来源：http://xko.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://wqz.daria6918.cn

[T36] Lua：函数
来源：http://ssk.cqqwz.cn

function add(a, b) return a + b end
来源：http://vdz.shanyushiyangtech.top

[T37] Lua：字符串拼接
来源：http://mqz.hfpthk.cn

"a" .. "b"
来源：http://lbz.yanxiufei.cn

[T38] Lua：条件
来源：http://zif.sxryk.cn

if x > 0 then print("正") end
来源：http://wbv.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://kaj.zhiwuduotai.top

string.find(s, "%d+")
来源：http://pku.ybcxt.top

[T40] Lua：元表
来源：http://ijl.yfazqb.com

setmetatable({}, { __index = base })
来源：http://ohn.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://szu.birdmap.top

print "Hello\n";
来源：http://pot.gogol.net.cn

[T42] Perl：变量类型
来源：http://olo.zhaomingkeji.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yei.fengsongda.top

[T43] Perl：字符串插值
来源：http://fsk.zhaomingkeji.xyz

"值: $a"
来源：http://qfp.hongshengwenyu.top

[T44] Perl：条件
来源：http://snb.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://vbp.zdqjudy.top

[T45] Perl：数组遍历
来源：http://sfh.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://xng.tianlin.xyz

[T46] Perl：哈希操作
来源：http://yxw.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ctu.guannengcc.top

[T47] Perl：正则捕获
来源：http://gfp.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vix.cheryme.top

[T48] Perl：正则替换
来源：http://hbr.ydjk.org.cn

$s =~ s/old/new/g;
来源：http://aqj.fktsv.cn

[T49] Perl：函数
来源：http://oex.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oza.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://vqg.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zzx.bjfxy.top

while (my $line = <$fh>) { print $line; }
来源：http://ccu.jyoumei.cn

[T51] Scala：Hello World
来源：http://mwf.xylfe.cn

println("Hello")
来源：http://bjf.yvedp.cn

[T52] Scala：变量
来源：http://hoz.xuanzx.com

val a = 1;  var b = 2
来源：http://eqk.hfpthk.cn

[T53] Scala：字符串插值
来源：http://ubr.zdbjq.cn

s"值: $b"
来源：http://zaz.haohaochexian.top

[T54] Scala：集合映射
来源：http://fja.xuetiantiany.cn

List(1, 2, 3).map(_ * 2)
来源：http://bsi.smart0.xyz

[T55] Scala：集合过滤
来源：http://bcl.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://kmx.hongshengwenyu.top

[T56] Scala：样例类
来源：http://ebn.9152youxi.cn

case class User(name: String, age: Int)
来源：http://suf.c1oappe.top

[T57] Scala：模式匹配
来源：http://ydo.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yjx.birdmap.top

[T58] Scala：函数定义
来源：http://snn.hongshengwenyu.top

def add(a: Int, b: Int): Int = a + b
来源：http://lxa.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://gdj.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://vsf.hesvh.cn

[T60] Scala：折叠
来源：http://gzi.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://npi.hammf.cn

================================================================================
来源：http://bvt.chenlongwang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sys.yj20258.top

================================================================================
来源：http://vhw.316326.xyz

[U01] Py：创建虚拟环境
来源：http://arw.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://lly.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://iup.zdqjudy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rhm.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://qtc.pycfn.com

from dotenv import load_dotenv; load_dotenv()
来源：http://qcf.316326.xyz

[U04] Py：变量调试打印
来源：http://beo.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mjo.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://siv.zhoulong.xyz

list(dict.fromkeys(arr))
来源：http://zzk.snrcjt.cn

[U06] Py：合并两个字典
来源：http://rgo.ydzc1.top

{**a, **b}
来源：http://lyo.zycfv.cn

[U07] Py：反转字典键值
来源：http://fjf.zhongyouzk.top

{v: k for k, v in d.items()}
来源：http://qgu.zdbjq.cn

[U08] Py：展平二维列表
来源：http://ire.sweek.top

[y for x in nested for y in x]
来源：http://rfv.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://hcj.vehdjk.com

max(d, key=d.get)
来源：http://bvj.sweek.top

[U10] Py：按值排序字典
来源：http://wvt.pycfn.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sfp.cdnleiting.top

[U11] Py：生成器表达式
来源：http://gyz.hammf.cn

(x * 2 for x in arr)
来源：http://hpx.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rvz.mhx1999.top

Counter(arr).most_common(3)
来源：http://xqb.shzxlz.cn

[U13] Py：固定长度队列
来源：http://bsd.fanxiaobao.xyz

deque(maxlen=10)
来源：http://lco.sweek.top

[U14] Py：分组收集到列表
来源：http://pco.xziqi.cn

defaultdict(list)
来源：http://jyw.aizwys.cn

[U15] Py：高精度计时
来源：http://mgq.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://mlr.sysykeji.top

[U16] Py：命令行参数解析
来源：http://tlm.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ayl.epnwcf.com

[U17] Py：初始化日志
来源：http://avt.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://yvs.dashuyun.cn

[U18] Py：预编译正则
来源：http://rwa.aibaodan.cn

pat = re.compile(r"\d+")
来源：http://dkq.bjfxy.top

[U19] Py：正则替换带回调
来源：http://maa.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://viq.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://igj.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://kee.ivvv.top

[U21] Py：自定义上下文管理器
来源：http://chy.c1oappe.top

@contextlib.contextmanager
来源：http://nvw.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://blr.sweek.top

list(zip(*m))
来源：http://qiu.ybcxt.top

[U23] Py：分块读取大文件
来源：http://lkz.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yrg.zhongyouzk.top

[U24] Py：路径操作
来源：http://jlv.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gsn.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://cya.hammf.cn

csv.DictReader(f)
来源：http://kcu.vehdjk.com

[U26] Py：并发下载
来源：http://eag.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dmp.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://uxe.xylfe.cn

aiohttp.ClientSession() 配合 async with
来源：http://mif.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://xzo.ppjwa.cn

UserId = int
来源：http://cmf.gogol.net.cn

[U29] Py：属性校验
来源：http://oyp.shuidangran.top

@property 与 @x.setter 配合
来源：http://gcg.xingfuxueyuan.xyz

[U30] Py：数据类
来源：http://cpx.gaohongyu789.top

@dataclass(slots=True)
来源：http://ryu.zhaomingkeji.xyz

[U31] Py：单测
来源：http://oox.yvedp.cn

python -m pytest -q
来源：http://bli.chenzaomai.com

[U32] Py：代码格式化
来源：http://ehe.guannengcc.top

ruff format . && ruff check --fix .
来源：http://pmn.svipenyu.cn

[U33] Py：打包发布
来源：http://fcm.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://uhm.jyoumei.cn

[U34] Py：判断编码
来源：http://ivj.hnxiangtu.top

chardet.detect(raw)
来源：http://fsb.yangfankeji.com

[U35] Py：发送邮件
来源：http://usu.ybcxt.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rxp.daria6918.cn

[U36] Py：定时任务
来源：http://sas.vehdjk.com

schedule.every(10).minutes.do(job)
来源：http://mud.andypj.xyz

[U37] Py：读写 Excel
来源：http://hhv.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wqi.tian-w.cn

[U38] Py：获取脚本所在目录
来源：http://vae.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://ztc.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://mvz.cqqwz.cn

sys.stdout.isatty()
来源：http://kir.fengsongda.top

[U40] Py：打印到标准错误
来源：http://shu.havefunace.top

print("err", file=sys.stderr)
来源：http://fxh.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://lbg.zdbjq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lob.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://val.bbcook.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mca.chenlongwang.top

[U43] PHP：声明命名空间
来源：http://rfa.hongshengwenyu.top

namespace App\Http;
来源：http://vtb.xziqi.cn

[U44] PHP：开启严格类型
来源：http://tlw.quarkkingdee.top

declare(strict_types=1);
来源：http://xsr.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://ccl.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://say.chenlongwang.top

[U46] PHP：可空类型
来源：http://trg.jqgfzy.top

?string $name = null
来源：http://aca.ivvv.top

[U47] PHP：联合类型
来源：http://its.fengsongda.top

int|string $id
来源：http://sax.cdnleiting.top

[U48] PHP：纯枚举
来源：http://umg.meibo888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tbt.vehdjk.com

[U49] PHP：只读属性
来源：http://ykq.nanxuanxn.top

public readonly string $name
来源：http://fod.pengpengdd.cyou

[U50] PHP：构造器属性提升
来源：http://dmo.meibo888.top

public function __construct(private int $id) {}
来源：http://feu.jianghu66.top

[U51] PHP：数组解构
来源：http://zkr.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://nvr.yj20258888.top

[U52] PHP：箭头函数
来源：http://mgm.ppjwa.cn

$double = fn($x) => $x * 2;
来源：http://ygb.tarul.cn

[U53] PHP：空合并运算符
来源：http://jdi.feifeiyinyue.top

$v = $a ?? $b ?? "default";
来源：http://ilt.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://alx.jqgufenzy.top

$obj?->method()
来源：http://kfw.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://jjt.zycfv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qrl.yongpay.top

[U56] PHP：命名参数
来源：http://yrf.zhixingplan.top

f(a: 1, b: 2)
来源：http://aey.hnqzz.top


<!-- 参考信息 -->