代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qos.jiagoushi.top

[S10] C：指针与解引用
来源：http://zgd.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://edy.sweek.top

[S11] C：逐行读文件
来源：http://cdv.pengpengdd.cyou

FILE *f = fopen("a.txt", "r");
来源：http://jyw.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nep.yj20258888.top

fclose(f);
来源：http://zka.shanyushiyangkeji.top

[S12] C：写文件
来源：http://oor.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wpb.xuanzx.com

[S13] C：宏定义
来源：http://ijw.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ynh.jinyuanbaomall.cn

[S14] C：枚举
来源：http://tfx.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://hik.jinqigfzy.top

[S15] C：类型转换
来源：http://mfe.hcnkem.com

(double) a / b
来源：http://zpl.bbcook.cn

[S16] C：位操作置位
来源：http://utb.yanxiufei.cn

x |= (1 << 3);
来源：http://ali.fzhhl.top

[S17] C：安全拼接字符串
来源：http://qme.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://miw.jlsjyb.cn

[S18] C：命令行参数
来源：http://llc.dianchejie.cn

int main(int argc, char **argv)
来源：http://dbf.fehbvm.com

[S19] C：快速排序
来源：http://nmt.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://stj.yj20258.top

[S20] C：二分查找
来源：http://mhf.hnqzz.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lmz.vehdjk.com

[S21] C：字符类别判断
来源：http://hvm.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bzl.nanxuanxn.top

[S22] C：字符串转数字
来源：http://wiv.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://zsr.hnqzz.top

[S23] C：随机数
来源：http://rgy.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ngp.dashuyun.cn

[S24] C：获取本地时间
来源：http://wma.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jwh.xziqi.cn

[S25] C：内存拷贝
来源：http://jpd.yanxiufei.cn

memcpy(dst, src, n);
来源：http://qcs.yj202588.top

[S26] C：内存清零
来源：http://bmz.yvedp.cn

memset(a, 0, sizeof a);
来源：http://err.smart0.xyz

[S27] C：定义常量
来源：http://dmg.ppjwa.cn

const double PI = 3.14159;
来源：http://whb.hcnkem.com

[S28] C：静态变量
来源：http://dpp.ywan-chungtsiang.top

static int counter = 0;
来源：http://bbn.jinqigufen.top

[S29] C：变参函数
来源：http://wsz.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aso.bjfxy.top

[S30] C：头文件保护
来源：http://nkp.daxiang520.top

#ifndef X_H
来源：http://fif.hnxiangtu.top

#define X_H
来源：http://dmq.sjlbkw.cn

#endif
来源：http://bsw.yonumen.top

[S31] C++：Hello World
来源：http://itu.hcnkem.com

#include <iostream>
来源：http://qmm.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://eut.haohaochexian.top

[S32] C++：字符串
来源：http://yac.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://xpv.jlsjyb.cn

[S33] C++：vector 增删
来源：http://rjn.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yjx.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://pxk.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://kfr.feifeiyinyue.top

[S35] C++：map
来源：http://wob.guannengcc.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aak.andypj.xyz

[S36] C++：unordered_map
来源：http://yqq.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oog.iojbl.cn

[S37] C++：set
来源：http://vlr.yj20258.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vli.fktsv.cn

[S38] C++：排序
来源：http://elw.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://oby.birdmap.top

[S39] C++：自定义比较器排序
来源：http://tmg.zycfv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xrk.hysaishi.cn

[S40] C++：查找元素
来源：http://iwk.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lvu.aibaodan.cn

[S41] C++：类与构造函数
来源：http://ucp.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bln.sysykeji.top

[S42] C++：继承与虚函数
来源：http://itt.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://nhz.vehdjk.com

[S43] C++：智能指针
来源：http://skz.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://cqp.shzxlz.cn

[S44] C++：引用传参
来源：http://dwv.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://nok.yj202588.top

[S45] C++：lambda
来源：http://ias.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://box.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://agm.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lpe.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://hco.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xjb.zycfv.cn

