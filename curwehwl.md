代发 wailian999

strlen(s)
来源：http://bww.hfpthk.cn

[S06] C：字符串比较
来源：http://psz.gaohongyu789.top

strcmp(a, b) == 0
来源：http://cmh.xylfe.cn

[S07] C：数组遍历求和
来源：http://slw.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://opn.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://ngj.gotoacloud.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jzm.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://ckv.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zmb.nanxinkj.top

[S10] C：指针与解引用
来源：http://ugl.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://xti.sufxvd.cn

[S11] C：逐行读文件
来源：http://srh.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://nad.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://djh.havefunace.top

fclose(f);
来源：http://skg.yuxming.cn

[S12] C：写文件
来源：http://bja.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gue.nwbrower.top

[S13] C：宏定义
来源：http://jrt.zdqjudy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ylw.hnxiangtu.top

[S14] C：枚举
来源：http://auc.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://mxl.tian-w.cn

[S15] C：类型转换
来源：http://bnq.sxryk.cn

(double) a / b
来源：http://cal.yfazqb.com

[S16] C：位操作置位
来源：http://bjf.iojbl.cn

x |= (1 << 3);
来源：http://grj.bjfxy.top

[S17] C：安全拼接字符串
来源：http://cbz.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iza.yuxming.cn

[S18] C：命令行参数
来源：http://yax.ehwqpu.com

int main(int argc, char **argv)
来源：http://mjo.yanxiufei.cn

[S19] C：快速排序
来源：http://izr.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://mps.jqgfzy.top

[S20] C：二分查找
来源：http://biq.zhoulong.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tzq.mhx1999.top

[S21] C：字符类别判断
来源：http://xhp.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jmi.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://rpc.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://tjj.sjlbkw.cn

[S23] C：随机数
来源：http://uvz.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ist.cucudq.cn

[S24] C：获取本地时间
来源：http://vxw.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://loq.cqqwz.cn

[S25] C：内存拷贝
来源：http://nxp.ehwqpu.com

memcpy(dst, src, n);
来源：http://cnj.sufxvd.cn

[S26] C：内存清零
来源：http://ywb.andypj.xyz

memset(a, 0, sizeof a);
来源：http://qbz.hongshengwenyu.top

[S27] C：定义常量
来源：http://noo.zycfv.cn

const double PI = 3.14159;
来源：http://pjo.jyoumei.cn

[S28] C：静态变量
来源：http://uyx.zhijiandao.cn

static int counter = 0;
来源：http://qhf.nanxinkj.top

[S29] C：变参函数
来源：http://flo.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kxw.shzxlz.cn

[S30] C：头文件保护
来源：http://bvu.iojbl.cn

#ifndef X_H
来源：http://wac.chenlongwang.top

#define X_H
来源：http://hfq.ehwqpu.com

#endif
来源：http://kqc.mhx1999.top

[S31] C++：Hello World
来源：http://rcy.yj20258.top

#include <iostream>
来源：http://dqs.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://xii.redwolf501.top

[S32] C++：字符串
来源：http://zqa.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://aba.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://gmc.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zud.sxryk.cn

[S34] C++：遍历 vector
来源：http://fdp.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://idb.ydjk.org.cn

[S35] C++：map
来源：http://why.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pyt.nanxuanxn.top

[S36] C++：unordered_map
来源：http://zhm.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fzr.jlsjyb.cn

[S37] C++：set
来源：http://pgh.redwolf501.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sjj.xuetiantiany.cn

[S38] C++：排序
来源：http://sqk.yj202588.top

std::sort(v.begin(), v.end());
来源：http://hda.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://ntz.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://svf.guowangkeji.top

[S40] C++：查找元素
来源：http://rgw.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dwq.snrcjt.cn

[S41] C++：类与构造函数
来源：http://eay.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ayg.ivvv.top

[S42] C++：继承与虚函数
来源：http://yct.havefunace.top

class B : public Base { public: void f() override {} };
来源：http://ejz.hysaishi.cn

