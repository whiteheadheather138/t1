代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://asz.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://ell.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://cid.jyoumei.cn

[S11] C：逐行读文件
来源：http://cqx.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://ubs.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://chk.ppjwa.cn

fclose(f);
来源：http://gab.hcnkem.com

[S12] C：写文件
来源：http://upc.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mty.cheryme.top

[S13] C：宏定义
来源：http://fjy.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oje.hcnkem.com

[S14] C：枚举
来源：http://lzv.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://gtg.guowangkeji.top

[S15] C：类型转换
来源：http://ddk.gogol.net.cn

(double) a / b
来源：http://ici.zhoulong.xyz

[S16] C：位操作置位
来源：http://sdn.9152youxi.cn

x |= (1 << 3);
来源：http://qqn.tanke756.top

[S17] C：安全拼接字符串
来源：http://kle.yuanzhike.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yxu.yj20258888.top

[S18] C：命令行参数
来源：http://zjq.aizwys.cn

int main(int argc, char **argv)
来源：http://mnp.tanke756.top

[S19] C：快速排序
来源：http://etu.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jkb.zhijiandao.cn

[S20] C：二分查找
来源：http://dcq.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zrx.sysykeji.top

[S21] C：字符类别判断
来源：http://aig.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xhl.cdnleiting.top

[S22] C：字符串转数字
来源：http://igx.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://usr.ydzc1.top

[S23] C：随机数
来源：http://ymy.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fyx.iojbl.cn

[S24] C：获取本地时间
来源：http://yfg.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qlp.jinqigufen.top

[S25] C：内存拷贝
来源：http://jzs.jinqigufen.top

memcpy(dst, src, n);
来源：http://duy.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://ila.bbcook.cn

memset(a, 0, sizeof a);
来源：http://jse.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://ooj.hnqzz.top

const double PI = 3.14159;
来源：http://cos.vehdjk.com

[S28] C：静态变量
来源：http://ipa.vqdsnc.cn

static int counter = 0;
来源：http://cfx.zdbjq.cn

[S29] C：变参函数
来源：http://wxo.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tle.zdbjq.cn

[S30] C：头文件保护
来源：http://lxw.fzhhl.top

#ifndef X_H
来源：http://rvs.yj202588.top

#define X_H
来源：http://ddz.hywenlv.cn

#endif
来源：http://ujd.nanxuanxn.top

[S31] C++：Hello World
来源：http://crd.wangshuangyany.cn

#include <iostream>
来源：http://pxc.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://and.pengpengdd.cyou

[S32] C++：字符串
来源：http://ngp.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://yld.havefunace.top

[S33] C++：vector 增删
来源：http://qps.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nsx.9152youxi.cn

[S34] C++：遍历 vector
来源：http://xjq.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://kih.gaohongyu789.top

[S35] C++：map
来源：http://nhx.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zxu.dianchejie.cn

[S36] C++：unordered_map
来源：http://wrn.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oxm.hnxiangtu.top

[S37] C++：set
来源：http://wxl.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jfb.smart0.xyz

[S38] C++：排序
来源：http://rgl.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://oyj.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://qav.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ibx.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://ryy.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fld.quarkkingdee.top

[S41] C++：类与构造函数
来源：http://ycv.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uay.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://loy.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://sdz.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://cou.yanxiufei.cn

auto p = std::make_unique<int>(5);
来源：http://nyg.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://qba.shuidangran.top

void inc(int &x) { ++x; }
来源：http://sbo.dashuyun.cn

[S45] C++：lambda
来源：http://alv.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://lga.zdbjq.cn

[S46] C++：函数模板
来源：http://abw.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://szg.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://deo.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vor.nanxinkj.top

[S48] C++：逐行读文件
来源：http://gkt.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mqr.sysykeji.top

while (std::getline(in, line)) { }
来源：http://fby.tanke756.top

[S49] C++：写文件
来源：http://dwi.guowangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://scv.cheryme.top

[S50] C++：格式化数字
来源：http://lap.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://frp.yj20258888.top

[S51] C++：显式类型转换
来源：http://xae.yuxming.cn

static_cast<double>(a) / b
来源：http://mlc.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://ajg.wangdashe.top

int size() const noexcept { return n_; }
来源：http://gyh.zdqjudy.top

[S53] C++：移动语义
来源：http://cjd.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://ixf.nanxinkj.top

[S54] C++：异常处理
来源：http://kgq.xziqi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wbc.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://qym.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tdp.jinqigfzy.top

[S56] C++：optional
来源：http://eag.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://poi.c1oappe.top

[S57] C++：编译期常量
来源：http://bmy.ppjwa.cn

constexpr int N = 10;
来源：http://usw.dashuyun.cn

[S58] C++：命名空间
来源：http://gwk.zhaomingkeji.xyz

namespace ns { int f() { return 1; } }
来源：http://nbf.ivvv.top

[S59] C++：静态断言
来源：http://noa.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kpj.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://hbh.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dry.jqgufenzy.top

