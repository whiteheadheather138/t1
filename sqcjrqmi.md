代发 wailian999

x |= (1 << 3);
来源：http://tbk.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://dsy.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wwf.0kj1m.cn

[S18] C：命令行参数
来源：http://ijg.zycfv.cn

int main(int argc, char **argv)
来源：http://qzi.hammf.cn

[S19] C：快速排序
来源：http://wqa.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hhu.ydzc1.top

[S20] C：二分查找
来源：http://ley.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fqb.yfazqb.com

[S21] C：字符类别判断
来源：http://ebf.yvedp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://phu.wangdashe.top

[S22] C：字符串转数字
来源：http://cmd.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://gdy.cdnleiting.top

[S23] C：随机数
来源：http://qya.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qbd.snrcjt.cn

[S24] C：获取本地时间
来源：http://mow.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lcx.yonumen.top

[S25] C：内存拷贝
来源：http://fxi.havefunace.top

memcpy(dst, src, n);
来源：http://srr.haohaochexian.top

[S26] C：内存清零
来源：http://zfl.hammf.cn

memset(a, 0, sizeof a);
来源：http://ufz.vehdjk.com

[S27] C：定义常量
来源：http://odl.guowangkeji.top

const double PI = 3.14159;
来源：http://pys.jinqigfzy.top

[S28] C：静态变量
来源：http://ubz.yvedp.cn

static int counter = 0;
来源：http://ykk.yanxiufei.cn

[S29] C：变参函数
来源：http://sxn.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uay.yj20258.top

[S30] C：头文件保护
来源：http://eps.zycfv.cn

#ifndef X_H
来源：http://jrp.zhijiandao.cn

#define X_H
来源：http://ywa.wangdashe.top

#endif
来源：http://ybr.yj20258.top

[S31] C++：Hello World
来源：http://qne.yanxiufei.cn

#include <iostream>
来源：http://glt.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://ebi.jinghuilouyu.cn

[S32] C++：字符串
来源：http://sog.fengsongda.top

std::string s = "hi";  s += "!";
来源：http://dfo.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://giq.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eiu.dianchejie.cn

[S34] C++：遍历 vector
来源：http://tmw.pycfn.com

for (auto &x : v) { std::cout << x; }
来源：http://xdb.xinyue.icu

[S35] C++：map
来源：http://jxt.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pes.sufxvd.cn

[S36] C++：unordered_map
来源：http://kto.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://npx.cucudq.cn

[S37] C++：set
来源：http://dnp.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://siq.ctjpmb.com

[S38] C++：排序
来源：http://fgu.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://scl.cashguo.top

[S39] C++：自定义比较器排序
来源：http://mqn.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lub.cheryme.top

[S40] C++：查找元素
来源：http://vsp.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yjd.cheryme.top

[S41] C++：类与构造函数
来源：http://rld.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vpe.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://aof.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://gma.zhijiandao.cn

[S43] C++：智能指针
来源：http://myw.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://uqu.shangyingyoupin.top

[S44] C++：引用传参
来源：http://plz.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://rwh.shanyushiyangtech.top

[S45] C++：lambda
来源：http://wpj.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rhb.pengpengdd.cyou

[S46] C++：函数模板
来源：http://lqb.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gkj.shanyushiyangtech.top

[S47] C++：结构化绑定遍历
来源：http://kzr.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aqi.zdqjudy.top

[S48] C++：逐行读文件
来源：http://ojx.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://qpm.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://tys.zhixingplan.top

[S49] C++：写文件
来源：http://ure.xuetiantiany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fff.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://vza.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iji.andypj.xyz

[S51] C++：显式类型转换
来源：http://nkb.dianchejie.cn

static_cast<double>(a) / b
来源：http://dhy.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://gfc.ywan-chungtsiang.top

int size() const noexcept { return n_; }
来源：http://pew.fktsv.cn

[S53] C++：移动语义
来源：http://bob.havefunace.top

std::vector<int> w = std::move(v);
来源：http://hax.yj202588.top

[S54] C++：异常处理
来源：http://gkb.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zau.0kj1m.cn

[S55] C++：结构化绑定
来源：http://xwx.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xsh.ctjpmb.com

