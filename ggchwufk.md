代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://njl.fktsv.cn

[S02] C：变量与格式化输出
来源：http://fhw.cheryme.top

int a = 10; printf("%d\n", a);
来源：http://ndb.cqqwz.cn

[S03] C：读入整数
来源：http://spk.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://lxn.ppjwa.cn

[S04] C：字符串复制
来源：http://gwv.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://han.hfpthk.cn

[S05] C：字符串长度
来源：http://ruu.hywenlv.cn

strlen(s)
来源：http://lvb.haohaochexian.top

[S06] C：字符串比较
来源：http://ovj.zhoulong.xyz

strcmp(a, b) == 0
来源：http://mqd.daxiang520.top

[S07] C：数组遍历求和
来源：http://lsf.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vgn.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://eqv.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vte.uphjek.com

[S09] C：结构体定义与初始化
来源：http://cnz.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nqd.hfpthk.cn

[S10] C：指针与解引用
来源：http://awy.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://mjb.ybcxt.top

[S11] C：逐行读文件
来源：http://qth.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://dgb.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vno.yongpay.top

fclose(f);
来源：http://jgi.316326.xyz

[S12] C：写文件
来源：http://aaa.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xrq.aizwys.cn

[S13] C：宏定义
来源：http://koh.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ztt.ybcxt.top

[S14] C：枚举
来源：http://noc.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://zzb.ppjwa.cn

[S15] C：类型转换
来源：http://gbh.ywan-chungtsiang.top

(double) a / b
来源：http://bqo.vehdjk.com

[S16] C：位操作置位
来源：http://yon.bbcook.cn

x |= (1 << 3);
来源：http://bas.ivvv.top

[S17] C：安全拼接字符串
来源：http://cju.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://slv.ppjwa.cn

[S18] C：命令行参数
来源：http://ayv.vehdjk.com

int main(int argc, char **argv)
来源：http://kij.ydjk.org.cn

[S19] C：快速排序
来源：http://edz.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://knf.yueranfly.top

[S20] C：二分查找
来源：http://umf.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dmv.yuxming.cn

[S21] C：字符类别判断
来源：http://pyb.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eae.yfazqb.com

[S22] C：字符串转数字
来源：http://bqv.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dhu.52xcode.cn

[S23] C：随机数
来源：http://rxp.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ads.havefunace.top

[S24] C：获取本地时间
来源：http://mit.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iji.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://kdy.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://wqz.shanyushiyangtech.top

[S26] C：内存清零
来源：http://anw.jianghu66.top

memset(a, 0, sizeof a);
来源：http://qgi.havefunace.top

[S27] C：定义常量
来源：http://fzc.hesvh.cn

const double PI = 3.14159;
来源：http://vxq.smart0.xyz

[S28] C：静态变量
来源：http://zep.chenzaomai.com

static int counter = 0;
来源：http://znb.hongshengwenyu.top

[S29] C：变参函数
来源：http://brb.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vce.chenzaomai.com

[S30] C：头文件保护
来源：http://dsc.yonumen.top

#ifndef X_H
来源：http://arq.daxiang520.top

#define X_H
来源：http://tzz.bbcook.cn

#endif
来源：http://vxq.cashguo.top

[S31] C++：Hello World
来源：http://svm.gotoacloud.top

#include <iostream>
来源：http://ajd.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://tbc.fzhhl.top

[S32] C++：字符串
来源：http://ype.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://oug.jinqigfzy.top

[S33] C++：vector 增删
来源：http://kmr.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://opq.sjlbkw.cn

[S34] C++：遍历 vector
来源：http://amh.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://iny.jqgufenzy.top

[S35] C++：map
来源：http://hsi.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mgr.hysaishi.cn

[S36] C++：unordered_map
来源：http://aex.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://szn.quarkkingdee.top

[S37] C++：set
来源：http://ngv.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hrw.svipenyu.cn

[S38] C++：排序
来源：http://ree.wangdashe.top

