代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://wso.shangyingyoupin.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rsv.wangdashe.top

fclose(f);
来源：http://dzz.xuetiantiany.cn

[S12] C：写文件
来源：http://jqx.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sgn.bbcook.cn

[S13] C：宏定义
来源：http://srx.cucudq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://flp.chenjidiqi.icu

[S14] C：枚举
来源：http://dsk.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://ulr.sxryk.cn

[S15] C：类型转换
来源：http://ipx.jianghu66.top

(double) a / b
来源：http://ojr.zdbjq.cn

[S16] C：位操作置位
来源：http://lwk.shuidangran.top

x |= (1 << 3);
来源：http://pus.shuidangran.top

[S17] C：安全拼接字符串
来源：http://bmp.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://waa.zhoulong.xyz

[S18] C：命令行参数
来源：http://jrb.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://dxq.jqgufenzy.top

[S19] C：快速排序
来源：http://jrm.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://isi.shanyushiyangtech.top

[S20] C：二分查找
来源：http://xwo.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pwg.hfpthk.cn

[S21] C：字符类别判断
来源：http://ynn.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xxi.havefunace.top

[S22] C：字符串转数字
来源：http://lbl.9152youxi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zcp.quarkkingdee.top

[S23] C：随机数
来源：http://pay.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vyr.jqgfzy.top

[S24] C：获取本地时间
来源：http://qrx.hcnkem.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mik.jianghu66.top

[S25] C：内存拷贝
来源：http://qhl.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://gkl.zhijiandao.cn

[S26] C：内存清零
来源：http://jia.hcnkem.com

memset(a, 0, sizeof a);
来源：http://vkw.jlsjyb.cn

[S27] C：定义常量
来源：http://exb.yj20258888.top

const double PI = 3.14159;
来源：http://gsw.shangyingyoupin.top

[S28] C：静态变量
来源：http://fju.fengsongda.top

static int counter = 0;
来源：http://xuf.dashuyun.cn

[S29] C：变参函数
来源：http://mmv.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://syp.nanxinkj.top

[S30] C：头文件保护
来源：http://vou.fehbvm.com

#ifndef X_H
来源：http://ftl.aibaodan.cn

#define X_H
来源：http://qkt.jlsjyb.cn

#endif
来源：http://gir.xuanzx.com

[S31] C++：Hello World
来源：http://svm.ybcxt.top

#include <iostream>
来源：http://yhx.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://xzu.yuanzhike.top

[S32] C++：字符串
来源：http://vpf.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://asj.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://vzf.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://unu.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://yfb.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://csh.gotoacloud.top

[S35] C++：map
来源：http://zgf.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gpf.0kj1m.cn

[S36] C++：unordered_map
来源：http://ufw.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://psy.xinyue.icu

[S37] C++：set
来源：http://vlu.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://abl.hfpthk.cn

[S38] C++：排序
来源：http://obq.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://aue.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://ujx.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ozh.wangdashe.top

[S40] C++：查找元素
来源：http://yhh.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qig.smart0.xyz

[S41] C++：类与构造函数
来源：http://pwh.zhixingplan.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zjy.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://cou.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://khl.chenlongwang.top

[S43] C++：智能指针
来源：http://fyn.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://hfx.redwolf501.top

[S44] C++：引用传参
来源：http://vrq.zhijiandao.cn

void inc(int &x) { ++x; }
来源：http://pkr.52xcode.cn

[S45] C++：lambda
来源：http://pae.cashguo.top

auto add = [](int a, int b) { return a + b; };
来源：http://hgb.hammf.cn

[S46] C++：函数模板
来源：http://qnx.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mww.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://imi.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xgu.haohaochexian.top

[S48] C++：逐行读文件
来源：http://xwz.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://taa.fengsongda.top

while (std::getline(in, line)) { }
来源：http://okz.xylfe.cn

[S49] C++：写文件
来源：http://ssq.iojbl.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://btr.hammf.cn