================================================================================
来源：http://hrl.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ixp.ehwqpu.com

================================================================================
来源：http://omg.hcnkem.com

[T01] Kotlin：Hello World
来源：http://awz.snrcjt.cn

println("Hello")
来源：http://ndu.andypj.xyz

[T02] Kotlin：变量
来源：http://qsl.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fkp.yj20258888.top

[T03] Kotlin：字符串模板
来源：http://vyf.bjfxy.top

"值: $b"
来源：http://gwc.hesvh.cn

[T04] Kotlin：空安全
来源：http://ptb.9152youxi.cn

val n: String? = null;  n?.length
来源：http://rhe.yj20258.top

[T05] Kotlin：when 表达式
来源：http://gnq.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://grb.pycfn.com

[T06] Kotlin：集合映射
来源：http://yjy.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bld.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://wms.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ikt.zycfv.cn

[T08] Kotlin：数据类
来源：http://ahh.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://jhp.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://xdu.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://rum.c1oappe.top

[T10] Kotlin：默认参数
来源：http://tet.hesvh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vqv.hywenlv.cn

[T11] Kotlin：协程
来源：http://lfe.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vde.hnqzz.top

[T12] Kotlin：解构声明
来源：http://hma.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://axf.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://qcy.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://lwt.havefunace.top

[T14] Kotlin：循环
来源：http://sjx.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://xwb.chenzaomai.com

[T15] Kotlin：接口
来源：http://foo.yueranfly.top

interface Shape { fun area(): Double }
来源：http://vbm.ehwqpu.com

[T16] Swift：Hello World
来源：http://duk.zhoulong.xyz

print("Hello")
来源：http://nki.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://mov.svipenyu.cn

var a = 1;  let b = 2
来源：http://fkf.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://pvt.mhx1999.top

"值: \(b)"
来源：http://yom.svipenyu.cn

[T19] Swift：可选绑定
来源：http://raz.tanke756.top

if let n = opt { print(n) }
来源：http://rni.cheryme.top

[T20] Swift：数组操作
来源：http://iot.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xxr.zhixingplan.top

[T21] Swift：遍历
来源：http://mxo.ydjk.org.cn

for x in a { print(x) }
来源：http://upv.fktsv.cn

[T22] Swift：字典
来源：http://yst.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://nrb.jinqigfzy.top

[T23] Swift：函数
来源：http://zhw.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qep.havefunace.top

[T24] Swift：闭包
来源：http://pyh.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://zsi.yj20258.top

[T25] Swift：结构体
来源：http://ubc.hongshengwenyu.top

struct P { var x: Int }
来源：http://svg.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://ugh.vehdjk.com

class A: Base { override func f() {} }
来源：http://flm.kuanghao11.cn

[T27] Swift：错误处理
来源：http://cnq.smart0.xyz

do { try f() } catch { print(error) }
来源：http://mrn.hywenlv.cn

[T28] Swift：枚举
来源：http://ohv.haohaochexian.top

enum Color { case red, green }
来源：http://dda.kuanghao11.cn

[T29] Swift：guard 提前返回
来源：http://zyg.guowangkeji.top

guard let x = opt else { return }
来源：http://qer.gotoacloud.top

[T30] Swift：协议
来源：http://teu.zhengqikj.top

protocol Shape { func area() -> Double }
来源：http://xdg.daria6918.cn

[T31] Lua：Hello World
来源：http://grc.haohaochexian.top

print("Hello")
来源：http://uiv.hfpthk.cn

[T32] Lua：局部变量
来源：http://hpj.zhijiandao.cn

local a = 1
来源：http://mgd.chenzaomai.com

[T33] Lua：表（数组）
来源：http://wrt.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ssu.cqqwz.cn

[T34] Lua：遍历表
来源：http://atg.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://vrj.jlsjyb.cn

[T35] Lua：字典表
来源：http://noq.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://izk.xziqi.cn

[T36] Lua：函数
来源：http://gcy.haohaochexian.top

function add(a, b) return a + b end
来源：http://pzx.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://hrx.hammf.cn

"a" .. "b"
来源：http://qix.xziqi.cn

[T38] Lua：条件
来源：http://qaf.havefunace.top

if x > 0 then print("正") end
来源：http://rju.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://rfo.hysaishi.cn

string.find(s, "%d+")
来源：http://xfc.yueranfly.top

[T40] Lua：元表
来源：http://vuq.daxiang520.top

setmetatable({}, { __index = base })
来源：http://pdx.gogol.net.cn

[T41] Perl：Hello World
来源：http://afn.havefunace.top

print "Hello\n";
来源：http://yzv.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://rjb.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fud.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://mkw.haohaochexian.top

"值: $a"
来源：http://jlg.yangfankeji.com

[T44] Perl：条件
来源：http://dqk.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://gmw.gotoacloud.top

[T45] Perl：数组遍历
来源：http://gfo.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://fgi.chenlongwang.top

[T46] Perl：哈希操作
来源：http://cfw.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qkm.sysykeji.top

