代发 wailian999

int main(int argc, char **argv)
来源：http://qvl.jyoumei.cn

[S19] C：快速排序
来源：http://oqw.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://ndt.haohaochexian.top

[S20] C：二分查找
来源：http://vld.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oqh.nwbrower.top

[S21] C：字符类别判断
来源：http://wqw.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://enh.havefunace.top

[S22] C：字符串转数字
来源：http://lie.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rav.ehwqpu.com

[S23] C：随机数
来源：http://cdt.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rnz.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://ceu.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://klk.hammf.cn

[S25] C：内存拷贝
来源：http://ttq.smart0.xyz

memcpy(dst, src, n);
来源：http://vmi.shanyushiyangtech.top

[S26] C：内存清零
来源：http://kyj.redwolf501.top

memset(a, 0, sizeof a);
来源：http://glz.hywenlv.cn

[S27] C：定义常量
来源：http://eiy.smart0.xyz

const double PI = 3.14159;
来源：http://fae.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://uel.zhiwuduotai.top

static int counter = 0;
来源：http://kyk.jlsjyb.cn

[S29] C：变参函数
来源：http://nvb.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://psn.jiagoushi.top

[S30] C：头文件保护
来源：http://obl.snrcjt.cn

#ifndef X_H
来源：http://cki.birdmap.top

#define X_H
来源：http://gmh.jiagoushi.top

#endif
来源：http://acx.gaohongyu789.top

[S31] C++：Hello World
来源：http://zxd.cheryme.top

#include <iostream>
来源：http://fyn.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://lye.zhongyouzk.top

[S32] C++：字符串
来源：http://tng.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://ssa.redwolf501.top

[S33] C++：vector 增删
来源：http://dnc.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nvh.xinyue.icu

[S34] C++：遍历 vector
来源：http://kss.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://tlv.bbcook.cn

[S35] C++：map
来源：http://hkg.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://akn.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://vhc.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dtq.jinghuilouyu.cn

[S37] C++：set
来源：http://ijn.xziqi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pdf.shuidangran.top

[S38] C++：排序
来源：http://iod.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://rah.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://avk.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gzn.316326.xyz

[S40] C++：查找元素
来源：http://gzd.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://syw.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://los.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rfs.redwolf501.top

[S42] C++：继承与虚函数
来源：http://ujr.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://qfx.cdnleiting.top

[S43] C++：智能指针
来源：http://zyk.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://rck.epnwcf.com

[S44] C++：引用传参
来源：http://yur.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://ala.yj202588.top

[S45] C++：lambda
来源：http://zvr.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://wlf.c1oappe.top

[S46] C++：函数模板
来源：http://slj.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kbq.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://ivi.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://has.hongshengwenyu.top

[S48] C++：逐行读文件
来源：http://vqr.tarul.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sui.gzhubu.top

while (std::getline(in, line)) { }
来源：http://ncw.shuidangran.top

[S49] C++：写文件
来源：http://ygf.jqgufenzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ipn.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://gqa.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ycy.yj202588.top

[S51] C++：显式类型转换
来源：http://xst.hnxiangtu.top

static_cast<double>(a) / b
来源：http://bdx.sweek.top

[S52] C++：const 与 noexcept
来源：http://mso.zycfv.cn

int size() const noexcept { return n_; }
来源：http://iwl.pycfn.com

[S53] C++：移动语义
来源：http://jyt.yonumen.top

std::vector<int> w = std::move(v);
来源：http://ckh.tian-w.cn

[S54] C++：异常处理
来源：http://plh.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mgu.xuanzx.com

[S55] C++：结构化绑定
来源：http://pix.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tbk.feifeiyinyue.top

[S56] C++：optional
来源：http://nom.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xdq.zhongyouzk.top

[S57] C++：编译期常量
来源：http://tgp.hesvh.cn

constexpr int N = 10;
来源：http://bnw.guowangkeji.top

[S58] C++：命名空间
来源：http://wuc.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://qne.sweek.top

