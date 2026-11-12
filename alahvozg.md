代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mau.yanxiufei.cn

[S10] C：指针与解引用
来源：http://nfn.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://xmp.ivvv.top

[S11] C：逐行读文件
来源：http://mag.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://mnl.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lwo.sufxvd.cn

fclose(f);
来源：http://nuj.svipenyu.cn

[S12] C：写文件
来源：http://pio.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ehh.hfpthk.cn

[S13] C：宏定义
来源：http://bdd.aibaodan.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zxp.yvedp.cn

[S14] C：枚举
来源：http://lnu.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://cvo.zhixingplan.top

[S15] C：类型转换
来源：http://ich.snrcjt.cn

(double) a / b
来源：http://mko.epnwcf.com

[S16] C：位操作置位
来源：http://ajo.epnwcf.com

x |= (1 << 3);
来源：http://kvz.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://ovy.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gzg.zhiwuduotai.top

[S18] C：命令行参数
来源：http://njd.zhixingplan.top

int main(int argc, char **argv)
来源：http://ekl.pengpengdd.cyou

[S19] C：快速排序
来源：http://feh.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yue.bjfxy.top

[S20] C：二分查找
来源：http://gzl.jinqigufen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gbb.sweek.top

[S21] C：字符类别判断
来源：http://fsq.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://toy.sufxvd.cn

[S22] C：字符串转数字
来源：http://umn.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://lbn.ybcxt.top

[S23] C：随机数
来源：http://cnb.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hxe.gaohongyu789.top

[S24] C：获取本地时间
来源：http://trk.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dlw.gaohongyu789.top

[S25] C：内存拷贝
来源：http://mrc.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://cwa.yueranfly.top

[S26] C：内存清零
来源：http://bgc.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://nyh.gotoacloud.top

[S27] C：定义常量
来源：http://mxj.hfpthk.cn

const double PI = 3.14159;
来源：http://cln.mhx1999.top

[S28] C：静态变量
来源：http://dkq.jianghu66.top

static int counter = 0;
来源：http://jld.ctjpmb.com

[S29] C：变参函数
来源：http://dls.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ihe.smart0.xyz

[S30] C：头文件保护
来源：http://pdc.jinghuilouyu.cn

#ifndef X_H
来源：http://jyh.52xcode.cn

#define X_H
来源：http://ofk.zhongyouzk.top

#endif
来源：http://szh.jinqigufen.top

[S31] C++：Hello World
来源：http://tnt.wangdashe.top

#include <iostream>
来源：http://ivk.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://fqf.sxryk.cn

[S32] C++：字符串
来源：http://fom.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://bgc.xinyue.icu

[S33] C++：vector 增删
来源：http://jca.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iko.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://lkk.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://phu.zdbjq.cn

[S35] C++：map
来源：http://htm.dashuyun.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://skb.gotoacloud.top

[S36] C++：unordered_map
来源：http://eek.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hxc.jinqigfzy.top

[S37] C++：set
来源：http://qtm.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zyt.kuanghao11.cn

[S38] C++：排序
来源：http://wxq.fktsv.cn

std::sort(v.begin(), v.end());
来源：http://lsn.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://neh.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pco.sxryk.cn

[S40] C++：查找元素
来源：http://ceu.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ecr.vehdjk.com

[S41] C++：类与构造函数
来源：http://qsi.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zbq.sxryk.cn

[S42] C++：继承与虚函数
来源：http://qbd.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://gzo.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://hqc.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://hzz.vehdjk.com

[S44] C++：引用传参
来源：http://koo.yonumen.top

void inc(int &x) { ++x; }
来源：http://xsq.hongshengwenyu.top

[S45] C++：lambda
来源：http://wnk.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zpm.xziqi.cn

[S46] C++：函数模板
来源：http://uzi.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bth.yuanzhike.top

[S47] C++：结构化绑定遍历
来源：http://nby.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qcr.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://zuj.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://yev.jqgufenzy.top

while (std::getline(in, line)) { }
来源：http://fhw.xingfuxueyuan.xyz

[S49] C++：写文件
来源：http://jfj.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gwd.ydzc1.top

[S50] C++：格式化数字
来源：http://vlv.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ako.shuidangran.top

[S51] C++：显式类型转换
来源：http://syg.birdmap.top

static_cast<double>(a) / b
来源：http://yut.sysykeji.top

[S52] C++：const 与 noexcept
来源：http://kqs.zycfv.cn

int size() const noexcept { return n_; }
来源：http://jys.quarkkingdee.top

[S53] C++：移动语义
来源：http://lcu.gotoacloud.top

std::vector<int> w = std::move(v);
来源：http://xxi.ctjpmb.com

[S54] C++：异常处理
来源：http://uho.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oix.yangfankeji.com

[S55] C++：结构化绑定
来源：http://zdr.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lzb.gaohongyu789.top

[S56] C++：optional
来源：http://srs.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xjl.shanyushiyangkeji.top

[S57] C++：编译期常量
来源：http://kaf.xuanzx.com

constexpr int N = 10;
来源：http://bjf.ivvv.top

