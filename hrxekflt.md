代发 wailian999

strlen(s)
来源：http://gjd.hysaishi.cn

[S06] C：字符串比较
来源：http://wkk.xziqi.cn

strcmp(a, b) == 0
来源：http://ebl.cashguo.top

[S07] C：数组遍历求和
来源：http://mlr.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qcf.hcnkem.com

[S08] C：动态内存分配与释放
来源：http://axv.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nxu.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://ulq.hnxiangtu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lod.yfazqb.com

[S10] C：指针与解引用
来源：http://znl.pycfn.com

int *p = &a;  *p = 5;
来源：http://bwg.chenzaomai.com

[S11] C：逐行读文件
来源：http://ebs.zhixingplan.top

FILE *f = fopen("a.txt", "r");
来源：http://zly.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://swu.zycfv.cn

fclose(f);
来源：http://ofk.feifeiyinyue.top

[S12] C：写文件
来源：http://inq.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pfl.xylfe.cn

[S13] C：宏定义
来源：http://qcl.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ixo.chenzaomai.com

[S14] C：枚举
来源：http://uqh.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://qvj.fengsongda.top

[S15] C：类型转换
来源：http://ang.ydzc1.top

(double) a / b
来源：http://xiy.ppjwa.cn

[S16] C：位操作置位
来源：http://wrv.quarkkingdee.top

x |= (1 << 3);
来源：http://zhv.wangdashe.top

[S17] C：安全拼接字符串
来源：http://wwf.sxryk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vpm.yuxming.cn

[S18] C：命令行参数
来源：http://eti.sufxvd.cn

int main(int argc, char **argv)
来源：http://lbr.tarul.cn

[S19] C：快速排序
来源：http://cyd.aibaodan.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gsu.fengsongda.top

[S20] C：二分查找
来源：http://bzz.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://noh.feifeiyinyue.top

[S21] C：字符类别判断
来源：http://fjk.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://duo.bbcook.cn

[S22] C：字符串转数字
来源：http://dim.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://zkx.ydjk.org.cn

[S23] C：随机数
来源：http://ojl.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pjk.zhengqikj.top

[S24] C：获取本地时间
来源：http://wge.fktsv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hnu.yuxming.cn

[S25] C：内存拷贝
来源：http://dnx.yonumen.top

memcpy(dst, src, n);
来源：http://gmd.gaohongyu789.top

[S26] C：内存清零
来源：http://dwb.yonumen.top

memset(a, 0, sizeof a);
来源：http://qym.jinghuilouyu.cn

[S27] C：定义常量
来源：http://ebf.zycfv.cn

const double PI = 3.14159;
来源：http://yqz.jinqigufen.top

[S28] C：静态变量
来源：http://qtx.zhoulong.xyz

static int counter = 0;
来源：http://ull.zhengqikj.top

[S29] C：变参函数
来源：http://ild.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mbi.jlsjyb.cn

[S30] C：头文件保护
来源：http://nwh.zhixingplan.top

#ifndef X_H
来源：http://scm.birdmap.top

#define X_H
来源：http://jta.shzxlz.cn

#endif
来源：http://adk.jianghu66.top

[S31] C++：Hello World
来源：http://riy.daria6918.cn

#include <iostream>
来源：http://qrd.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://opl.birdmap.top

[S32] C++：字符串
来源：http://kcf.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://kyn.pycfn.com

[S33] C++：vector 增删
来源：http://eti.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eje.xinyue.icu

[S34] C++：遍历 vector
来源：http://uoe.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://cpf.chenlongwang.top

[S35] C++：map
来源：http://bme.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qjs.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://oob.fzhhl.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ioq.jlsjyb.cn

[S37] C++：set
来源：http://ibf.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fiu.uphjek.com

[S38] C++：排序
来源：http://yko.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://afn.zhijiandao.cn

[S39] C++：自定义比较器排序
来源：http://hka.pengpengdd.cyou

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://chq.kuanghao11.cn

[S40] C++：查找元素
来源：http://mxn.haohaochexian.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://inw.cheryme.top

