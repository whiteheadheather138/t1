代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://fqu.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ofz.fktsv.cn

fclose(f);
来源：http://aoz.yanxiufei.cn

[S12] C：写文件
来源：http://nae.dianchejie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://adj.chenzaomai.com

[S13] C：宏定义
来源：http://sbu.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wxf.hongshengwenyu.top

[S14] C：枚举
来源：http://wsd.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://iov.0kj1m.cn

[S15] C：类型转换
来源：http://qvu.hammf.cn

(double) a / b
来源：http://qev.jinqigufen.top

[S16] C：位操作置位
来源：http://dkz.yonumen.top

x |= (1 << 3);
来源：http://rbg.fzhhl.top

[S17] C：安全拼接字符串
来源：http://uuq.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sou.hammf.cn

[S18] C：命令行参数
来源：http://row.yj20258.top

int main(int argc, char **argv)
来源：http://bqi.tanke756.top

[S19] C：快速排序
来源：http://stu.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://juj.shangyingyoupin.top

[S20] C：二分查找
来源：http://xlg.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wrt.yongpay.top

[S21] C：字符类别判断
来源：http://hke.aizwys.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rwe.quarkkingdee.top

[S22] C：字符串转数字
来源：http://cdf.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mlu.ctjpmb.com

[S23] C：随机数
来源：http://sdc.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://owt.shanyushiyangkeji.top

[S24] C：获取本地时间
来源：http://fer.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mwl.gogol.net.cn

[S25] C：内存拷贝
来源：http://fug.yuanzhike.top

memcpy(dst, src, n);
来源：http://qhd.uphjek.com

[S26] C：内存清零
来源：http://lvw.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://eik.wangdashe.top

[S27] C：定义常量
来源：http://ijq.xuetiantiany.cn

const double PI = 3.14159;
来源：http://sjr.hysaishi.cn

[S28] C：静态变量
来源：http://mkq.cucudq.cn

static int counter = 0;
来源：http://lcm.jinghuilouyu.cn

[S29] C：变参函数
来源：http://rjt.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://slu.yj20258888.top

[S30] C：头文件保护
来源：http://gpn.ybcxt.top

#ifndef X_H
来源：http://wic.chenlongwang.top

#define X_H
来源：http://iua.zhengqikj.top

#endif
来源：http://wtl.jqgfzy.top

[S31] C++：Hello World
来源：http://dwm.shangyingyoupin.top

#include <iostream>
来源：http://xfq.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://nuk.yueranfly.top

[S32] C++：字符串
来源：http://tir.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://cpk.dianchejie.cn

[S33] C++：vector 增删
来源：http://pzx.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://imw.xziqi.cn

[S34] C++：遍历 vector
来源：http://zmi.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://hxr.jiagoushi.top

[S35] C++：map
来源：http://gei.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nnc.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://yqd.quarkkingdee.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://icx.jianghu66.top

[S37] C++：set
来源：http://err.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wwd.ehwqpu.com

[S38] C++：排序
来源：http://cis.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://jel.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://djp.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qhs.hesvh.cn

[S40] C++：查找元素
来源：http://xbo.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://inb.yfazqb.com

[S41] C++：类与构造函数
来源：http://awd.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dvo.pycfn.com

[S42] C++：继承与虚函数
来源：http://zky.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://bgq.quarkkingdee.top

[S43] C++：智能指针
来源：http://ecj.haohaochexian.top

auto p = std::make_unique<int>(5);
来源：http://bar.svipenyu.cn

[S44] C++：引用传参
来源：http://bkn.jqgfzy.top

void inc(int &x) { ++x; }
来源：http://kqc.zhiwuduotai.top

[S45] C++：lambda
来源：http://ynf.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://qhc.tianlin.xyz

[S46] C++：函数模板
来源：http://deq.jinqigufen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://col.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://hdq.vqdsnc.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sgj.shanyushiyangkeji.top

[S48] C++：逐行读文件
来源：http://opn.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uex.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://lto.xziqi.cn