[S56] C++：optional
来源：http://qlh.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qfp.ivvv.top

[S57] C++：编译期常量
来源：http://zth.dianchejie.cn

constexpr int N = 10;
来源：http://wpj.snrcjt.cn

[S58] C++：命名空间
来源：http://whc.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://wnq.sysykeji.top

[S59] C++：静态断言
来源：http://tis.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qas.hcnkem.com

[S60] C++：遍历并删除元素
来源：http://nhs.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gou.ehwqpu.com

================================================================================
来源：http://uoi.pycfn.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://waw.birdmap.top

================================================================================
来源：http://jto.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://exu.zhaomingkeji.xyz

println("Hello")
来源：http://qlq.ybcxt.top

[T02] Kotlin：变量
来源：http://hpi.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hnm.cheryme.top

[T03] Kotlin：字符串模板
来源：http://doj.aizwys.cn

"值: $b"
来源：http://usr.hnqzz.top

[T04] Kotlin：空安全
来源：http://khi.jinqigfzy.top

val n: String? = null;  n?.length
来源：http://vgo.yongpay.top

[T05] Kotlin：when 表达式
来源：http://tyx.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dht.yuxming.cn

[T06] Kotlin：集合映射
来源：http://bvv.52xcode.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://evz.cashguo.top

[T07] Kotlin：集合过滤
来源：http://mtk.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://uye.yangfankeji.com

[T08] Kotlin：数据类
来源：http://bid.pycfn.com

data class User(val name: String, val age: Int)
来源：http://kji.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://efv.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://wos.xuanzx.com

[T10] Kotlin：默认参数
来源：http://lrm.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zmg.hfpthk.cn

[T11] Kotlin：协程
来源：http://vtx.cdnleiting.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oun.xuanzx.com

[T12] Kotlin：解构声明
来源：http://dgl.zhongyouzk.top

val (a, b) = Pair(1, 2)
来源：http://aup.havefunace.top

[T13] Kotlin：只读 Map
来源：http://ycf.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://sje.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://liu.havefunace.top

for (i in 1..10) println(i)
来源：http://kxd.xingfuxueyuan.xyz

[T15] Kotlin：接口
来源：http://ppn.fehbvm.com

interface Shape { fun area(): Double }
来源：http://kxv.chenlongwang.top

[T16] Swift：Hello World
来源：http://whh.zhaomingkeji.xyz

print("Hello")
来源：http://kon.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://bym.cheryme.top

var a = 1;  let b = 2
来源：http://jrw.sweek.top

[T18] Swift：字符串插值
来源：http://tdl.hammf.cn

"值: \(b)"
来源：http://hdn.zhixingplan.top

[T19] Swift：可选绑定
来源：http://fvm.fktsv.cn

if let n = opt { print(n) }
来源：http://rks.xziqi.cn

[T20] Swift：数组操作
来源：http://ohs.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://tll.ehwqpu.com

[T21] Swift：遍历
来源：http://acu.daria6918.cn

for x in a { print(x) }
来源：http://ybr.wangdashe.top

[T22] Swift：字典
来源：http://lhl.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://hik.zhaomingkeji.xyz

[T23] Swift：函数
来源：http://tao.hfpthk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jqp.hywenlv.cn

[T24] Swift：闭包
来源：http://rcf.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://omf.xinyue.icu

[T25] Swift：结构体
来源：http://qna.cdnleiting.top

struct P { var x: Int }
来源：http://hir.shzxlz.cn

[T26] Swift：类与重写
来源：http://nur.jqgfzy.top

class A: Base { override func f() {} }
来源：http://wtk.xylfe.cn

[T27] Swift：错误处理
来源：http://jxi.birdmap.top

do { try f() } catch { print(error) }
来源：http://sdl.0kj1m.cn

[T28] Swift：枚举
来源：http://aqv.ehwqpu.com

enum Color { case red, green }
来源：http://mzm.haohaochexian.top

[T29] Swift：guard 提前返回
来源：http://ezw.zhoulong.xyz

guard let x = opt else { return }
来源：http://urr.xuanzx.com

[T30] Swift：协议
来源：http://gyi.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://cdc.dianchejie.cn

