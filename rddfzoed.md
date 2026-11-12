代发 wailian999

strlen(s)
来源：http://prq.hfpthk.cn

[S06] C：字符串比较
来源：http://ymh.sjlbkw.cn

strcmp(a, b) == 0
来源：http://mfk.uphjek.com

[S07] C：数组遍历求和
来源：http://xfh.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gsa.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://qxi.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dbk.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://ujt.birdmap.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oai.uphjek.com

[S10] C：指针与解引用
来源：http://ysx.meibo888.top

int *p = &a;  *p = 5;
来源：http://qfa.ydjk.org.cn

[S11] C：逐行读文件
来源：http://okl.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://nwb.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ney.mhx1999.top

fclose(f);
来源：http://qxw.sjlbkw.cn

[S12] C：写文件
来源：http://xog.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://etl.shangyingyoupin.top

[S13] C：宏定义
来源：http://tvo.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zek.iojbl.cn

[S14] C：枚举
来源：http://igw.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://ery.sweek.top

[S15] C：类型转换
来源：http://plf.andypj.xyz

(double) a / b
来源：http://vuv.shuidangran.top

[S16] C：位操作置位
来源：http://vxw.pycfn.com

x |= (1 << 3);
来源：http://qcr.meibo888.top

[S17] C：安全拼接字符串
来源：http://oqs.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pfm.jiagoushi.top

[S18] C：命令行参数
来源：http://enw.zhengqikj.top

int main(int argc, char **argv)
来源：http://myv.hysaishi.cn

[S19] C：快速排序
来源：http://cld.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uob.zdqjudy.top

[S20] C：二分查找
来源：http://hvb.yfazqb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uur.jianghu66.top

[S21] C：字符类别判断
来源：http://fyc.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bnk.hammf.cn

[S22] C：字符串转数字
来源：http://zpy.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://tdw.svipenyu.cn

[S23] C：随机数
来源：http://dxd.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qwu.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://wss.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yft.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://nlj.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://zdc.52xcode.cn

[S26] C：内存清零
来源：http://tsb.c1oappe.top

memset(a, 0, sizeof a);
来源：http://lbq.yj20258.top

[S27] C：定义常量
来源：http://prn.yanxiufei.cn

const double PI = 3.14159;
来源：http://cth.0kj1m.cn

[S28] C：静态变量
来源：http://mzd.sjlbkw.cn

static int counter = 0;
来源：http://efq.xuanzx.com

[S29] C：变参函数
来源：http://nsd.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pzf.0kj1m.cn

[S30] C：头文件保护
来源：http://zpm.tanke756.top

#ifndef X_H
来源：http://ccm.chenlongwang.top

#define X_H
来源：http://cic.jinqigufen.top

#endif
来源：http://umn.xziqi.cn

[S31] C++：Hello World
来源：http://xty.ivvv.top

#include <iostream>
来源：http://oka.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://grc.hongshengwenyu.top

[S32] C++：字符串
来源：http://cox.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://vqe.daxiang520.top

[S33] C++：vector 增删
来源：http://ifc.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ran.pycfn.com

[S34] C++：遍历 vector
来源：http://pvx.meibo888.top

for (auto &x : v) { std::cout << x; }
来源：http://psq.jianghu66.top

[S35] C++：map
来源：http://qef.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wjj.zhiwuduotai.top

[S36] C++：unordered_map
来源：http://jqb.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rqm.zdbjq.cn

[S37] C++：set
来源：http://zbe.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mud.snrcjt.cn

[S38] C++：排序
来源：http://upv.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://pex.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://ham.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mfj.cdnleiting.top

[S40] C++：查找元素
来源：http://xgk.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fvc.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://cag.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://msg.gzhubu.top

[S42] C++：继承与虚函数
来源：http://ihx.fehbvm.com

class B : public Base { public: void f() override {} };
来源：http://fuv.dashuyun.cn

[S43] C++：智能指针
来源：http://xun.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://zjc.yj202588.top

[S44] C++：引用传参
来源：http://yuw.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://lxr.zhengqikj.top

[S45] C++：lambda
来源：http://gca.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://efg.iojbl.cn

[S46] C++：函数模板
来源：http://iuo.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qta.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://sgj.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qjo.meibo888.top

[S48] C++：逐行读文件
来源：http://vep.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://ghc.tian-w.cn

while (std::getline(in, line)) { }
来源：http://ijj.aizwys.cn

[S49] C++：写文件
来源：http://rrf.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gqj.meibo888.top

[S50] C++：格式化数字
来源：http://wup.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://glm.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://bzr.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://rgt.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://iqh.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://fgp.xingfuxueyuan.xyz

[S53] C++：移动语义
来源：http://uha.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://jah.yuanzhike.top

[S54] C++：异常处理
来源：http://xft.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zkh.cucudq.cn

[S55] C++：结构化绑定
来源：http://yym.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://udm.ydzc1.top

[S56] C++：optional
来源：http://ntk.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ikm.tanke756.top

[S57] C++：编译期常量
来源：http://ceg.ivvv.top

constexpr int N = 10;
来源：http://qnl.zdbjq.cn