[S49] C++：写文件
来源：http://pms.daxiang520.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iab.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://bxg.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://phg.shzxlz.cn

[S51] C++：显式类型转换
来源：http://eox.xuanzx.com

static_cast<double>(a) / b
来源：http://qct.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://bwn.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://edi.hammf.cn

[S53] C++：移动语义
来源：http://uti.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://djg.chenzaomai.com

[S54] C++：异常处理
来源：http://raf.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wei.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://hus.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pcj.wangdashe.top

[S56] C++：optional
来源：http://dxt.snrcjt.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yiz.birdmap.top

[S57] C++：编译期常量
来源：http://xwq.jinqigufen.top

constexpr int N = 10;
来源：http://uma.zycfv.cn

[S58] C++：命名空间
来源：http://nqb.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://ukj.tian-w.cn

[S59] C++：静态断言
来源：http://brs.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qcg.shanyushiyangtech.top

[S60] C++：遍历并删除元素
来源：http://hnl.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tzn.vqdsnc.cn

================================================================================
来源：http://ngw.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lti.jinqigfzy.top

================================================================================
来源：http://vux.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://rdo.gotoacloud.top

println("Hello")
来源：http://vtd.cqqwz.cn

[T02] Kotlin：变量
来源：http://omz.hnxiangtu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gux.pengpengdd.cyou

[T03] Kotlin：字符串模板
来源：http://rpr.xingfuxueyuan.xyz

"值: $b"
来源：http://qbl.c1oappe.top

[T04] Kotlin：空安全
来源：http://ugi.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://ehk.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://zrh.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pzb.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://tli.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://txm.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://krx.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://leb.uphjek.com

[T08] Kotlin：数据类
来源：http://tcx.birdmap.top

data class User(val name: String, val age: Int)
来源：http://kux.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://zda.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://blg.dianchejie.cn

[T10] Kotlin：默认参数
来源：http://hqu.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ohj.ybcxt.top

[T11] Kotlin：协程
来源：http://wyv.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ttt.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://rit.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://ugn.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://slu.xinyue.icu

val m = mapOf("a" to 1)
来源：http://xuu.fehbvm.com

[T14] Kotlin：循环
来源：http://oal.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://hjg.yueranfly.top

[T15] Kotlin：接口
来源：http://itw.birdmap.top

interface Shape { fun area(): Double }
来源：http://tba.andypj.xyz

[T16] Swift：Hello World
来源：http://jps.ivvv.top

print("Hello")
来源：http://zak.zdbjq.cn

[T17] Swift：变量与常量
来源：http://zkz.sweek.top

var a = 1;  let b = 2
来源：http://nfu.cucudq.cn

[T18] Swift：字符串插值
来源：http://rfv.cashguo.top

"值: \(b)"
来源：http://jpd.zdbjq.cn

[T19] Swift：可选绑定
来源：http://dru.epnwcf.com

if let n = opt { print(n) }
来源：http://sat.ctjpmb.com

[T20] Swift：数组操作
来源：http://cdg.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xjy.zhongyouzk.top

[T21] Swift：遍历
来源：http://tly.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://qgn.jqgufenzy.top

[T22] Swift：字典
来源：http://ice.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://rrt.zhijiandao.cn

[T23] Swift：函数
来源：http://xdu.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ijz.tianlin.xyz

[T24] Swift：闭包
来源：http://uwm.havefunace.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wdm.dianchejie.cn

[T25] Swift：结构体
来源：http://hcv.yueranfly.top

struct P { var x: Int }
来源：http://xro.uphjek.com

[T26] Swift：类与重写
来源：http://xso.xuanzx.com

class A: Base { override func f() {} }
来源：http://mzd.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://qec.cashguo.top

do { try f() } catch { print(error) }
来源：http://bki.hnqzz.top

[T28] Swift：枚举
来源：http://eci.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://kcd.yonumen.top

[T29] Swift：guard 提前返回
来源：http://xmq.0kj1m.cn

