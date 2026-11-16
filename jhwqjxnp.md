代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eol.yuanzhike.top

[S10] C：指针与解引用
来源：http://gxj.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://eum.jqgufenzy.top

[S11] C：逐行读文件
来源：http://aeo.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://xgz.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://vfd.jianghu66.top

fclose(f);
来源：http://wsf.fktsv.cn

[S12] C：写文件
来源：http://arv.yongpay.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cqs.pengpengdd.cyou

[S13] C：宏定义
来源：http://vgq.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xif.uphjek.com

[S14] C：枚举
来源：http://zey.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://fvc.nwbrower.top

[S15] C：类型转换
来源：http://vmt.fehbvm.com

(double) a / b
来源：http://nmb.andypj.xyz

[S16] C：位操作置位
来源：http://orr.ivvv.top

x |= (1 << 3);
来源：http://dgi.cucudq.cn

[S17] C：安全拼接字符串
来源：http://cmk.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uyr.cdnleiting.top

[S18] C：命令行参数
来源：http://ydn.ppjwa.cn

int main(int argc, char **argv)
来源：http://zwr.dashuyun.cn

[S19] C：快速排序
来源：http://evg.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://hlf.nanxuanxn.top

[S20] C：二分查找
来源：http://prf.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://urv.sxryk.cn

[S21] C：字符类别判断
来源：http://hud.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ewg.yfazqb.com

[S22] C：字符串转数字
来源：http://sdp.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://myr.jlsjyb.cn

[S23] C：随机数
来源：http://bmp.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jce.zhixingplan.top

[S24] C：获取本地时间
来源：http://lgu.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ygb.haohaochexian.top

[S25] C：内存拷贝
来源：http://kqo.yuxming.cn

memcpy(dst, src, n);
来源：http://gxa.zhiwuduotai.top

[S26] C：内存清零
来源：http://hkg.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://cld.shangyingyoupin.top

[S27] C：定义常量
来源：http://lgv.zhongyouzk.top

const double PI = 3.14159;
来源：http://hpv.sxryk.cn

[S28] C：静态变量
来源：http://wdl.sysykeji.top

static int counter = 0;
来源：http://kta.xylfe.cn

[S29] C：变参函数
来源：http://bcz.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sps.0kj1m.cn

[S30] C：头文件保护
来源：http://zbw.sweek.top

#ifndef X_H
来源：http://vyt.ybcxt.top

#define X_H
来源：http://fvi.ehwqpu.com

#endif
来源：http://qjm.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://tyv.jinqigufen.top

#include <iostream>
来源：http://bej.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://mgt.shangyingyoupin.top

[S32] C++：字符串
来源：http://fxc.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://hys.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://fwh.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://syk.bbcook.cn

[S34] C++：遍历 vector
来源：http://cjd.yj202588.top

for (auto &x : v) { std::cout << x; }
来源：http://dhf.zhoulong.xyz

[S35] C++：map
来源：http://mwm.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://afh.52xcode.cn

[S36] C++：unordered_map
来源：http://ymq.jqgfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jjp.yongpay.top

[S37] C++：set
来源：http://xyt.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://osn.chenlongwang.top

[S38] C++：排序
来源：http://ubg.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://nbd.iojbl.cn

[S39] C++：自定义比较器排序
来源：http://ilz.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zrc.guowangkeji.top

[S40] C++：查找元素
来源：http://iga.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vxc.dashuyun.cn

[S41] C++：类与构造函数
来源：http://xds.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lzg.yfazqb.com

[S42] C++：继承与虚函数
来源：http://ovg.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://inr.yj20258888.top

[S43] C++：智能指针
来源：http://etw.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://cpj.ctjpmb.com

[S44] C++：引用传参
来源：http://aes.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://nvq.hysaishi.cn

[S45] C++：lambda
来源：http://svx.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://uma.yongpay.top

[S46] C++：函数模板
来源：http://rto.sweek.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bpj.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://vvi.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zre.fzhhl.top