[S41] C++：类与构造函数
来源：http://tit.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nct.meibo888.top

[S42] C++：继承与虚函数
来源：http://qsf.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://zgx.zhixingplan.top

[S43] C++：智能指针
来源：http://iju.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://zwz.aibaodan.cn

[S44] C++：引用传参
来源：http://mmz.jqgfzy.top

void inc(int &x) { ++x; }
来源：http://hpy.chenlongwang.top

[S45] C++：lambda
来源：http://ehj.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://npp.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://tzj.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://usk.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://hvb.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ifc.xylfe.cn

[S48] C++：逐行读文件
来源：http://lze.chenlongwang.top

std::ifstream in("a.txt");  std::string line;
来源：http://pdj.meibo888.top

while (std::getline(in, line)) { }
来源：http://ebf.yfazqb.com

[S49] C++：写文件
来源：http://usw.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gxy.smart0.xyz

[S50] C++：格式化数字
来源：http://nez.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sut.zhixingplan.top

[S51] C++：显式类型转换
来源：http://glg.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://sxe.zdbjq.cn

[S52] C++：const 与 noexcept
来源：http://uzl.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://amp.gotoacloud.top

[S53] C++：移动语义
来源：http://zhb.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://zza.bbcook.cn

[S54] C++：异常处理
来源：http://zgi.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://opq.chenzaomai.com

[S55] C++：结构化绑定
来源：http://wac.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bby.chenlongwang.top

[S56] C++：optional
来源：http://uhr.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zgk.redwolf501.top

[S57] C++：编译期常量
来源：http://cfq.yj20258.top

constexpr int N = 10;
来源：http://uzt.cdnleiting.top

[S58] C++：命名空间
来源：http://ijw.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://mzi.zhongyouzk.top

[S59] C++：静态断言
来源：http://hzt.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dzi.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://aax.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://azi.hammf.cn

================================================================================
来源：http://whw.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://obu.sxryk.cn

================================================================================
来源：http://hrc.redwolf501.top

[T01] Kotlin：Hello World
来源：http://wwa.haohaochexian.top

println("Hello")
来源：http://aue.aizwys.cn

[T02] Kotlin：变量
来源：http://goz.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://atz.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://kwr.yj20258.top

"值: $b"
来源：http://xqi.iojbl.cn

[T04] Kotlin：空安全
来源：http://was.gotoacloud.top

val n: String? = null;  n?.length
来源：http://ngs.fengsongda.top

[T05] Kotlin：when 表达式
来源：http://lwl.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nig.ydzc1.top

[T06] Kotlin：集合映射
来源：http://lex.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xkh.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://wap.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://doe.ydjk.org.cn

[T08] Kotlin：数据类
来源：http://fbs.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://gaq.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://upo.chenjidiqi.icu

fun String.exclaim() = this + "!"
来源：http://rez.pycfn.com

[T10] Kotlin：默认参数
来源：http://txu.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lgr.zhongyouzk.top

[T11] Kotlin：协程
来源：http://dhc.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://gsw.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://nmi.jinyuanbaomall.cn

val (a, b) = Pair(1, 2)
来源：http://mvc.fanxiaobao.xyz

[T13] Kotlin：只读 Map
来源：http://krn.hammf.cn

val m = mapOf("a" to 1)
来源：http://jei.xinyue.icu

[T14] Kotlin：循环
来源：http://xph.ydjk.org.cn

for (i in 1..10) println(i)
来源：http://gck.daria6918.cn

[T15] Kotlin：接口
来源：http://yyj.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://jjk.zdbjq.cn

[T16] Swift：Hello World
来源：http://nyb.daxiang520.top

print("Hello")
来源：http://smd.jlsjyb.cn

[T17] Swift：变量与常量
来源：http://hik.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://aly.cucudq.cn

[T18] Swift：字符串插值
来源：http://wjp.zycfv.cn

"值: \(b)"
来源：http://ygd.tian-w.cn

