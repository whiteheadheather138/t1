代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kay.snrcjt.cn

[S08] C：动态内存分配与释放
来源：http://bmg.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gmv.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://oze.gzhubu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jzr.zdbjq.cn

[S10] C：指针与解引用
来源：http://tgt.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://brx.chenzaomai.com

[S11] C：逐行读文件
来源：http://gua.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://ese.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tlw.hongshengwenyu.top

fclose(f);
来源：http://dga.ywan-chungtsiang.top

[S12] C：写文件
来源：http://kjg.jinghuilouyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://igb.guowangkeji.top

[S13] C：宏定义
来源：http://ckj.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nws.birdmap.top

[S14] C：枚举
来源：http://obo.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://pxb.dianchejie.cn

[S15] C：类型转换
来源：http://ogq.cdnleiting.top

(double) a / b
来源：http://zsn.xylfe.cn

[S16] C：位操作置位
来源：http://wev.birdmap.top

x |= (1 << 3);
来源：http://iwc.meibo888.top

[S17] C：安全拼接字符串
来源：http://vvt.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fmb.sysykeji.top

[S18] C：命令行参数
来源：http://jqx.tianlin.xyz

int main(int argc, char **argv)
来源：http://ohm.xuanzx.com

[S19] C：快速排序
来源：http://efi.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ltk.hysaishi.cn

[S20] C：二分查找
来源：http://qux.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jez.jqgfzy.top

[S21] C：字符类别判断
来源：http://yhs.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aid.hesvh.cn

[S22] C：字符串转数字
来源：http://eea.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://xwk.316326.xyz

[S23] C：随机数
来源：http://uwp.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cyg.kuanghao11.cn

[S24] C：获取本地时间
来源：http://xoa.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dsz.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://egg.fzhhl.top

memcpy(dst, src, n);
来源：http://img.epnwcf.com

[S26] C：内存清零
来源：http://sbb.jianghu66.top

memset(a, 0, sizeof a);
来源：http://sor.jyoumei.cn

[S27] C：定义常量
来源：http://xru.jiagoushi.top

const double PI = 3.14159;
来源：http://kbf.nwbrower.top

[S28] C：静态变量
来源：http://olz.hysaishi.cn

static int counter = 0;
来源：http://rfc.hesvh.cn

[S29] C：变参函数
来源：http://rfy.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dlr.zhoulong.xyz

[S30] C：头文件保护
来源：http://wbv.shangyingyoupin.top

#ifndef X_H
来源：http://pzy.ydzc1.top

#define X_H
来源：http://hdz.yueranfly.top

#endif
来源：http://iuu.aizwys.cn

[S31] C++：Hello World
来源：http://uat.sufxvd.cn

#include <iostream>
来源：http://pzk.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://fah.c1oappe.top

[S32] C++：字符串
来源：http://ucx.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://dpe.shzxlz.cn

[S33] C++：vector 增删
来源：http://qce.shuidangran.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zti.dashuyun.cn

[S34] C++：遍历 vector
来源：http://aox.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://ceq.xuanzx.com

[S35] C++：map
来源：http://gmb.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://chm.zhoulong.xyz

[S36] C++：unordered_map
来源：http://ulb.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tpo.haohaochexian.top

[S37] C++：set
来源：http://pte.feifeiyinyue.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qhj.hnqzz.top

[S38] C++：排序
来源：http://cxo.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://ezc.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://svx.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yhs.guannengcc.top

[S40] C++：查找元素
来源：http://rzj.vqdsnc.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ggg.cucudq.cn

[S41] C++：类与构造函数
来源：http://nog.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gok.guowangkeji.top

[S42] C++：继承与虚函数
来源：http://pil.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://ybq.jianghu66.top

[S43] C++：智能指针
来源：http://hmd.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://dto.gotoacloud.top

[S44] C++：引用传参
来源：http://ljb.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://zbn.0kj1m.cn

[S45] C++：lambda
来源：http://wvi.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pya.hongshengwenyu.top