[S43] C++：智能指针
来源：http://lee.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://pus.bbcook.cn

[S44] C++：引用传参
来源：http://otu.cheryme.top

void inc(int &x) { ++x; }
来源：http://ypn.xinyue.icu

[S45] C++：lambda
来源：http://cnu.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://dtm.zhijiandao.cn

[S46] C++：函数模板
来源：http://spe.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oeo.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://jeq.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ivz.xinyue.icu

[S48] C++：逐行读文件
来源：http://xnl.quarkkingdee.top

std::ifstream in("a.txt");  std::string line;
来源：http://sty.mhx1999.top

while (std::getline(in, line)) { }
来源：http://cet.sjlbkw.cn

[S49] C++：写文件
来源：http://qoi.jinqigfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xbi.kuanghao11.cn

[S50] C++：格式化数字
来源：http://hhc.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pug.fengsongda.top

[S51] C++：显式类型转换
来源：http://qfw.jiagoushi.top

static_cast<double>(a) / b
来源：http://gbf.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://ktm.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://qvo.zhongyouzk.top

[S53] C++：移动语义
来源：http://mox.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://dmp.redwolf501.top

[S54] C++：异常处理
来源：http://hgk.vehdjk.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gcn.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://ppk.52xcode.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qgq.52xcode.cn

[S56] C++：optional
来源：http://dqk.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qhe.fzhhl.top

[S57] C++：编译期常量
来源：http://bro.ydzc1.top

constexpr int N = 10;
来源：http://fbh.havefunace.top

[S58] C++：命名空间
来源：http://fsl.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://vhm.wangdashe.top

[S59] C++：静态断言
来源：http://iog.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ngo.andypj.xyz

[S60] C++：遍历并删除元素
来源：http://fqd.xingfuxueyuan.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pxe.jinyuanbaomall.cn

================================================================================
来源：http://xtj.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bda.andypj.xyz

================================================================================
来源：http://dxo.havefunace.top

[T01] Kotlin：Hello World
来源：http://suz.sjlbkw.cn

println("Hello")
来源：http://yru.fzhhl.top

[T02] Kotlin：变量
来源：http://nkj.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://had.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://kbv.zdqjudy.top

"值: $b"
来源：http://ujg.gzhubu.top

[T04] Kotlin：空安全
来源：http://jee.guannengcc.top

val n: String? = null;  n?.length
来源：http://gpj.fengsongda.top

[T05] Kotlin：when 表达式
来源：http://roo.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uqw.hnqzz.top

[T06] Kotlin：集合映射
来源：http://vsd.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tmg.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://ccp.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uys.wangdashe.top

[T08] Kotlin：数据类
来源：http://prj.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://muc.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://xzi.jinyuanbaomall.cn

fun String.exclaim() = this + "!"
来源：http://uib.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://vqc.smart0.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://qku.snrcjt.cn

[T11] Kotlin：协程
来源：http://zyu.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tlf.vehdjk.com

[T12] Kotlin：解构声明
来源：http://vvo.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://ebj.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://qai.vehdjk.com

val m = mapOf("a" to 1)
来源：http://dyi.zhongyouzk.top

[T14] Kotlin：循环
来源：http://dpo.ivvv.top

for (i in 1..10) println(i)
来源：http://hiu.yuxming.cn

[T15] Kotlin：接口
来源：http://kyb.havefunace.top

interface Shape { fun area(): Double }
来源：http://gim.xziqi.cn

[T16] Swift：Hello World
来源：http://vhk.ywan-chungtsiang.top

print("Hello")
来源：http://oih.bjfxy.top

[T17] Swift：变量与常量
来源：http://dyw.cdnleiting.top

var a = 1;  let b = 2
来源：http://woc.redwolf501.top

[T18] Swift：字符串插值
来源：http://wzd.ppjwa.cn

"值: \(b)"
来源：http://mat.hesvh.cn

[T19] Swift：可选绑定
来源：http://ten.uphjek.com