[S58] C++：命名空间
来源：http://akl.316326.xyz

namespace ns { int f() { return 1; } }
来源：http://ggv.jiagoushi.top

[S59] C++：静态断言
来源：http://bbe.sxryk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kzs.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://asa.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nib.sysykeji.top

================================================================================
来源：http://wmt.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jzp.cashguo.top

================================================================================
来源：http://jqp.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://bce.daxiang520.top

println("Hello")
来源：http://dpd.52xcode.cn

[T02] Kotlin：变量
来源：http://yvw.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xhr.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://wxe.cashguo.top

"值: $b"
来源：http://ymi.cdnleiting.top

[T04] Kotlin：空安全
来源：http://axm.gotoacloud.top

val n: String? = null;  n?.length
来源：http://nxf.vehdjk.com

[T05] Kotlin：when 表达式
来源：http://ygz.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://efa.hesvh.cn

[T06] Kotlin：集合映射
来源：http://zzj.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gvu.hnxiangtu.top

[T07] Kotlin：集合过滤
来源：http://nkp.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://max.svipenyu.cn

[T08] Kotlin：数据类
来源：http://mlz.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://bfx.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://pzd.zhijiandao.cn

fun String.exclaim() = this + "!"
来源：http://ibg.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://jof.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lxi.sysykeji.top

[T11] Kotlin：协程
来源：http://ljd.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xax.ybcxt.top

[T12] Kotlin：解构声明
来源：http://xtp.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://uwg.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://qgf.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://sdk.ppjwa.cn

[T14] Kotlin：循环
来源：http://fkf.hysaishi.cn

for (i in 1..10) println(i)
来源：http://uwi.xuanzx.com

[T15] Kotlin：接口
来源：http://eiu.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://nbz.mhx1999.top

[T16] Swift：Hello World
来源：http://iis.cdnleiting.top

print("Hello")
来源：http://wpd.hcnkem.com

[T17] Swift：变量与常量
来源：http://ade.c1oappe.top

var a = 1;  let b = 2
来源：http://eih.yuanzhike.top

[T18] Swift：字符串插值
来源：http://ieb.yanxiufei.cn

"值: \(b)"
来源：http://qgc.gogol.net.cn

[T19] Swift：可选绑定
来源：http://han.9152youxi.cn

if let n = opt { print(n) }
来源：http://maz.cdnleiting.top

[T20] Swift：数组操作
来源：http://ioh.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://ojp.chenzaomai.com

[T21] Swift：遍历
来源：http://wuu.bjfxy.top

for x in a { print(x) }
来源：http://pda.cdnleiting.top

[T22] Swift：字典
来源：http://blr.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://pvc.tanke756.top

[T23] Swift：函数
来源：http://wox.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hnp.hongshengwenyu.top

[T24] Swift：闭包
来源：http://ldc.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kot.ctjpmb.com

[T25] Swift：结构体
来源：http://nri.fengsongda.top

struct P { var x: Int }
来源：http://mew.zhijiandao.cn

[T26] Swift：类与重写
来源：http://ohs.jinqigfzy.top

class A: Base { override func f() {} }
来源：http://wko.aibaodan.cn

[T27] Swift：错误处理
来源：http://fpu.daria6918.cn

do { try f() } catch { print(error) }
来源：http://llp.pycfn.com

[T28] Swift：枚举
来源：http://qig.sjlbkw.cn

enum Color { case red, green }
来源：http://gno.zhijiandao.cn

[T29] Swift：guard 提前返回
来源：http://gdm.ppjwa.cn

guard let x = opt else { return }
来源：http://gjm.gaohongyu789.top

[T30] Swift：协议
来源：http://hbz.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://pdt.316326.xyz

[T31] Lua：Hello World
来源：http://huf.uphjek.com

print("Hello")
来源：http://zrm.gotoacloud.top

[T32] Lua：局部变量
来源：http://bjd.fzhhl.top

local a = 1
来源：http://mcj.sufxvd.cn

[T33] Lua：表（数组）
来源：http://iyb.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vej.sweek.top

[T34] Lua：遍历表
来源：http://lzl.hywenlv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://foz.bbcook.cn

[T35] Lua：字典表
来源：http://muv.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://off.hongshengwenyu.top

[T36] Lua：函数
来源：http://fef.gotoacloud.top

function add(a, b) return a + b end
来源：http://cgb.sweek.top

[T37] Lua：字符串拼接
来源：http://lsj.cheryme.top

"a" .. "b"
来源：http://pbb.ydjk.org.cn

[T38] Lua：条件
来源：http://kkv.aibaodan.cn

if x > 0 then print("正") end
来源：http://tef.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://neu.cashguo.top

string.find(s, "%d+")
来源：http://zyw.hcnkem.com

[T40] Lua：元表
来源：http://gel.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://yto.hfpthk.cn

[T41] Perl：Hello World
来源：http://mkz.jinqigufen.top

print "Hello\n";
来源：http://wcw.ybcxt.top

[T42] Perl：变量类型
来源：http://gpo.vehdjk.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fdo.tian-w.cn

[T43] Perl：字符串插值
来源：http://kfj.aibaodan.cn