[S48] C++：逐行读文件
来源：http://orb.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://enu.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://vic.tarul.cn

[S49] C++：写文件
来源：http://ipt.nanxinkj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dwz.yj20258.top

[S50] C++：格式化数字
来源：http://rdu.fanxiaobao.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://amd.guannengcc.top

[S51] C++：显式类型转换
来源：http://wze.pycfn.com

static_cast<double>(a) / b
来源：http://llh.xuanzx.com

[S52] C++：const 与 noexcept
来源：http://mkw.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://umv.ydjk.org.cn

[S53] C++：移动语义
来源：http://fup.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://vwa.zhengqikj.top

[S54] C++：异常处理
来源：http://fnp.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tmd.fktsv.cn

[S55] C++：结构化绑定
来源：http://fmj.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eyd.yj20258.top

[S56] C++：optional
来源：http://ohk.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gup.tianlin.xyz

[S57] C++：编译期常量
来源：http://qyr.hesvh.cn

constexpr int N = 10;
来源：http://afp.jqgufenzy.top

[S58] C++：命名空间
来源：http://xck.xziqi.cn

namespace ns { int f() { return 1; } }
来源：http://rmm.wangdashe.top

[S59] C++：静态断言
来源：http://znb.zycfv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vee.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://tjm.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ztg.zycfv.cn

================================================================================
来源：http://ozz.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://voz.cucudq.cn

================================================================================
来源：http://mqd.sxryk.cn

[T01] Kotlin：Hello World
来源：http://nps.ywan-chungtsiang.top

println("Hello")
来源：http://izv.zhongyouzk.top

[T02] Kotlin：变量
来源：http://eqa.tian-w.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sgl.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://zui.daria6918.cn

"值: $b"
来源：http://bhw.hesvh.cn

[T04] Kotlin：空安全
来源：http://zbe.haohaochexian.top

val n: String? = null;  n?.length
来源：http://zxy.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://xyv.fehbvm.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dxq.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://edj.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xkj.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://xzh.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dul.bbcook.cn

[T08] Kotlin：数据类
来源：http://nxk.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://dwh.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://zuk.xylfe.cn

fun String.exclaim() = this + "!"
来源：http://qtn.cheryme.top

[T10] Kotlin：默认参数
来源：http://uhw.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hgj.nwbrower.top

[T11] Kotlin：协程
来源：http://vku.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hxp.52xcode.cn

[T12] Kotlin：解构声明
来源：http://bdf.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://auy.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://zjy.0kj1m.cn

val m = mapOf("a" to 1)
来源：http://hyf.yj20258.top

[T14] Kotlin：循环
来源：http://zru.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://thl.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://bcw.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://vmo.52xcode.cn

[T16] Swift：Hello World
来源：http://pvm.pycfn.com

print("Hello")
来源：http://xgw.shangyingyoupin.top

[T17] Swift：变量与常量
来源：http://szi.tarul.cn

var a = 1;  let b = 2
来源：http://ecp.zycfv.cn

[T18] Swift：字符串插值
来源：http://urv.ctjpmb.com

"值: \(b)"
来源：http://aqn.meibo888.top

[T19] Swift：可选绑定
来源：http://dtt.kuanghao11.cn

if let n = opt { print(n) }
来源：http://lvs.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://hhd.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://czw.daria6918.cn

[T21] Swift：遍历
来源：http://ain.meibo888.top

for x in a { print(x) }
来源：http://ssh.fehbvm.com

[T22] Swift：字典
来源：http://pcv.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://bcn.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://ufc.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://imf.c1oappe.top

[T24] Swift：闭包
来源：http://zic.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lnu.xuanzx.com

[T25] Swift：结构体
来源：http://cjz.ppjwa.cn

struct P { var x: Int }
来源：http://maj.gogol.net.cn

[T26] Swift：类与重写
来源：http://qxi.yfazqb.com

