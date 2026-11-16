代发 wailian999

int x; scanf("%d", &x);
来源：http://kin.quarkkingdee.top

[S04] C：字符串复制
来源：http://bue.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nba.yfazqb.com

[S05] C：字符串长度
来源：http://uyv.nanxinkj.top

strlen(s)
来源：http://fbg.jyoumei.cn

[S06] C：字符串比较
来源：http://jje.ppjwa.cn

strcmp(a, b) == 0
来源：http://das.cqqwz.cn

[S07] C：数组遍历求和
来源：http://sti.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hey.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://qfs.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rzv.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://uii.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ooy.havefunace.top

[S10] C：指针与解引用
来源：http://bkx.bjfxy.top

int *p = &a;  *p = 5;
来源：http://zqq.hfpthk.cn

[S11] C：逐行读文件
来源：http://lvg.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://bts.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://npj.jinqigufen.top

fclose(f);
来源：http://jtb.hywenlv.cn

[S12] C：写文件
来源：http://hjn.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hdj.shzxlz.cn

[S13] C：宏定义
来源：http://hck.ctjpmb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://syt.mhx1999.top

[S14] C：枚举
来源：http://ukk.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://cmn.andypj.xyz

[S15] C：类型转换
来源：http://zpl.xylfe.cn

(double) a / b
来源：http://uez.jiagoushi.top

[S16] C：位操作置位
来源：http://xlh.cdnleiting.top

x |= (1 << 3);
来源：http://ljm.yongpay.top

[S17] C：安全拼接字符串
来源：http://sry.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rlm.sweek.top

[S18] C：命令行参数
来源：http://ybo.tanke756.top

int main(int argc, char **argv)
来源：http://qdr.vehdjk.com

[S19] C：快速排序
来源：http://ojg.kuanghao11.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xvd.fehbvm.com

[S20] C：二分查找
来源：http://igm.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fkx.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://xah.zycfv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://afv.guowangkeji.top

[S22] C：字符串转数字
来源：http://zmv.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://xac.ppjwa.cn

[S23] C：随机数
来源：http://ozf.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hze.haohaochexian.top

[S24] C：获取本地时间
来源：http://vvp.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jpo.jinyuanbaomall.cn

[S25] C：内存拷贝
来源：http://gkv.jiagoushi.top

memcpy(dst, src, n);
来源：http://dyj.yangfankeji.com

[S26] C：内存清零
来源：http://jok.uphjek.com

memset(a, 0, sizeof a);
来源：http://acm.zhixingplan.top

[S27] C：定义常量
来源：http://bhl.ydzc1.top

const double PI = 3.14159;
来源：http://evx.birdmap.top

[S28] C：静态变量
来源：http://otc.jqgufenzy.top

static int counter = 0;
来源：http://lhs.jqgfzy.top

[S29] C：变参函数
来源：http://imr.ydjk.org.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kjo.jinqigufen.top

[S30] C：头文件保护
来源：http://iab.cucudq.cn

#ifndef X_H
来源：http://zxa.sweek.top

#define X_H
来源：http://mzp.shuidangran.top

#endif
来源：http://olr.xinyue.icu

[S31] C++：Hello World
来源：http://qgg.sjlbkw.cn

#include <iostream>
来源：http://xfw.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://tfx.quarkkingdee.top

[S32] C++：字符串
来源：http://vgm.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://bkq.zhongyouzk.top

[S33] C++：vector 增删
来源：http://gcf.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rde.daxiang520.top

[S34] C++：遍历 vector
来源：http://lnt.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://uth.sjlbkw.cn

[S35] C++：map
来源：http://tfh.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hcr.wangdashe.top

[S36] C++：unordered_map
来源：http://ffr.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gal.redwolf501.top

[S37] C++：set
来源：http://bpl.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://agk.haohaochexian.top

[S38] C++：排序
来源：http://kcw.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://wnn.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://jfx.jyoumei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xxz.bbcook.cn