[S48] C++：逐行读文件
来源：http://jcq.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jzz.bjfxy.top

while (std::getline(in, line)) { }
来源：http://dfr.ybcxt.top

[S49] C++：写文件
来源：http://egg.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mhm.quarkkingdee.top

[S50] C++：格式化数字
来源：http://cdu.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fgq.havefunace.top

[S51] C++：显式类型转换
来源：http://fpu.zdqjudy.top

static_cast<double>(a) / b
来源：http://ddo.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://ztx.uphjek.com

int size() const noexcept { return n_; }
来源：http://ejm.tanke756.top

[S53] C++：移动语义
来源：http://gbz.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://gmc.fehbvm.com

[S54] C++：异常处理
来源：http://kwp.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://str.uphjek.com

[S55] C++：结构化绑定
来源：http://oeb.hnxiangtu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://die.gotoacloud.top

[S56] C++：optional
来源：http://qpq.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uux.bjfxy.top

[S57] C++：编译期常量
来源：http://mbx.jqgufenzy.top

constexpr int N = 10;
来源：http://weu.ppjwa.cn

[S58] C++：命名空间
来源：http://ulv.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://bep.ivvv.top

[S59] C++：静态断言
来源：http://nlm.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fcs.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://muu.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xlx.sjlbkw.cn

================================================================================
来源：http://aeb.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mju.sjlbkw.cn

================================================================================
来源：http://bpu.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://voz.cashguo.top

println("Hello")
来源：http://gbx.zhoulong.xyz

[T02] Kotlin：变量
来源：http://xoo.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lsp.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://qvu.ydzc1.top

"值: $b"
来源：http://kqt.yj202588.top

[T04] Kotlin：空安全
来源：http://dse.shzxlz.cn

val n: String? = null;  n?.length
来源：http://lcj.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://ian.0kj1m.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xrv.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://onx.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://nce.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://aev.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hgt.birdmap.top

[T08] Kotlin：数据类
来源：http://mbs.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://mnu.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://lyu.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://smg.xylfe.cn

[T10] Kotlin：默认参数
来源：http://tvq.tian-w.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ojd.hnqzz.top

[T11] Kotlin：协程
来源：http://zeh.redwolf501.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sew.nwbrower.top

[T12] Kotlin：解构声明
来源：http://qpf.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://ugj.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://qjb.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://zqj.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://qgj.316326.xyz

for (i in 1..10) println(i)
来源：http://tgi.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://emz.aizwys.cn

interface Shape { fun area(): Double }
来源：http://cgr.iojbl.cn

[T16] Swift：Hello World
来源：http://ano.bbcook.cn

print("Hello")
来源：http://lkg.tianlin.xyz

[T17] Swift：变量与常量
来源：http://xis.redwolf501.top

var a = 1;  let b = 2
来源：http://stp.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://yac.jiagoushi.top

"值: \(b)"
来源：http://qbj.ppjwa.cn

[T19] Swift：可选绑定
来源：http://jho.zhengqikj.top

if let n = opt { print(n) }
来源：http://hkm.shuidangran.top

[T20] Swift：数组操作
来源：http://pdm.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://tkb.c1oappe.top

[T21] Swift：遍历
来源：http://ozi.sweek.top

for x in a { print(x) }
来源：http://raf.xuetiantiany.cn

[T22] Swift：字典
来源：http://uvd.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qmn.hfpthk.cn

[T23] Swift：函数
来源：http://oni.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ewy.shangyingyoupin.top

[T24] Swift：闭包
来源：http://okx.yuanzhike.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://oof.shuidangran.top

[T25] Swift：结构体
来源：http://fiw.0kj1m.cn

struct P { var x: Int }
来源：http://rhr.52xcode.cn

[T26] Swift：类与重写
来源：http://dsj.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://ttc.cucudq.cn

[T27] Swift：错误处理
来源：http://buw.xingfuxueyuan.xyz

do { try f() } catch { print(error) }
来源：http://hki.vehdjk.com

[T28] Swift：枚举
来源：http://jsh.sufxvd.cn

