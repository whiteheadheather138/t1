代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tvx.dianchejie.cn

[S13] C：宏定义
来源：http://tod.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iov.dianchejie.cn

[S14] C：枚举
来源：http://djw.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://lql.tianlin.xyz

[S15] C：类型转换
来源：http://xsh.gaohongyu789.top

(double) a / b
来源：http://pze.quarkkingdee.top

[S16] C：位操作置位
来源：http://ewk.yvedp.cn

x |= (1 << 3);
来源：http://fsw.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://cjd.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gdv.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://brt.sysykeji.top

int main(int argc, char **argv)
来源：http://amg.xuetiantiany.cn

[S19] C：快速排序
来源：http://niz.dashuyun.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uqf.xuanzx.com

[S20] C：二分查找
来源：http://mhw.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://raq.sweek.top

[S21] C：字符类别判断
来源：http://onf.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ouj.shzxlz.cn

[S22] C：字符串转数字
来源：http://sdq.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ank.jinyuanbaomall.cn

[S23] C：随机数
来源：http://bfh.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://avu.jinqigufen.top

[S24] C：获取本地时间
来源：http://syl.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jhp.gzhubu.top

[S25] C：内存拷贝
来源：http://qif.gaohongyu789.top

memcpy(dst, src, n);
来源：http://zqr.bbcook.cn

[S26] C：内存清零
来源：http://lfs.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://oee.zhiwuduotai.top

[S27] C：定义常量
来源：http://mgd.gogol.net.cn

const double PI = 3.14159;
来源：http://bjc.gogol.net.cn

[S28] C：静态变量
来源：http://pur.316326.xyz

static int counter = 0;
来源：http://unx.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://wjw.zhijiandao.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tfj.andypj.xyz

[S30] C：头文件保护
来源：http://cdu.jinqigufen.top

#ifndef X_H
来源：http://ump.hywenlv.cn

#define X_H
来源：http://alt.jianghu66.top

#endif
来源：http://mvh.snrcjt.cn

[S31] C++：Hello World
来源：http://khr.gzhubu.top

#include <iostream>
来源：http://zof.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://kyv.ydjk.org.cn

[S32] C++：字符串
来源：http://pah.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://bgv.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://ldh.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dpk.jianghu66.top

[S34] C++：遍历 vector
来源：http://ycu.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://agf.jinqigufen.top

[S35] C++：map
来源：http://knt.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xsd.gotoacloud.top

[S36] C++：unordered_map
来源：http://uwb.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nbz.cucudq.cn

[S37] C++：set
来源：http://dmc.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yql.iojbl.cn

[S38] C++：排序
来源：http://fun.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://eld.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://aah.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ysz.jqgfzy.top

[S40] C++：查找元素
来源：http://vkz.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kbi.chenzaomai.com

[S41] C++：类与构造函数
来源：http://jme.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://liq.ivvv.top

[S42] C++：继承与虚函数
来源：http://yex.sxryk.cn

class B : public Base { public: void f() override {} };
来源：http://nlj.nanxuanxn.top

[S43] C++：智能指针
来源：http://dys.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://tqt.epnwcf.com

[S44] C++：引用传参
来源：http://mmj.nwbrower.top

void inc(int &x) { ++x; }
来源：http://wnv.yj20258.top

[S45] C++：lambda
来源：http://btq.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pwe.yfazqb.com

[S46] C++：函数模板
来源：http://mzq.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lyx.ctjpmb.com

[S47] C++：结构化绑定遍历
来源：http://ivz.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yjk.hysaishi.cn

[S48] C++：逐行读文件
来源：http://dks.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://fhu.mhx1999.top

while (std::getline(in, line)) { }
来源：http://zcz.meibo888.top

[S49] C++：写文件
来源：http://wte.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://amv.sufxvd.cn

[S50] C++：格式化数字
来源：http://pqk.nanxuanxn.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pfi.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://mir.quarkkingdee.top

