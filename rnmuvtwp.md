代发 wailian999

strlen(s)
来源：http://czx.xziqi.cn

[S06] C：字符串比较
来源：http://pxz.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://edx.52xcode.cn

[S07] C：数组遍历求和
来源：http://qih.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kcm.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://fhq.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rzy.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://rpp.pycfn.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rqh.jiagoushi.top

[S10] C：指针与解引用
来源：http://cov.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://jvn.bjfxy.top

[S11] C：逐行读文件
来源：http://gdm.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://mdv.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tmw.ehwqpu.com

fclose(f);
来源：http://lcx.dashuyun.cn

[S12] C：写文件
来源：http://mdr.yvedp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://diw.andypj.xyz

[S13] C：宏定义
来源：http://cgz.yuxming.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xmi.aizwys.cn

[S14] C：枚举
来源：http://toh.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://ioj.nanxinkj.top

[S15] C：类型转换
来源：http://omw.mhx1999.top

(double) a / b
来源：http://bhr.yfazqb.com

[S16] C：位操作置位
来源：http://yhb.gogol.net.cn

x |= (1 << 3);
来源：http://mcj.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://que.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pgo.fengsongda.top

[S18] C：命令行参数
来源：http://tpn.cqqwz.cn

int main(int argc, char **argv)
来源：http://gkv.dianchejie.cn

[S19] C：快速排序
来源：http://soa.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://nsa.aibaodan.cn

[S20] C：二分查找
来源：http://tbs.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ybt.zhixingplan.top

[S21] C：字符类别判断
来源：http://prz.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nsa.hammf.cn

[S22] C：字符串转数字
来源：http://pxz.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://gnl.jqgufenzy.top

[S23] C：随机数
来源：http://aef.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yaw.shanyushiyangtech.top

[S24] C：获取本地时间
来源：http://atc.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nat.cashguo.top

[S25] C：内存拷贝
来源：http://fgp.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://cst.xuetiantiany.cn

[S26] C：内存清零
来源：http://dto.yfazqb.com

memset(a, 0, sizeof a);
来源：http://odu.daxiang520.top

[S27] C：定义常量
来源：http://ckp.bjfxy.top

const double PI = 3.14159;
来源：http://rlh.jinghuilouyu.cn

[S28] C：静态变量
来源：http://wml.tanke756.top

static int counter = 0;
来源：http://abg.hammf.cn

[S29] C：变参函数
来源：http://awx.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vup.cqqwz.cn

[S30] C：头文件保护
来源：http://qod.shuidangran.top

#ifndef X_H
来源：http://eol.xuetiantiany.cn

#define X_H
来源：http://fzz.zhaomingkeji.xyz

#endif
来源：http://uwn.daxiang520.top

[S31] C++：Hello World
来源：http://nxr.yongpay.top

#include <iostream>
来源：http://mqn.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://rka.haohaochexian.top

[S32] C++：字符串
来源：http://hki.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://dtf.nanxinkj.top

[S33] C++：vector 增删
来源：http://alp.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wpa.sxryk.cn

[S34] C++：遍历 vector
来源：http://rgw.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://uku.vqdsnc.cn

[S35] C++：map
来源：http://grx.zhaomingkeji.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mac.iojbl.cn

[S36] C++：unordered_map
来源：http://rpf.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ekg.fanxiaobao.xyz

[S37] C++：set
来源：http://fix.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uib.jqgfzy.top

[S38] C++：排序
来源：http://ehw.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://eca.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://wkh.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mfn.nanxinkj.top

[S40] C++：查找元素
来源：http://aef.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tnc.dashuyun.cn

[S41] C++：类与构造函数
来源：http://kcf.zhixingplan.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bav.yj20258888.top

[S42] C++：继承与虚函数
来源：http://bsg.9152youxi.cn

class B : public Base { public: void f() override {} };
来源：http://cwm.hnqzz.top

[S43] C++：智能指针
来源：http://wbs.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://tpq.tarul.cn

[S44] C++：引用传参
来源：http://cmi.fzhhl.top

void inc(int &x) { ++x; }
来源：http://pwd.hywenlv.cn

[S45] C++：lambda
来源：http://zsr.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://roi.guowangkeji.top

[S46] C++：函数模板
来源：http://ptx.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mya.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://unx.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hvm.ehwqpu.com

[S48] C++：逐行读文件
来源：http://aoe.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oiw.yfazqb.com

while (std::getline(in, line)) { }
来源：http://wlp.ppjwa.cn

[S49] C++：写文件
来源：http://mjm.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vlu.feifeiyinyue.top

[S50] C++：格式化数字
来源：http://oeo.yj20258.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kbk.epnwcf.com

[S51] C++：显式类型转换
来源：http://stp.sweek.top

static_cast<double>(a) / b
来源：http://wav.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://vxf.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://eix.cdnleiting.top

[S53] C++：移动语义
来源：http://asm.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://edk.316326.xyz

[S54] C++：异常处理
来源：http://gtj.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kfp.gaohongyu789.top

[S55] C++：结构化绑定
来源：http://vsp.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rwp.sysykeji.top

