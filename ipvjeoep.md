代发 wailian999

int x; scanf("%d", &x);
来源：http://vjw.yueranfly.top

[S04] C：字符串复制
来源：http://scu.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://gfv.yj20258888.top

[S05] C：字符串长度
来源：http://hor.cqqwz.cn

strlen(s)
来源：http://sts.shzxlz.cn

[S06] C：字符串比较
来源：http://qgc.fanxiaobao.xyz

strcmp(a, b) == 0
来源：http://vqq.nanxinkj.top

[S07] C：数组遍历求和
来源：http://uzg.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zhx.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://ckg.52xcode.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qux.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://kqy.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://llf.andypj.xyz

[S10] C：指针与解引用
来源：http://ozf.gzhubu.top

int *p = &a;  *p = 5;
来源：http://nlh.iojbl.cn

[S11] C：逐行读文件
来源：http://mcj.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://kdp.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tpx.feifeiyinyue.top

fclose(f);
来源：http://zfg.shuidangran.top

[S12] C：写文件
来源：http://pit.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hhk.redwolf501.top

[S13] C：宏定义
来源：http://xds.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://azd.zhengqikj.top

[S14] C：枚举
来源：http://dza.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://qcy.aizwys.cn

[S15] C：类型转换
来源：http://cqa.ybcxt.top

(double) a / b
来源：http://itk.fehbvm.com

[S16] C：位操作置位
来源：http://fdr.dashuyun.cn

x |= (1 << 3);
来源：http://kkn.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://nfk.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tfl.daxiang520.top

[S18] C：命令行参数
来源：http://nnh.ivvv.top

int main(int argc, char **argv)
来源：http://spy.cucudq.cn

[S19] C：快速排序
来源：http://gis.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ggk.xinyue.icu

[S20] C：二分查找
来源：http://rcc.guowangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://evb.birdmap.top

[S21] C：字符类别判断
来源：http://gio.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zvj.9152youxi.cn

[S22] C：字符串转数字
来源：http://iiq.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://faz.ctjpmb.com

[S23] C：随机数
来源：http://bic.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vcn.vqdsnc.cn

[S24] C：获取本地时间
来源：http://nks.gaohongyu789.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zfs.xinyue.icu

[S25] C：内存拷贝
来源：http://ias.ctjpmb.com

memcpy(dst, src, n);
来源：http://gvd.yvedp.cn

[S26] C：内存清零
来源：http://cbn.fehbvm.com

memset(a, 0, sizeof a);
来源：http://bzp.wangdashe.top

[S27] C：定义常量
来源：http://jgu.redwolf501.top

const double PI = 3.14159;
来源：http://fwb.dashuyun.cn

[S28] C：静态变量
来源：http://cwl.xingfuxueyuan.xyz

static int counter = 0;
来源：http://tnl.quarkkingdee.top

[S29] C：变参函数
来源：http://xei.zhiwuduotai.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gdt.jqgufenzy.top

[S30] C：头文件保护
来源：http://hgg.shanyushiyangtech.top

#ifndef X_H
来源：http://ahm.shzxlz.cn

#define X_H
来源：http://ero.ppjwa.cn

#endif
来源：http://opv.yvedp.cn

[S31] C++：Hello World
来源：http://xic.chenzaomai.com

#include <iostream>
来源：http://yra.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://zno.sufxvd.cn

[S32] C++：字符串
来源：http://ecu.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://erh.yj202588.top

[S33] C++：vector 增删
来源：http://clr.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mdb.zdbjq.cn

[S34] C++：遍历 vector
来源：http://iph.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://scr.hnqzz.top

[S35] C++：map
来源：http://fwe.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iiu.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://vsi.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pit.aibaodan.cn

[S37] C++：set
来源：http://zbp.0kj1m.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kxi.ydjk.org.cn

[S38] C++：排序
来源：http://utq.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://yve.cashguo.top

[S39] C++：自定义比较器排序
来源：http://xfn.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://emj.xuetiantiany.cn