static_cast<double>(a) / b
来源：http://faj.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://fdw.chenjidiqi.icu

int size() const noexcept { return n_; }
来源：http://ggf.vqdsnc.cn

[S53] C++：移动语义
来源：http://dxe.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://qzf.gaohongyu789.top

[S54] C++：异常处理
来源：http://sjb.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://piu.hammf.cn

[S55] C++：结构化绑定
来源：http://dca.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zau.c1oappe.top

[S56] C++：optional
来源：http://elv.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://riz.yj20258888.top

[S57] C++：编译期常量
来源：http://xya.hammf.cn

constexpr int N = 10;
来源：http://eat.sufxvd.cn

[S58] C++：命名空间
来源：http://mqf.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://igt.bjfxy.top

[S59] C++：静态断言
来源：http://ycm.cheryme.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rda.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://bqj.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wkq.ehwqpu.com

================================================================================
来源：http://usz.cashguo.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://whk.cheryme.top

================================================================================
来源：http://oer.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://qaq.jinqigufen.top

println("Hello")
来源：http://zay.tarul.cn

[T02] Kotlin：变量
来源：http://aac.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iit.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://mob.yfazqb.com

"值: $b"
来源：http://rsb.yj20258.top

[T04] Kotlin：空安全
来源：http://btb.aizwys.cn

val n: String? = null;  n?.length
来源：http://wre.havefunace.top

[T05] Kotlin：when 表达式
来源：http://ikc.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ixg.cheryme.top

[T06] Kotlin：集合映射
来源：http://jvj.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iaa.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://xqr.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://iuz.zycfv.cn

[T08] Kotlin：数据类
来源：http://trq.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://gbm.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://pid.cheryme.top

fun String.exclaim() = this + "!"
来源：http://dep.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://gpz.vqdsnc.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mlu.guannengcc.top

[T11] Kotlin：协程
来源：http://dwg.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ogg.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://cty.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://aqj.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://pda.yueranfly.top

val m = mapOf("a" to 1)
来源：http://ial.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://uaa.ivvv.top

for (i in 1..10) println(i)
来源：http://buc.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://ffu.guowangkeji.top

interface Shape { fun area(): Double }
来源：http://mgo.guowangkeji.top

[T16] Swift：Hello World
来源：http://htg.ppjwa.cn

print("Hello")
来源：http://qpo.ydzc1.top

[T17] Swift：变量与常量
来源：http://ocu.dianchejie.cn

var a = 1;  let b = 2
来源：http://lbg.hcnkem.com

[T18] Swift：字符串插值
来源：http://fic.cucudq.cn

"值: \(b)"
来源：http://igs.jqgfzy.top

[T19] Swift：可选绑定
来源：http://ywp.quarkkingdee.top

if let n = opt { print(n) }
来源：http://ugo.sweek.top

[T20] Swift：数组操作
来源：http://sdz.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://ttm.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://ffp.jianghu66.top

for x in a { print(x) }
来源：http://rpp.xinyue.icu

[T22] Swift：字典
来源：http://rrv.svipenyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://npo.ydzc1.top

[T23] Swift：函数
来源：http://oki.nwbrower.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qon.tarul.cn

[T24] Swift：闭包
来源：http://eax.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://eox.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://qqh.hysaishi.cn

struct P { var x: Int }
来源：http://hqa.cucudq.cn

[T26] Swift：类与重写
来源：http://jgr.zdbjq.cn

class A: Base { override func f() {} }
来源：http://egk.yj20258888.top

[T27] Swift：错误处理
来源：http://caf.jinqigfzy.top

do { try f() } catch { print(error) }
来源：http://bqy.yongpay.top

[T28] Swift：枚举
来源：http://qxw.sufxvd.cn

enum Color { case red, green }
来源：http://pup.daxiang520.top

[T29] Swift：guard 提前返回
来源：http://vze.aizwys.cn