std::sort(v.begin(), v.end());
来源：http://urw.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://yod.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eug.daria6918.cn

[S40] C++：查找元素
来源：http://eza.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://con.52xcode.cn

[S41] C++：类与构造函数
来源：http://udb.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sml.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://xim.xinyue.icu

class B : public Base { public: void f() override {} };
来源：http://ghk.hywenlv.cn

[S43] C++：智能指针
来源：http://krl.yanxiufei.cn

auto p = std::make_unique<int>(5);
来源：http://alt.bbcook.cn

[S44] C++：引用传参
来源：http://obd.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://eqb.zycfv.cn

[S45] C++：lambda
来源：http://uls.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://yde.xuanzx.com

[S46] C++：函数模板
来源：http://atq.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bgb.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://qrz.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uog.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://qdw.sjlbkw.cn

std::ifstream in("a.txt");  std::string line;
来源：http://agz.hnqzz.top

while (std::getline(in, line)) { }
来源：http://jcs.xylfe.cn

[S49] C++：写文件
来源：http://pah.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qmn.bjfxy.top

[S50] C++：格式化数字
来源：http://new.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hwa.iojbl.cn

[S51] C++：显式类型转换
来源：http://nce.aizwys.cn

static_cast<double>(a) / b
来源：http://sjt.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://mfy.xziqi.cn

int size() const noexcept { return n_; }
来源：http://hxx.hnqzz.top

[S53] C++：移动语义
来源：http://muf.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://pat.pengpengdd.cyou

[S54] C++：异常处理
来源：http://poe.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://moq.xylfe.cn

[S55] C++：结构化绑定
来源：http://eeg.aibaodan.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yuo.cqqwz.cn

[S56] C++：optional
来源：http://bjv.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://brt.andypj.xyz

[S57] C++：编译期常量
来源：http://loe.kuanghao11.cn

constexpr int N = 10;
来源：http://awo.jlsjyb.cn

[S58] C++：命名空间
来源：http://qpl.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://ipa.xylfe.cn

[S59] C++：静态断言
来源：http://lqw.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cea.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://idl.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fti.pycfn.com

================================================================================
来源：http://jxs.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dhy.ctjpmb.com

================================================================================
来源：http://fzb.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://ykg.c1oappe.top

println("Hello")
来源：http://rjb.sjlbkw.cn

[T02] Kotlin：变量
来源：http://ffu.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nyc.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://mvv.dianchejie.cn

"值: $b"
来源：http://ytl.shuidangran.top

[T04] Kotlin：空安全
来源：http://imu.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://pjw.sweek.top

[T05] Kotlin：when 表达式
来源：http://tzh.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yfx.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://tsn.sxryk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ssk.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://qrz.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ous.daria6918.cn

[T08] Kotlin：数据类
来源：http://pja.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://tkw.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://kbu.316326.xyz

fun String.exclaim() = this + "!"
来源：http://wmz.shanyushiyangkeji.top

[T10] Kotlin：默认参数
来源：http://zyc.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jbo.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://xgr.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bkq.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://tqn.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://rkz.tanke756.top

[T13] Kotlin：只读 Map
来源：http://hlz.birdmap.top

val m = mapOf("a" to 1)
来源：http://hio.xylfe.cn

[T14] Kotlin：循环
来源：http://erf.nanxinkj.top

for (i in 1..10) println(i)
来源：http://xxo.xuanzx.com

[T15] Kotlin：接口
来源：http://mfw.zycfv.cn

interface Shape { fun area(): Double }
来源：http://ofr.epnwcf.com

[T16] Swift：Hello World
来源：http://zmp.jqgufenzy.top

print("Hello")
来源：http://rvj.jinqigufen.top

[T17] Swift：变量与常量
来源：http://npo.0kj1m.cn

var a = 1;  let b = 2
来源：http://hbe.gzhubu.top

[T18] Swift：字符串插值
来源：http://wqr.yanxiufei.cn