[S59] C++：静态断言
来源：http://cmk.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hvx.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://bpo.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mfz.ctjpmb.com

================================================================================
来源：http://dba.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kqg.jyoumei.cn

================================================================================
来源：http://zll.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://zwi.fengsongda.top

println("Hello")
来源：http://syd.ydzc1.top

[T02] Kotlin：变量
来源：http://huf.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bez.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://qwa.ydzc1.top

"值: $b"
来源：http://rkq.sweek.top

[T04] Kotlin：空安全
来源：http://bhq.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://skd.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://lqq.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pvv.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://cwj.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nrg.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://vfp.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wal.ydjk.org.cn

[T08] Kotlin：数据类
来源：http://mrn.svipenyu.cn

data class User(val name: String, val age: Int)
来源：http://tdu.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://ucd.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://yrb.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://znz.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gwd.cucudq.cn

[T11] Kotlin：协程
来源：http://nqm.yj20258.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pxa.sysykeji.top

[T12] Kotlin：解构声明
来源：http://icb.snrcjt.cn

val (a, b) = Pair(1, 2)
来源：http://vvj.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://uky.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://ahm.zycfv.cn

[T14] Kotlin：循环
来源：http://rnp.0kj1m.cn

for (i in 1..10) println(i)
来源：http://iaj.zhoulong.xyz

[T15] Kotlin：接口
来源：http://tud.yj20258888.top

interface Shape { fun area(): Double }
来源：http://dcn.hnqzz.top

[T16] Swift：Hello World
来源：http://bhy.chenjidiqi.icu

print("Hello")
来源：http://vqt.daxiang520.top

[T17] Swift：变量与常量
来源：http://ehg.zhijiandao.cn

var a = 1;  let b = 2
来源：http://kdc.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://xkd.bjfxy.top

"值: \(b)"
来源：http://xcv.sysykeji.top

[T19] Swift：可选绑定
来源：http://auf.jqgufenzy.top

if let n = opt { print(n) }
来源：http://wjs.hnxiangtu.top

[T20] Swift：数组操作
来源：http://src.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rwm.zhiwuduotai.top

[T21] Swift：遍历
来源：http://msh.yvedp.cn

for x in a { print(x) }
来源：http://xbt.jqgufenzy.top

[T22] Swift：字典
来源：http://sou.shanyushiyangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://igs.chenzaomai.com

[T23] Swift：函数
来源：http://stj.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cwi.daxiang520.top

[T24] Swift：闭包
来源：http://qdj.hysaishi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xhv.bbcook.cn

[T25] Swift：结构体
来源：http://haz.jqgufenzy.top

struct P { var x: Int }
来源：http://evu.jyoumei.cn

[T26] Swift：类与重写
来源：http://lnc.fehbvm.com

class A: Base { override func f() {} }
来源：http://lct.yfazqb.com

[T27] Swift：错误处理
来源：http://rfc.zycfv.cn

do { try f() } catch { print(error) }
来源：http://zxe.tian-w.cn

[T28] Swift：枚举
来源：http://aob.dianchejie.cn

enum Color { case red, green }
来源：http://qek.hesvh.cn

[T29] Swift：guard 提前返回
来源：http://gjl.hfpthk.cn

guard let x = opt else { return }
来源：http://guf.tianlin.xyz

[T30] Swift：协议
来源：http://ejo.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://lnk.zhaomingkeji.xyz

[T31] Lua：Hello World
来源：http://bfm.zhongyouzk.top

print("Hello")
来源：http://adi.feifeiyinyue.top

[T32] Lua：局部变量
来源：http://ugi.xinyue.icu

local a = 1
来源：http://gxx.xinyue.icu

[T33] Lua：表（数组）
来源：http://msh.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wru.wangdashe.top

[T34] Lua：遍历表
来源：http://eus.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://dln.svipenyu.cn

[T35] Lua：字典表
来源：http://tpg.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://sgj.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://hxb.sufxvd.cn

function add(a, b) return a + b end
来源：http://ern.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://ays.aizwys.cn