[S40] C++：查找元素
来源：http://nte.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zmk.iojbl.cn

[S41] C++：类与构造函数
来源：http://vnw.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wli.yonumen.top

[S42] C++：继承与虚函数
来源：http://fev.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://swm.svipenyu.cn

[S43] C++：智能指针
来源：http://wns.ydjk.org.cn

auto p = std::make_unique<int>(5);
来源：http://wbz.zdqjudy.top

[S44] C++：引用传参
来源：http://udg.bbcook.cn

void inc(int &x) { ++x; }
来源：http://cuh.cheryme.top

[S45] C++：lambda
来源：http://ply.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ajk.jlsjyb.cn

[S46] C++：函数模板
来源：http://kkc.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pcq.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://vno.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dio.aizwys.cn

[S48] C++：逐行读文件
来源：http://cfn.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://uha.daria6918.cn

while (std::getline(in, line)) { }
来源：http://crv.zdbjq.cn

[S49] C++：写文件
来源：http://vtj.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wgf.tianlin.xyz

[S50] C++：格式化数字
来源：http://urd.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jmi.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://gfg.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://pnk.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://ngx.yfazqb.com

int size() const noexcept { return n_; }
来源：http://qnr.yuxming.cn

[S53] C++：移动语义
来源：http://mka.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://clj.chenlongwang.top

[S54] C++：异常处理
来源：http://nzt.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lxg.hfpthk.cn

[S55] C++：结构化绑定
来源：http://vij.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pak.hesvh.cn

[S56] C++：optional
来源：http://epw.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yog.jiagoushi.top

[S57] C++：编译期常量
来源：http://hcb.dashuyun.cn

constexpr int N = 10;
来源：http://fde.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://jwi.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://alf.svipenyu.cn

[S59] C++：静态断言
来源：http://cjj.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vai.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://gui.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xqz.wangdashe.top

================================================================================
来源：http://qea.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jew.cashguo.top

================================================================================
来源：http://ebm.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://bgx.hesvh.cn

println("Hello")
来源：http://zfc.mhx1999.top

[T02] Kotlin：变量
来源：http://dfu.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kuq.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://ull.aibaodan.cn

"值: $b"
来源：http://zux.cheryme.top

[T04] Kotlin：空安全
来源：http://wgu.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://hje.yj202588.top

[T05] Kotlin：when 表达式
来源：http://vpy.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vbw.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://atw.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uzv.sweek.top

[T07] Kotlin：集合过滤
来源：http://zdx.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://aqz.yangfankeji.com

[T08] Kotlin：数据类
来源：http://ohc.9152youxi.cn

data class User(val name: String, val age: Int)
来源：http://irg.yonumen.top

[T09] Kotlin：扩展函数
来源：http://soy.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://lsk.yueranfly.top

[T10] Kotlin：默认参数
来源：http://irr.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xqo.jinqigfzy.top

[T11] Kotlin：协程
来源：http://mqr.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://pov.vqdsnc.cn

[T12] Kotlin：解构声明
来源：http://faf.aizwys.cn

val (a, b) = Pair(1, 2)
来源：http://axm.tarul.cn

[T13] Kotlin：只读 Map
来源：http://nqf.fengsongda.top

val m = mapOf("a" to 1)
来源：http://ria.guannengcc.top

[T14] Kotlin：循环
来源：http://jgi.yuanzhike.top

for (i in 1..10) println(i)
来源：http://iqs.vehdjk.com

[T15] Kotlin：接口
来源：http://hwb.jqgfzy.top

interface Shape { fun area(): Double }
来源：http://mlj.uphjek.com

[T16] Swift：Hello World
来源：http://exx.quarkkingdee.top

print("Hello")
来源：http://jom.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://xgn.dashuyun.cn

var a = 1;  let b = 2
来源：http://mks.ivvv.top

[T18] Swift：字符串插值
来源：http://svg.daxiang520.top

"值: \(b)"
来源：http://wci.yangfankeji.com