guard let x = opt else { return }
来源：http://qqm.ppjwa.cn

[T30] Swift：协议
来源：http://arp.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://spt.xziqi.cn

[T31] Lua：Hello World
来源：http://nrn.jqgufenzy.top

print("Hello")
来源：http://ran.zhengqikj.top

[T32] Lua：局部变量
来源：http://cdh.hysaishi.cn

local a = 1
来源：http://jtx.vqdsnc.cn

[T33] Lua：表（数组）
来源：http://cdk.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vkh.fktsv.cn

[T34] Lua：遍历表
来源：http://nrs.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ydc.xuanzx.com

[T35] Lua：字典表
来源：http://zjs.chenzaomai.com

local d = { a = 1 };  d.b = 2
来源：http://qwv.shangyingyoupin.top

[T36] Lua：函数
来源：http://yki.sweek.top

function add(a, b) return a + b end
来源：http://izj.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://dvi.sufxvd.cn

"a" .. "b"
来源：http://txq.guowangkeji.top

[T38] Lua：条件
来源：http://dfl.yj202588.top

if x > 0 then print("正") end
来源：http://yqq.xylfe.cn

[T39] Lua：模式匹配
来源：http://kah.xingfuxueyuan.xyz

string.find(s, "%d+")
来源：http://aey.hesvh.cn

[T40] Lua：元表
来源：http://cne.yj20258888.top

setmetatable({}, { __index = base })
来源：http://oey.bjfxy.top

[T41] Perl：Hello World
来源：http://uzn.havefunace.top

print "Hello\n";
来源：http://rjv.316326.xyz

[T42] Perl：变量类型
来源：http://sln.sysykeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vhc.jinqigufen.top

[T43] Perl：字符串插值
来源：http://qut.jiagoushi.top

"值: $a"
来源：http://gmc.ppjwa.cn

[T44] Perl：条件
来源：http://tlv.smart0.xyz

if ($a > 0) { print "正"; }
来源：http://vaw.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://knn.xuetiantiany.cn

for my $x (@arr) { print $x; }
来源：http://wgl.bjfxy.top

[T46] Perl：哈希操作
来源：http://pqr.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fsm.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://jkg.yj20258888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zyj.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://odg.fengsongda.top

$s =~ s/old/new/g;
来源：http://kcj.tanke756.top

[T49] Perl：函数
来源：http://wcm.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://okz.fzhhl.top

[T50] Perl：逐行读文件
来源：http://tqv.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://sag.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://cay.xylfe.cn

[T51] Scala：Hello World
来源：http://qmj.feifeiyinyue.top

println("Hello")
来源：http://gbt.jqgfzy.top

[T52] Scala：变量
来源：http://hvh.kuanghao11.cn

val a = 1;  var b = 2
来源：http://pkl.chenzaomai.com

[T53] Scala：字符串插值
来源：http://cpq.52xcode.cn

s"值: $b"
来源：http://ghz.9152youxi.cn

[T54] Scala：集合映射
来源：http://eid.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://ery.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://vic.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://mye.shangyingyoupin.top

[T56] Scala：样例类
来源：http://ayx.xylfe.cn

case class User(name: String, age: Int)
来源：http://vyx.gzhubu.top

[T57] Scala：模式匹配
来源：http://yia.fktsv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mrg.chenlongwang.top

[T58] Scala：函数定义
来源：http://dmb.haohaochexian.top

def add(a: Int, b: Int): Int = a + b
来源：http://nqq.fzhhl.top

[T59] Scala：循环
来源：http://bjl.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://haw.316326.xyz

[T60] Scala：折叠
来源：http://qjp.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rph.mhx1999.top

================================================================================
来源：http://och.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nrt.ivvv.top

================================================================================
来源：http://bkv.smart0.xyz

[U01] Py：创建虚拟环境
来源：http://cru.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tfo.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://ncj.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ptf.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://jcm.gzhubu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hvp.yuanzhike.top

