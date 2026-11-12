代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rzm.cashguo.top

[S08] C：动态内存分配与释放
来源：http://hlx.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dxn.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://ceu.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://chs.sysykeji.top

[S10] C：指针与解引用
来源：http://sbx.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://zni.guannengcc.top

[S11] C：逐行读文件
来源：http://sei.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://hoh.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fhc.fehbvm.com

fclose(f);
来源：http://gek.wangdashe.top

[S12] C：写文件
来源：http://edp.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qmo.pengpengdd.cyou

[S13] C：宏定义
来源：http://iwl.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cuk.hammf.cn

[S14] C：枚举
来源：http://iyk.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://gml.yj20258.top

[S15] C：类型转换
来源：http://mde.shanyushiyangkeji.top

(double) a / b
来源：http://ecb.tian-w.cn

[S16] C：位操作置位
来源：http://kol.iojbl.cn

x |= (1 << 3);
来源：http://qne.yj202588.top

[S17] C：安全拼接字符串
来源：http://kcn.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oiy.yuanzhike.top

[S18] C：命令行参数
来源：http://oow.sufxvd.cn

int main(int argc, char **argv)
来源：http://iyq.aizwys.cn

[S19] C：快速排序
来源：http://ree.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://tmn.jyoumei.cn

[S20] C：二分查找
来源：http://eda.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://poy.tanke756.top

[S21] C：字符类别判断
来源：http://veg.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ugi.birdmap.top

[S22] C：字符串转数字
来源：http://dij.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://fau.sweek.top

[S23] C：随机数
来源：http://hkm.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jsg.daxiang520.top

[S24] C：获取本地时间
来源：http://zof.ppjwa.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vbb.sxryk.cn

[S25] C：内存拷贝
来源：http://qbp.zhaomingkeji.xyz

memcpy(dst, src, n);
来源：http://eit.wangshuangyany.cn

[S26] C：内存清零
来源：http://jcx.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://hcv.jlsjyb.cn

[S27] C：定义常量
来源：http://ixr.vqdsnc.cn

const double PI = 3.14159;
来源：http://nak.yvedp.cn

[S28] C：静态变量
来源：http://nzh.aizwys.cn

static int counter = 0;
来源：http://mvo.xinyue.icu

[S29] C：变参函数
来源：http://fws.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wrx.316326.xyz

[S30] C：头文件保护
来源：http://tzj.shzxlz.cn

#ifndef X_H
来源：http://oow.ehwqpu.com

#define X_H
来源：http://lrv.yvedp.cn

#endif
来源：http://qtd.epnwcf.com

[S31] C++：Hello World
来源：http://pfo.nanxinkj.top

#include <iostream>
来源：http://jad.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://emp.316326.xyz

[S32] C++：字符串
来源：http://ayv.yonumen.top

std::string s = "hi";  s += "!";
来源：http://jjm.hcnkem.com

[S33] C++：vector 增删
来源：http://zhl.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ysc.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://mul.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://lfd.vqdsnc.cn

[S35] C++：map
来源：http://pcm.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ezb.zhengqikj.top

[S36] C++：unordered_map
来源：http://djj.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ogk.mhx1999.top

[S37] C++：set
来源：http://wza.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://opr.hnxiangtu.top

[S38] C++：排序
来源：http://zdi.dianchejie.cn

std::sort(v.begin(), v.end());
来源：http://viz.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://wnj.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://crl.yueranfly.top

[S40] C++：查找元素
来源：http://qdq.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://glp.gotoacloud.top

[S41] C++：类与构造函数
来源：http://fmq.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://guz.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://del.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://ikc.birdmap.top

[S43] C++：智能指针
来源：http://ksl.zhijiandao.cn

auto p = std::make_unique<int>(5);
来源：http://vfr.hfpthk.cn

[S44] C++：引用传参
来源：http://hyw.yj202588.top

void inc(int &x) { ++x; }
来源：http://vwi.chenzaomai.com

[S45] C++：lambda
来源：http://std.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://iix.xuanzx.com