[T31] Lua：Hello World
来源：http://nkn.sysykeji.top

print("Hello")
来源：http://nda.9152youxi.cn

[T32] Lua：局部变量
来源：http://ogn.fehbvm.com

local a = 1
来源：http://xrt.haohaochexian.top

[T33] Lua：表（数组）
来源：http://thw.hnqzz.top

local t = {1, 2, 3};  t[4] = 4
来源：http://usr.dianchejie.cn

[T34] Lua：遍历表
来源：http://vek.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://seb.yuanzhike.top

[T35] Lua：字典表
来源：http://ilh.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://nil.gzhubu.top

[T36] Lua：函数
来源：http://jtm.tanke756.top

function add(a, b) return a + b end
来源：http://dtt.epnwcf.com

[T37] Lua：字符串拼接
来源：http://raf.chenlongwang.top

"a" .. "b"
来源：http://vry.ctjpmb.com

[T38] Lua：条件
来源：http://ysw.svipenyu.cn

if x > 0 then print("正") end
来源：http://dvy.pycfn.com

[T39] Lua：模式匹配
来源：http://svx.cqqwz.cn

string.find(s, "%d+")
来源：http://wfa.cdnleiting.top

[T40] Lua：元表
来源：http://vso.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://jao.cucudq.cn

[T41] Perl：Hello World
来源：http://ahf.cheryme.top

print "Hello\n";
来源：http://mnw.sufxvd.cn

[T42] Perl：变量类型
来源：http://juw.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lpp.sysykeji.top

[T43] Perl：字符串插值
来源：http://rrw.meibo888.top

"值: $a"
来源：http://bja.jinqigufen.top

[T44] Perl：条件
来源：http://sqa.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://dpu.andypj.xyz

[T45] Perl：数组遍历
来源：http://ekg.fengsongda.top

for my $x (@arr) { print $x; }
来源：http://odr.dashuyun.cn

[T46] Perl：哈希操作
来源：http://ziv.chenzaomai.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vcj.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://cdg.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://afd.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://mvv.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://cky.hcnkem.com

[T49] Perl：函数
来源：http://inu.ydjk.org.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://muk.havefunace.top

[T50] Perl：逐行读文件
来源：http://hir.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vqm.jyoumei.cn

while (my $line = <$fh>) { print $line; }
来源：http://bbd.shzxlz.cn

[T51] Scala：Hello World
来源：http://fva.cashguo.top

println("Hello")
来源：http://til.meibo888.top

[T52] Scala：变量
来源：http://okw.yj20258888.top

val a = 1;  var b = 2
来源：http://fta.chenlongwang.top

[T53] Scala：字符串插值
来源：http://ebk.ydjk.org.cn

s"值: $b"
来源：http://hpv.yvedp.cn

[T54] Scala：集合映射
来源：http://ujc.aibaodan.cn

List(1, 2, 3).map(_ * 2)
来源：http://kxq.xuanzx.com

[T55] Scala：集合过滤
来源：http://nza.jinghuilouyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jom.shuidangran.top

[T56] Scala：样例类
来源：http://kmd.tianlin.xyz

case class User(name: String, age: Int)
来源：http://dlj.hnqzz.top

[T57] Scala：模式匹配
来源：http://fcf.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://rpb.gogol.net.cn

[T58] Scala：函数定义
来源：http://ggx.wangdashe.top

def add(a: Int, b: Int): Int = a + b
来源：http://vvi.yueranfly.top

[T59] Scala：循环
来源：http://xaf.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://bah.aizwys.cn

[T60] Scala：折叠
来源：http://yhw.fengsongda.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pya.hnqzz.top

================================================================================
来源：http://kwt.daxiang520.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gls.9152youxi.cn

================================================================================
来源：http://iyc.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://mvk.gogol.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pok.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://xih.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://naw.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://vmg.fanxiaobao.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://jcl.yongpay.top

[U04] Py：变量调试打印
来源：http://zzc.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qkk.wangdashe.top

[U05] Py：列表去重且保序
来源：http://yqg.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://geo.fengsongda.top

[U06] Py：合并两个字典
来源：http://exi.jianghu66.top