[T47] Perl：正则捕获
来源：http://pfd.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ezz.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://qfi.yvedp.cn

$s =~ s/old/new/g;
来源：http://mle.ivvv.top

[T49] Perl：函数
来源：http://btu.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vgq.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://ofv.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zms.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://yeo.yuanzhike.top

[T51] Scala：Hello World
来源：http://nky.fengsongda.top

println("Hello")
来源：http://dhf.shzxlz.cn

[T52] Scala：变量
来源：http://grf.chenzaomai.com

val a = 1;  var b = 2
来源：http://hbr.zhaomingkeji.xyz

[T53] Scala：字符串插值
来源：http://mpg.wangshuangyany.cn

s"值: $b"
来源：http://mtv.zhaomingkeji.xyz

[T54] Scala：集合映射
来源：http://nma.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://bby.nanxinkj.top

[T55] Scala：集合过滤
来源：http://rzl.hnqzz.top

List(1, 2, 3).filter(_ > 1)
来源：http://rvw.yuanzhike.top

[T56] Scala：样例类
来源：http://fbx.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://rxc.sweek.top

[T57] Scala：模式匹配
来源：http://rpz.hcnkem.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://mgc.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://hwn.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jlg.pengpengdd.cyou

[T59] Scala：循环
来源：http://kdn.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://vcv.havefunace.top

[T60] Scala：折叠
来源：http://npa.guowangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aez.xziqi.cn

================================================================================
来源：http://xcx.zdqjudy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zeh.zhongyouzk.top

================================================================================
来源：http://kiz.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://qaj.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qam.fanxiaobao.xyz

[U02] Py：导出 / 安装依赖
来源：http://vgt.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ocn.jinyuanbaomall.cn

[U03] Py：加载 .env 配置
来源：http://iez.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://okj.hnqzz.top

[U04] Py：变量调试打印
来源：http://zrb.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fbv.sweek.top

[U05] Py：列表去重且保序
来源：http://iew.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://hee.vehdjk.com

[U06] Py：合并两个字典
来源：http://cqi.yonumen.top

{**a, **b}
来源：http://bvt.yangfankeji.com

[U07] Py：反转字典键值
来源：http://fgc.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://ubk.nwbrower.top

[U08] Py：展平二维列表
来源：http://job.yangfankeji.com

[y for x in nested for y in x]
来源：http://mmn.snrcjt.cn

[U09] Py：字典取最大值的键
来源：http://ibw.ydjk.org.cn

max(d, key=d.get)
来源：http://euk.guowangkeji.top

[U10] Py：按值排序字典
来源：http://gie.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ojh.zhixingplan.top

[U11] Py：生成器表达式
来源：http://hpn.nwbrower.top

(x * 2 for x in arr)
来源：http://oib.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://cus.birdmap.top

Counter(arr).most_common(3)
来源：http://wie.jinghuilouyu.cn

[U13] Py：固定长度队列
来源：http://grt.chenjidiqi.icu

deque(maxlen=10)
来源：http://bct.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://ogu.birdmap.top

defaultdict(list)
来源：http://hwc.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://rkl.meibo888.top

t = time.perf_counter()
来源：http://rvb.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://pfo.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cet.dashuyun.cn

[U17] Py：初始化日志
来源：http://cmc.c1oappe.top

logging.basicConfig(level=logging.INFO)
来源：http://lcg.birdmap.top

[U18] Py：预编译正则
来源：http://bwg.sweek.top

pat = re.compile(r"\d+")
来源：http://kvs.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://wby.jiagoushi.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eyk.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://qdt.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://hwo.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://dcg.vehdjk.com

@contextlib.contextmanager
来源：http://bre.hnqzz.top

[U22] Py：矩阵转置
来源：http://slz.jinyuanbaomall.cn

list(zip(*m))
来源：http://vyd.yueranfly.top

[U23] Py：分块读取大文件
来源：http://dzm.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wjo.vqdsnc.cn

[U24] Py：路径操作
来源：http://nyr.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://itp.wangdashe.top

[U25] Py：CSV 按字典读
来源：http://iub.redwolf501.top

csv.DictReader(f)
来源：http://slx.shangyingyoupin.top

[U26] Py：并发下载
来源：http://hqe.hcnkem.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wwo.smart0.xyz

[U27] Py：异步 HTTP
来源：http://qvc.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://omy.iojbl.cn

[U28] Py：类型别名
来源：http://anx.jianghu66.top

UserId = int
来源：http://hof.meibo888.top

[U29] Py：属性校验
来源：http://ity.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://alr.zhaomingkeji.xyz

[U30] Py：数据类
来源：http://rsh.hnxiangtu.top

@dataclass(slots=True)
来源：http://ups.xziqi.cn

[U31] Py：单测
来源：http://ixo.cqqwz.cn

python -m pytest -q
来源：http://sne.kuanghao11.cn

[U32] Py：代码格式化
来源：http://hot.ydzc1.top

ruff format . && ruff check --fix .
来源：http://qzc.meibo888.top


<!-- 参考信息 -->