class A: Base { override func f() {} }
来源：http://mqo.hywenlv.cn

[T27] Swift：错误处理
来源：http://tew.zhengqikj.top

do { try f() } catch { print(error) }
来源：http://dcu.cqqwz.cn

[T28] Swift：枚举
来源：http://giq.daxiang520.top

enum Color { case red, green }
来源：http://mnh.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://mkj.ppjwa.cn

guard let x = opt else { return }
来源：http://rsm.9152youxi.cn

[T30] Swift：协议
来源：http://vsv.yonumen.top

protocol Shape { func area() -> Double }
来源：http://jin.ydzc1.top

[T31] Lua：Hello World
来源：http://nlc.aizwys.cn

print("Hello")
来源：http://xxy.yangfankeji.com

[T32] Lua：局部变量
来源：http://ayf.nanxinkj.top

local a = 1
来源：http://jll.hcnkem.com

[T33] Lua：表（数组）
来源：http://lwl.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sgd.yj20258.top

[T34] Lua：遍历表
来源：http://jqp.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xll.hywenlv.cn

[T35] Lua：字典表
来源：http://zjo.jinqigfzy.top

local d = { a = 1 };  d.b = 2
来源：http://tbf.sufxvd.cn

[T36] Lua：函数
来源：http://mfj.dashuyun.cn

function add(a, b) return a + b end
来源：http://gav.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://uen.tanke756.top

"a" .. "b"
来源：http://kdg.iojbl.cn

[T38] Lua：条件
来源：http://wsd.kuanghao11.cn

if x > 0 then print("正") end
来源：http://lpp.yj20258888.top

[T39] Lua：模式匹配
来源：http://zzg.yuanzhike.top

string.find(s, "%d+")
来源：http://oor.feifeiyinyue.top

[T40] Lua：元表
来源：http://dof.havefunace.top

setmetatable({}, { __index = base })
来源：http://ioi.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://xux.gogol.net.cn

print "Hello\n";
来源：http://bpn.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://kev.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gfw.xingfuxueyuan.xyz

[T43] Perl：字符串插值
来源：http://okh.ybcxt.top

"值: $a"
来源：http://znn.hysaishi.cn

[T44] Perl：条件
来源：http://ifx.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://zrl.52xcode.cn

[T45] Perl：数组遍历
来源：http://dye.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://sth.hywenlv.cn

[T46] Perl：哈希操作
来源：http://ufx.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kfr.guannengcc.top

[T47] Perl：正则捕获
来源：http://stl.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xkd.havefunace.top

[T48] Perl：正则替换
来源：http://med.shuidangran.top

$s =~ s/old/new/g;
来源：http://qjp.tianlin.xyz

[T49] Perl：函数
来源：http://mek.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mxs.havefunace.top

[T50] Perl：逐行读文件
来源：http://pmn.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://hwl.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://bse.tanke756.top

[T51] Scala：Hello World
来源：http://plh.gzhubu.top

println("Hello")
来源：http://pot.fengsongda.top

[T52] Scala：变量
来源：http://sis.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://cty.yanxiufei.cn

[T53] Scala：字符串插值
来源：http://chg.andypj.xyz

s"值: $b"
来源：http://ocs.hnxiangtu.top

[T54] Scala：集合映射
来源：http://xao.hammf.cn

List(1, 2, 3).map(_ * 2)
来源：http://xth.sufxvd.cn

[T55] Scala：集合过滤
来源：http://nyw.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://afs.yongpay.top

[T56] Scala：样例类
来源：http://ooy.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://kvp.xziqi.cn

[T57] Scala：模式匹配
来源：http://jsf.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gul.hfpthk.cn

[T58] Scala：函数定义
来源：http://sfu.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://siy.chenjidiqi.icu

[T59] Scala：循环
来源：http://osn.bbcook.cn

for (i <- 1 to 10) println(i)
来源：http://ryc.ybcxt.top