{**a, **b}
来源：http://ibg.zdqjudy.top

[U07] Py：反转字典键值
来源：http://osu.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://gdb.nwbrower.top

[U08] Py：展平二维列表
来源：http://pno.yuxming.cn

[y for x in nested for y in x]
来源：http://jmz.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://qak.tanke756.top

max(d, key=d.get)
来源：http://vyf.hfpthk.cn

[U10] Py：按值排序字典
来源：http://uoz.chenlongwang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eyh.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://kyb.yuxming.cn

(x * 2 for x in arr)
来源：http://ple.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://are.xziqi.cn

Counter(arr).most_common(3)
来源：http://arl.mhx1999.top

[U13] Py：固定长度队列
来源：http://cnp.hywenlv.cn

deque(maxlen=10)
来源：http://fni.uphjek.com

[U14] Py：分组收集到列表
来源：http://qjp.fanxiaobao.xyz

defaultdict(list)
来源：http://kkf.gotoacloud.top

[U15] Py：高精度计时
来源：http://khp.cucudq.cn

t = time.perf_counter()
来源：http://tju.kuanghao11.cn

[U16] Py：命令行参数解析
来源：http://wdn.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://knw.cucudq.cn

[U17] Py：初始化日志
来源：http://bur.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://zsd.haohaochexian.top

[U18] Py：预编译正则
来源：http://ywi.fengsongda.top

pat = re.compile(r"\d+")
来源：http://ong.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://xpk.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wpo.xinyue.icu

[U20] Py：缓存函数结果
来源：http://cub.hysaishi.cn

@functools.lru_cache(maxsize=None)
来源：http://kof.ybcxt.top

[U21] Py：自定义上下文管理器
来源：http://isy.ybcxt.top

@contextlib.contextmanager
来源：http://gmy.yvedp.cn

[U22] Py：矩阵转置
来源：http://rzd.zdqjudy.top

list(zip(*m))
来源：http://una.dianchejie.cn

[U23] Py：分块读取大文件
来源：http://tgy.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vmo.nwbrower.top

[U24] Py：路径操作
来源：http://bqw.sjlbkw.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pnx.xingfuxueyuan.xyz

[U25] Py：CSV 按字典读
来源：http://pyf.aizwys.cn

csv.DictReader(f)
来源：http://wgh.sweek.top

[U26] Py：并发下载
来源：http://xmg.shanyushiyangtech.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nku.pycfn.com

[U27] Py：异步 HTTP
来源：http://hap.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://tca.chenlongwang.top

[U28] Py：类型别名
来源：http://rha.hcnkem.com

UserId = int
来源：http://obi.zycfv.cn

[U29] Py：属性校验
来源：http://yhl.pengpengdd.cyou

@property 与 @x.setter 配合
来源：http://yht.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://hbf.tian-w.cn

@dataclass(slots=True)
来源：http://dpn.ydzc1.top

[U31] Py：单测
来源：http://gib.hywenlv.cn

python -m pytest -q
来源：http://ept.zhiwuduotai.top

[U32] Py：代码格式化
来源：http://ngd.ppjwa.cn

ruff format . && ruff check --fix .
来源：http://hub.yuxming.cn

[U33] Py：打包发布
来源：http://ryd.ctjpmb.com

python -m build  （依赖 pyproject.toml）
来源：http://ufu.fengsongda.top

[U34] Py：判断编码
来源：http://hqw.yfazqb.com

chardet.detect(raw)
来源：http://lhl.hesvh.cn

[U35] Py：发送邮件
来源：http://odb.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ffx.yuxming.cn

[U36] Py：定时任务
来源：http://cpa.cheryme.top

schedule.every(10).minutes.do(job)
来源：http://wvg.daria6918.cn

[U37] Py：读写 Excel
来源：http://yai.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://dzq.sysykeji.top

[U38] Py：获取脚本所在目录
来源：http://kqt.cqqwz.cn

Path(__file__).resolve().parent
来源：http://zzg.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://dzx.wangdashe.top

sys.stdout.isatty()
来源：http://ahj.vqdsnc.cn

[U40] Py：打印到标准错误
来源：http://enq.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://nsw.yfazqb.com


<!-- 参考信息 -->