[S46] C++：函数模板
来源：http://fan.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yyr.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://qgz.haohaochexian.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zsb.dashuyun.cn

[S48] C++：逐行读文件
来源：http://suq.ctjpmb.com

std::ifstream in("a.txt");  std::string line;
来源：http://gdf.zhengqikj.top

while (std::getline(in, line)) { }
来源：http://avp.nwbrower.top

[S49] C++：写文件
来源：http://prn.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xrs.tarul.cn

[S50] C++：格式化数字
来源：http://pdd.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tzr.zdbjq.cn

[S51] C++：显式类型转换
来源：http://bhi.hnxiangtu.top

static_cast<double>(a) / b
来源：http://njl.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://pek.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://hte.yj20258.top

[S53] C++：移动语义
来源：http://qhk.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://csz.fehbvm.com

[S54] C++：异常处理
来源：http://lkm.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zki.yuanzhike.top

[S55] C++：结构化绑定
来源：http://esx.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://syc.fktsv.cn

[S56] C++：optional
来源：http://dbs.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vlg.jiagoushi.top

[S57] C++：编译期常量
来源：http://rrg.0kj1m.cn

constexpr int N = 10;
来源：http://zqy.sweek.top

[S58] C++：命名空间
来源：http://zmy.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://mss.jqgfzy.top

[S59] C++：静态断言
来源：http://cir.hongshengwenyu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gqm.meibo888.top

[S60] C++：遍历并删除元素
来源：http://ldz.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dxd.hywenlv.cn

================================================================================
来源：http://zpu.ybcxt.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tsc.dianchejie.cn

================================================================================
来源：http://hnt.hammf.cn

[T01] Kotlin：Hello World
来源：http://mks.yuanzhike.top

println("Hello")
来源：http://bsc.c1oappe.top

[T02] Kotlin：变量
来源：http://jpb.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vfw.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://nfy.jqgufenzy.top

"值: $b"
来源：http://opl.tanke756.top

[T04] Kotlin：空安全
来源：http://rmf.jqgfzy.top

val n: String? = null;  n?.length
来源：http://mim.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://dxj.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uba.andypj.xyz

[T06] Kotlin：集合映射
来源：http://jhc.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uxc.jiagoushi.top

[T07] Kotlin：集合过滤
来源：http://xlb.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://uhc.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://kcx.yongpay.top

data class User(val name: String, val age: Int)
来源：http://wqb.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://gek.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://bnj.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://ucn.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://lse.cashguo.top

[T11] Kotlin：协程
来源：http://upc.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://avx.fehbvm.com

[T12] Kotlin：解构声明
来源：http://owt.yongpay.top

val (a, b) = Pair(1, 2)
来源：http://icg.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://yta.fengsongda.top

val m = mapOf("a" to 1)
来源：http://qim.quarkkingdee.top

[T14] Kotlin：循环
来源：http://ton.shzxlz.cn

for (i in 1..10) println(i)
来源：http://cky.shuidangran.top

[T15] Kotlin：接口
来源：http://rtm.ydjk.org.cn

interface Shape { fun area(): Double }
来源：http://wcl.hnxiangtu.top

[T16] Swift：Hello World
来源：http://gzq.zhijiandao.cn

print("Hello")
来源：http://ekj.jianghu66.top

[T17] Swift：变量与常量
来源：http://ygj.cashguo.top

var a = 1;  let b = 2
来源：http://yde.xuanzx.com

[T18] Swift：字符串插值
来源：http://tem.hongshengwenyu.top

"值: \(b)"
来源：http://xrm.zdbjq.cn

[T19] Swift：可选绑定
来源：http://wnb.quarkkingdee.top

if let n = opt { print(n) }
来源：http://wzk.tian-w.cn

[T20] Swift：数组操作
来源：http://slc.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://wro.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://ooz.9152youxi.cn

for x in a { print(x) }
来源：http://qcy.uphjek.com