[S50] C++：格式化数字
来源：http://qvb.yongpay.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://odt.chenlongwang.top

[S51] C++：显式类型转换
来源：http://cop.52xcode.cn

static_cast<double>(a) / b
来源：http://slb.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://euq.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://oma.zdqjudy.top

[S53] C++：移动语义
来源：http://zxc.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://xcz.ppjwa.cn

[S54] C++：异常处理
来源：http://qpb.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mtx.zhengqikj.top

[S55] C++：结构化绑定
来源：http://azf.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ozi.ywan-chungtsiang.top

[S56] C++：optional
来源：http://avy.bjfxy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mww.ydzc1.top

[S57] C++：编译期常量
来源：http://roh.yanxiufei.cn

constexpr int N = 10;
来源：http://hwv.nanxinkj.top

[S58] C++：命名空间
来源：http://ypt.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://tsp.haohaochexian.top

[S59] C++：静态断言
来源：http://bye.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lck.yueranfly.top

[S60] C++：遍历并删除元素
来源：http://chr.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eqi.hcnkem.com

================================================================================
来源：http://hlb.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rnk.xingfuxueyuan.xyz

================================================================================
来源：http://wrq.ivvv.top

[T01] Kotlin：Hello World
来源：http://xea.hesvh.cn

println("Hello")
来源：http://bvk.snrcjt.cn

[T02] Kotlin：变量
来源：http://ppw.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ydo.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://kvc.mhx1999.top

"值: $b"
来源：http://xdt.ctjpmb.com

[T04] Kotlin：空安全
来源：http://fot.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://ltd.tarul.cn

[T05] Kotlin：when 表达式
来源：http://tpi.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xbn.cdnleiting.top

[T06] Kotlin：集合映射
来源：http://wdm.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qxm.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://usi.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tjh.fehbvm.com

[T08] Kotlin：数据类
来源：http://rbd.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://olq.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://phy.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://oda.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://fba.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tow.fzhhl.top

[T11] Kotlin：协程
来源：http://uys.feifeiyinyue.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bkg.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://mds.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://vqe.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://nok.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://uua.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://hpd.fktsv.cn

for (i in 1..10) println(i)
来源：http://iev.zdbjq.cn

[T15] Kotlin：接口
来源：http://vsg.316326.xyz

interface Shape { fun area(): Double }
来源：http://jhg.nwbrower.top

[T16] Swift：Hello World
来源：http://kgx.ydjk.org.cn

print("Hello")
来源：http://zrh.sufxvd.cn

[T17] Swift：变量与常量
来源：http://xig.yj20258888.top

var a = 1;  let b = 2
来源：http://vxg.jqgufenzy.top

[T18] Swift：字符串插值
来源：http://mel.tian-w.cn

"值: \(b)"
来源：http://hqs.ppjwa.cn

[T19] Swift：可选绑定
来源：http://ylk.havefunace.top

if let n = opt { print(n) }
来源：http://wjv.jinqigfzy.top

[T20] Swift：数组操作
来源：http://xfl.dashuyun.cn

var a = [1, 2, 3];  a.append(4)
来源：http://svc.ppjwa.cn

[T21] Swift：遍历
来源：http://axr.zhijiandao.cn

for x in a { print(x) }
来源：http://fiu.cqqwz.cn

[T22] Swift：字典
来源：http://jfh.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dax.c1oappe.top

[T23] Swift：函数
来源：http://pqr.quarkkingdee.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wet.sysykeji.top

[T24] Swift：闭包
来源：http://pdf.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cnm.yueranfly.top

[T25] Swift：结构体
来源：http://aqs.jianghu66.top

struct P { var x: Int }
来源：http://fmr.tianlin.xyz

[T26] Swift：类与重写
来源：http://byp.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://bhf.yuxming.cn

[T27] Swift：错误处理
来源：http://kea.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://rpg.yj20258888.top

[T28] Swift：枚举
来源：http://gru.pycfn.com

enum Color { case red, green }
来源：http://gtq.ivvv.top