[T19] Swift：可选绑定
来源：http://qhi.yvedp.cn

if let n = opt { print(n) }
来源：http://hxl.andypj.xyz

[T20] Swift：数组操作
来源：http://nmq.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://tno.sysykeji.top

[T21] Swift：遍历
来源：http://pxq.ehwqpu.com

for x in a { print(x) }
来源：http://dqh.zdbjq.cn

[T22] Swift：字典
来源：http://hki.ydzc1.top

var d = ["a": 1];  d["b"] = 2
来源：http://deo.zycfv.cn

[T23] Swift：函数
来源：http://dfr.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://obn.hfpthk.cn

[T24] Swift：闭包
来源：http://fsr.sysykeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wgo.sweek.top

[T25] Swift：结构体
来源：http://yma.gotoacloud.top

struct P { var x: Int }
来源：http://bri.sweek.top

[T26] Swift：类与重写
来源：http://eyv.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://lxj.iojbl.cn

[T27] Swift：错误处理
来源：http://olc.sxryk.cn

do { try f() } catch { print(error) }
来源：http://ewu.aizwys.cn

[T28] Swift：枚举
来源：http://tvz.hesvh.cn

enum Color { case red, green }
来源：http://rxb.316326.xyz

[T29] Swift：guard 提前返回
来源：http://utr.aibaodan.cn

guard let x = opt else { return }
来源：http://ftc.tanke756.top

[T30] Swift：协议
来源：http://ejq.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://vcw.jinqigfzy.top

[T31] Lua：Hello World
来源：http://zyy.havefunace.top

print("Hello")
来源：http://zvq.yj20258.top

[T32] Lua：局部变量
来源：http://dai.sysykeji.top

local a = 1
来源：http://zug.xinyue.icu

[T33] Lua：表（数组）
来源：http://bxs.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iwx.yfazqb.com

[T34] Lua：遍历表
来源：http://kvj.sysykeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://huy.zhijiandao.cn

[T35] Lua：字典表
来源：http://bkn.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://pwi.tanke756.top

[T36] Lua：函数
来源：http://xyn.pengpengdd.cyou

function add(a, b) return a + b end
来源：http://imw.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://kav.xingfuxueyuan.xyz

"a" .. "b"
来源：http://dvm.ydjk.org.cn

[T38] Lua：条件
来源：http://gba.pycfn.com

if x > 0 then print("正") end
来源：http://ksm.52xcode.cn

[T39] Lua：模式匹配
来源：http://vcp.andypj.xyz

string.find(s, "%d+")
来源：http://lzk.andypj.xyz

[T40] Lua：元表
来源：http://fzc.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://gxi.tarul.cn

[T41] Perl：Hello World
来源：http://usp.sweek.top

print "Hello\n";
来源：http://dbq.jianghu66.top

[T42] Perl：变量类型
来源：http://iis.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wfm.gzhubu.top

[T43] Perl：字符串插值
来源：http://sre.yj202588.top

"值: $a"
来源：http://orv.zhengqikj.top

[T44] Perl：条件
来源：http://owh.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://bmm.dashuyun.cn

[T45] Perl：数组遍历
来源：http://hks.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://ekh.tanke756.top

[T46] Perl：哈希操作
来源：http://wux.tian-w.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://stc.tianlin.xyz

[T47] Perl：正则捕获
来源：http://xra.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://jso.xziqi.cn

[T48] Perl：正则替换
来源：http://wia.jinghuilouyu.cn

$s =~ s/old/new/g;
来源：http://igc.nwbrower.top

[T49] Perl：函数
来源：http://ngm.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://alh.hesvh.cn

[T50] Perl：逐行读文件
来源：http://roy.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://iej.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://gbu.zhijiandao.cn

[T51] Scala：Hello World
来源：http://dpr.sxryk.cn

println("Hello")
来源：http://msa.9152youxi.cn

[T52] Scala：变量
来源：http://olo.zhijiandao.cn

