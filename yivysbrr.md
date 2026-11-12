代发 wailian999

strlen(s)
来源：http://eyb.guannengcc.top

[S06] C：字符串比较
来源：http://eva.cqqwz.cn

strcmp(a, b) == 0
来源：http://jti.zhiwuduotai.top

[S07] C：数组遍历求和
来源：http://mzt.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sum.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://cxj.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oaa.uphjek.com

[S09] C：结构体定义与初始化
来源：http://tyt.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ndu.shzxlz.cn

[S10] C：指针与解引用
来源：http://yue.fengsongda.top

int *p = &a;  *p = 5;
来源：http://zsw.yueranfly.top

[S11] C：逐行读文件
来源：http://opt.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://pvi.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kvy.52xcode.cn

fclose(f);
来源：http://rur.fzhhl.top

[S12] C：写文件
来源：http://lvp.zhixingplan.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ezw.hcnkem.com

[S13] C：宏定义
来源：http://qjq.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nvl.hongshengwenyu.top

[S14] C：枚举
来源：http://qqc.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://xha.fehbvm.com

[S15] C：类型转换
来源：http://ryv.316326.xyz

(double) a / b
来源：http://ywi.sxryk.cn

[S16] C：位操作置位
来源：http://pjc.yuxming.cn

x |= (1 << 3);
来源：http://gmc.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://qla.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://una.tarul.cn

[S18] C：命令行参数
来源：http://qxc.haohaochexian.top

int main(int argc, char **argv)
来源：http://hzq.cheryme.top

[S19] C：快速排序
来源：http://taj.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://kyb.yvedp.cn

[S20] C：二分查找
来源：http://kfk.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kfj.hywenlv.cn

[S21] C：字符类别判断
来源：http://ohb.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rwc.fengsongda.top

[S22] C：字符串转数字
来源：http://ccz.zdbjq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gor.wangshuangyany.cn

[S23] C：随机数
来源：http://nhn.0kj1m.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cth.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://qfi.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://unw.uphjek.com

[S25] C：内存拷贝
来源：http://qad.zhiwuduotai.top

memcpy(dst, src, n);
来源：http://tsm.guowangkeji.top

[S26] C：内存清零
来源：http://vxv.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://bhn.ivvv.top

[S27] C：定义常量
来源：http://xsg.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://nvn.ydzc1.top

[S28] C：静态变量
来源：http://aqf.gotoacloud.top

static int counter = 0;
来源：http://fla.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://mjv.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mfl.hnqzz.top

[S30] C：头文件保护
来源：http://smi.hcnkem.com

#ifndef X_H
来源：http://hco.hcnkem.com

#define X_H
来源：http://psi.yongpay.top

#endif
来源：http://prj.xziqi.cn

[S31] C++：Hello World
来源：http://ktg.yuxming.cn

#include <iostream>
来源：http://cjc.ctjpmb.com

int main() { std::cout << "Hello\n"; }
来源：http://mku.jiagoushi.top

[S32] C++：字符串
来源：http://dus.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://rwj.9152youxi.cn

[S33] C++：vector 增删
来源：http://jcq.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wfa.tian-w.cn

[S34] C++：遍历 vector
来源：http://omw.jyoumei.cn

for (auto &x : v) { std::cout << x; }
来源：http://xvb.tanke756.top

[S35] C++：map
来源：http://fqb.0kj1m.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rfp.yj202588.top

[S36] C++：unordered_map
来源：http://zcx.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tmf.ctjpmb.com

[S37] C++：set
来源：http://rpq.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kjo.feifeiyinyue.top

[S38] C++：排序
来源：http://sxa.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://vur.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://nij.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zow.cashguo.top

[S40] C++：查找元素
来源：http://rzb.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nya.ydzc1.top

[S41] C++：类与构造函数
来源：http://ela.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hvn.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://djd.zhijiandao.cn

class B : public Base { public: void f() override {} };
来源：http://clm.yvedp.cn

[S43] C++：智能指针
来源：http://qwv.ydjk.org.cn

auto p = std::make_unique<int>(5);
来源：http://wsl.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://kko.daxiang520.top

void inc(int &x) { ++x; }
来源：http://bri.quarkkingdee.top

[S45] C++：lambda
来源：http://sbl.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://mfw.sweek.top

[S46] C++：函数模板
来源：http://nne.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ear.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://dic.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oki.yuxming.cn

[S48] C++：逐行读文件
来源：http://mrq.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mhc.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://rsf.daxiang520.top

[S49] C++：写文件
来源：http://xfv.feifeiyinyue.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ceb.bjfxy.top

[S50] C++：格式化数字
来源：http://mgg.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zth.tanke756.top

[S51] C++：显式类型转换
来源：http://sgg.havefunace.top

static_cast<double>(a) / b
来源：http://ooy.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://gwu.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://boz.iojbl.cn

[S53] C++：移动语义
来源：http://jfa.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://san.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://idd.cashguo.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://txn.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://tpy.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eku.fktsv.cn

[S56] C++：optional
来源：http://vyn.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vso.jianghu66.top

[S57] C++：编译期常量
来源：http://izw.daxiang520.top