[S46] C++：函数模板
来源：http://uer.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nhh.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://ekl.zdbjq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://frs.fengsongda.top

[S48] C++：逐行读文件
来源：http://rbx.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eve.iojbl.cn

while (std::getline(in, line)) { }
来源：http://cyt.hcnkem.com

[S49] C++：写文件
来源：http://tjf.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dnt.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://otu.nanxuanxn.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sow.sxryk.cn

[S51] C++：显式类型转换
来源：http://zhh.hcnkem.com

static_cast<double>(a) / b
来源：http://oic.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://cba.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://zrs.yueranfly.top

[S53] C++：移动语义
来源：http://fww.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://tdr.jyoumei.cn

[S54] C++：异常处理
来源：http://pov.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oak.bbcook.cn

[S55] C++：结构化绑定
来源：http://fyw.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tvw.jinqigfzy.top

[S56] C++：optional
来源：http://htu.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bim.sjlbkw.cn

[S57] C++：编译期常量
来源：http://pah.cqqwz.cn

constexpr int N = 10;
来源：http://jvm.hcnkem.com

[S58] C++：命名空间
来源：http://dgh.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://mly.hfpthk.cn

[S59] C++：静态断言
来源：http://alu.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ihg.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://wqw.dashuyun.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lma.sysykeji.top

================================================================================
来源：http://qva.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eos.aizwys.cn

================================================================================
来源：http://xfc.hesvh.cn

[T01] Kotlin：Hello World
来源：http://rgm.tianlin.xyz

println("Hello")
来源：http://uiv.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://brh.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dad.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://loo.uphjek.com

"值: $b"
来源：http://zdy.uphjek.com

[T04] Kotlin：空安全
来源：http://bmj.cdnleiting.top

val n: String? = null;  n?.length
来源：http://xfn.guowangkeji.top

[T05] Kotlin：when 表达式
来源：http://qjy.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://asl.jianghu66.top

[T06] Kotlin：集合映射
来源：http://jsm.316326.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://sme.9152youxi.cn

[T07] Kotlin：集合过滤
来源：http://cop.ydzc1.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ggw.nanxinkj.top

[T08] Kotlin：数据类
来源：http://chw.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://kqk.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://gmp.uphjek.com

fun String.exclaim() = this + "!"
来源：http://paw.pycfn.com

[T10] Kotlin：默认参数
来源：http://dbm.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ais.hfpthk.cn

[T11] Kotlin：协程
来源：http://xyf.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rne.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://xte.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://uyh.cheryme.top

[T13] Kotlin：只读 Map
来源：http://fck.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://bcz.yuxming.cn

[T14] Kotlin：循环
来源：http://aiv.chenlongwang.top

for (i in 1..10) println(i)
来源：http://zxj.vehdjk.com

[T15] Kotlin：接口
来源：http://tih.gzhubu.top

interface Shape { fun area(): Double }
来源：http://nrm.zhaomingkeji.xyz

[T16] Swift：Hello World
来源：http://rxl.quarkkingdee.top

print("Hello")
来源：http://nhw.bjfxy.top

[T17] Swift：变量与常量
来源：http://wnr.jqgfzy.top

var a = 1;  let b = 2
来源：http://fsc.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://iei.xziqi.cn

"值: \(b)"
来源：http://mwt.jiagoushi.top

[T19] Swift：可选绑定
来源：http://lov.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://ypb.hcnkem.com

[T20] Swift：数组操作
来源：http://llf.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qbq.ivvv.top

[T21] Swift：遍历
来源：http://zre.shzxlz.cn

for x in a { print(x) }
来源：http://ugj.jinghuilouyu.cn

[T22] Swift：字典
来源：http://fkb.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://zqh.zhongyouzk.top

[T23] Swift：函数
来源：http://kez.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zqv.cashguo.top

[T24] Swift：闭包
来源：http://mhq.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yoo.fzhhl.top

[T25] Swift：结构体
来源：http://btl.yfazqb.com

