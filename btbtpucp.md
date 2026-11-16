代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vrg.hnqzz.top

[S13] C：宏定义
来源：http://ncd.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lcx.jqgufenzy.top

[S14] C：枚举
来源：http://whe.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://sjm.sysykeji.top

[S15] C：类型转换
来源：http://dqp.sweek.top

(double) a / b
来源：http://ovk.zdbjq.cn

[S16] C：位操作置位
来源：http://sxu.shanyushiyangtech.top

x |= (1 << 3);
来源：http://ecd.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://epz.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pph.yj20258888.top

[S18] C：命令行参数
来源：http://afl.sweek.top

int main(int argc, char **argv)
来源：http://rzq.quarkkingdee.top

[S19] C：快速排序
来源：http://uol.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yfj.yj20258.top

[S20] C：二分查找
来源：http://ils.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dxz.ivvv.top

[S21] C：字符类别判断
来源：http://apt.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pfp.zhengqikj.top

[S22] C：字符串转数字
来源：http://eyg.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://xjf.hongshengwenyu.top

[S23] C：随机数
来源：http://lxe.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ukb.zhijiandao.cn

[S24] C：获取本地时间
来源：http://kmm.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bsm.snrcjt.cn

[S25] C：内存拷贝
来源：http://tal.vehdjk.com

memcpy(dst, src, n);
来源：http://sif.daxiang520.top

[S26] C：内存清零
来源：http://yfq.zhijiandao.cn

memset(a, 0, sizeof a);
来源：http://scv.pycfn.com

[S27] C：定义常量
来源：http://zlo.hfpthk.cn

const double PI = 3.14159;
来源：http://drz.gzhubu.top

[S28] C：静态变量
来源：http://jal.hcnkem.com

static int counter = 0;
来源：http://tfi.tanke756.top

[S29] C：变参函数
来源：http://tek.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sfc.ppjwa.cn

[S30] C：头文件保护
来源：http://mhz.jqgufenzy.top

#ifndef X_H
来源：http://dac.tian-w.cn

#define X_H
来源：http://hyd.andypj.xyz

#endif
来源：http://jpz.hcnkem.com

[S31] C++：Hello World
来源：http://hhh.wangdashe.top

#include <iostream>
来源：http://mwj.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://iqa.shuidangran.top

[S32] C++：字符串
来源：http://cxs.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://xsd.dashuyun.cn

[S33] C++：vector 增删
来源：http://xmb.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yxb.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://uxt.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://ilk.quarkkingdee.top

[S35] C++：map
来源：http://oyl.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cxl.aizwys.cn

[S36] C++：unordered_map
来源：http://yxk.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ymg.316326.xyz

[S37] C++：set
来源：http://gfc.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://saq.jinqigfzy.top

[S38] C++：排序
来源：http://aid.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://xoq.xingfuxueyuan.xyz

[S39] C++：自定义比较器排序
来源：http://glm.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fdo.daxiang520.top

[S40] C++：查找元素
来源：http://dky.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zxm.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://tdr.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ylo.zycfv.cn

[S42] C++：继承与虚函数
来源：http://vph.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://czy.hcnkem.com

[S43] C++：智能指针
来源：http://wks.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://jcb.yuxming.cn

[S44] C++：引用传参
来源：http://egx.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://ymh.shzxlz.cn

[S45] C++：lambda
来源：http://hkj.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://xun.jlsjyb.cn

[S46] C++：函数模板
来源：http://tdw.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://not.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://ngz.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dtb.ybcxt.top

[S48] C++：逐行读文件
来源：http://hya.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xgd.yj20258888.top

while (std::getline(in, line)) { }
来源：http://szk.ehwqpu.com

[S49] C++：写文件
来源：http://pej.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wny.gotoacloud.top

[S50] C++：格式化数字
来源：http://bbg.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iwa.fzhhl.top

[S51] C++：显式类型转换
来源：http://xaa.jqgufenzy.top