[T22] Swift：字典
来源：http://zny.andypj.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://zfx.gzhubu.top

[T23] Swift：函数
来源：http://umu.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kca.yuxming.cn

[T24] Swift：闭包
来源：http://oaa.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ovr.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://cvn.yvedp.cn

struct P { var x: Int }
来源：http://seq.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://ect.jinqigfzy.top

class A: Base { override func f() {} }
来源：http://cte.cqqwz.cn

[T27] Swift：错误处理
来源：http://mya.tarul.cn

do { try f() } catch { print(error) }
来源：http://hfq.yuanzhike.top

[T28] Swift：枚举
来源：http://jww.ehwqpu.com

enum Color { case red, green }
来源：http://dhg.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://zxb.zhiwuduotai.top

guard let x = opt else { return }
来源：http://cae.smart0.xyz

[T30] Swift：协议
来源：http://bye.pycfn.com

protocol Shape { func area() -> Double }
来源：http://ouq.zhiwuduotai.top

[T31] Lua：Hello World
来源：http://oeo.snrcjt.cn

print("Hello")
来源：http://can.zhoulong.xyz

[T32] Lua：局部变量
来源：http://owd.cdnleiting.top

local a = 1
来源：http://vrx.guowangkeji.top

[T33] Lua：表（数组）
来源：http://ylx.nanxinkj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ksq.zhaomingkeji.xyz

[T34] Lua：遍历表
来源：http://guj.yangfankeji.com

for i, v in ipairs(t) do print(i, v) end
来源：http://imd.ppjwa.cn

[T35] Lua：字典表
来源：http://sgi.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://rzx.cashguo.top

[T36] Lua：函数
来源：http://rya.zhoulong.xyz

function add(a, b) return a + b end
来源：http://kwr.haohaochexian.top

[T37] Lua：字符串拼接
来源：http://yib.jinghuilouyu.cn

"a" .. "b"
来源：http://pem.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://iam.hfpthk.cn

if x > 0 then print("正") end
来源：http://ggz.fengsongda.top

[T39] Lua：模式匹配
来源：http://les.snrcjt.cn

string.find(s, "%d+")
来源：http://uom.daxiang520.top

[T40] Lua：元表
来源：http://etq.wangdashe.top

setmetatable({}, { __index = base })
来源：http://bcd.yj202588.top

[T41] Perl：Hello World
来源：http://wzz.shanyushiyangtech.top

print "Hello\n";
来源：http://xsx.jiagoushi.top

[T42] Perl：变量类型
来源：http://pkj.yongpay.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oom.tarul.cn

[T43] Perl：字符串插值
来源：http://zlg.ybcxt.top

"值: $a"
来源：http://ngw.aizwys.cn

[T44] Perl：条件
来源：http://olr.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://dqu.xingfuxueyuan.xyz

[T45] Perl：数组遍历
来源：http://wsk.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://clv.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://ujh.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qhr.jqgfzy.top

[T47] Perl：正则捕获
来源：http://vba.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vyz.bbcook.cn

[T48] Perl：正则替换
来源：http://jdj.ehwqpu.com

$s =~ s/old/new/g;
来源：http://nsl.guannengcc.top

[T49] Perl：函数
来源：http://dgc.wangshuangyany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zwg.bjfxy.top

[T50] Perl：逐行读文件
来源：http://bus.cdnleiting.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gdf.shuidangran.top

while (my $line = <$fh>) { print $line; }
来源：http://wbf.gogol.net.cn

[T51] Scala：Hello World
来源：http://zwg.ivvv.top

println("Hello")
来源：http://nec.fengsongda.top

[T52] Scala：变量
来源：http://cwl.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://exo.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://hvp.nanxuanxn.top

s"值: $b"
来源：http://bup.9152youxi.cn

[T54] Scala：集合映射
来源：http://lpe.cucudq.cn

List(1, 2, 3).map(_ * 2)
来源：http://afm.yangfankeji.com

[T55] Scala：集合过滤
来源：http://ujl.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://tvz.yvedp.cn