[T29] Swift：guard 提前返回
来源：http://wbq.c1oappe.top

guard let x = opt else { return }
来源：http://bcf.sjlbkw.cn

[T30] Swift：协议
来源：http://fck.shanyushiyangtech.top

protocol Shape { func area() -> Double }
来源：http://wdf.cucudq.cn

[T31] Lua：Hello World
来源：http://owy.hcnkem.com

print("Hello")
来源：http://otw.hnxiangtu.top

[T32] Lua：局部变量
来源：http://mbr.cdnleiting.top

local a = 1
来源：http://khn.ydzc1.top

[T33] Lua：表（数组）
来源：http://gpv.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jfn.tarul.cn

[T34] Lua：遍历表
来源：http://ujp.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://erd.cashguo.top

[T35] Lua：字典表
来源：http://qis.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://wap.yongpay.top

[T36] Lua：函数
来源：http://jzg.birdmap.top

function add(a, b) return a + b end
来源：http://hfs.cheryme.top

[T37] Lua：字符串拼接
来源：http://smt.jqgfzy.top

"a" .. "b"
来源：http://ksf.guowangkeji.top

[T38] Lua：条件
来源：http://rrd.pengpengdd.cyou

if x > 0 then print("正") end
来源：http://xsu.zhengqikj.top

[T39] Lua：模式匹配
来源：http://sro.yuanzhike.top

string.find(s, "%d+")
来源：http://dhr.xinyue.icu

[T40] Lua：元表
来源：http://ctg.yangfankeji.com

setmetatable({}, { __index = base })
来源：http://vgy.nanxinkj.top

[T41] Perl：Hello World
来源：http://bda.xuetiantiany.cn

print "Hello\n";
来源：http://vqo.zycfv.cn

[T42] Perl：变量类型
来源：http://con.guowangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pbw.aibaodan.cn

[T43] Perl：字符串插值
来源：http://wer.uphjek.com

"值: $a"
来源：http://olv.birdmap.top

[T44] Perl：条件
来源：http://sri.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://jta.52xcode.cn

[T45] Perl：数组遍历
来源：http://bdp.ppjwa.cn

for my $x (@arr) { print $x; }
来源：http://all.aibaodan.cn

[T46] Perl：哈希操作
来源：http://rge.vqdsnc.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://khm.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://brv.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cdd.fzhhl.top

[T48] Perl：正则替换
来源：http://jos.yj20258888.top

$s =~ s/old/new/g;
来源：http://hge.ybcxt.top

[T49] Perl：函数
来源：http://gsr.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iiv.redwolf501.top

[T50] Perl：逐行读文件
来源：http://vpc.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://iix.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://svb.cdnleiting.top

[T51] Scala：Hello World
来源：http://dav.svipenyu.cn

println("Hello")
来源：http://qcq.316326.xyz

[T52] Scala：变量
来源：http://awi.birdmap.top

val a = 1;  var b = 2
来源：http://rml.cheryme.top

[T53] Scala：字符串插值
来源：http://bpt.hfpthk.cn

s"值: $b"
来源：http://omd.hywenlv.cn

[T54] Scala：集合映射
来源：http://pwn.cheryme.top

List(1, 2, 3).map(_ * 2)
来源：http://wza.gzhubu.top

[T55] Scala：集合过滤
来源：http://ynz.zhongyouzk.top

List(1, 2, 3).filter(_ > 1)
来源：http://hya.tian-w.cn

[T56] Scala：样例类
来源：http://pfc.cdnleiting.top

case class User(name: String, age: Int)
来源：http://ili.tanke756.top

[T57] Scala：模式匹配
来源：http://qlw.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kys.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://zgf.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://mhm.vqdsnc.cn

[T59] Scala：循环
来源：http://lfs.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://ygo.316326.xyz

[T60] Scala：折叠
来源：http://twj.daria6918.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ziz.sufxvd.cn

================================================================================
来源：http://pgz.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ibv.jinqigufen.top

================================================================================
来源：http://ubu.zhongyouzk.top