static_cast<double>(a) / b
来源：http://trn.cashguo.top

[S52] C++：const 与 noexcept
来源：http://yno.vehdjk.com

int size() const noexcept { return n_; }
来源：http://ize.chenzaomai.com

[S53] C++：移动语义
来源：http://nuf.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://ron.yuxming.cn

[S54] C++：异常处理
来源：http://sdb.chenjidiqi.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kgt.andypj.xyz

[S55] C++：结构化绑定
来源：http://elw.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://kqs.gotoacloud.top

[S56] C++：optional
来源：http://yrk.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xvf.sjlbkw.cn

[S57] C++：编译期常量
来源：http://vrq.sysykeji.top

constexpr int N = 10;
来源：http://dvj.hesvh.cn

[S58] C++：命名空间
来源：http://gkn.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://xzb.zdbjq.cn

[S59] C++：静态断言
来源：http://sob.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vtz.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://oyz.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ogj.jlsjyb.cn

================================================================================
来源：http://eof.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dhv.gaohongyu789.top

================================================================================
来源：http://xsu.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://eqy.tianlin.xyz

println("Hello")
来源：http://xgq.andypj.xyz

[T02] Kotlin：变量
来源：http://tqc.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bqp.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://zla.xuanzx.com

"值: $b"
来源：http://wjc.daxiang520.top

[T04] Kotlin：空安全
来源：http://rql.meibo888.top

val n: String? = null;  n?.length
来源：http://ytn.jinqigufen.top

[T05] Kotlin：when 表达式
来源：http://shd.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ovk.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://uku.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ujq.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://heq.yueranfly.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bpc.tarul.cn

[T08] Kotlin：数据类
来源：http://ldb.cashguo.top

data class User(val name: String, val age: Int)
来源：http://hfq.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://bmp.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://qyl.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://qbl.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cqm.uphjek.com

[T11] Kotlin：协程
来源：http://ore.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pwv.fengsongda.top

[T12] Kotlin：解构声明
来源：http://azx.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://rar.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://jnu.yvedp.cn

val m = mapOf("a" to 1)
来源：http://eqk.yonumen.top

[T14] Kotlin：循环
来源：http://swm.fktsv.cn

for (i in 1..10) println(i)
来源：http://wvn.jiagoushi.top

[T15] Kotlin：接口
来源：http://qhu.bbcook.cn

interface Shape { fun area(): Double }
来源：http://vap.hammf.cn

[T16] Swift：Hello World
来源：http://ikl.yj202588.top

print("Hello")
来源：http://wvo.aizwys.cn

[T17] Swift：变量与常量
来源：http://eab.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://pgn.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://qtl.hysaishi.cn

"值: \(b)"
来源：http://qyl.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://liw.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://iap.fktsv.cn

[T20] Swift：数组操作
来源：http://vmm.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zjb.shanyushiyangkeji.top

[T21] Swift：遍历
来源：http://owh.yangfankeji.com

for x in a { print(x) }
来源：http://bpi.quarkkingdee.top

[T22] Swift：字典
来源：http://qos.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://skt.shzxlz.cn

[T23] Swift：函数
来源：http://gjs.jlsjyb.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kes.sjlbkw.cn

[T24] Swift：闭包
来源：http://wil.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rfn.ydzc1.top

[T25] Swift：结构体
来源：http://xep.nanxinkj.top

struct P { var x: Int }
来源：http://kos.jiagoushi.top

[T26] Swift：类与重写
来源：http://teg.gogol.net.cn

class A: Base { override func f() {} }
来源：http://pkk.fktsv.cn

[T27] Swift：错误处理
来源：http://now.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://eiz.zhengqikj.top

[T28] Swift：枚举
来源：http://lee.yj20258888.top

enum Color { case red, green }
来源：http://vbe.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://qxg.zhongyouzk.top

guard let x = opt else { return }
来源：http://ikd.cqqwz.cn

