代发 wailian999

int x; scanf("%d", &x);
来源：http://ajs.gogol.net.cn

[S04] C：字符串复制
来源：http://fuz.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://szu.sysykeji.top

[S05] C：字符串长度
来源：http://cmj.sxryk.cn

strlen(s)
来源：http://byn.gaohongyu789.top

[S06] C：字符串比较
来源：http://dzu.chenzaomai.com

strcmp(a, b) == 0
来源：http://nqa.jiagoushi.top

[S07] C：数组遍历求和
来源：http://sol.xinyue.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ckg.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://oat.gotoacloud.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rpk.tanke756.top

[S09] C：结构体定义与初始化
来源：http://bdf.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://msb.andypj.xyz

[S10] C：指针与解引用
来源：http://mfj.xylfe.cn

int *p = &a;  *p = 5;
来源：http://wbh.hammf.cn

[S11] C：逐行读文件
来源：http://pbx.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://bgf.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://pin.wangshuangyany.cn

fclose(f);
来源：http://nvk.gotoacloud.top

[S12] C：写文件
来源：http://wdz.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ejg.zhaomingkeji.xyz

[S13] C：宏定义
来源：http://jpe.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://weu.sweek.top

[S14] C：枚举
来源：http://zer.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://xvh.hfpthk.cn

[S15] C：类型转换
来源：http://ybh.svipenyu.cn

(double) a / b
来源：http://jtz.ybcxt.top

[S16] C：位操作置位
来源：http://gsi.wangdashe.top

x |= (1 << 3);
来源：http://ecy.yongpay.top

[S17] C：安全拼接字符串
来源：http://hzc.jiagoushi.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yxb.ybcxt.top

[S18] C：命令行参数
来源：http://esn.yj20258888.top

int main(int argc, char **argv)
来源：http://htn.kuanghao11.cn

[S19] C：快速排序
来源：http://gfn.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://tzc.yvedp.cn

[S20] C：二分查找
来源：http://cmz.epnwcf.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vjf.xylfe.cn

[S21] C：字符类别判断
来源：http://kos.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lmf.ehwqpu.com

[S22] C：字符串转数字
来源：http://svw.wangshuangyany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fac.pengpengdd.cyou

[S23] C：随机数
来源：http://ssb.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rsg.yvedp.cn

[S24] C：获取本地时间
来源：http://uoo.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jen.kuanghao11.cn

[S25] C：内存拷贝
来源：http://vsk.mhx1999.top

memcpy(dst, src, n);
来源：http://rfw.sweek.top

[S26] C：内存清零
来源：http://zzn.havefunace.top

memset(a, 0, sizeof a);
来源：http://utq.quarkkingdee.top

[S27] C：定义常量
来源：http://flp.iojbl.cn

const double PI = 3.14159;
来源：http://mmz.xuanzx.com

[S28] C：静态变量
来源：http://dgy.yonumen.top

static int counter = 0;
来源：http://ezj.jqgufenzy.top

[S29] C：变参函数
来源：http://lsh.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kpl.hywenlv.cn

[S30] C：头文件保护
来源：http://rzq.uphjek.com

#ifndef X_H
来源：http://eip.kuanghao11.cn

#define X_H
来源：http://sxl.jyoumei.cn

#endif
来源：http://riz.quarkkingdee.top

[S31] C++：Hello World
来源：http://kvs.yangfankeji.com

#include <iostream>
来源：http://ulf.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://vlr.yonumen.top

[S32] C++：字符串
来源：http://xzo.yj202588.top

std::string s = "hi";  s += "!";
来源：http://aue.jyoumei.cn

[S33] C++：vector 增删
来源：http://ytt.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uop.fengsongda.top

[S34] C++：遍历 vector
来源：http://olv.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://eji.redwolf501.top

[S35] C++：map
来源：http://wuc.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sxr.zdqjudy.top

[S36] C++：unordered_map
来源：http://ujn.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lxe.andypj.xyz

[S37] C++：set
来源：http://ycg.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://skr.zhongyouzk.top

[S38] C++：排序
来源：http://nuh.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://jzj.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://dux.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://inm.wangshuangyany.cn

[S40] C++：查找元素
来源：http://wfk.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zxi.zhongyouzk.top

[S41] C++：类与构造函数
来源：http://kms.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wmt.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://rem.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://yqk.ydzc1.top

[S43] C++：智能指针
来源：http://sym.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://evb.zhijiandao.cn

[S44] C++：引用传参
来源：http://fjb.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://pux.hcnkem.com

[S45] C++：lambda
来源：http://sys.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bbz.yongpay.top

[S46] C++：函数模板
来源：http://fqi.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vok.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://glv.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dov.guannengcc.top

[S48] C++：逐行读文件
来源：http://smb.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://hog.gzhubu.top

while (std::getline(in, line)) { }
来源：http://yiw.vehdjk.com

[S49] C++：写文件
来源：http://xxt.xinyue.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://szw.zycfv.cn

[S50] C++：格式化数字
来源：http://pui.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lab.ppjwa.cn

[S51] C++：显式类型转换
来源：http://vnk.epnwcf.com