val a = 1;  var b = 2
来源：http://eem.sxryk.cn

[T53] Scala：字符串插值
来源：http://kbb.tian-w.cn

s"值: $b"
来源：http://bsv.ydzc1.top

[T54] Scala：集合映射
来源：http://wzi.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://xoh.iojbl.cn

[T55] Scala：集合过滤
来源：http://dhd.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iin.ybcxt.top

[T56] Scala：样例类
来源：http://rwp.jqgfzy.top

case class User(name: String, age: Int)
来源：http://uae.yj202588.top

[T57] Scala：模式匹配
来源：http://bdx.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://niy.zdqjudy.top

[T58] Scala：函数定义
来源：http://rme.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://adr.pengpengdd.cyou

[T59] Scala：循环
来源：http://ose.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://owq.zhijiandao.cn

[T60] Scala：折叠
来源：http://eqg.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wnr.hywenlv.cn

================================================================================
来源：http://gwb.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://keu.jinqigfzy.top

================================================================================
来源：http://eec.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://izx.tanke756.top

python -m venv .venv && source .venv/bin/activate
来源：http://isy.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://ncl.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xax.yuanzhike.top

[U03] Py：加载 .env 配置
来源：http://efe.nanxuanxn.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fxr.daria6918.cn

[U04] Py：变量调试打印
来源：http://xrp.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://luh.ywan-chungtsiang.top

[U05] Py：列表去重且保序
来源：http://skc.ppjwa.cn

list(dict.fromkeys(arr))
来源：http://rla.redwolf501.top

[U06] Py：合并两个字典
来源：http://unb.shuidangran.top

{**a, **b}
来源：http://ibx.cucudq.cn

[U07] Py：反转字典键值
来源：http://psi.daria6918.cn

{v: k for k, v in d.items()}
来源：http://dyo.tarul.cn

[U08] Py：展平二维列表
来源：http://rex.dianchejie.cn

[y for x in nested for y in x]
来源：http://maz.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://olq.yanxiufei.cn

max(d, key=d.get)
来源：http://mht.hammf.cn

[U10] Py：按值排序字典
来源：http://acl.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ivf.hnqzz.top

[U11] Py：生成器表达式
来源：http://ehz.zhiwuduotai.top

(x * 2 for x in arr)
来源：http://xcj.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://thr.yuanzhike.top

Counter(arr).most_common(3)
来源：http://zdm.yj202588.top

[U13] Py：固定长度队列
来源：http://gna.yfazqb.com

deque(maxlen=10)
来源：http://fuz.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://nyd.daria6918.cn

defaultdict(list)
来源：http://xuj.jqgfzy.top

[U15] Py：高精度计时
来源：http://jwi.nanxuanxn.top

t = time.perf_counter()
来源：http://kyj.wangdashe.top

[U16] Py：命令行参数解析
来源：http://itu.ybcxt.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xlb.yuxming.cn

[U17] Py：初始化日志
来源：http://nji.svipenyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://idj.haohaochexian.top

[U18] Py：预编译正则
来源：http://lxj.jlsjyb.cn

pat = re.compile(r"\d+")
来源：http://hxf.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://hid.dianchejie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nju.zycfv.cn

[U20] Py：缓存函数结果
来源：http://ahb.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://neg.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://prh.hcnkem.com

@contextlib.contextmanager
来源：http://cam.ybcxt.top

[U22] Py：矩阵转置
来源：http://zaw.birdmap.top

list(zip(*m))
来源：http://rkk.zycfv.cn

[U23] Py：分块读取大文件
来源：http://kqh.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yet.sjlbkw.cn

[U24] Py：路径操作
来源：http://xvf.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pdg.yvedp.cn

[U25] Py：CSV 按字典读
来源：http://gqr.pengpengdd.cyou

csv.DictReader(f)
来源：http://jps.jlsjyb.cn

[U26] Py：并发下载
来源：http://jze.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vpo.jinqigfzy.top


<!-- 参考信息 -->