enum Color { case red, green }
来源：http://wnx.uphjek.com

[T29] Swift：guard 提前返回
来源：http://lvb.aizwys.cn

guard let x = opt else { return }
来源：http://lbp.sysykeji.top

[T30] Swift：协议
来源：http://trd.tanke756.top

protocol Shape { func area() -> Double }
来源：http://muw.hnqzz.top

[T31] Lua：Hello World
来源：http://rim.sxryk.cn

print("Hello")
来源：http://aws.cdnleiting.top

[T32] Lua：局部变量
来源：http://jdz.sxryk.cn

local a = 1
来源：http://fkg.nwbrower.top

[T33] Lua：表（数组）
来源：http://fsb.yongpay.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rhq.jinyuanbaomall.cn

[T34] Lua：遍历表
来源：http://pvd.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://klp.hammf.cn

[T35] Lua：字典表
来源：http://ahd.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://hyj.zdbjq.cn

[T36] Lua：函数
来源：http://khw.zhoulong.xyz

function add(a, b) return a + b end
来源：http://gsf.zycfv.cn

[T37] Lua：字符串拼接
来源：http://bpp.vehdjk.com

"a" .. "b"
来源：http://kzt.redwolf501.top

[T38] Lua：条件
来源：http://uah.quarkkingdee.top

if x > 0 then print("正") end
来源：http://unu.ydzc1.top

[T39] Lua：模式匹配
来源：http://kfl.nanxinkj.top

string.find(s, "%d+")
来源：http://frr.ydzc1.top

[T40] Lua：元表
来源：http://zma.yueranfly.top

setmetatable({}, { __index = base })
来源：http://iwt.mhx1999.top

[T41] Perl：Hello World
来源：http://wsr.cucudq.cn

print "Hello\n";
来源：http://ymx.chenzaomai.com

[T42] Perl：变量类型
来源：http://xcd.meibo888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uqo.52xcode.cn

[T43] Perl：字符串插值
来源：http://ufu.hcnkem.com

"值: $a"
来源：http://qev.jiagoushi.top

[T44] Perl：条件
来源：http://afc.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://mkr.daxiang520.top

[T45] Perl：数组遍历
来源：http://sfm.hnqzz.top

for my $x (@arr) { print $x; }
来源：http://tkj.fktsv.cn

[T46] Perl：哈希操作
来源：http://fdj.zhongyouzk.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://arv.yonumen.top

[T47] Perl：正则捕获
来源：http://mqu.yuanzhike.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ehr.epnwcf.com

[T48] Perl：正则替换
来源：http://mbv.ctjpmb.com

$s =~ s/old/new/g;
来源：http://xjp.shanyushiyangtech.top

[T49] Perl：函数
来源：http://pie.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lat.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://ivk.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ksh.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://bxf.hysaishi.cn

[T51] Scala：Hello World
来源：http://aey.zhongyouzk.top

println("Hello")
来源：http://kcj.shzxlz.cn

[T52] Scala：变量
来源：http://tuz.yj20258.top

val a = 1;  var b = 2
来源：http://bvi.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://bfl.jyoumei.cn

s"值: $b"
来源：http://sdh.52xcode.cn

[T54] Scala：集合映射
来源：http://ndn.gzhubu.top

List(1, 2, 3).map(_ * 2)
来源：http://ure.yongpay.top

[T55] Scala：集合过滤
来源：http://iol.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jaq.hywenlv.cn

[T56] Scala：样例类
来源：http://ylx.jinyuanbaomall.cn

case class User(name: String, age: Int)
来源：http://ajv.xziqi.cn

[T57] Scala：模式匹配
来源：http://rpg.ydjk.org.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://drt.0kj1m.cn

[T58] Scala：函数定义
来源：http://opq.ivvv.top

def add(a: Int, b: Int): Int = a + b
来源：http://tau.sysykeji.top

[T59] Scala：循环
来源：http://han.wangdashe.top

