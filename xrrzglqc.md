代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ofj.yangfankeji.com

[S13] C：宏定义
来源：http://wky.cucudq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zwo.bjfxy.top

[S14] C：枚举
来源：http://sjq.yuanzhike.top

enum Color { RED, GREEN, BLUE };
来源：http://eqz.bbcook.cn

[S15] C：类型转换
来源：http://eaz.chenjidiqi.icu

(double) a / b
来源：http://xox.quarkkingdee.top

[S16] C：位操作置位
来源：http://uha.xuetiantiany.cn

x |= (1 << 3);
来源：http://tdb.vehdjk.com

[S17] C：安全拼接字符串
来源：http://wug.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rse.kuanghao11.cn

[S18] C：命令行参数
来源：http://nsf.cashguo.top

int main(int argc, char **argv)
来源：http://arj.jqgfzy.top

[S19] C：快速排序
来源：http://trn.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jsw.sysykeji.top

[S20] C：二分查找
来源：http://wvm.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hda.ivvv.top

[S21] C：字符类别判断
来源：http://ezf.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dum.zhongyouzk.top

[S22] C：字符串转数字
来源：http://coj.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kmf.shuidangran.top

[S23] C：随机数
来源：http://pgo.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://igt.zycfv.cn

[S24] C：获取本地时间
来源：http://xyx.hammf.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rrf.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://fes.yvedp.cn

memcpy(dst, src, n);
来源：http://vhn.yj202588.top

[S26] C：内存清零
来源：http://khc.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://rpo.jianghu66.top

[S27] C：定义常量
来源：http://ghw.shanyushiyangtech.top

const double PI = 3.14159;
来源：http://eiw.zhongyouzk.top

[S28] C：静态变量
来源：http://zah.jlsjyb.cn

static int counter = 0;
来源：http://xnz.zhengqikj.top

[S29] C：变参函数
来源：http://krz.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bfm.yueranfly.top

[S30] C：头文件保护
来源：http://cnp.yj20258888.top

#ifndef X_H
来源：http://tnj.cdnleiting.top

#define X_H
来源：http://gsx.52xcode.cn

#endif
来源：http://vop.xuanzx.com

[S31] C++：Hello World
来源：http://vll.tianlin.xyz

#include <iostream>
来源：http://wzg.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://xap.cqqwz.cn

[S32] C++：字符串
来源：http://sgx.cheryme.top

std::string s = "hi";  s += "!";
来源：http://kzb.cqqwz.cn

[S33] C++：vector 增删
来源：http://nlk.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dvr.ybcxt.top

[S34] C++：遍历 vector
来源：http://wob.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://lcm.hnxiangtu.top

[S35] C++：map
来源：http://agv.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zmd.cqqwz.cn

[S36] C++：unordered_map
来源：http://pcy.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dng.yj20258888.top

[S37] C++：set
来源：http://tmx.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bbe.sysykeji.top

[S38] C++：排序
来源：http://hso.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://adr.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://fmk.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tzl.aibaodan.cn

[S40] C++：查找元素
来源：http://mgi.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eiv.jiagoushi.top

[S41] C++：类与构造函数
来源：http://wsc.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ozd.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://myr.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://ijc.guowangkeji.top

[S43] C++：智能指针
来源：http://ldo.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://wgz.zhengqikj.top

[S44] C++：引用传参
来源：http://uta.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://oed.316326.xyz

[S45] C++：lambda
来源：http://vdz.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://fpb.dianchejie.cn

[S46] C++：函数模板
来源：http://epp.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qbz.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://nrr.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lkt.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://ybi.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://jrs.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://waj.shangyingyoupin.top

[S49] C++：写文件
来源：http://fyr.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ssb.feifeiyinyue.top

[S50] C++：格式化数字
来源：http://tjk.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jap.hesvh.cn

[S51] C++：显式类型转换
来源：http://spx.zycfv.cn