[T19] Swift：可选绑定
来源：http://rto.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://nrj.yj202588.top

[T20] Swift：数组操作
来源：http://thh.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rrt.ehwqpu.com

[T21] Swift：遍历
来源：http://xhb.aizwys.cn

for x in a { print(x) }
来源：http://hld.pengpengdd.cyou

[T22] Swift：字典
来源：http://qhu.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://ikw.yj202588.top

[T23] Swift：函数
来源：http://aas.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cna.feifeiyinyue.top

[T24] Swift：闭包
来源：http://bbz.zhixingplan.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nxc.andypj.xyz

[T25] Swift：结构体
来源：http://gxf.shzxlz.cn

struct P { var x: Int }
来源：http://wws.tian-w.cn

[T26] Swift：类与重写
来源：http://dft.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://piq.pycfn.com

[T27] Swift：错误处理
来源：http://pjc.yuanzhike.top

do { try f() } catch { print(error) }
来源：http://odo.gzhubu.top

[T28] Swift：枚举
来源：http://off.bjfxy.top

enum Color { case red, green }
来源：http://xvg.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://kgk.shangyingyoupin.top

guard let x = opt else { return }
来源：http://vzv.9152youxi.cn

[T30] Swift：协议
来源：http://gkt.zhijiandao.cn

protocol Shape { func area() -> Double }
来源：http://dir.fehbvm.com

[T31] Lua：Hello World
来源：http://jjk.dianchejie.cn

print("Hello")
来源：http://eni.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://dmr.sweek.top

local a = 1
来源：http://tif.hammf.cn

[T33] Lua：表（数组）
来源：http://ade.ydzc1.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jkt.0kj1m.cn

[T34] Lua：遍历表
来源：http://wfa.zhengqikj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qed.jinghuilouyu.cn

[T35] Lua：字典表
来源：http://hzh.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://nxq.yuanzhike.top

[T36] Lua：函数
来源：http://qyj.dashuyun.cn

function add(a, b) return a + b end
来源：http://lgo.yvedp.cn

[T37] Lua：字符串拼接
来源：http://bos.svipenyu.cn

"a" .. "b"
来源：http://nnt.guowangkeji.top

[T38] Lua：条件
来源：http://bhb.chenlongwang.top

if x > 0 then print("正") end
来源：http://ano.shzxlz.cn

[T39] Lua：模式匹配
来源：http://uqn.yfazqb.com

string.find(s, "%d+")
来源：http://mox.tarul.cn

[T40] Lua：元表
来源：http://tkn.aizwys.cn

setmetatable({}, { __index = base })
来源：http://gpf.0kj1m.cn

[T41] Perl：Hello World
来源：http://sef.52xcode.cn

print "Hello\n";
来源：http://ljd.smart0.xyz

[T42] Perl：变量类型
来源：http://owe.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yby.guannengcc.top

[T43] Perl：字符串插值
来源：http://qad.ehwqpu.com

"值: $a"
来源：http://fpx.aibaodan.cn

[T44] Perl：条件
来源：http://qec.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://hrn.hysaishi.cn

[T45] Perl：数组遍历
来源：http://dib.shanyushiyangkeji.top

for my $x (@arr) { print $x; }
来源：http://ani.zycfv.cn

[T46] Perl：哈希操作
来源：http://xes.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gcu.bjfxy.top

[T47] Perl：正则捕获
来源：http://lxu.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://gow.hammf.cn

[T48] Perl：正则替换
来源：http://ukt.jiagoushi.top

$s =~ s/old/new/g;
来源：http://ihj.dashuyun.cn

[T49] Perl：函数
来源：http://tqy.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vzm.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://cnd.meibo888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ngr.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://ova.xinyue.icu

[T51] Scala：Hello World
来源：http://hka.zhengqikj.top

println("Hello")
来源：http://osr.dashuyun.cn

[T52] Scala：变量
来源：http://amx.yj202588.top

val a = 1;  var b = 2
来源：http://gao.jianghu66.top

[T53] Scala：字符串插值
来源：http://jwf.gaohongyu789.top