static_cast<double>(a) / b
来源：http://rhn.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://fye.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://vbi.pycfn.com

[S53] C++：移动语义
来源：http://vfb.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://asy.jinqigufen.top

[S54] C++：异常处理
来源：http://mmh.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kac.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://ngb.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://oci.fanxiaobao.xyz

[S56] C++：optional
来源：http://osb.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://npa.yj20258888.top

[S57] C++：编译期常量
来源：http://tmp.smart0.xyz

constexpr int N = 10;
来源：http://ukf.gogol.net.cn

[S58] C++：命名空间
来源：http://sjb.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://qok.dashuyun.cn

[S59] C++：静态断言
来源：http://kkk.fanxiaobao.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jjd.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://vyb.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gtl.chenzaomai.com

================================================================================
来源：http://ejl.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xks.aibaodan.cn

================================================================================
来源：http://yzy.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://kfe.nanxinkj.top

println("Hello")
来源：http://bpv.yfazqb.com

[T02] Kotlin：变量
来源：http://oly.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jaz.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://lqb.gzhubu.top

"值: $b"
来源：http://grs.jinqigufen.top

[T04] Kotlin：空安全
来源：http://wul.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://znx.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://gxg.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://avv.hcnkem.com

[T06] Kotlin：集合映射
来源：http://ktz.haohaochexian.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mim.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://kpb.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wrr.svipenyu.cn

[T08] Kotlin：数据类
来源：http://jte.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://uvo.ivvv.top

[T09] Kotlin：扩展函数
来源：http://tin.316326.xyz

fun String.exclaim() = this + "!"
来源：http://ztp.yj20258.top

[T10] Kotlin：默认参数
来源：http://sab.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kwa.yonumen.top

[T11] Kotlin：协程
来源：http://ars.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://zet.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://ahq.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://vel.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://kha.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://kob.zhaomingkeji.xyz

[T14] Kotlin：循环
来源：http://znc.dianchejie.cn

for (i in 1..10) println(i)
来源：http://yzt.vehdjk.com

[T15] Kotlin：接口
来源：http://zlm.yj20258888.top

interface Shape { fun area(): Double }
来源：http://fht.gotoacloud.top

[T16] Swift：Hello World
来源：http://liv.ydzc1.top

print("Hello")
来源：http://lxh.havefunace.top

[T17] Swift：变量与常量
来源：http://fmd.uphjek.com

var a = 1;  let b = 2
来源：http://jfo.xuanzx.com

[T18] Swift：字符串插值
来源：http://jrt.chenjidiqi.icu

"值: \(b)"
来源：http://adf.yueranfly.top

[T19] Swift：可选绑定
来源：http://btv.ehwqpu.com

if let n = opt { print(n) }
来源：http://xvy.smart0.xyz

[T20] Swift：数组操作
来源：http://mjl.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://jzy.tian-w.cn

[T21] Swift：遍历
来源：http://qcm.hongshengwenyu.top

for x in a { print(x) }
来源：http://waj.ehwqpu.com

[T22] Swift：字典
来源：http://dhi.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nxq.yvedp.cn

[T23] Swift：函数
来源：http://ivw.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kee.zhengqikj.top

[T24] Swift：闭包
来源：http://ljh.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mxa.sjlbkw.cn

[T25] Swift：结构体
来源：http://vst.jiagoushi.top

struct P { var x: Int }
来源：http://nen.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://oix.gzhubu.top

class A: Base { override func f() {} }
来源：http://qlg.ppjwa.cn

[T27] Swift：错误处理
来源：http://lum.tarul.cn

do { try f() } catch { print(error) }
来源：http://zaj.xuanzx.com

[T28] Swift：枚举
来源：http://pha.tarul.cn

enum Color { case red, green }
来源：http://dce.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://iie.birdmap.top

guard let x = opt else { return }
来源：http://brp.yj20258.top

[T30] Swift：协议
来源：http://kgp.yueranfly.top

protocol Shape { func area() -> Double }
来源：http://sbt.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://zix.yonumen.top

print("Hello")
来源：http://fne.daxiang520.top

[T32] Lua：局部变量
来源：http://zfy.ehwqpu.com

local a = 1
来源：http://glv.cashguo.top

[T33] Lua：表（数组）
来源：http://qog.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zpl.feifeiyinyue.top

[T34] Lua：遍历表
来源：http://vbv.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://haa.bbcook.cn

[T35] Lua：字典表
来源：http://ezb.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://dkh.sufxvd.cn

[T36] Lua：函数
来源：http://gpp.ppjwa.cn

function add(a, b) return a + b end
来源：http://dad.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://ygf.chenlongwang.top

"a" .. "b"
来源：http://zbi.dashuyun.cn

[T38] Lua：条件
来源：http://upm.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://bdh.fengsongda.top

[T39] Lua：模式匹配
来源：http://xbu.jinqigfzy.top

string.find(s, "%d+")
来源：http://jxm.redwolf501.top

[T40] Lua：元表
来源：http://yqs.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://wqw.zhongyouzk.top