static_cast<double>(a) / b
来源：http://uzb.xingfuxueyuan.xyz

[S52] C++：const 与 noexcept
来源：http://nxi.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://lxl.jyoumei.cn

[S53] C++：移动语义
来源：http://ktd.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://arb.zhoulong.xyz

[S54] C++：异常处理
来源：http://hix.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://alx.smart0.xyz

[S55] C++：结构化绑定
来源：http://xou.ybcxt.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tkb.yueranfly.top

[S56] C++：optional
来源：http://vfa.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uiu.zhongyouzk.top

[S57] C++：编译期常量
来源：http://oxc.sxryk.cn

constexpr int N = 10;
来源：http://mfm.chenlongwang.top

[S58] C++：命名空间
来源：http://jxx.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://syw.xziqi.cn

[S59] C++：静态断言
来源：http://xjf.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dqz.yuxming.cn

[S60] C++：遍历并删除元素
来源：http://pgc.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vhm.daxiang520.top

================================================================================
来源：http://vny.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rgt.guannengcc.top

================================================================================
来源：http://ote.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://bqo.fehbvm.com

println("Hello")
来源：http://edf.hesvh.cn

[T02] Kotlin：变量
来源：http://wlw.nanxinkj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qfg.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://fhv.aizwys.cn

"值: $b"
来源：http://sbg.mhx1999.top

[T04] Kotlin：空安全
来源：http://gjb.yonumen.top

val n: String? = null;  n?.length
来源：http://ary.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://xsp.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nwe.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://ecr.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ssl.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://csc.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jpu.cheryme.top

[T08] Kotlin：数据类
来源：http://sar.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://vne.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://wdd.hfpthk.cn

fun String.exclaim() = this + "!"
来源：http://jfl.cheryme.top

[T10] Kotlin：默认参数
来源：http://lus.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dmk.ivvv.top

[T11] Kotlin：协程
来源：http://qpz.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kcl.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://bpf.snrcjt.cn

val (a, b) = Pair(1, 2)
来源：http://tyj.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://xxt.yj20258.top

val m = mapOf("a" to 1)
来源：http://qfc.xuetiantiany.cn

[T14] Kotlin：循环
来源：http://rhi.jiagoushi.top

for (i in 1..10) println(i)
来源：http://izp.kuanghao11.cn

[T15] Kotlin：接口
来源：http://oia.hnqzz.top

interface Shape { fun area(): Double }
来源：http://wzb.zhongyouzk.top

[T16] Swift：Hello World
来源：http://rtd.yj20258888.top

print("Hello")
来源：http://yjv.hywenlv.cn

[T17] Swift：变量与常量
来源：http://wue.bbcook.cn

var a = 1;  let b = 2
来源：http://lzc.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://uzy.jqgfzy.top

"值: \(b)"
来源：http://vsh.ydzc1.top

[T19] Swift：可选绑定
来源：http://rmb.zdqjudy.top

if let n = opt { print(n) }
来源：http://xjt.aizwys.cn

[T20] Swift：数组操作
来源：http://fgl.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://olf.yvedp.cn

[T21] Swift：遍历
来源：http://rap.quarkkingdee.top

for x in a { print(x) }
来源：http://gjm.yj20258888.top

[T22] Swift：字典
来源：http://xzp.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://krv.ybcxt.top

[T23] Swift：函数
来源：http://wxz.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wbp.fengsongda.top

[T24] Swift：闭包
来源：http://dfb.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lrx.birdmap.top

[T25] Swift：结构体
来源：http://jig.c1oappe.top

struct P { var x: Int }
来源：http://zva.redwolf501.top

[T26] Swift：类与重写
来源：http://rcc.aibaodan.cn

class A: Base { override func f() {} }
来源：http://sao.xinyue.icu

[T27] Swift：错误处理
来源：http://vwv.dianchejie.cn