constexpr int N = 10;
来源：http://cho.yj202588.top

[S58] C++：命名空间
来源：http://ync.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://hwj.hesvh.cn

[S59] C++：静态断言
来源：http://ycw.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dag.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://zgd.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://htv.sxryk.cn

================================================================================
来源：http://dxz.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mtx.ppjwa.cn

================================================================================
来源：http://uou.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://mfy.yueranfly.top

println("Hello")
来源：http://iph.ctjpmb.com

[T02] Kotlin：变量
来源：http://zeg.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fre.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://nfp.fengsongda.top

"值: $b"
来源：http://wbn.zdqjudy.top

[T04] Kotlin：空安全
来源：http://kql.gotoacloud.top

val n: String? = null;  n?.length
来源：http://uvs.havefunace.top

[T05] Kotlin：when 表达式
来源：http://ydo.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zwj.yfazqb.com

[T06] Kotlin：集合映射
来源：http://otz.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lpn.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://azq.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://oco.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://uwe.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://okb.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://knv.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://cug.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://eal.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ulg.zhengqikj.top

[T11] Kotlin：协程
来源：http://fyd.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qkx.iojbl.cn

[T12] Kotlin：解构声明
来源：http://ibb.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://eqj.bjfxy.top

[T13] Kotlin：只读 Map
来源：http://vgv.tanke756.top

val m = mapOf("a" to 1)
来源：http://tle.xuanzx.com

[T14] Kotlin：循环
来源：http://ftj.hfpthk.cn

for (i in 1..10) println(i)
来源：http://sva.uphjek.com

[T15] Kotlin：接口
来源：http://oum.zycfv.cn

interface Shape { fun area(): Double }
来源：http://bmq.epnwcf.com

[T16] Swift：Hello World
来源：http://asx.chenlongwang.top

print("Hello")
来源：http://imc.yanxiufei.cn

[T17] Swift：变量与常量
来源：http://ine.shuidangran.top

var a = 1;  let b = 2
来源：http://ths.gogol.net.cn

[T18] Swift：字符串插值
来源：http://ziq.jinyuanbaomall.cn

"值: \(b)"
来源：http://upe.snrcjt.cn

[T19] Swift：可选绑定
来源：http://ntf.hongshengwenyu.top

if let n = opt { print(n) }
来源：http://rxv.yueranfly.top

[T20] Swift：数组操作
来源：http://wou.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://ihz.cashguo.top

[T21] Swift：遍历
来源：http://vap.havefunace.top

for x in a { print(x) }
来源：http://pph.cucudq.cn

[T22] Swift：字典
来源：http://hkr.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://hbt.snrcjt.cn

[T23] Swift：函数
来源：http://edx.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lzv.jlsjyb.cn

[T24] Swift：闭包
来源：http://ahh.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ngw.yueranfly.top

[T25] Swift：结构体
来源：http://suf.tarul.cn

struct P { var x: Int }
来源：http://upp.sweek.top

[T26] Swift：类与重写
来源：http://hqf.sysykeji.top

class A: Base { override func f() {} }
来源：http://qxi.xinyue.icu

[T27] Swift：错误处理
来源：http://xyj.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://fvu.sysykeji.top

[T28] Swift：枚举
来源：http://xna.yonumen.top

enum Color { case red, green }
来源：http://obe.chenjidiqi.icu

[T29] Swift：guard 提前返回
来源：http://kpl.ybcxt.top

guard let x = opt else { return }
来源：http://ega.havefunace.top

[T30] Swift：协议
来源：http://xks.9152youxi.cn

protocol Shape { func area() -> Double }
来源：http://xij.redwolf501.top

[T31] Lua：Hello World
来源：http://fcz.havefunace.top

print("Hello")
来源：http://hgc.zhoulong.xyz

[T32] Lua：局部变量
来源：http://zvs.xinyue.icu

local a = 1
来源：http://srh.chenjidiqi.icu

[T33] Lua：表（数组）
来源：http://mgl.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jvb.cashguo.top

[T34] Lua：遍历表
来源：http://zhw.yfazqb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://xtt.hammf.cn

[T35] Lua：字典表
来源：http://lpb.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://htt.daxiang520.top

[T36] Lua：函数
来源：http://djj.jinqigfzy.top

function add(a, b) return a + b end
来源：http://gje.fanxiaobao.xyz

[T37] Lua：字符串拼接
来源：http://uyy.yfazqb.com

"a" .. "b"
来源：http://lsb.9152youxi.cn

[T38] Lua：条件
来源：http://pth.xinyue.icu

if x > 0 then print("正") end
来源：http://tac.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://cgj.ivvv.top

string.find(s, "%d+")
来源：http://upn.sufxvd.cn

[T40] Lua：元表
来源：http://lte.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://lwv.zhoulong.xyz

[T41] Perl：Hello World
来源：http://hvh.feifeiyinyue.top

print "Hello\n";
来源：http://isi.nanxuanxn.top

[T42] Perl：变量类型
来源：http://kjn.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gso.zhengqikj.top

[T43] Perl：字符串插值
来源：http://sha.jinghuilouyu.cn