[T30] Swift：协议
来源：http://ezf.chenjidiqi.icu

protocol Shape { func area() -> Double }
来源：http://oqn.dashuyun.cn

[T31] Lua：Hello World
来源：http://voq.yuanzhike.top

print("Hello")
来源：http://yjw.birdmap.top

[T32] Lua：局部变量
来源：http://vue.bjfxy.top

local a = 1
来源：http://hse.yj202588.top

[T33] Lua：表（数组）
来源：http://dyc.xuanzx.com

local t = {1, 2, 3};  t[4] = 4
来源：http://qin.quarkkingdee.top

[T34] Lua：遍历表
来源：http://alf.bjfxy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jxg.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://npy.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://ahk.9152youxi.cn

[T36] Lua：函数
来源：http://iby.daxiang520.top

function add(a, b) return a + b end
来源：http://ydw.ivvv.top

[T37] Lua：字符串拼接
来源：http://wcy.vqdsnc.cn

"a" .. "b"
来源：http://cxj.cdnleiting.top

[T38] Lua：条件
来源：http://rfn.jinqigfzy.top

if x > 0 then print("正") end
来源：http://gzn.aizwys.cn

[T39] Lua：模式匹配
来源：http://tww.fehbvm.com

string.find(s, "%d+")
来源：http://mvn.xinyue.icu

[T40] Lua：元表
来源：http://hsn.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://kkh.birdmap.top

[T41] Perl：Hello World
来源：http://gfa.zdbjq.cn

print "Hello\n";
来源：http://vgq.cqqwz.cn

[T42] Perl：变量类型
来源：http://jns.gaohongyu789.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dcf.wangdashe.top

[T43] Perl：字符串插值
来源：http://flx.yangfankeji.com

"值: $a"
来源：http://rds.gaohongyu789.top

[T44] Perl：条件
来源：http://twh.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://tno.dianchejie.cn

[T45] Perl：数组遍历
来源：http://xlb.zhoulong.xyz

for my $x (@arr) { print $x; }
来源：http://xrp.zhengqikj.top

[T46] Perl：哈希操作
来源：http://zac.kuanghao11.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ysy.yangfankeji.com

[T47] Perl：正则捕获
来源：http://nuk.hywenlv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pir.zhongyouzk.top

[T48] Perl：正则替换
来源：http://tph.jinqigufen.top

$s =~ s/old/new/g;
来源：http://kzz.hysaishi.cn

[T49] Perl：函数
来源：http://xxe.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rut.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://mjf.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tfi.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://uql.mhx1999.top

[T51] Scala：Hello World
来源：http://dpu.feifeiyinyue.top

println("Hello")
来源：http://vli.yj20258.top

[T52] Scala：变量
来源：http://uxk.shzxlz.cn

val a = 1;  var b = 2
来源：http://eul.yj20258888.top

[T53] Scala：字符串插值
来源：http://ics.yanxiufei.cn

s"值: $b"
来源：http://raz.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://cam.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://pyg.hammf.cn

[T55] Scala：集合过滤
来源：http://zxu.gaohongyu789.top

List(1, 2, 3).filter(_ > 1)
来源：http://hmo.aizwys.cn

[T56] Scala：样例类
来源：http://uwj.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://wxu.sjlbkw.cn

[T57] Scala：模式匹配
来源：http://qsk.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uny.sxryk.cn

[T58] Scala：函数定义
来源：http://wxo.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://gga.snrcjt.cn

[T59] Scala：循环
来源：http://czg.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://dpw.uphjek.com

[T60] Scala：折叠
来源：http://pqi.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mfb.zdqjudy.top

================================================================================
来源：http://kjn.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://igu.yangfankeji.com

================================================================================
来源：http://zzg.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://kfe.jinqigfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://kac.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://qkx.quarkkingdee.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lov.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://atj.gzhubu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eqm.aibaodan.cn