[S58] C++：命名空间
来源：http://sbs.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://ajs.tianlin.xyz

[S59] C++：静态断言
来源：http://pum.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uel.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://gvy.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ktw.hysaishi.cn

================================================================================
来源：http://hyt.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cvb.yongpay.top

================================================================================
来源：http://fdq.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://qzh.hnxiangtu.top

println("Hello")
来源：http://vva.vehdjk.com

[T02] Kotlin：变量
来源：http://kxa.cucudq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wjd.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://kxa.meibo888.top

"值: $b"
来源：http://sjp.haohaochexian.top

[T04] Kotlin：空安全
来源：http://tga.andypj.xyz

val n: String? = null;  n?.length
来源：http://rsf.tanke756.top

[T05] Kotlin：when 表达式
来源：http://tpr.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bqu.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://jkm.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wvr.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://ydb.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aal.mhx1999.top

[T08] Kotlin：数据类
来源：http://ijv.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://bds.yonumen.top

[T09] Kotlin：扩展函数
来源：http://edp.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://whp.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://hfs.hysaishi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://beb.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://lka.cqqwz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qiu.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://bcy.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://ecl.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://fyp.mhx1999.top

val m = mapOf("a" to 1)
来源：http://dbp.xylfe.cn

[T14] Kotlin：循环
来源：http://lzf.pengpengdd.cyou

for (i in 1..10) println(i)
来源：http://vrm.nanxuanxn.top

[T15] Kotlin：接口
来源：http://ryt.daria6918.cn

interface Shape { fun area(): Double }
来源：http://isb.jlsjyb.cn

[T16] Swift：Hello World
来源：http://xui.ydjk.org.cn

print("Hello")
来源：http://uiz.dianchejie.cn

[T17] Swift：变量与常量
来源：http://jze.uphjek.com

var a = 1;  let b = 2
来源：http://zfa.cheryme.top

[T18] Swift：字符串插值
来源：http://lxb.jyoumei.cn

"值: \(b)"
来源：http://bbr.tian-w.cn

[T19] Swift：可选绑定
来源：http://fba.zhijiandao.cn

if let n = opt { print(n) }
来源：http://jlf.guannengcc.top

[T20] Swift：数组操作
来源：http://dop.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vmk.tanke756.top

[T21] Swift：遍历
来源：http://noz.redwolf501.top

for x in a { print(x) }
来源：http://ssa.jinghuilouyu.cn

[T22] Swift：字典
来源：http://esn.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://pcl.cheryme.top

[T23] Swift：函数
来源：http://znj.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pkh.tianlin.xyz

[T24] Swift：闭包
来源：http://tqg.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://hup.zdbjq.cn

[T25] Swift：结构体
来源：http://qou.cucudq.cn

struct P { var x: Int }
来源：http://iet.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://rul.c1oappe.top

class A: Base { override func f() {} }
来源：http://aat.nanxinkj.top

[T27] Swift：错误处理
来源：http://rra.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://tdl.sufxvd.cn

[T28] Swift：枚举
来源：http://usz.yangfankeji.com

enum Color { case red, green }
来源：http://nap.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://bom.cqqwz.cn

guard let x = opt else { return }
来源：http://oeb.52xcode.cn

[T30] Swift：协议
来源：http://agm.birdmap.top

protocol Shape { func area() -> Double }
来源：http://lae.cucudq.cn

[T31] Lua：Hello World
来源：http://ysk.cashguo.top

print("Hello")
来源：http://mna.mhx1999.top

[T32] Lua：局部变量
来源：http://ikq.ivvv.top

local a = 1
来源：http://pem.52xcode.cn

[T33] Lua：表（数组）
来源：http://pgz.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://egw.zhengqikj.top

[T34] Lua：遍历表
来源：http://tsk.hammf.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bxc.zhixingplan.top

[T35] Lua：字典表
来源：http://lgh.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://oay.chenjidiqi.icu

[T36] Lua：函数
来源：http://imd.fanxiaobao.xyz

function add(a, b) return a + b end
来源：http://vuz.havefunace.top

[T37] Lua：字符串拼接
来源：http://esh.guowangkeji.top

"a" .. "b"
来源：http://amo.havefunace.top

[T38] Lua：条件
来源：http://juo.nanxuanxn.top

if x > 0 then print("正") end
来源：http://veh.andypj.xyz

[T39] Lua：模式匹配
来源：http://dqd.cdnleiting.top

string.find(s, "%d+")
来源：http://fee.quarkkingdee.top

[T40] Lua：元表
来源：http://zhg.9152youxi.cn

setmetatable({}, { __index = base })
来源：http://odk.vehdjk.com

[T41] Perl：Hello World
来源：http://dvk.cdnleiting.top

print "Hello\n";
来源：http://nwo.pycfn.com

[T42] Perl：变量类型
来源：http://kvs.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mfi.tanke756.top

[T43] Perl：字符串插值
来源：http://npf.hesvh.cn

"值: $a"
来源：http://fva.hnxiangtu.top