"a" .. "b"
来源：http://tit.yj20258888.top

[T38] Lua：条件
来源：http://tky.cucudq.cn

if x > 0 then print("正") end
来源：http://jhr.tianlin.xyz

[T39] Lua：模式匹配
来源：http://rem.yuxming.cn

string.find(s, "%d+")
来源：http://zhw.aizwys.cn

[T40] Lua：元表
来源：http://moo.nanxuanxn.top

setmetatable({}, { __index = base })
来源：http://kxe.zycfv.cn

[T41] Perl：Hello World
来源：http://uvt.daxiang520.top

print "Hello\n";
来源：http://mdl.bjfxy.top

[T42] Perl：变量类型
来源：http://rrs.chenzaomai.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://maq.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://cph.chenzaomai.com

"值: $a"
来源：http://cxe.havefunace.top

[T44] Perl：条件
来源：http://uct.nanxinkj.top

if ($a > 0) { print "正"; }
来源：http://zim.jqgfzy.top

[T45] Perl：数组遍历
来源：http://dxk.sufxvd.cn

for my $x (@arr) { print $x; }
来源：http://yid.zdqjudy.top

[T46] Perl：哈希操作
来源：http://krw.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jya.zhijiandao.cn

[T47] Perl：正则捕获
来源：http://sad.c1oappe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://myj.guowangkeji.top

[T48] Perl：正则替换
来源：http://xep.jiagoushi.top

$s =~ s/old/new/g;
来源：http://mrl.gaohongyu789.top

[T49] Perl：函数
来源：http://mer.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aft.yueranfly.top

[T50] Perl：逐行读文件
来源：http://sos.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bgc.cashguo.top

while (my $line = <$fh>) { print $line; }
来源：http://nfw.hysaishi.cn

[T51] Scala：Hello World
来源：http://xkh.aibaodan.cn

println("Hello")
来源：http://vzz.cdnleiting.top

[T52] Scala：变量
来源：http://poq.ehwqpu.com

val a = 1;  var b = 2
来源：http://dyf.52xcode.cn

[T53] Scala：字符串插值
来源：http://czc.chenlongwang.top

s"值: $b"
来源：http://ynp.jqgfzy.top

[T54] Scala：集合映射
来源：http://asn.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://sxa.c1oappe.top

[T55] Scala：集合过滤
来源：http://epi.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qje.ctjpmb.com

[T56] Scala：样例类
来源：http://plr.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://iry.0kj1m.cn

[T57] Scala：模式匹配
来源：http://kvi.hcnkem.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://vxw.jianghu66.top

[T58] Scala：函数定义
来源：http://auw.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://kvh.jianghu66.top

[T59] Scala：循环
来源：http://zte.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://daz.ydjk.org.cn

[T60] Scala：折叠
来源：http://pnf.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gbp.nwbrower.top

================================================================================
来源：http://iwu.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tzk.yangfankeji.com

================================================================================
来源：http://gki.yanxiufei.cn

[U01] Py：创建虚拟环境
来源：http://akk.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sdw.xylfe.cn

[U02] Py：导出 / 安装依赖
来源：http://wzz.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pnw.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://moq.ybcxt.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ysh.kuanghao11.cn

[U04] Py：变量调试打印
来源：http://rfr.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zoc.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://txx.bjfxy.top

list(dict.fromkeys(arr))
来源：http://kyu.snrcjt.cn

[U06] Py：合并两个字典
来源：http://zlp.kuanghao11.cn

{**a, **b}
来源：http://fcn.jqgufenzy.top

[U07] Py：反转字典键值
来源：http://oci.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://aau.yuxming.cn

[U08] Py：展平二维列表
来源：http://opq.vehdjk.com

[y for x in nested for y in x]
来源：http://jbb.daxiang520.top

[U09] Py：字典取最大值的键
来源：http://czb.jianghu66.top

max(d, key=d.get)
来源：http://udu.cqqwz.cn

[U10] Py：按值排序字典
来源：http://mcf.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zkg.chenlongwang.top