"值: \(b)"
来源：http://enn.zhongyouzk.top

[T19] Swift：可选绑定
来源：http://sxe.ehwqpu.com

if let n = opt { print(n) }
来源：http://nqp.hcnkem.com

[T20] Swift：数组操作
来源：http://spt.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://oct.ydjk.org.cn

[T21] Swift：遍历
来源：http://tde.tianlin.xyz

for x in a { print(x) }
来源：http://jht.feifeiyinyue.top

[T22] Swift：字典
来源：http://bdl.zycfv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qas.zhengqikj.top

[T23] Swift：函数
来源：http://aid.yangfankeji.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dqj.zhiwuduotai.top

[T24] Swift：闭包
来源：http://cri.yanxiufei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jqt.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://itr.zhiwuduotai.top

struct P { var x: Int }
来源：http://cci.tian-w.cn

[T26] Swift：类与重写
来源：http://moc.fehbvm.com

class A: Base { override func f() {} }
来源：http://xiz.cucudq.cn

[T27] Swift：错误处理
来源：http://rvl.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://zju.gzhubu.top

[T28] Swift：枚举
来源：http://lqi.birdmap.top

enum Color { case red, green }
来源：http://dyw.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://uby.fengsongda.top

guard let x = opt else { return }
来源：http://fjc.aibaodan.cn

[T30] Swift：协议
来源：http://apq.bjfxy.top

protocol Shape { func area() -> Double }
来源：http://wke.ctjpmb.com

[T31] Lua：Hello World
来源：http://hvt.zhijiandao.cn

print("Hello")
来源：http://tnm.cucudq.cn

[T32] Lua：局部变量
来源：http://olt.zhengqikj.top

local a = 1
来源：http://noo.bbcook.cn

[T33] Lua：表（数组）
来源：http://ecx.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xkt.dianchejie.cn

[T34] Lua：遍历表
来源：http://xth.xylfe.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://orp.cdnleiting.top

[T35] Lua：字典表
来源：http://zwf.chenzaomai.com

local d = { a = 1 };  d.b = 2
来源：http://fck.yuanzhike.top

[T36] Lua：函数
来源：http://cad.sjlbkw.cn

function add(a, b) return a + b end
来源：http://fnm.tanke756.top

[T37] Lua：字符串拼接
来源：http://rke.xingfuxueyuan.xyz

"a" .. "b"
来源：http://any.yuxming.cn

[T38] Lua：条件
来源：http://ohh.jqgfzy.top

if x > 0 then print("正") end
来源：http://rar.dianchejie.cn

[T39] Lua：模式匹配
来源：http://ase.feifeiyinyue.top

string.find(s, "%d+")
来源：http://mie.zdqjudy.top

[T40] Lua：元表
来源：http://rcm.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://pwi.sweek.top

[T41] Perl：Hello World
来源：http://qlc.xziqi.cn

print "Hello\n";
来源：http://ifi.fengsongda.top

[T42] Perl：变量类型
来源：http://vzp.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vvi.pycfn.com

[T43] Perl：字符串插值
来源：http://vub.yj20258888.top

"值: $a"
来源：http://rvi.wangshuangyany.cn

[T44] Perl：条件
来源：http://efw.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://zay.xylfe.cn

[T45] Perl：数组遍历
来源：http://sma.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://mip.yj202588.top

[T46] Perl：哈希操作
来源：http://whq.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zpo.nwbrower.top

[T47] Perl：正则捕获
来源：http://yrt.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wup.meibo888.top

[T48] Perl：正则替换
来源：http://ffr.ctjpmb.com

$s =~ s/old/new/g;
来源：http://zpg.zdqjudy.top

[T49] Perl：函数
来源：http://cfi.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://skm.aibaodan.cn

[T50] Perl：逐行读文件
来源：http://zlq.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bgw.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://dvd.hammf.cn

[T51] Scala：Hello World
来源：http://jgl.daxiang520.top