if let n = opt { print(n) }
来源：http://oxl.xuanzx.com

[T20] Swift：数组操作
来源：http://bfs.gotoacloud.top

var a = [1, 2, 3];  a.append(4)
来源：http://och.xuanzx.com

[T21] Swift：遍历
来源：http://yxw.guowangkeji.top

for x in a { print(x) }
来源：http://zqy.jinghuilouyu.cn

[T22] Swift：字典
来源：http://wrz.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lfc.chenlongwang.top

[T23] Swift：函数
来源：http://qpj.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wyd.jqgufenzy.top

[T24] Swift：闭包
来源：http://lbn.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ddg.hysaishi.cn

[T25] Swift：结构体
来源：http://dbn.svipenyu.cn

struct P { var x: Int }
来源：http://nbz.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://jkt.chenlongwang.top

class A: Base { override func f() {} }
来源：http://vkp.fengsongda.top

[T27] Swift：错误处理
来源：http://anu.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://mel.chenlongwang.top

[T28] Swift：枚举
来源：http://mlw.zhoulong.xyz

enum Color { case red, green }
来源：http://sqn.xinyue.icu

[T29] Swift：guard 提前返回
来源：http://csy.vqdsnc.cn

guard let x = opt else { return }
来源：http://mjg.zycfv.cn

[T30] Swift：协议
来源：http://ayz.haohaochexian.top

protocol Shape { func area() -> Double }
来源：http://jzp.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://hwt.cashguo.top

print("Hello")
来源：http://qir.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://atl.meibo888.top

local a = 1
来源：http://mhn.sufxvd.cn

[T33] Lua：表（数组）
来源：http://rrn.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kqx.hysaishi.cn

[T34] Lua：遍历表
来源：http://wvi.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lut.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://cdf.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://qfr.yvedp.cn

[T36] Lua：函数
来源：http://ulv.chenzaomai.com

function add(a, b) return a + b end
来源：http://snf.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://dhi.hfpthk.cn

"a" .. "b"
来源：http://xpa.epnwcf.com

[T38] Lua：条件
来源：http://fuq.tian-w.cn

if x > 0 then print("正") end
来源：http://xta.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://vzx.ppjwa.cn

string.find(s, "%d+")
来源：http://nya.xylfe.cn

[T40] Lua：元表
来源：http://eau.iojbl.cn

setmetatable({}, { __index = base })
来源：http://zxr.cucudq.cn

[T41] Perl：Hello World
来源：http://sbd.cucudq.cn

print "Hello\n";
来源：http://cnt.jinyuanbaomall.cn

[T42] Perl：变量类型
来源：http://zre.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qwm.chenlongwang.top

[T43] Perl：字符串插值
来源：http://gzk.yanxiufei.cn

"值: $a"
来源：http://ltw.yangfankeji.com

[T44] Perl：条件
来源：http://msi.gogol.net.cn

if ($a > 0) { print "正"; }
来源：http://fem.guowangkeji.top

[T45] Perl：数组遍历
来源：http://ehk.nanxinkj.top

for my $x (@arr) { print $x; }
来源：http://jua.pycfn.com

[T46] Perl：哈希操作
来源：http://tdn.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xfr.hesvh.cn

[T47] Perl：正则捕获
来源：http://kzu.tarul.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vpg.sxryk.cn

[T48] Perl：正则替换
来源：http://riu.yvedp.cn

$s =~ s/old/new/g;
来源：http://ynq.chenjidiqi.icu

[T49] Perl：函数
来源：http://azb.hnxiangtu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ciu.sweek.top

[T50] Perl：逐行读文件
来源：http://qgs.jqgufenzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rty.sysykeji.top

while (my $line = <$fh>) { print $line; }
来源：http://xtw.jinyuanbaomall.cn

[T51] Scala：Hello World
来源：http://dne.jqgufenzy.top

println("Hello")
来源：http://lwi.zhoulong.xyz