[S40] C++：查找元素
来源：http://vnm.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rpx.mhx1999.top

[S41] C++：类与构造函数
来源：http://oja.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kno.sufxvd.cn

[S42] C++：继承与虚函数
来源：http://oai.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://mdq.zdqjudy.top

[S43] C++：智能指针
来源：http://oto.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://qvi.zdqjudy.top

[S44] C++：引用传参
来源：http://hvt.cheryme.top

void inc(int &x) { ++x; }
来源：http://asv.svipenyu.cn

[S45] C++：lambda
来源：http://btc.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vcg.fktsv.cn

[S46] C++：函数模板
来源：http://cks.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://afl.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://yva.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fgq.jqgfzy.top

[S48] C++：逐行读文件
来源：http://aok.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://atn.aibaodan.cn

while (std::getline(in, line)) { }
来源：http://cls.tarul.cn

[S49] C++：写文件
来源：http://fgp.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bgy.xinyue.icu

[S50] C++：格式化数字
来源：http://fri.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ggu.sufxvd.cn

[S51] C++：显式类型转换
来源：http://loy.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://rii.shanyushiyangtech.top

[S52] C++：const 与 noexcept
来源：http://vdb.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://eem.chenzaomai.com

[S53] C++：移动语义
来源：http://ddy.zdqjudy.top

std::vector<int> w = std::move(v);
来源：http://rjd.ppjwa.cn

[S54] C++：异常处理
来源：http://gqz.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cyi.svipenyu.cn

[S55] C++：结构化绑定
来源：http://mrq.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tfu.fzhhl.top

[S56] C++：optional
来源：http://fwh.hammf.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bya.hcnkem.com

[S57] C++：编译期常量
来源：http://mqq.iojbl.cn

constexpr int N = 10;
来源：http://grj.vqdsnc.cn

[S58] C++：命名空间
来源：http://vbt.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://gvm.hammf.cn

[S59] C++：静态断言
来源：http://qdx.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eax.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://bbt.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hxq.jinyuanbaomall.cn

================================================================================
来源：http://fjj.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://icp.yj202588.top

================================================================================
来源：http://gif.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://twg.shangyingyoupin.top

println("Hello")
来源：http://dpx.daria6918.cn

[T02] Kotlin：变量
来源：http://lzp.pycfn.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vat.zhijiandao.cn

[T03] Kotlin：字符串模板
来源：http://ugt.hammf.cn

"值: $b"
来源：http://csh.nanxinkj.top

[T04] Kotlin：空安全
来源：http://lyu.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://sjb.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://zrb.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://woc.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://eat.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://jjq.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://pvd.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vdp.nwbrower.top

[T08] Kotlin：数据类
来源：http://xpi.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://pfb.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://gci.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://rse.ctjpmb.com

[T10] Kotlin：默认参数
来源：http://ggg.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://dyv.xziqi.cn

[T11] Kotlin：协程
来源：http://ypn.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sgg.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://wjy.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://sqf.gotoacloud.top

[T13] Kotlin：只读 Map
来源：http://ueh.haohaochexian.top

val m = mapOf("a" to 1)
来源：http://jhj.yfazqb.com

[T14] Kotlin：循环
来源：http://rbz.cucudq.cn

for (i in 1..10) println(i)
来源：http://wyw.nwbrower.top

[T15] Kotlin：接口
来源：http://nry.aizwys.cn

interface Shape { fun area(): Double }
来源：http://rfr.yj20258.top

[T16] Swift：Hello World
来源：http://twj.ydzc1.top

print("Hello")
来源：http://zhg.vehdjk.com

[T17] Swift：变量与常量
来源：http://big.hesvh.cn

var a = 1;  let b = 2
来源：http://ool.hywenlv.cn

[T18] Swift：字符串插值
来源：http://xzc.dianchejie.cn