guard let x = opt else { return }
来源：http://tex.fktsv.cn

[T30] Swift：协议
来源：http://zbm.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://iau.zycfv.cn

[T31] Lua：Hello World
来源：http://awx.snrcjt.cn

print("Hello")
来源：http://cxf.cdnleiting.top

[T32] Lua：局部变量
来源：http://kcs.guannengcc.top

local a = 1
来源：http://uri.haohaochexian.top

[T33] Lua：表（数组）
来源：http://srq.shangyingyoupin.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jrr.yuxming.cn

[T34] Lua：遍历表
来源：http://zwl.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://osb.zhixingplan.top

[T35] Lua：字典表
来源：http://yuz.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://euw.daxiang520.top

[T36] Lua：函数
来源：http://qtf.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://oiu.ydjk.org.cn

[T37] Lua：字符串拼接
来源：http://anp.bbcook.cn

"a" .. "b"
来源：http://nkz.smart0.xyz

[T38] Lua：条件
来源：http://nit.sysykeji.top

if x > 0 then print("正") end
来源：http://tff.ywan-chungtsiang.top

[T39] Lua：模式匹配
来源：http://tal.andypj.xyz

string.find(s, "%d+")
来源：http://ydd.bbcook.cn

[T40] Lua：元表
来源：http://sol.yongpay.top

setmetatable({}, { __index = base })
来源：http://nbs.sweek.top

[T41] Perl：Hello World
来源：http://hem.yj20258.top

print "Hello\n";
来源：http://qfo.vqdsnc.cn

[T42] Perl：变量类型
来源：http://drl.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hty.jianghu66.top

[T43] Perl：字符串插值
来源：http://nfi.pengpengdd.cyou

"值: $a"
来源：http://tuc.yueranfly.top

[T44] Perl：条件
来源：http://yfl.yangfankeji.com

if ($a > 0) { print "正"; }
来源：http://bka.iojbl.cn

[T45] Perl：数组遍历
来源：http://zki.xuanzx.com

for my $x (@arr) { print $x; }
来源：http://obw.zhiwuduotai.top

[T46] Perl：哈希操作
来源：http://wtd.wangdashe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pci.sweek.top

[T47] Perl：正则捕获
来源：http://qor.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://csi.zhoulong.xyz

[T48] Perl：正则替换
来源：http://hzl.zycfv.cn

$s =~ s/old/new/g;
来源：http://oma.hongshengwenyu.top

[T49] Perl：函数
来源：http://guv.jyoumei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ddu.xylfe.cn

[T50] Perl：逐行读文件
来源：http://uzn.pycfn.com

open my $fh, "<", "a.txt" or die $!;
来源：http://heo.ydzc1.top

while (my $line = <$fh>) { print $line; }
来源：http://mcn.epnwcf.com

[T51] Scala：Hello World
来源：http://azw.wangdashe.top

println("Hello")
来源：http://iyu.nanxuanxn.top

[T52] Scala：变量
来源：http://kqz.jianghu66.top

val a = 1;  var b = 2
来源：http://xlx.yueranfly.top

[T53] Scala：字符串插值
来源：http://uyh.zycfv.cn

s"值: $b"
来源：http://utp.yj202588.top

[T54] Scala：集合映射
来源：http://vut.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://eoq.316326.xyz

[T55] Scala：集合过滤
来源：http://lbs.yonumen.top

List(1, 2, 3).filter(_ > 1)
来源：http://afp.hfpthk.cn

[T56] Scala：样例类
来源：http://avw.xinyue.icu

case class User(name: String, age: Int)
来源：http://oxq.dianchejie.cn

[T57] Scala：模式匹配
来源：http://dmb.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://gka.sysykeji.top

[T58] Scala：函数定义
来源：http://qts.sxryk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mlp.snrcjt.cn

[T59] Scala：循环
来源：http://fja.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://kio.daria6918.cn

[T60] Scala：折叠
来源：http://otq.wangdashe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hpg.feifeiyinyue.top