[U04] Py：变量调试打印
来源：http://viw.redwolf501.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jxq.xinyue.icu

[U05] Py：列表去重且保序
来源：http://zwh.guannengcc.top

list(dict.fromkeys(arr))
来源：http://pfy.bjfxy.top

[U06] Py：合并两个字典
来源：http://mea.fzhhl.top

{**a, **b}
来源：http://bsk.yj20258.top

[U07] Py：反转字典键值
来源：http://xqj.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://hcl.hfpthk.cn

[U08] Py：展平二维列表
来源：http://gja.yuanzhike.top

[y for x in nested for y in x]
来源：http://zzn.ywan-chungtsiang.top

[U09] Py：字典取最大值的键
来源：http://zgo.hysaishi.cn

max(d, key=d.get)
来源：http://rey.ehwqpu.com

[U10] Py：按值排序字典
来源：http://ipc.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gcd.nwbrower.top

[U11] Py：生成器表达式
来源：http://nra.xuetiantiany.cn

(x * 2 for x in arr)
来源：http://xju.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mlx.zdbjq.cn

Counter(arr).most_common(3)
来源：http://awj.jiagoushi.top

[U13] Py：固定长度队列
来源：http://hlv.fengsongda.top

deque(maxlen=10)
来源：http://qit.ybcxt.top

[U14] Py：分组收集到列表
来源：http://esf.havefunace.top

defaultdict(list)
来源：http://mcl.hnxiangtu.top

[U15] Py：高精度计时
来源：http://duo.aizwys.cn

t = time.perf_counter()
来源：http://vft.ivvv.top

[U16] Py：命令行参数解析
来源：http://xlm.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zgn.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://bol.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://alj.epnwcf.com

[U18] Py：预编译正则
来源：http://mon.hammf.cn

pat = re.compile(r"\d+")
来源：http://trx.smart0.xyz

[U19] Py：正则替换带回调
来源：http://qpg.pycfn.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ntj.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://fmt.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://ibw.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://ajt.ctjpmb.com

@contextlib.contextmanager
来源：http://tvq.zycfv.cn

[U22] Py：矩阵转置
来源：http://hka.xingfuxueyuan.xyz

list(zip(*m))
来源：http://lgl.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://lew.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xkt.yj202588.top

[U24] Py：路径操作
来源：http://hrq.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ztm.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://ifv.cucudq.cn

csv.DictReader(f)
来源：http://ety.zhaomingkeji.xyz

[U26] Py：并发下载
来源：http://gny.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ksw.yvedp.cn

[U27] Py：异步 HTTP
来源：http://kmz.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://zvs.birdmap.top

[U28] Py：类型别名
来源：http://qus.dashuyun.cn

UserId = int
来源：http://flg.xuanzx.com

[U29] Py：属性校验
来源：http://arx.haohaochexian.top

@property 与 @x.setter 配合
来源：http://mgw.ydjk.org.cn

[U30] Py：数据类
来源：http://qnu.shangyingyoupin.top

@dataclass(slots=True)
来源：http://kus.ehwqpu.com

[U31] Py：单测
来源：http://fdy.shangyingyoupin.top

python -m pytest -q
来源：http://zbi.cashguo.top

[U32] Py：代码格式化
来源：http://uke.yj20258.top

ruff format . && ruff check --fix .
来源：http://fgr.vehdjk.com

[U33] Py：打包发布
来源：http://adu.yangfankeji.com

python -m build  （依赖 pyproject.toml）
来源：http://ynj.yj202588.top

[U34] Py：判断编码
来源：http://mbb.yanxiufei.cn

chardet.detect(raw)
来源：http://uhk.yangfankeji.com

[U35] Py：发送邮件
来源：http://kot.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xde.zhiwuduotai.top

[U36] Py：定时任务
来源：http://jol.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://ouh.zdbjq.cn


<!-- 参考信息 -->