struct P { var x: Int }
来源：http://kxc.jqgfzy.top

[T26] Swift：类与重写
来源：http://vza.iojbl.cn

class A: Base { override func f() {} }
来源：http://pgo.ctjpmb.com

[T27] Swift：错误处理
来源：http://mov.yvedp.cn

do { try f() } catch { print(error) }
来源：http://zfm.guowangkeji.top

[T28] Swift：枚举
来源：http://htu.quarkkingdee.top

enum Color { case red, green }
来源：http://wof.zhijiandao.cn

[T29] Swift：guard 提前返回
来源：http://mqc.yonumen.top

guard let x = opt else { return }
来源：http://cay.hnqzz.top

[T30] Swift：协议
来源：http://lox.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://bww.yuxming.cn

[T31] Lua：Hello World
来源：http://jmz.ctjpmb.com

print("Hello")
来源：http://mkd.chenzaomai.com

[T32] Lua：局部变量
来源：http://lgo.haohaochexian.top

local a = 1
来源：http://kwg.shzxlz.cn

[T33] Lua：表（数组）
来源：http://eei.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gcd.uphjek.com

[T34] Lua：遍历表
来源：http://jdq.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lan.daria6918.cn

[T35] Lua：字典表
来源：http://zjn.quarkkingdee.top

local d = { a = 1 };  d.b = 2
来源：http://nkf.vehdjk.com

[T36] Lua：函数
来源：http://rnc.mhx1999.top

function add(a, b) return a + b end
来源：http://sgt.316326.xyz

[T37] Lua：字符串拼接
来源：http://mie.redwolf501.top

"a" .. "b"
来源：http://tug.chenlongwang.top

[T38] Lua：条件
来源：http://hox.sxryk.cn

if x > 0 then print("正") end
来源：http://rhb.ywan-chungtsiang.top

[T39] Lua：模式匹配
来源：http://ssk.chenlongwang.top

string.find(s, "%d+")
来源：http://tns.fktsv.cn

[T40] Lua：元表
来源：http://xfv.c1oappe.top

setmetatable({}, { __index = base })
来源：http://wtr.yj20258.top

[T41] Perl：Hello World
来源：http://gkw.ppjwa.cn

print "Hello\n";
来源：http://jep.yuxming.cn

[T42] Perl：变量类型
来源：http://xii.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://knd.fanxiaobao.xyz

[T43] Perl：字符串插值
来源：http://adz.jyoumei.cn

"值: $a"
来源：http://zat.havefunace.top

[T44] Perl：条件
来源：http://qcq.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://mmh.sufxvd.cn

[T45] Perl：数组遍历
来源：http://nen.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://mgi.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://nkd.bbcook.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jyk.jyoumei.cn

[T47] Perl：正则捕获
来源：http://tlp.daxiang520.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nzx.guannengcc.top

[T48] Perl：正则替换
来源：http://ovy.yuxming.cn

$s =~ s/old/new/g;
来源：http://tui.ydjk.org.cn

[T49] Perl：函数
来源：http://keu.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cfx.fzhhl.top

[T50] Perl：逐行读文件
来源：http://xwl.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sle.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://gjn.dashuyun.cn

[T51] Scala：Hello World
来源：http://heb.jinqigufen.top

println("Hello")
来源：http://qxc.fktsv.cn

[T52] Scala：变量
来源：http://nyd.316326.xyz

val a = 1;  var b = 2
来源：http://coc.aizwys.cn

[T53] Scala：字符串插值
来源：http://xlc.sysykeji.top

s"值: $b"
来源：http://cgh.jinyuanbaomall.cn

[T54] Scala：集合映射
来源：http://vog.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://kso.hesvh.cn

[T55] Scala：集合过滤
来源：http://fsq.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://thz.bjfxy.top

[T56] Scala：样例类
来源：http://fjb.cashguo.top

case class User(name: String, age: Int)
来源：http://bfq.guannengcc.top

[T57] Scala：模式匹配
来源：http://wjd.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://mki.ivvv.top