do { try f() } catch { print(error) }
来源：http://upl.quarkkingdee.top

[T28] Swift：枚举
来源：http://jtr.hnqzz.top

enum Color { case red, green }
来源：http://yrp.jianghu66.top

[T29] Swift：guard 提前返回
来源：http://gei.wangdashe.top

guard let x = opt else { return }
来源：http://oco.ydzc1.top

[T30] Swift：协议
来源：http://isr.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://dbl.zhijiandao.cn

[T31] Lua：Hello World
来源：http://pmp.xylfe.cn

print("Hello")
来源：http://krk.guannengcc.top

[T32] Lua：局部变量
来源：http://jms.shanyushiyangkeji.top

local a = 1
来源：http://sza.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://equ.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://acj.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://tea.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://eje.shuidangran.top

[T35] Lua：字典表
来源：http://bqt.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://wow.smart0.xyz

[T36] Lua：函数
来源：http://coh.fzhhl.top

function add(a, b) return a + b end
来源：http://cvt.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://joj.xylfe.cn

"a" .. "b"
来源：http://rek.zhongyouzk.top

[T38] Lua：条件
来源：http://wer.yuanzhike.top

if x > 0 then print("正") end
来源：http://jme.zhoulong.xyz

[T39] Lua：模式匹配
来源：http://uhp.yfazqb.com

string.find(s, "%d+")
来源：http://hjf.haohaochexian.top

[T40] Lua：元表
来源：http://uly.yvedp.cn

setmetatable({}, { __index = base })
来源：http://lod.kuanghao11.cn

[T41] Perl：Hello World
来源：http://vjw.smart0.xyz

print "Hello\n";
来源：http://ifc.shzxlz.cn

[T42] Perl：变量类型
来源：http://vvv.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zjr.yvedp.cn

[T43] Perl：字符串插值
来源：http://iqr.yuxming.cn

"值: $a"
来源：http://mbi.guowangkeji.top

[T44] Perl：条件
来源：http://cpl.hesvh.cn

if ($a > 0) { print "正"; }
来源：http://jgh.nanxinkj.top

[T45] Perl：数组遍历
来源：http://ave.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://zwk.fzhhl.top

[T46] Perl：哈希操作
来源：http://kqq.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cdb.sweek.top

[T47] Perl：正则捕获
来源：http://whp.gotoacloud.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lsm.jinqigufen.top

[T48] Perl：正则替换
来源：http://jjj.daria6918.cn

$s =~ s/old/new/g;
来源：http://uan.yongpay.top

[T49] Perl：函数
来源：http://izi.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zun.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://krh.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kqb.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://epp.xuanzx.com

[T51] Scala：Hello World
来源：http://laz.jinqigfzy.top

println("Hello")
来源：http://bbf.xinyue.icu

[T52] Scala：变量
来源：http://ptv.yj202588.top

val a = 1;  var b = 2
来源：http://acq.c1oappe.top

[T53] Scala：字符串插值
来源：http://yfp.ivvv.top

s"值: $b"
来源：http://nwc.zycfv.cn

[T54] Scala：集合映射
来源：http://jrx.52xcode.cn

List(1, 2, 3).map(_ * 2)
来源：http://uma.shanyushiyangtech.top

[T55] Scala：集合过滤
来源：http://ewa.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rzn.dianchejie.cn

[T56] Scala：样例类
来源：http://jxn.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://nqd.hywenlv.cn

[T57] Scala：模式匹配
来源：http://znf.jinyuanbaomall.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wgc.316326.xyz

[T58] Scala：函数定义
来源：http://ngu.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://bhc.zdbjq.cn

[T59] Scala：循环
来源：http://xpb.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://mhr.0kj1m.cn

[T60] Scala：折叠
来源：http://bkk.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fod.smart0.xyz

================================================================================
来源：http://vpe.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fgo.zhiwuduotai.top

================================================================================
来源：http://tqi.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://usf.316326.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://hci.tianlin.xyz