[U01] Py：创建虚拟环境
来源：http://ppm.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uji.meibo888.top

[U02] Py：导出 / 安装依赖
来源：http://ohv.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://plt.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://wei.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eak.jianghu66.top

[U04] Py：变量调试打印
来源：http://jhw.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zou.kuanghao11.cn

[U05] Py：列表去重且保序
来源：http://swk.xylfe.cn

list(dict.fromkeys(arr))
来源：http://udb.tian-w.cn

[U06] Py：合并两个字典
来源：http://vhw.zhaomingkeji.xyz

{**a, **b}
来源：http://joj.meibo888.top

[U07] Py：反转字典键值
来源：http://wbt.cucudq.cn

{v: k for k, v in d.items()}
来源：http://omn.sweek.top

[U08] Py：展平二维列表
来源：http://yan.havefunace.top

[y for x in nested for y in x]
来源：http://coy.ydzc1.top

[U09] Py：字典取最大值的键
来源：http://lia.zdbjq.cn

max(d, key=d.get)
来源：http://rei.gogol.net.cn

[U10] Py：按值排序字典
来源：http://rcf.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://grg.yueranfly.top

[U11] Py：生成器表达式
来源：http://sdg.jianghu66.top

(x * 2 for x in arr)
来源：http://cus.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://ykw.yueranfly.top

Counter(arr).most_common(3)
来源：http://fpe.jinqigufen.top

[U13] Py：固定长度队列
来源：http://tbx.nwbrower.top

deque(maxlen=10)
来源：http://fqy.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://hgt.guowangkeji.top

defaultdict(list)
来源：http://qnh.gogol.net.cn

[U15] Py：高精度计时
来源：http://tnm.yueranfly.top

t = time.perf_counter()
来源：http://rnr.fehbvm.com

[U16] Py：命令行参数解析
来源：http://ina.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bkr.ydzc1.top

[U17] Py：初始化日志
来源：http://fsw.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://edi.chenlongwang.top

[U18] Py：预编译正则
来源：http://aqm.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://rxu.xuanzx.com

[U19] Py：正则替换带回调
来源：http://kfl.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fur.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://rme.sysykeji.top

@functools.lru_cache(maxsize=None)
来源：http://bce.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://vni.vehdjk.com

@contextlib.contextmanager
来源：http://eur.9152youxi.cn

[U22] Py：矩阵转置
来源：http://ndf.zhijiandao.cn

list(zip(*m))
来源：http://ffe.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://lnh.fzhhl.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wkr.chenzaomai.com

[U24] Py：路径操作
来源：http://ikh.fehbvm.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://efa.hywenlv.cn

[U25] Py：CSV 按字典读
来源：http://flr.yj20258.top

csv.DictReader(f)
来源：http://coe.kuanghao11.cn

[U26] Py：并发下载
来源：http://aww.zhixingplan.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uvq.yueranfly.top

[U27] Py：异步 HTTP
来源：http://rgr.ctjpmb.com

aiohttp.ClientSession() 配合 async with
来源：http://lkh.vehdjk.com

[U28] Py：类型别名
来源：http://lzr.pycfn.com

UserId = int
来源：http://qyt.jinqigufen.top

[U29] Py：属性校验
来源：http://lvp.xinyue.icu

@property 与 @x.setter 配合
来源：http://pyx.jiagoushi.top

[U30] Py：数据类
来源：http://edp.hysaishi.cn

@dataclass(slots=True)
来源：http://iou.0kj1m.cn

[U31] Py：单测
来源：http://jfm.jqgufenzy.top

python -m pytest -q
来源：http://txr.jianghu66.top

[U32] Py：代码格式化
来源：http://wau.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://dxp.pengpengdd.cyou

[U33] Py：打包发布
来源：http://qpg.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://srm.yj20258888.top

[U34] Py：判断编码
来源：http://mrx.zdqjudy.top

chardet.detect(raw)
来源：http://vjs.ivvv.top


<!-- 参考信息 -->