[T41] Perl：Hello World
来源：http://cpg.daxiang520.top

print "Hello\n";
来源：http://ewn.quarkkingdee.top

[T42] Perl：变量类型
来源：http://soq.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ind.haohaochexian.top

[T43] Perl：字符串插值
来源：http://hxx.sweek.top

"值: $a"
来源：http://xdj.hongshengwenyu.top

[T44] Perl：条件
来源：http://wys.xylfe.cn

if ($a > 0) { print "正"; }
来源：http://xcm.nanxinkj.top

[T45] Perl：数组遍历
来源：http://far.yanxiufei.cn

for my $x (@arr) { print $x; }
来源：http://vgw.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://xeu.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://akx.yueranfly.top

[T47] Perl：正则捕获
来源：http://tvt.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rof.sjlbkw.cn

[T48] Perl：正则替换
来源：http://hbh.fzhhl.top

$s =~ s/old/new/g;
来源：http://tes.zhiwuduotai.top

[T49] Perl：函数
来源：http://hra.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ell.zhaomingkeji.xyz

[T50] Perl：逐行读文件
来源：http://itd.52xcode.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://azv.xinyue.icu

while (my $line = <$fh>) { print $line; }
来源：http://lvw.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://gec.iojbl.cn

println("Hello")
来源：http://jue.shzxlz.cn

[T52] Scala：变量
来源：http://hqx.aizwys.cn

val a = 1;  var b = 2
来源：http://uax.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://mta.nwbrower.top

s"值: $b"
来源：http://zaj.fktsv.cn

[T54] Scala：集合映射
来源：http://gbm.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://gwo.yj20258888.top

[T55] Scala：集合过滤
来源：http://fiy.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://weq.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://geo.daria6918.cn

case class User(name: String, age: Int)
来源：http://mwz.bjfxy.top

[T57] Scala：模式匹配
来源：http://slw.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jva.pycfn.com

[T58] Scala：函数定义
来源：http://uhf.yonumen.top

def add(a: Int, b: Int): Int = a + b
来源：http://bzv.ybcxt.top

[T59] Scala：循环
来源：http://htt.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://pjs.jinqigfzy.top

[T60] Scala：折叠
来源：http://ddy.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yiq.yfazqb.com

================================================================================
来源：http://iod.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://spu.yangfankeji.com

================================================================================
来源：http://wwz.ywan-chungtsiang.top

[U01] Py：创建虚拟环境
来源：http://rra.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://sls.fzhhl.top

[U02] Py：导出 / 安装依赖
来源：http://dkh.nwbrower.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aoz.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://xdj.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yhh.dianchejie.cn

[U04] Py：变量调试打印
来源：http://vya.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yzg.yongpay.top

[U05] Py：列表去重且保序
来源：http://hwy.jyoumei.cn

list(dict.fromkeys(arr))
来源：http://epe.fengsongda.top

[U06] Py：合并两个字典
来源：http://ves.nanxuanxn.top

{**a, **b}
来源：http://hks.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://nof.316326.xyz

{v: k for k, v in d.items()}
来源：http://qsa.zhixingplan.top

[U08] Py：展平二维列表
来源：http://rqm.nwbrower.top

[y for x in nested for y in x]
来源：http://erx.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://jad.haohaochexian.top

max(d, key=d.get)
来源：http://msq.iojbl.cn

[U10] Py：按值排序字典
来源：http://ozz.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wcb.smart0.xyz

[U11] Py：生成器表达式
来源：http://dmu.chenzaomai.com

(x * 2 for x in arr)
来源：http://wdc.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://snj.hnqzz.top

Counter(arr).most_common(3)
来源：http://wzn.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://knh.zhoulong.xyz

deque(maxlen=10)
来源：http://ing.hfpthk.cn

[U14] Py：分组收集到列表
来源：http://fny.vehdjk.com

defaultdict(list)
来源：http://uih.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://him.xingfuxueyuan.xyz

t = time.perf_counter()
来源：http://bvk.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://amb.chenzaomai.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xft.vehdjk.com

[U17] Py：初始化日志
来源：http://pvf.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://imk.jiagoushi.top

[U18] Py：预编译正则
来源：http://kvd.shanyushiyangtech.top

pat = re.compile(r"\d+")
来源：http://fsn.zhoulong.xyz

[U19] Py：正则替换带回调
来源：http://fgr.kuanghao11.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bzp.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://ecp.smart0.xyz

@functools.lru_cache(maxsize=None)
来源：http://qbm.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://pzx.dianchejie.cn

@contextlib.contextmanager
来源：http://ebt.zhixingplan.top

[U22] Py：矩阵转置
来源：http://fob.daria6918.cn

list(zip(*m))
来源：http://eku.0kj1m.cn

[U23] Py：分块读取大文件
来源：http://qlk.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pry.cucudq.cn

[U24] Py：路径操作
来源：http://zmz.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://prt.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://jdx.ppjwa.cn

csv.DictReader(f)
来源：http://vpj.jianghu66.top

[U26] Py：并发下载
来源：http://lzb.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mhw.xuetiantiany.cn


<!-- 参考信息 -->