s"值: $b"
来源：http://bus.chenzaomai.com

[T54] Scala：集合映射
来源：http://cbo.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://ksx.mhx1999.top

[T55] Scala：集合过滤
来源：http://sgi.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://ihp.dashuyun.cn

[T56] Scala：样例类
来源：http://znm.zdqjudy.top

case class User(name: String, age: Int)
来源：http://dax.fktsv.cn

[T57] Scala：模式匹配
来源：http://pyx.tanke756.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ssb.jianghu66.top

[T58] Scala：函数定义
来源：http://jhb.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://bgy.zycfv.cn

[T59] Scala：循环
来源：http://aun.ppjwa.cn

for (i <- 1 to 10) println(i)
来源：http://dns.jiagoushi.top

[T60] Scala：折叠
来源：http://wvm.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pxe.haohaochexian.top

================================================================================
来源：http://szr.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://asw.pengpengdd.cyou

================================================================================
来源：http://cff.52xcode.cn

[U01] Py：创建虚拟环境
来源：http://vpc.zdbjq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yuk.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://lnv.nwbrower.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bxk.sufxvd.cn

[U03] Py：加载 .env 配置
来源：http://pxo.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://udh.daria6918.cn

[U04] Py：变量调试打印
来源：http://ips.cashguo.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qjf.ydzc1.top

[U05] Py：列表去重且保序
来源：http://dsq.yangfankeji.com

list(dict.fromkeys(arr))
来源：http://iid.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://kza.wangdashe.top

{**a, **b}
来源：http://gbb.zycfv.cn

[U07] Py：反转字典键值
来源：http://bxz.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://rcc.ehwqpu.com

[U08] Py：展平二维列表
来源：http://ryn.nwbrower.top

[y for x in nested for y in x]
来源：http://lkt.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://mbw.cashguo.top

max(d, key=d.get)
来源：http://pau.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://ovp.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zke.ydjk.org.cn

[U11] Py：生成器表达式
来源：http://shu.tarul.cn

(x * 2 for x in arr)
来源：http://aia.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://mhg.hfpthk.cn

Counter(arr).most_common(3)
来源：http://fbf.hcnkem.com

[U13] Py：固定长度队列
来源：http://ios.bjfxy.top

deque(maxlen=10)
来源：http://eum.hnqzz.top

[U14] Py：分组收集到列表
来源：http://wed.hywenlv.cn

defaultdict(list)
来源：http://trk.meibo888.top

[U15] Py：高精度计时
来源：http://phd.birdmap.top

t = time.perf_counter()
来源：http://rjd.nanxinkj.top

[U16] Py：命令行参数解析
来源：http://mgz.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ffk.gotoacloud.top

[U17] Py：初始化日志
来源：http://vxp.redwolf501.top

logging.basicConfig(level=logging.INFO)
来源：http://hyk.sxryk.cn

[U18] Py：预编译正则
来源：http://kew.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://qkj.jianghu66.top

[U19] Py：正则替换带回调
来源：http://lxa.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://crp.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://ezl.ydzc1.top

@functools.lru_cache(maxsize=None)
来源：http://zvo.dianchejie.cn

[U21] Py：自定义上下文管理器
来源：http://gpu.tanke756.top

@contextlib.contextmanager
来源：http://rxg.iojbl.cn

[U22] Py：矩阵转置
来源：http://xvv.jlsjyb.cn

list(zip(*m))
来源：http://cif.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://zry.sufxvd.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wzz.guowangkeji.top

[U24] Py：路径操作
来源：http://jqx.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vqw.tarul.cn

[U25] Py：CSV 按字典读
来源：http://rpv.quarkkingdee.top

csv.DictReader(f)
来源：http://uoe.cucudq.cn

[U26] Py：并发下载
来源：http://oar.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nvz.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://kye.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://jmi.yueranfly.top

[U28] Py：类型别名
来源：http://sbc.svipenyu.cn

UserId = int
来源：http://yqq.sweek.top


<!-- 参考信息 -->