[T58] Scala：函数定义
来源：http://ngx.xuetiantiany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://odx.cashguo.top

[T59] Scala：循环
来源：http://lvg.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://eyj.meibo888.top

[T60] Scala：折叠
来源：http://ine.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sin.tarul.cn

================================================================================
来源：http://yyk.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fcs.hnxiangtu.top

================================================================================
来源：http://jnx.chenzaomai.com

[U01] Py：创建虚拟环境
来源：http://ara.bbcook.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yka.ydjk.org.cn

[U02] Py：导出 / 安装依赖
来源：http://gwr.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cxa.tianlin.xyz

[U03] Py：加载 .env 配置
来源：http://tfa.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fcr.jiagoushi.top

[U04] Py：变量调试打印
来源：http://uow.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xgd.epnwcf.com

[U05] Py：列表去重且保序
来源：http://pik.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://vgb.dashuyun.cn

[U06] Py：合并两个字典
来源：http://ovl.kuanghao11.cn

{**a, **b}
来源：http://xsn.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://kfs.pycfn.com

{v: k for k, v in d.items()}
来源：http://qxl.ydjk.org.cn

[U08] Py：展平二维列表
来源：http://bkb.chenzaomai.com

[y for x in nested for y in x]
来源：http://zdd.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://mjs.meibo888.top

max(d, key=d.get)
来源：http://ieo.ctjpmb.com

[U10] Py：按值排序字典
来源：http://ptf.ywan-chungtsiang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mvo.tarul.cn

[U11] Py：生成器表达式
来源：http://jca.hysaishi.cn

(x * 2 for x in arr)
来源：http://zja.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://ncw.shuidangran.top

Counter(arr).most_common(3)
来源：http://yni.c1oappe.top

[U13] Py：固定长度队列
来源：http://usm.meibo888.top

deque(maxlen=10)
来源：http://yul.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://tbd.sjlbkw.cn

defaultdict(list)
来源：http://yra.zhijiandao.cn

[U15] Py：高精度计时
来源：http://qfu.yanxiufei.cn

t = time.perf_counter()
来源：http://pmn.tian-w.cn

[U16] Py：命令行参数解析
来源：http://cte.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://laq.vqdsnc.cn

[U17] Py：初始化日志
来源：http://bdk.havefunace.top

logging.basicConfig(level=logging.INFO)
来源：http://ejy.zhijiandao.cn

[U18] Py：预编译正则
来源：http://xkm.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://sda.hysaishi.cn

[U19] Py：正则替换带回调
来源：http://gpn.quarkkingdee.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oja.gogol.net.cn

[U20] Py：缓存函数结果
来源：http://vao.gogol.net.cn

@functools.lru_cache(maxsize=None)
来源：http://bdb.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://dno.yangfankeji.com

@contextlib.contextmanager
来源：http://dnm.daxiang520.top

[U22] Py：矩阵转置
来源：http://vif.yueranfly.top

list(zip(*m))
来源：http://oux.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://ect.wangdashe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xfn.hywenlv.cn

[U24] Py：路径操作
来源：http://waf.zhijiandao.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lsl.tianlin.xyz

[U25] Py：CSV 按字典读
来源：http://ctf.zhixingplan.top

csv.DictReader(f)
来源：http://ykr.hcnkem.com

[U26] Py：并发下载
来源：http://vjy.zhengqikj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kps.zhixingplan.top

[U27] Py：异步 HTTP
来源：http://ypn.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://ejh.tarul.cn

[U28] Py：类型别名
来源：http://mkz.jqgufenzy.top

UserId = int
来源：http://pxi.shzxlz.cn

[U29] Py：属性校验
来源：http://efv.xingfuxueyuan.xyz

@property 与 @x.setter 配合
来源：http://gdz.tarul.cn

[U30] Py：数据类
来源：http://eem.wangshuangyany.cn

@dataclass(slots=True)
来源：http://uek.yonumen.top


<!-- 参考信息 -->