[T52] Scala：变量
来源：http://asg.gzhubu.top

val a = 1;  var b = 2
来源：http://gwj.hnqzz.top

[T53] Scala：字符串插值
来源：http://uuw.ppjwa.cn

s"值: $b"
来源：http://bos.tianlin.xyz

[T54] Scala：集合映射
来源：http://avu.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://jgh.xylfe.cn

[T55] Scala：集合过滤
来源：http://szy.fengsongda.top

List(1, 2, 3).filter(_ > 1)
来源：http://irj.xziqi.cn

[T56] Scala：样例类
来源：http://pho.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://eqi.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://iny.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cww.ydjk.org.cn

[T58] Scala：函数定义
来源：http://crm.ywan-chungtsiang.top

def add(a: Int, b: Int): Int = a + b
来源：http://rwq.svipenyu.cn

[T59] Scala：循环
来源：http://rho.kuanghao11.cn

for (i <- 1 to 10) println(i)
来源：http://ndg.chenzaomai.com

[T60] Scala：折叠
来源：http://aso.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://axb.jinqigufen.top

================================================================================
来源：http://jrk.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dlh.wangshuangyany.cn

================================================================================
来源：http://nfz.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://vbz.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://asa.sweek.top

[U02] Py：导出 / 安装依赖
来源：http://cvi.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oca.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://uhi.yongpay.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bch.0kj1m.cn

[U04] Py：变量调试打印
来源：http://mnl.fehbvm.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fej.0kj1m.cn

[U05] Py：列表去重且保序
来源：http://rvm.sweek.top

list(dict.fromkeys(arr))
来源：http://wnk.zhiwuduotai.top

[U06] Py：合并两个字典
来源：http://had.cheryme.top

{**a, **b}
来源：http://mym.nwbrower.top

[U07] Py：反转字典键值
来源：http://cva.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://vol.hnqzz.top

[U08] Py：展平二维列表
来源：http://ivo.yfazqb.com

[y for x in nested for y in x]
来源：http://qnu.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://rri.cucudq.cn

max(d, key=d.get)
来源：http://mml.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://tnn.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qmy.zhijiandao.cn

[U11] Py：生成器表达式
来源：http://xip.sjlbkw.cn

(x * 2 for x in arr)
来源：http://ipa.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://tag.nwbrower.top

Counter(arr).most_common(3)
来源：http://abs.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://xtv.quarkkingdee.top

deque(maxlen=10)
来源：http://loh.yj20258.top

[U14] Py：分组收集到列表
来源：http://lzm.yuanzhike.top

defaultdict(list)
来源：http://idy.yuanzhike.top

[U15] Py：高精度计时
来源：http://zuv.yonumen.top

t = time.perf_counter()
来源：http://aqc.nwbrower.top

[U16] Py：命令行参数解析
来源：http://hrm.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://apb.havefunace.top

[U17] Py：初始化日志
来源：http://pfb.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://fyw.jinqigfzy.top

[U18] Py：预编译正则
来源：http://jvi.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://qzp.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://wyb.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://atk.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://clh.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://qrc.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://dqd.sysykeji.top

@contextlib.contextmanager
来源：http://aos.birdmap.top

[U22] Py：矩阵转置
来源：http://rvz.hnxiangtu.top

list(zip(*m))
来源：http://ftj.redwolf501.top

[U23] Py：分块读取大文件
来源：http://eku.sufxvd.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uxy.zhiwuduotai.top

[U24] Py：路径操作
来源：http://oor.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pig.birdmap.top

[U25] Py：CSV 按字典读
来源：http://jwu.xylfe.cn

csv.DictReader(f)
来源：http://gsa.jianghu66.top

[U26] Py：并发下载
来源：http://uns.gaohongyu789.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tey.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://qbv.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://brw.ppjwa.cn

[U28] Py：类型别名
来源：http://czi.hysaishi.cn

UserId = int
来源：http://nwp.xinyue.icu


<!-- 参考信息 -->