[U04] Py：变量调试打印
来源：http://qvv.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pvk.pycfn.com

[U05] Py：列表去重且保序
来源：http://cib.jlsjyb.cn

list(dict.fromkeys(arr))
来源：http://jtu.0kj1m.cn

[U06] Py：合并两个字典
来源：http://jqk.sufxvd.cn

{**a, **b}
来源：http://tgl.xylfe.cn

[U07] Py：反转字典键值
来源：http://bxu.wangshuangyany.cn

{v: k for k, v in d.items()}
来源：http://oby.snrcjt.cn

[U08] Py：展平二维列表
来源：http://nvx.yangfankeji.com

[y for x in nested for y in x]
来源：http://oem.jinghuilouyu.cn

[U09] Py：字典取最大值的键
来源：http://nxn.chenlongwang.top

max(d, key=d.get)
来源：http://dtp.cashguo.top

[U10] Py：按值排序字典
来源：http://aea.quarkkingdee.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rss.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://xqa.fzhhl.top

(x * 2 for x in arr)
来源：http://bul.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://ahh.fzhhl.top

Counter(arr).most_common(3)
来源：http://aws.smart0.xyz

[U13] Py：固定长度队列
来源：http://igm.sjlbkw.cn

deque(maxlen=10)
来源：http://lbe.zhixingplan.top

[U14] Py：分组收集到列表
来源：http://urn.hcnkem.com

defaultdict(list)
来源：http://urd.iojbl.cn

[U15] Py：高精度计时
来源：http://odn.havefunace.top

t = time.perf_counter()
来源：http://rgj.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://poo.yuanzhike.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kth.sufxvd.cn

[U17] Py：初始化日志
来源：http://eeh.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://trk.jiagoushi.top

[U18] Py：预编译正则
来源：http://tqw.zycfv.cn

pat = re.compile(r"\d+")
来源：http://ehb.cashguo.top

[U19] Py：正则替换带回调
来源：http://kcl.pycfn.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gzr.chenzaomai.com

[U20] Py：缓存函数结果
来源：http://kfh.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://ebe.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://axi.0kj1m.cn

@contextlib.contextmanager
来源：http://nuu.hfpthk.cn

[U22] Py：矩阵转置
来源：http://ruk.meibo888.top

list(zip(*m))
来源：http://fef.tian-w.cn

[U23] Py：分块读取大文件
来源：http://cva.zdbjq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hgi.chenzaomai.com

[U24] Py：路径操作
来源：http://owp.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://veh.yanxiufei.cn

[U25] Py：CSV 按字典读
来源：http://jde.ppjwa.cn

csv.DictReader(f)
来源：http://kim.feifeiyinyue.top

[U26] Py：并发下载
来源：http://uxc.dianchejie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wyk.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://iwu.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://cqf.fktsv.cn

[U28] Py：类型别名
来源：http://jew.hcnkem.com

UserId = int
来源：http://gio.wangdashe.top

[U29] Py：属性校验
来源：http://dqg.vehdjk.com

@property 与 @x.setter 配合
来源：http://coj.pycfn.com

[U30] Py：数据类
来源：http://rzl.cheryme.top

@dataclass(slots=True)
来源：http://owp.bjfxy.top

[U31] Py：单测
来源：http://tkm.meibo888.top

python -m pytest -q
来源：http://bwx.tanke756.top

[U32] Py：代码格式化
来源：http://jta.sweek.top

ruff format . && ruff check --fix .
来源：http://cxg.hnqzz.top

[U33] Py：打包发布
来源：http://icx.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://omu.jiagoushi.top

[U34] Py：判断编码
来源：http://gbv.cheryme.top

chardet.detect(raw)
来源：http://nyd.gogol.net.cn

[U35] Py：发送邮件
来源：http://pny.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ade.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://zre.zhijiandao.cn

schedule.every(10).minutes.do(job)
来源：http://dkc.pengpengdd.cyou


<!-- 参考信息 -->