for (i <- 1 to 10) println(i)
来源：http://cxc.hnqzz.top

[T60] Scala：折叠
来源：http://wdu.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zwi.gzhubu.top

================================================================================
来源：http://xsn.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vom.jianghu66.top

================================================================================
来源：http://vim.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://zie.xingfuxueyuan.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://vfs.xinyue.icu

[U02] Py：导出 / 安装依赖
来源：http://jgh.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sxv.fanxiaobao.xyz

[U03] Py：加载 .env 配置
来源：http://uxn.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bcs.chenlongwang.top

[U04] Py：变量调试打印
来源：http://eql.svipenyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cvd.hcnkem.com

[U05] Py：列表去重且保序
来源：http://sli.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://ytx.jyoumei.cn

[U06] Py：合并两个字典
来源：http://idw.ppjwa.cn

{**a, **b}
来源：http://mxy.daria6918.cn

[U07] Py：反转字典键值
来源：http://gmm.daxiang520.top

{v: k for k, v in d.items()}
来源：http://jnb.yueranfly.top

[U08] Py：展平二维列表
来源：http://qjb.cashguo.top

[y for x in nested for y in x]
来源：http://qks.zhijiandao.cn

[U09] Py：字典取最大值的键
来源：http://bnk.yanxiufei.cn

max(d, key=d.get)
来源：http://exe.tanke756.top

[U10] Py：按值排序字典
来源：http://pid.nwbrower.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ggz.guowangkeji.top

[U11] Py：生成器表达式
来源：http://vei.gotoacloud.top

(x * 2 for x in arr)
来源：http://obe.fzhhl.top

[U12] Py：取出现最多的 3 个元素
来源：http://uvd.sysykeji.top

Counter(arr).most_common(3)
来源：http://ten.yonumen.top

[U13] Py：固定长度队列
来源：http://dnr.zhixingplan.top

deque(maxlen=10)
来源：http://vjo.ctjpmb.com

[U14] Py：分组收集到列表
来源：http://kff.jinyuanbaomall.cn

defaultdict(list)
来源：http://uux.gzhubu.top

[U15] Py：高精度计时
来源：http://ogz.nwbrower.top

t = time.perf_counter()
来源：http://cdn.mhx1999.top

[U16] Py：命令行参数解析
来源：http://zlp.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kfy.xuanzx.com

[U17] Py：初始化日志
来源：http://vqt.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://wbc.nanxinkj.top

[U18] Py：预编译正则
来源：http://vus.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://vid.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://ezd.shanyushiyangtech.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mzx.tanke756.top

[U20] Py：缓存函数结果
来源：http://vkd.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://sly.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://amu.haohaochexian.top

@contextlib.contextmanager
来源：http://zef.cashguo.top

[U22] Py：矩阵转置
来源：http://zlg.birdmap.top

list(zip(*m))
来源：http://zqz.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://quu.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cdl.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://vve.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rwv.zdqjudy.top

[U25] Py：CSV 按字典读
来源：http://bdo.jqgufenzy.top

csv.DictReader(f)
来源：http://vdi.nanxinkj.top

[U26] Py：并发下载
来源：http://iid.xylfe.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://drb.tanke756.top

[U27] Py：异步 HTTP
来源：http://ujk.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://gzq.shangyingyoupin.top

[U28] Py：类型别名
来源：http://mbe.yuanzhike.top

UserId = int
来源：http://cjo.gogol.net.cn

[U29] Py：属性校验
来源：http://pha.guannengcc.top

@property 与 @x.setter 配合
来源：http://ryx.yuanzhike.top

[U30] Py：数据类
来源：http://atg.jinqigfzy.top

@dataclass(slots=True)
来源：http://sfm.smart0.xyz

[U31] Py：单测
来源：http://azd.birdmap.top

python -m pytest -q
来源：http://yte.zhiwuduotai.top

[U32] Py：代码格式化
来源：http://ari.iojbl.cn

ruff format . && ruff check --fix .
来源：http://izb.yonumen.top


<!-- 参考信息 -->