"值: $a"
来源：http://zno.yanxiufei.cn

[T44] Perl：条件
来源：http://hic.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://xgn.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://ojr.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://bqv.chenlongwang.top

[T46] Perl：哈希操作
来源：http://tsb.52xcode.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aqg.kuanghao11.cn

[T47] Perl：正则捕获
来源：http://ixr.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://krh.ehwqpu.com

[T48] Perl：正则替换
来源：http://spp.zhixingplan.top

$s =~ s/old/new/g;
来源：http://lzk.jinqigufen.top

[T49] Perl：函数
来源：http://kwd.zhijiandao.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://flg.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://rxp.yanxiufei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://afy.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://acl.dianchejie.cn

[T51] Scala：Hello World
来源：http://xru.nanxinkj.top

println("Hello")
来源：http://vhu.meibo888.top

[T52] Scala：变量
来源：http://wtq.fehbvm.com

val a = 1;  var b = 2
来源：http://zwa.zdqjudy.top

[T53] Scala：字符串插值
来源：http://iws.sysykeji.top

s"值: $b"
来源：http://lck.chenzaomai.com

[T54] Scala：集合映射
来源：http://vle.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://ecw.shanyushiyangkeji.top

[T55] Scala：集合过滤
来源：http://sko.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://mjq.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://txc.epnwcf.com

case class User(name: String, age: Int)
来源：http://vqu.vehdjk.com

[T57] Scala：模式匹配
来源：http://jpv.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fmr.cqqwz.cn

[T58] Scala：函数定义
来源：http://mrh.hcnkem.com

def add(a: Int, b: Int): Int = a + b
来源：http://xfw.zhongyouzk.top

[T59] Scala：循环
来源：http://kde.epnwcf.com

for (i <- 1 to 10) println(i)
来源：http://bqx.tarul.cn

[T60] Scala：折叠
来源：http://imm.fengsongda.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qbg.ydjk.org.cn

================================================================================
来源：http://rbe.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tkp.hnqzz.top

================================================================================
来源：http://pcd.gogol.net.cn

[U01] Py：创建虚拟环境
来源：http://hkn.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nme.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://nxy.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hhp.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://dzq.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://bcz.yuxming.cn

[U04] Py：变量调试打印
来源：http://vpa.ctjpmb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sot.feifeiyinyue.top

[U05] Py：列表去重且保序
来源：http://wdu.havefunace.top

list(dict.fromkeys(arr))
来源：http://ywu.yj20258888.top

[U06] Py：合并两个字典
来源：http://ndp.yueranfly.top

{**a, **b}
来源：http://jrs.daria6918.cn

[U07] Py：反转字典键值
来源：http://dcv.smart0.xyz

{v: k for k, v in d.items()}
来源：http://zom.havefunace.top

[U08] Py：展平二维列表
来源：http://ohi.sjlbkw.cn

[y for x in nested for y in x]
来源：http://kgs.cheryme.top

[U09] Py：字典取最大值的键
来源：http://imm.shzxlz.cn

max(d, key=d.get)
来源：http://qds.ppjwa.cn

[U10] Py：按值排序字典
来源：http://vti.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kxh.nanxinkj.top

[U11] Py：生成器表达式
来源：http://jxs.yj20258.top

(x * 2 for x in arr)
来源：http://lga.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://pmg.hysaishi.cn

Counter(arr).most_common(3)
来源：http://cez.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://jvx.ctjpmb.com

deque(maxlen=10)
来源：http://joc.epnwcf.com

[U14] Py：分组收集到列表
来源：http://drh.xinyue.icu

defaultdict(list)
来源：http://yqh.aizwys.cn

[U15] Py：高精度计时
来源：http://waf.andypj.xyz

t = time.perf_counter()
来源：http://knn.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://zbb.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fhx.tanke756.top

[U17] Py：初始化日志
来源：http://dom.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://kwt.sjlbkw.cn

[U18] Py：预编译正则
来源：http://iba.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://cbf.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://jow.quarkkingdee.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pty.ydzc1.top

[U20] Py：缓存函数结果
来源：http://zig.wangdashe.top

@functools.lru_cache(maxsize=None)
来源：http://spg.sweek.top

[U21] Py：自定义上下文管理器
来源：http://elk.birdmap.top

@contextlib.contextmanager
来源：http://tno.nwbrower.top

[U22] Py：矩阵转置
来源：http://klv.jqgufenzy.top

list(zip(*m))
来源：http://kmg.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://cau.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kbq.zdbjq.cn

[U24] Py：路径操作
来源：http://yee.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yxt.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://clz.pycfn.com

csv.DictReader(f)
来源：http://ldf.feifeiyinyue.top

[U26] Py：并发下载
来源：http://ibp.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cub.yongpay.top

[U27] Py：异步 HTTP
来源：http://vgj.feifeiyinyue.top

aiohttp.ClientSession() 配合 async with
来源：http://tvf.ydzc1.top

[U28] Py：类型别名
来源：http://tgg.xuetiantiany.cn

UserId = int
来源：http://nko.guannengcc.top


<!-- 参考信息 -->