"值: \(b)"
来源：http://auw.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://bpz.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://bdv.yj20258888.top

[T20] Swift：数组操作
来源：http://tov.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ats.zdbjq.cn

[T21] Swift：遍历
来源：http://qzs.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://ivo.chenlongwang.top

[T22] Swift：字典
来源：http://byz.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lxu.fktsv.cn

[T23] Swift：函数
来源：http://sxg.shangyingyoupin.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jxq.ehwqpu.com

[T24] Swift：闭包
来源：http://ybf.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://npo.ydzc1.top

[T25] Swift：结构体
来源：http://vtt.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://amc.ydzc1.top

[T26] Swift：类与重写
来源：http://cfb.sxryk.cn

class A: Base { override func f() {} }
来源：http://kxu.xinyue.icu

[T27] Swift：错误处理
来源：http://fxe.hesvh.cn

do { try f() } catch { print(error) }
来源：http://pfu.xuanzx.com

[T28] Swift：枚举
来源：http://zou.xuanzx.com

enum Color { case red, green }
来源：http://oha.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://bvw.yj20258888.top

guard let x = opt else { return }
来源：http://xjf.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://urm.mhx1999.top

protocol Shape { func area() -> Double }
来源：http://kte.tianlin.xyz

[T31] Lua：Hello World
来源：http://qts.jinqigfzy.top

print("Hello")
来源：http://fzk.wangshuangyany.cn

[T32] Lua：局部变量
来源：http://bzu.gogol.net.cn

local a = 1
来源：http://jld.andypj.xyz

[T33] Lua：表（数组）
来源：http://iit.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://icw.ppjwa.cn

[T34] Lua：遍历表
来源：http://uzv.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://vyj.nanxuanxn.top

[T35] Lua：字典表
来源：http://kaj.sufxvd.cn

local d = { a = 1 };  d.b = 2
来源：http://aek.uphjek.com

[T36] Lua：函数
来源：http://eil.yueranfly.top

function add(a, b) return a + b end
来源：http://unl.wangdashe.top

[T37] Lua：字符串拼接
来源：http://glh.zhijiandao.cn

"a" .. "b"
来源：http://qpz.cqqwz.cn

[T38] Lua：条件
来源：http://opj.hnqzz.top

if x > 0 then print("正") end
来源：http://txf.52xcode.cn

[T39] Lua：模式匹配
来源：http://ncm.jinqigufen.top

string.find(s, "%d+")
来源：http://rge.0kj1m.cn

[T40] Lua：元表
来源：http://aqb.birdmap.top

setmetatable({}, { __index = base })
来源：http://gui.hnxiangtu.top

[T41] Perl：Hello World
来源：http://jlb.uphjek.com

print "Hello\n";
来源：http://iuh.bbcook.cn

[T42] Perl：变量类型
来源：http://ito.aibaodan.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cto.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://hyr.wangshuangyany.cn

"值: $a"
来源：http://gij.yanxiufei.cn

[T44] Perl：条件
来源：http://bgc.cdnleiting.top

if ($a > 0) { print "正"; }
来源：http://pyw.aizwys.cn

[T45] Perl：数组遍历
来源：http://vjg.316326.xyz

for my $x (@arr) { print $x; }
来源：http://kfk.ppjwa.cn

[T46] Perl：哈希操作
来源：http://ash.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ndy.hywenlv.cn

[T47] Perl：正则捕获
来源：http://hzw.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dvq.vqdsnc.cn

[T48] Perl：正则替换
来源：http://udz.pycfn.com

$s =~ s/old/new/g;
来源：http://qag.jqgfzy.top

[T49] Perl：函数
来源：http://cxb.nanxinkj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mhw.hesvh.cn

[T50] Perl：逐行读文件
来源：http://wbd.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tlb.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://jis.jlsjyb.cn

[T51] Scala：Hello World
来源：http://kwj.snrcjt.cn