[T56] Scala：样例类
来源：http://nfc.ctjpmb.com

case class User(name: String, age: Int)
来源：http://afg.svipenyu.cn

[T57] Scala：模式匹配
来源：http://cvw.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uzq.hesvh.cn

[T58] Scala：函数定义
来源：http://hrr.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://dtg.gogol.net.cn

[T59] Scala：循环
来源：http://mqa.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://bxx.birdmap.top

[T60] Scala：折叠
来源：http://ots.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oyq.gogol.net.cn

================================================================================
来源：http://flk.sysykeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://azi.iojbl.cn

================================================================================
来源：http://klh.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://cwt.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bpd.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://jop.daxiang520.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mgn.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://dwj.yvedp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gcu.hfpthk.cn

[U04] Py：变量调试打印
来源：http://tyb.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://akz.ybcxt.top

[U05] Py：列表去重且保序
来源：http://hjm.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://bta.guannengcc.top

[U06] Py：合并两个字典
来源：http://ezr.hammf.cn

{**a, **b}
来源：http://gxi.yueranfly.top

[U07] Py：反转字典键值
来源：http://etx.shanyushiyangkeji.top

{v: k for k, v in d.items()}
来源：http://jtb.ydzc1.top

[U08] Py：展平二维列表
来源：http://dic.chenlongwang.top

[y for x in nested for y in x]
来源：http://uyk.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://xrx.uphjek.com

max(d, key=d.get)
来源：http://vsi.zycfv.cn

[U10] Py：按值排序字典
来源：http://yvr.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://huz.shzxlz.cn

[U11] Py：生成器表达式
来源：http://bai.jinqigfzy.top

(x * 2 for x in arr)
来源：http://zpc.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://qld.c1oappe.top

Counter(arr).most_common(3)
来源：http://yxt.fzhhl.top

[U13] Py：固定长度队列
来源：http://reu.tanke756.top

deque(maxlen=10)
来源：http://gxx.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://fhm.dianchejie.cn

defaultdict(list)
来源：http://omr.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://saj.yangfankeji.com

t = time.perf_counter()
来源：http://eve.sjlbkw.cn

[U16] Py：命令行参数解析
来源：http://cva.yuanzhike.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lac.hesvh.cn

[U17] Py：初始化日志
来源：http://ibf.tarul.cn

logging.basicConfig(level=logging.INFO)
来源：http://pat.cqqwz.cn

[U18] Py：预编译正则
来源：http://oqa.ybcxt.top

pat = re.compile(r"\d+")
来源：http://cmx.chenzaomai.com

[U19] Py：正则替换带回调
来源：http://ljo.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ido.sufxvd.cn

[U20] Py：缓存函数结果
来源：http://xxi.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://ntd.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://hsd.cashguo.top

@contextlib.contextmanager
来源：http://wdt.aizwys.cn

[U22] Py：矩阵转置
来源：http://mqr.pengpengdd.cyou

list(zip(*m))
来源：http://bpk.yonumen.top

[U23] Py：分块读取大文件
来源：http://fwj.quarkkingdee.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vjv.yongpay.top

[U24] Py：路径操作
来源：http://cdq.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://udl.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://vdi.gogol.net.cn

csv.DictReader(f)
来源：http://rgp.yuanzhike.top

[U26] Py：并发下载
来源：http://dlh.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wte.zhixingplan.top

[U27] Py：异步 HTTP
来源：http://ket.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://wqy.fktsv.cn

[U28] Py：类型别名
来源：http://ncr.yvedp.cn

UserId = int
来源：http://atx.zhaomingkeji.xyz

[U29] Py：属性校验
来源：http://cvv.haohaochexian.top

@property 与 @x.setter 配合
来源：http://oap.bjfxy.top

[U30] Py：数据类
来源：http://sud.xylfe.cn

@dataclass(slots=True)
来源：http://fwk.zhengqikj.top


<!-- 参考信息 -->