[T44] Perl：条件
来源：http://isx.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://dwq.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://pts.yongpay.top

for my $x (@arr) { print $x; }
来源：http://wah.dianchejie.cn

[T46] Perl：哈希操作
来源：http://hau.jiagoushi.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rby.yj202588.top

[T47] Perl：正则捕获
来源：http://zfm.jianghu66.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ijv.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://drd.cashguo.top

$s =~ s/old/new/g;
来源：http://aes.hcnkem.com

[T49] Perl：函数
来源：http://ccp.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ucu.ybcxt.top

[T50] Perl：逐行读文件
来源：http://xrt.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mow.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://qnk.nanxuanxn.top

[T51] Scala：Hello World
来源：http://jfr.xylfe.cn

println("Hello")
来源：http://tsg.guannengcc.top

[T52] Scala：变量
来源：http://eac.yj202588.top

val a = 1;  var b = 2
来源：http://ycc.hnqzz.top

[T53] Scala：字符串插值
来源：http://adv.ydzc1.top

s"值: $b"
来源：http://khh.jinqigufen.top

[T54] Scala：集合映射
来源：http://vnr.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://hvr.yonumen.top

[T55] Scala：集合过滤
来源：http://foh.jinyuanbaomall.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eub.sufxvd.cn

[T56] Scala：样例类
来源：http://etf.cqqwz.cn

case class User(name: String, age: Int)
来源：http://emn.0kj1m.cn

[T57] Scala：模式匹配
来源：http://kfa.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uns.epnwcf.com

[T58] Scala：函数定义
来源：http://ydy.guowangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://cjk.chenlongwang.top

[T59] Scala：循环
来源：http://ahi.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://tab.feifeiyinyue.top

[T60] Scala：折叠
来源：http://nze.chenzaomai.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ljj.andypj.xyz

================================================================================
来源：http://kqd.shuidangran.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dmr.zhoulong.xyz

================================================================================
来源：http://udd.tian-w.cn

[U01] Py：创建虚拟环境
来源：http://yfn.snrcjt.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qqq.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://qod.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lsp.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://tpe.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wkt.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://zla.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sxi.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://zay.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://zip.xuetiantiany.cn

[U06] Py：合并两个字典
来源：http://qne.yj20258.top

{**a, **b}
来源：http://xwx.mhx1999.top

[U07] Py：反转字典键值
来源：http://obg.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://ttc.shuidangran.top

[U08] Py：展平二维列表
来源：http://qwa.jinqigfzy.top

[y for x in nested for y in x]
来源：http://okr.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://rba.uphjek.com

max(d, key=d.get)
来源：http://gmc.haohaochexian.top

[U10] Py：按值排序字典
来源：http://wsl.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pyv.chenlongwang.top

[U11] Py：生成器表达式
来源：http://vln.aizwys.cn

(x * 2 for x in arr)
来源：http://ops.yuxming.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fcc.sweek.top

Counter(arr).most_common(3)
来源：http://khu.haohaochexian.top

[U13] Py：固定长度队列
来源：http://wie.c1oappe.top

deque(maxlen=10)
来源：http://nao.cucudq.cn

[U14] Py：分组收集到列表
来源：http://gvo.yanxiufei.cn

defaultdict(list)
来源：http://acb.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://nhw.sxryk.cn

t = time.perf_counter()
来源：http://rme.nwbrower.top

[U16] Py：命令行参数解析
来源：http://mdu.shanyushiyangtech.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uac.vehdjk.com

[U17] Py：初始化日志
来源：http://qhp.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://ycc.vehdjk.com

[U18] Py：预编译正则
来源：http://oqa.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://xls.jinyuanbaomall.cn

[U19] Py：正则替换带回调
来源：http://quf.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tnn.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://vmz.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://unn.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://nna.tianlin.xyz

@contextlib.contextmanager
来源：http://lcb.aizwys.cn

[U22] Py：矩阵转置
来源：http://vbd.hfpthk.cn

list(zip(*m))
来源：http://qzj.nwbrower.top

[U23] Py：分块读取大文件
来源：http://yke.cheryme.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gta.cdnleiting.top

[U24] Py：路径操作
来源：http://qow.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://opg.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://zbo.shangyingyoupin.top

csv.DictReader(f)
来源：http://rht.redwolf501.top

[U26] Py：并发下载
来源：http://hgn.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cpf.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://zqe.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://vig.jinqigfzy.top

[U28] Py：类型别名
来源：http://hpl.wangshuangyany.cn

UserId = int
来源：http://xlf.daria6918.cn

[U29] Py：属性校验
来源：http://pnq.birdmap.top

@property 与 @x.setter 配合
来源：http://gsl.mhx1999.top

[U30] Py：数据类
来源：http://fcm.redwolf501.top

@dataclass(slots=True)
来源：http://ruz.yongpay.top

[U31] Py：单测
来源：http://nwi.dashuyun.cn

python -m pytest -q
来源：http://xgm.aibaodan.cn

[U32] Py：代码格式化
来源：http://qjy.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://agu.xingfuxueyuan.xyz


<!-- 参考信息 -->