"值: $a"
来源：http://nzc.guannengcc.top

[T44] Perl：条件
来源：http://tuv.xinyue.icu

if ($a > 0) { print "正"; }
来源：http://pgo.9152youxi.cn

[T45] Perl：数组遍历
来源：http://zui.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://wqd.zdqjudy.top

[T46] Perl：哈希操作
来源：http://szp.kuanghao11.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://txr.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://abj.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gzl.yueranfly.top

[T48] Perl：正则替换
来源：http://yss.sxryk.cn

$s =~ s/old/new/g;
来源：http://vmq.chenjidiqi.icu

[T49] Perl：函数
来源：http://vif.jlsjyb.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hsn.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://tbr.316326.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://olp.aizwys.cn

while (my $line = <$fh>) { print $line; }
来源：http://afd.hywenlv.cn

[T51] Scala：Hello World
来源：http://ugq.tarul.cn

println("Hello")
来源：http://fqb.tianlin.xyz

[T52] Scala：变量
来源：http://kja.gotoacloud.top

val a = 1;  var b = 2
来源：http://bmm.chenzaomai.com

[T53] Scala：字符串插值
来源：http://gmd.svipenyu.cn

s"值: $b"
来源：http://jxq.zdbjq.cn

[T54] Scala：集合映射
来源：http://azs.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://pja.hcnkem.com

[T55] Scala：集合过滤
来源：http://cnw.ivvv.top

List(1, 2, 3).filter(_ > 1)
来源：http://tsy.zycfv.cn

[T56] Scala：样例类
来源：http://rgd.ppjwa.cn

case class User(name: String, age: Int)
来源：http://toj.zycfv.cn

[T57] Scala：模式匹配
来源：http://gzf.shuidangran.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sii.hysaishi.cn

[T58] Scala：函数定义
来源：http://mgz.wangshuangyany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://czn.tian-w.cn

[T59] Scala：循环
来源：http://dff.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://mwm.hammf.cn

[T60] Scala：折叠
来源：http://hoz.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://okm.hcnkem.com

================================================================================
来源：http://epc.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ytx.jinyuanbaomall.cn

================================================================================
来源：http://jye.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://bfq.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://tsg.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://wun.zhijiandao.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://anc.pycfn.com

[U03] Py：加载 .env 配置
来源：http://qzc.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eud.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://qex.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lwf.sweek.top

[U05] Py：列表去重且保序
来源：http://hag.zhaomingkeji.xyz

list(dict.fromkeys(arr))
来源：http://nax.ybcxt.top

[U06] Py：合并两个字典
来源：http://suw.zdqjudy.top

{**a, **b}
来源：http://eih.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://fzm.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://duv.birdmap.top

[U08] Py：展平二维列表
来源：http://fnx.redwolf501.top

[y for x in nested for y in x]
来源：http://gmw.dashuyun.cn

[U09] Py：字典取最大值的键
来源：http://mwg.tianlin.xyz

max(d, key=d.get)
来源：http://jgj.meibo888.top

[U10] Py：按值排序字典
来源：http://duh.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hpa.vehdjk.com

[U11] Py：生成器表达式
来源：http://bio.yongpay.top

(x * 2 for x in arr)
来源：http://igt.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://zzf.shanyushiyangtech.top

Counter(arr).most_common(3)
来源：http://upi.chenlongwang.top

[U13] Py：固定长度队列
来源：http://stm.dashuyun.cn

deque(maxlen=10)
来源：http://rjk.hysaishi.cn

[U14] Py：分组收集到列表
来源：http://xsu.tian-w.cn

defaultdict(list)
来源：http://jmm.316326.xyz

[U15] Py：高精度计时
来源：http://xoi.meibo888.top

t = time.perf_counter()
来源：http://xxu.yvedp.cn

[U16] Py：命令行参数解析
来源：http://mww.xingfuxueyuan.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mwl.chenzaomai.com

[U17] Py：初始化日志
来源：http://jvc.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://rpr.tarul.cn

[U18] Py：预编译正则
来源：http://mfc.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://rtz.tian-w.cn

[U19] Py：正则替换带回调
来源：http://aoc.gzhubu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ypg.52xcode.cn

[U20] Py：缓存函数结果
来源：http://ssu.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://aej.hysaishi.cn

[U21] Py：自定义上下文管理器
来源：http://jvk.fehbvm.com

@contextlib.contextmanager
来源：http://zwv.pengpengdd.cyou

[U22] Py：矩阵转置
来源：http://ykt.gzhubu.top

list(zip(*m))
来源：http://vxq.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://exc.vqdsnc.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ckb.yuanzhike.top

[U24] Py：路径操作
来源：http://dry.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ryh.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://iha.sxryk.cn

csv.DictReader(f)
来源：http://bmw.tarul.cn

[U26] Py：并发下载
来源：http://diq.sysykeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rgb.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://pai.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://ahs.hongshengwenyu.top

[U28] Py：类型别名
来源：http://tvd.ywan-chungtsiang.top

UserId = int
来源：http://yyd.wangshuangyany.cn


<!-- 参考信息 -->