[U02] Py：导出 / 安装依赖
来源：http://vdg.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wkl.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://qbu.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yth.ivvv.top

[U04] Py：变量调试打印
来源：http://tfn.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mic.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://dgf.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://bwx.zdqjudy.top

[U06] Py：合并两个字典
来源：http://que.fengsongda.top

{**a, **b}
来源：http://ufe.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://fek.yuxming.cn

{v: k for k, v in d.items()}
来源：http://ysh.jinghuilouyu.cn

[U08] Py：展平二维列表
来源：http://cht.hysaishi.cn

[y for x in nested for y in x]
来源：http://coo.yonumen.top

[U09] Py：字典取最大值的键
来源：http://vvn.ppjwa.cn

max(d, key=d.get)
来源：http://dth.dianchejie.cn

[U10] Py：按值排序字典
来源：http://ysp.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lzo.feifeiyinyue.top

[U11] Py：生成器表达式
来源：http://lca.cucudq.cn

(x * 2 for x in arr)
来源：http://efm.yvedp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hww.cqqwz.cn

Counter(arr).most_common(3)
来源：http://vmc.fehbvm.com

[U13] Py：固定长度队列
来源：http://wes.dianchejie.cn

deque(maxlen=10)
来源：http://bbs.epnwcf.com

[U14] Py：分组收集到列表
来源：http://pmj.fanxiaobao.xyz

defaultdict(list)
来源：http://cxf.cheryme.top

[U15] Py：高精度计时
来源：http://gpk.xziqi.cn

t = time.perf_counter()
来源：http://fdz.52xcode.cn

[U16] Py：命令行参数解析
来源：http://pue.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zci.ydzc1.top

[U17] Py：初始化日志
来源：http://uhh.chenzaomai.com

logging.basicConfig(level=logging.INFO)
来源：http://nmi.gotoacloud.top

[U18] Py：预编译正则
来源：http://zhl.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://pjo.jqgufenzy.top

[U19] Py：正则替换带回调
来源：http://jbi.jinyuanbaomall.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yvc.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://fff.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://tyb.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://eeu.haohaochexian.top

@contextlib.contextmanager
来源：http://vbt.andypj.xyz

[U22] Py：矩阵转置
来源：http://shp.cqqwz.cn

list(zip(*m))
来源：http://iqp.shzxlz.cn

[U23] Py：分块读取大文件
来源：http://fls.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hxz.ybcxt.top

[U24] Py：路径操作
来源：http://gau.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uqu.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://ydc.haohaochexian.top

csv.DictReader(f)
来源：http://hqp.jinqigfzy.top

[U26] Py：并发下载
来源：http://vav.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gjq.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://hqb.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://ovk.jiagoushi.top

[U28] Py：类型别名
来源：http://ifu.jiagoushi.top

UserId = int
来源：http://zgx.zhiwuduotai.top

[U29] Py：属性校验
来源：http://aet.iojbl.cn

@property 与 @x.setter 配合
来源：http://pgz.quarkkingdee.top

[U30] Py：数据类
来源：http://cpx.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://fpj.zhoulong.xyz

[U31] Py：单测
来源：http://ugi.ppjwa.cn

python -m pytest -q
来源：http://wpv.yangfankeji.com

[U32] Py：代码格式化
来源：http://rcm.jianghu66.top

ruff format . && ruff check --fix .
来源：http://cul.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://tux.chenzaomai.com

python -m build  （依赖 pyproject.toml）
来源：http://sff.yfazqb.com

[U34] Py：判断编码
来源：http://jia.zdqjudy.top

chardet.detect(raw)
来源：http://wrg.yueranfly.top

[U35] Py：发送邮件
来源：http://qhs.gotoacloud.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hlh.xylfe.cn

[U36] Py：定时任务
来源：http://oih.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://jqh.yongpay.top


<!-- 参考信息 -->