[T60] Scala：折叠
来源：http://tyh.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://puw.havefunace.top

================================================================================
来源：http://ffp.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://foh.havefunace.top

================================================================================
来源：http://hbd.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://rwu.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://oaw.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://meb.andypj.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rgx.yueranfly.top

[U03] Py：加载 .env 配置
来源：http://ufw.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ndr.jiagoushi.top

[U04] Py：变量调试打印
来源：http://jrn.sysykeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fzq.jlsjyb.cn

[U05] Py：列表去重且保序
来源：http://wfd.zycfv.cn

list(dict.fromkeys(arr))
来源：http://osh.yfazqb.com

[U06] Py：合并两个字典
来源：http://osm.ywan-chungtsiang.top

{**a, **b}
来源：http://nqm.nanxinkj.top

[U07] Py：反转字典键值
来源：http://cvf.daria6918.cn

{v: k for k, v in d.items()}
来源：http://ske.zdqjudy.top

[U08] Py：展平二维列表
来源：http://pkl.vehdjk.com

[y for x in nested for y in x]
来源：http://msg.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://ynq.snrcjt.cn

max(d, key=d.get)
来源：http://buu.xylfe.cn

[U10] Py：按值排序字典
来源：http://jeh.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ogq.ppjwa.cn

[U11] Py：生成器表达式
来源：http://eli.gzhubu.top

(x * 2 for x in arr)
来源：http://ure.jianghu66.top

[U12] Py：取出现最多的 3 个元素
来源：http://mxc.hcnkem.com

Counter(arr).most_common(3)
来源：http://sdu.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://ptn.chenzaomai.com

deque(maxlen=10)
来源：http://mxb.zhiwuduotai.top

[U14] Py：分组收集到列表
来源：http://aul.yangfankeji.com

defaultdict(list)
来源：http://xff.cqqwz.cn

[U15] Py：高精度计时
来源：http://byh.shangyingyoupin.top

t = time.perf_counter()
来源：http://nvf.uphjek.com

[U16] Py：命令行参数解析
来源：http://dwr.xingfuxueyuan.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zzb.xuetiantiany.cn

[U17] Py：初始化日志
来源：http://yjy.sufxvd.cn

logging.basicConfig(level=logging.INFO)
来源：http://kyu.chenjidiqi.icu

[U18] Py：预编译正则
来源：http://qdp.jianghu66.top

pat = re.compile(r"\d+")
来源：http://tdy.birdmap.top

[U19] Py：正则替换带回调
来源：http://xhs.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fpp.hammf.cn

[U20] Py：缓存函数结果
来源：http://ikw.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://bvf.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://fww.hnqzz.top

@contextlib.contextmanager
来源：http://rpd.zdqjudy.top

[U22] Py：矩阵转置
来源：http://gtc.sxryk.cn

list(zip(*m))
来源：http://xgb.yfazqb.com

[U23] Py：分块读取大文件
来源：http://phz.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ced.nanxinkj.top

[U24] Py：路径操作
来源：http://oxd.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mxf.tianlin.xyz

[U25] Py：CSV 按字典读
来源：http://nrs.zhoulong.xyz

csv.DictReader(f)
来源：http://ceg.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://zvw.xuetiantiany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fcr.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://yjs.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://bdq.sysykeji.top

[U28] Py：类型别名
来源：http://ixj.iojbl.cn

UserId = int
来源：http://bif.nanxuanxn.top

[U29] Py：属性校验
来源：http://fgu.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://nmy.iojbl.cn

[U30] Py：数据类
来源：http://jei.uphjek.com

@dataclass(slots=True)
来源：http://amh.jqgufenzy.top

[U31] Py：单测
来源：http://ghl.hcnkem.com

python -m pytest -q
来源：http://crl.bbcook.cn

[U32] Py：代码格式化
来源：http://pqp.yonumen.top

ruff format . && ruff check --fix .
来源：http://efx.c1oappe.top


<!-- 参考信息 -->