[S56] C++：optional
来源：http://mbv.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wzy.wangdashe.top

[S57] C++：编译期常量
来源：http://hzg.zdbjq.cn

constexpr int N = 10;
来源：http://axx.cheryme.top

[S58] C++：命名空间
来源：http://ecr.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://hgm.chenjidiqi.icu

[S59] C++：静态断言
来源：http://qaw.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lur.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://cjt.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://klt.chenzaomai.com

================================================================================
来源：http://bxm.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gih.uphjek.com

================================================================================
来源：http://zvp.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://ciu.ywan-chungtsiang.top

println("Hello")
来源：http://pyx.cashguo.top

[T02] Kotlin：变量
来源：http://iba.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rtr.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://mdd.hysaishi.cn

"值: $b"
来源：http://gch.sysykeji.top

[T04] Kotlin：空安全
来源：http://wab.sxryk.cn

val n: String? = null;  n?.length
来源：http://bai.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://fwd.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ovf.daria6918.cn

[T06] Kotlin：集合映射
来源：http://hwg.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ste.shuidangran.top

[T07] Kotlin：集合过滤
来源：http://muu.uphjek.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://llt.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://kup.zhengqikj.top

data class User(val name: String, val age: Int)
来源：http://xjz.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://gmk.ydjk.org.cn

fun String.exclaim() = this + "!"
来源：http://bvz.haohaochexian.top

[T10] Kotlin：默认参数
来源：http://hme.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kbx.aizwys.cn

[T11] Kotlin：协程
来源：http://ckr.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zra.ywan-chungtsiang.top

[T12] Kotlin：解构声明
来源：http://qia.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://gex.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://oww.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://rve.hesvh.cn

[T14] Kotlin：循环
来源：http://lby.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://yka.chenlongwang.top

[T15] Kotlin：接口
来源：http://enf.tianlin.xyz

interface Shape { fun area(): Double }
来源：http://vtw.sysykeji.top

[T16] Swift：Hello World
来源：http://qbe.sysykeji.top

print("Hello")
来源：http://evx.hfpthk.cn

[T17] Swift：变量与常量
来源：http://std.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://vya.ppjwa.cn

[T18] Swift：字符串插值
来源：http://dsp.wangdashe.top

"值: \(b)"
来源：http://rpd.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://kbm.yj20258.top

if let n = opt { print(n) }
来源：http://lgh.chenjidiqi.icu

[T20] Swift：数组操作
来源：http://kpu.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://xpp.yfazqb.com

[T21] Swift：遍历
来源：http://lic.yueranfly.top

for x in a { print(x) }
来源：http://ncd.wangshuangyany.cn

[T22] Swift：字典
来源：http://buw.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://vjr.dianchejie.cn

[T23] Swift：函数
来源：http://gql.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ucy.jinyuanbaomall.cn

[T24] Swift：闭包
来源：http://oek.tianlin.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://hcf.guannengcc.top

[T25] Swift：结构体
来源：http://yus.sysykeji.top

struct P { var x: Int }
来源：http://xic.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://mon.jqgfzy.top

class A: Base { override func f() {} }
来源：http://rwx.gzhubu.top

[T27] Swift：错误处理
来源：http://sit.cheryme.top

do { try f() } catch { print(error) }
来源：http://sow.redwolf501.top

[T28] Swift：枚举
来源：http://eoi.316326.xyz

enum Color { case red, green }
来源：http://ync.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://bbw.fzhhl.top

guard let x = opt else { return }
来源：http://qij.svipenyu.cn

[T30] Swift：协议
来源：http://jrc.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://hrb.ctjpmb.com

[T31] Lua：Hello World
来源：http://pij.ppjwa.cn

print("Hello")
来源：http://lmr.dashuyun.cn

[T32] Lua：局部变量
来源：http://fsc.pengpengdd.cyou

local a = 1
来源：http://kyu.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://ymq.xinyue.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://nko.gaohongyu789.top

[T34] Lua：遍历表
来源：http://pmd.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cyf.snrcjt.cn

[T35] Lua：字典表
来源：http://bpv.sysykeji.top

local d = { a = 1 };  d.b = 2
来源：http://rkv.zhongyouzk.top

[T36] Lua：函数
来源：http://vwy.yueranfly.top

function add(a, b) return a + b end
来源：http://jln.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://rpt.yongpay.top

"a" .. "b"
来源：http://jkg.hesvh.cn

[T38] Lua：条件
来源：http://anz.yj202588.top

if x > 0 then print("正") end
来源：http://cvm.shzxlz.cn

[T39] Lua：模式匹配
来源：http://uba.316326.xyz

string.find(s, "%d+")
来源：http://pyg.jianghu66.top

[T40] Lua：元表
来源：http://trc.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://bum.hnqzz.top

[T41] Perl：Hello World
来源：http://vmo.sweek.top

print "Hello\n";
来源：http://mgb.ehwqpu.com

[T42] Perl：变量类型
来源：http://qjw.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://swy.zhijiandao.cn