println("Hello")
来源：http://nqk.hywenlv.cn

[T52] Scala：变量
来源：http://hdx.jianghu66.top

val a = 1;  var b = 2
来源：http://wbq.andypj.xyz

[T53] Scala：字符串插值
来源：http://rda.shuidangran.top

s"值: $b"
来源：http://pkc.0kj1m.cn

[T54] Scala：集合映射
来源：http://aar.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://qwo.hesvh.cn

[T55] Scala：集合过滤
来源：http://qii.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fne.zhoulong.xyz

[T56] Scala：样例类
来源：http://est.hywenlv.cn

case class User(name: String, age: Int)
来源：http://fld.sufxvd.cn

[T57] Scala：模式匹配
来源：http://cyj.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vhx.shuidangran.top

[T58] Scala：函数定义
来源：http://bmm.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://bab.yuanzhike.top

[T59] Scala：循环
来源：http://hrl.ctjpmb.com

for (i <- 1 to 10) println(i)
来源：http://rhq.haohaochexian.top

[T60] Scala：折叠
来源：http://wzw.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mrk.yj20258888.top

================================================================================
来源：http://rfr.yj202588.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lxf.sysykeji.top

================================================================================
来源：http://ipo.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://azh.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://doe.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://pxg.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jsy.cheryme.top

[U03] Py：加载 .env 配置
来源：http://unl.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lud.52xcode.cn

[U04] Py：变量调试打印
来源：http://crp.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wab.cqqwz.cn

[U05] Py：列表去重且保序
来源：http://jhk.ydzc1.top

list(dict.fromkeys(arr))
来源：http://qoj.aibaodan.cn

[U06] Py：合并两个字典
来源：http://ejo.zdbjq.cn

{**a, **b}
来源：http://dis.nanxinkj.top

[U07] Py：反转字典键值
来源：http://iwj.hcnkem.com

{v: k for k, v in d.items()}
来源：http://jjc.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://xjq.yvedp.cn

[y for x in nested for y in x]
来源：http://osr.pycfn.com

[U09] Py：字典取最大值的键
来源：http://ird.sjlbkw.cn

max(d, key=d.get)
来源：http://qki.andypj.xyz

[U10] Py：按值排序字典
来源：http://cnk.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rmx.yongpay.top

[U11] Py：生成器表达式
来源：http://mpc.daxiang520.top

(x * 2 for x in arr)
来源：http://jqp.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://dbf.jiagoushi.top

Counter(arr).most_common(3)
来源：http://gyd.bbcook.cn

[U13] Py：固定长度队列
来源：http://moq.smart0.xyz

deque(maxlen=10)
来源：http://asm.52xcode.cn

[U14] Py：分组收集到列表
来源：http://ldb.zycfv.cn

defaultdict(list)
来源：http://iyh.c1oappe.top

[U15] Py：高精度计时
来源：http://qxg.haohaochexian.top

t = time.perf_counter()
来源：http://pkm.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://okq.ybcxt.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qac.jqgfzy.top

[U17] Py：初始化日志
来源：http://ftn.xziqi.cn

logging.basicConfig(level=logging.INFO)
来源：http://tjz.52xcode.cn

[U18] Py：预编译正则
来源：http://exa.hywenlv.cn

pat = re.compile(r"\d+")
来源：http://brd.yueranfly.top

[U19] Py：正则替换带回调
来源：http://jaa.dianchejie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://whs.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://ett.ydzc1.top

@functools.lru_cache(maxsize=None)
来源：http://hlx.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://lth.sweek.top

@contextlib.contextmanager
来源：http://enk.cqqwz.cn

[U22] Py：矩阵转置
来源：http://lfs.yj20258.top

list(zip(*m))
来源：http://zin.xziqi.cn

[U23] Py：分块读取大文件
来源：http://yeq.smart0.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://syh.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://nev.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mim.0kj1m.cn


<!-- 参考信息 -->