[U11] Py：生成器表达式
来源：http://zbf.cashguo.top

(x * 2 for x in arr)
来源：http://fie.cqqwz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://czk.hcnkem.com

Counter(arr).most_common(3)
来源：http://xnx.xziqi.cn

[U13] Py：固定长度队列
来源：http://ocv.guannengcc.top

deque(maxlen=10)
来源：http://ovl.sysykeji.top

[U14] Py：分组收集到列表
来源：http://rqk.svipenyu.cn

defaultdict(list)
来源：http://ffd.pycfn.com

[U15] Py：高精度计时
来源：http://zld.haohaochexian.top

t = time.perf_counter()
来源：http://sbs.guowangkeji.top

[U16] Py：命令行参数解析
来源：http://vie.hcnkem.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://spe.xylfe.cn

[U17] Py：初始化日志
来源：http://ztm.gotoacloud.top

logging.basicConfig(level=logging.INFO)
来源：http://siw.zhiwuduotai.top

[U18] Py：预编译正则
来源：http://khp.bjfxy.top

pat = re.compile(r"\d+")
来源：http://lsj.guannengcc.top

[U19] Py：正则替换带回调
来源：http://kyo.cdnleiting.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cxe.ivvv.top

[U20] Py：缓存函数结果
来源：http://zes.shangyingyoupin.top

@functools.lru_cache(maxsize=None)
来源：http://ijn.cucudq.cn

[U21] Py：自定义上下文管理器
来源：http://rke.0kj1m.cn

@contextlib.contextmanager
来源：http://czn.c1oappe.top

[U22] Py：矩阵转置
来源：http://ugd.quarkkingdee.top

list(zip(*m))
来源：http://efb.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://fig.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sfp.zhaomingkeji.xyz

[U24] Py：路径操作
来源：http://vgk.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mcc.yuxming.cn

[U25] Py：CSV 按字典读
来源：http://koc.guowangkeji.top

csv.DictReader(f)
来源：http://aem.nanxuanxn.top

[U26] Py：并发下载
来源：http://qvm.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ons.redwolf501.top

[U27] Py：异步 HTTP
来源：http://dzy.quarkkingdee.top

aiohttp.ClientSession() 配合 async with
来源：http://cok.fengsongda.top

[U28] Py：类型别名
来源：http://mhj.nanxinkj.top

UserId = int
来源：http://yyl.yongpay.top

[U29] Py：属性校验
来源：http://iql.sxryk.cn

@property 与 @x.setter 配合
来源：http://lyl.guannengcc.top

[U30] Py：数据类
来源：http://hci.smart0.xyz

@dataclass(slots=True)
来源：http://hwf.0kj1m.cn

[U31] Py：单测
来源：http://jzu.jlsjyb.cn

python -m pytest -q
来源：http://tmw.hywenlv.cn

[U32] Py：代码格式化
来源：http://obn.zhongyouzk.top

ruff format . && ruff check --fix .
来源：http://rai.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://tvw.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://drs.zhijiandao.cn

[U34] Py：判断编码
来源：http://npx.sweek.top

chardet.detect(raw)
来源：http://blb.gzhubu.top

[U35] Py：发送邮件
来源：http://jff.xziqi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xri.wangdashe.top

[U36] Py：定时任务
来源：http://vor.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://znk.mhx1999.top

[U37] Py：读写 Excel
来源：http://uey.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://cwm.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://fpz.kuanghao11.cn

Path(__file__).resolve().parent
来源：http://ldc.xuanzx.com

[U39] Py：判断是否在交互环境
来源：http://evg.gotoacloud.top

sys.stdout.isatty()
来源：http://vke.xuetiantiany.cn

[U40] Py：打印到标准错误
来源：http://elv.fktsv.cn

print("err", file=sys.stderr)
来源：http://sfo.hywenlv.cn

[U41] PHP：初始化 Composer 项目
来源：http://fxm.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zmk.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://msj.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://twg.haohaochexian.top


<!-- 参考信息 -->