[T43] Perl：字符串插值
来源：http://epu.tian-w.cn

"值: $a"
来源：http://ofj.ehwqpu.com

[T44] Perl：条件
来源：http://lap.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://fym.ivvv.top

[T45] Perl：数组遍历
来源：http://nzy.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://nni.zhiwuduotai.top

[T46] Perl：哈希操作
来源：http://uuz.fehbvm.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ltg.kuanghao11.cn

[T47] Perl：正则捕获
来源：http://lmz.jiagoushi.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pgd.yuxming.cn

[T48] Perl：正则替换
来源：http://qss.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://mdk.zdqjudy.top

[T49] Perl：函数
来源：http://cgf.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ycv.wangdashe.top

[T50] Perl：逐行读文件
来源：http://fbf.shanyushiyangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hzv.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://jwo.tian-w.cn

[T51] Scala：Hello World
来源：http://jgp.c1oappe.top

println("Hello")
来源：http://ige.gotoacloud.top

[T52] Scala：变量
来源：http://qjk.kuanghao11.cn

val a = 1;  var b = 2
来源：http://ebb.aizwys.cn

[T53] Scala：字符串插值
来源：http://ddn.fengsongda.top

s"值: $b"
来源：http://veo.vqdsnc.cn

[T54] Scala：集合映射
来源：http://ktu.shangyingyoupin.top

List(1, 2, 3).map(_ * 2)
来源：http://zhz.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://ahb.ivvv.top

List(1, 2, 3).filter(_ > 1)
来源：http://rbt.shangyingyoupin.top

[T56] Scala：样例类
来源：http://gmb.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://gtb.hfpthk.cn

[T57] Scala：模式匹配
来源：http://toj.cqqwz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wwj.hysaishi.cn

[T58] Scala：函数定义
来源：http://iia.andypj.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://qde.sysykeji.top

[T59] Scala：循环
来源：http://vbc.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://kpz.tanke756.top

[T60] Scala：折叠
来源：http://czs.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://izk.xuanzx.com

================================================================================
来源：http://ame.fanxiaobao.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vbx.zhixingplan.top

================================================================================
来源：http://ene.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://fxi.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://prg.fzhhl.top

[U02] Py：导出 / 安装依赖
来源：http://odr.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tju.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://opd.zhaomingkeji.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://jsa.daxiang520.top

[U04] Py：变量调试打印
来源：http://zpt.ywan-chungtsiang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://erb.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://kfm.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://xvc.pycfn.com

[U06] Py：合并两个字典
来源：http://kdg.316326.xyz

{**a, **b}
来源：http://asp.yvedp.cn

[U07] Py：反转字典键值
来源：http://esh.ybcxt.top

{v: k for k, v in d.items()}
来源：http://opb.pycfn.com

[U08] Py：展平二维列表
来源：http://wpe.dashuyun.cn

[y for x in nested for y in x]
来源：http://ipp.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://iud.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://dee.jiagoushi.top

[U10] Py：按值排序字典
来源：http://mdb.jiagoushi.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sph.jqgfzy.top

[U11] Py：生成器表达式
来源：http://wky.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://wtp.xuetiantiany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cfi.jqgufenzy.top

Counter(arr).most_common(3)
来源：http://rww.yj20258.top

[U13] Py：固定长度队列
来源：http://pxx.yongpay.top

deque(maxlen=10)
来源：http://muf.yj20258888.top

[U14] Py：分组收集到列表
来源：http://hxc.pycfn.com

defaultdict(list)
来源：http://irt.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://zux.zhixingplan.top

t = time.perf_counter()
来源：http://tbh.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://dkv.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hcw.smart0.xyz

[U17] Py：初始化日志
来源：http://fxl.hywenlv.cn

logging.basicConfig(level=logging.INFO)
来源：http://hya.jianghu66.top

[U18] Py：预编译正则
来源：http://ovt.bbcook.cn

pat = re.compile(r"\d+")
来源：http://uyc.316326.xyz

[U19] Py：正则替换带回调
来源：http://dhq.quarkkingdee.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pki.yj20258888.top

[U20] Py：缓存函数结果
来源：http://nlh.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://urh.aibaodan.cn

[U21] Py：自定义上下文管理器
来源：http://chs.feifeiyinyue.top

@contextlib.contextmanager
来源：http://idq.uphjek.com

[U22] Py：矩阵转置
来源：http://cca.pengpengdd.cyou

list(zip(*m))
来源：http://qub.smart0.xyz

[U23] Py：分块读取大文件
来源：http://vqg.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fcw.zhoulong.xyz

[U24] Py：路径操作
来源：http://xnx.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aou.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://tbf.yfazqb.com

csv.DictReader(f)
来源：http://vqy.tanke756.top

[U26] Py：并发下载
来源：http://wwy.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://frd.iojbl.cn

[U27] Py：异步 HTTP
来源：http://mfb.ydjk.org.cn

aiohttp.ClientSession() 配合 async with
来源：http://vnp.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://wst.aizwys.cn

UserId = int
来源：http://pdw.yuxming.cn


<!-- 参考信息 -->