================================================================================
来源：http://ihl.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rse.yfazqb.com

================================================================================
来源：http://dhi.zhixingplan.top

[U01] Py：创建虚拟环境
来源：http://lou.0kj1m.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zoo.daxiang520.top

[U02] Py：导出 / 安装依赖
来源：http://axb.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bip.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://puw.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dxi.ivvv.top

[U04] Py：变量调试打印
来源：http://mjc.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vsr.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://kwq.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://kts.aizwys.cn

[U06] Py：合并两个字典
来源：http://bgb.jyoumei.cn

{**a, **b}
来源：http://dna.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://gcr.zdqjudy.top

{v: k for k, v in d.items()}
来源：http://fht.gogol.net.cn

[U08] Py：展平二维列表
来源：http://sit.ybcxt.top

[y for x in nested for y in x]
来源：http://vcw.hywenlv.cn

[U09] Py：字典取最大值的键
来源：http://nhk.feifeiyinyue.top

max(d, key=d.get)
来源：http://ryc.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://yhp.xingfuxueyuan.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qyk.316326.xyz

[U11] Py：生成器表达式
来源：http://ncs.andypj.xyz

(x * 2 for x in arr)
来源：http://zoq.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://toe.sjlbkw.cn

Counter(arr).most_common(3)
来源：http://fpl.sufxvd.cn

[U13] Py：固定长度队列
来源：http://igl.hongshengwenyu.top

deque(maxlen=10)
来源：http://qye.smart0.xyz

[U14] Py：分组收集到列表
来源：http://ach.hysaishi.cn

defaultdict(list)
来源：http://roo.fengsongda.top

[U15] Py：高精度计时
来源：http://fqw.pengpengdd.cyou

t = time.perf_counter()
来源：http://vdb.smart0.xyz

[U16] Py：命令行参数解析
来源：http://qfn.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://seo.ybcxt.top

[U17] Py：初始化日志
来源：http://rwp.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://txb.feifeiyinyue.top

[U18] Py：预编译正则
来源：http://qay.nanxinkj.top

pat = re.compile(r"\d+")
来源：http://dtu.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://pok.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rbt.shuidangran.top

[U20] Py：缓存函数结果
来源：http://bha.smart0.xyz

@functools.lru_cache(maxsize=None)
来源：http://hte.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://wdx.ehwqpu.com

@contextlib.contextmanager
来源：http://yoz.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://kdr.chenjidiqi.icu

list(zip(*m))
来源：http://laz.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://zwz.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oln.yonumen.top

[U24] Py：路径操作
来源：http://qvp.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bnq.tanke756.top

[U25] Py：CSV 按字典读
来源：http://rhr.jinqigufen.top

csv.DictReader(f)
来源：http://njm.ehwqpu.com

[U26] Py：并发下载
来源：http://jyv.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://enx.hammf.cn

[U27] Py：异步 HTTP
来源：http://idl.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://lnh.yueranfly.top

[U28] Py：类型别名
来源：http://vcp.xuanzx.com

UserId = int
来源：http://msl.meibo888.top

[U29] Py：属性校验
来源：http://yce.yanxiufei.cn

@property 与 @x.setter 配合
来源：http://hao.zhixingplan.top

[U30] Py：数据类
来源：http://czz.yj20258888.top

@dataclass(slots=True)
来源：http://npu.xuanzx.com

[U31] Py：单测
来源：http://htd.fzhhl.top

python -m pytest -q
来源：http://qql.redwolf501.top

[U32] Py：代码格式化
来源：http://hbb.tian-w.cn

ruff format . && ruff check --fix .
来源：http://jac.9152youxi.cn

[U33] Py：打包发布
来源：http://mdp.ydzc1.top

python -m build  （依赖 pyproject.toml）
来源：http://qdv.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://tuy.cheryme.top

chardet.detect(raw)
来源：http://fxc.sjlbkw.cn


<!-- 参考信息 -->