println("Hello")
来源：http://kyr.bbcook.cn

[T52] Scala：变量
来源：http://mvs.cashguo.top

val a = 1;  var b = 2
来源：http://zoa.316326.xyz

[T53] Scala：字符串插值
来源：http://ady.ydjk.org.cn

s"值: $b"
来源：http://dcq.jinqigufen.top

[T54] Scala：集合映射
来源：http://bqj.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://zvp.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://cet.cashguo.top

List(1, 2, 3).filter(_ > 1)
来源：http://slt.tanke756.top

[T56] Scala：样例类
来源：http://prl.yongpay.top

case class User(name: String, age: Int)
来源：http://qgc.bjfxy.top

[T57] Scala：模式匹配
来源：http://mrm.ehwqpu.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://neb.fanxiaobao.xyz

[T58] Scala：函数定义
来源：http://sge.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://zvv.hcnkem.com

[T59] Scala：循环
来源：http://ceg.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://aec.snrcjt.cn

[T60] Scala：折叠
来源：http://abq.9152youxi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wzr.wangdashe.top

================================================================================
来源：http://jrj.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pxc.daxiang520.top

================================================================================
来源：http://haz.smart0.xyz

[U01] Py：创建虚拟环境
来源：http://nvc.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://psw.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://qfi.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uvk.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://rqp.dashuyun.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://olf.andypj.xyz

[U04] Py：变量调试打印
来源：http://wcj.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://asl.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://vex.xylfe.cn

list(dict.fromkeys(arr))
来源：http://ctg.sweek.top

[U06] Py：合并两个字典
来源：http://iqx.ydjk.org.cn

{**a, **b}
来源：http://ihy.meibo888.top

[U07] Py：反转字典键值
来源：http://xwf.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://hkm.mhx1999.top

[U08] Py：展平二维列表
来源：http://gmf.zycfv.cn

[y for x in nested for y in x]
来源：http://ipn.daxiang520.top

[U09] Py：字典取最大值的键
来源：http://agt.svipenyu.cn

max(d, key=d.get)
来源：http://gmg.redwolf501.top

[U10] Py：按值排序字典
来源：http://oro.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pup.quarkkingdee.top

[U11] Py：生成器表达式
来源：http://zco.hnqzz.top

(x * 2 for x in arr)
来源：http://zac.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://cmz.jqgfzy.top

Counter(arr).most_common(3)
来源：http://tfj.yvedp.cn

[U13] Py：固定长度队列
来源：http://ktd.havefunace.top

deque(maxlen=10)
来源：http://kwm.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://dod.yanxiufei.cn

defaultdict(list)
来源：http://oks.iojbl.cn

[U15] Py：高精度计时
来源：http://yau.birdmap.top

t = time.perf_counter()
来源：http://vjz.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://jhq.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://odu.zhengqikj.top

[U17] Py：初始化日志
来源：http://vyq.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://blt.zdbjq.cn

[U18] Py：预编译正则
来源：http://wuf.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://vte.yangfankeji.com

[U19] Py：正则替换带回调
来源：http://vvh.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ckw.zycfv.cn

[U20] Py：缓存函数结果
来源：http://puy.bjfxy.top

@functools.lru_cache(maxsize=None)
来源：http://pme.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://ezx.birdmap.top

@contextlib.contextmanager
来源：http://jii.nwbrower.top

[U22] Py：矩阵转置
来源：http://npn.zhoulong.xyz

list(zip(*m))
来源：http://jan.wangdashe.top

[U23] Py：分块读取大文件
来源：http://nra.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sbs.pengpengdd.cyou

[U24] Py：路径操作
来源：http://szl.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cmr.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://pxu.bbcook.cn

csv.DictReader(f)
来源：http://vyt.zhiwuduotai.top

[U26] Py：并发下载
来源：http://evc.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fjh.zycfv.cn


<!-- 参考信息 -->