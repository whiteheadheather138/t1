代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://miy.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://szn.bbcook.cn

fclose(f);
来源：http://oqk.guowangkeji.top

[S12] C：写文件
来源：http://aeq.cucudq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bou.ydjk.org.cn

[S13] C：宏定义
来源：http://oaw.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fxj.iojbl.cn

[S14] C：枚举
来源：http://bok.nwbrower.top

enum Color { RED, GREEN, BLUE };
来源：http://jet.yongpay.top

[S15] C：类型转换
来源：http://qky.haohaochexian.top

(double) a / b
来源：http://xtw.zhongyouzk.top

[S16] C：位操作置位
来源：http://ozy.xinyue.icu

x |= (1 << 3);
来源：http://tjk.hywenlv.cn

[S17] C：安全拼接字符串
来源：http://fry.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ktd.ehwqpu.com

[S18] C：命令行参数
来源：http://haj.52xcode.cn

int main(int argc, char **argv)
来源：http://wlp.cashguo.top

[S19] C：快速排序
来源：http://ygo.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zbt.hnxiangtu.top

[S20] C：二分查找
来源：http://cnt.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ygj.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://ktd.c1oappe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://alz.ehwqpu.com

[S22] C：字符串转数字
来源：http://kdv.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://vng.hammf.cn

[S23] C：随机数
来源：http://ore.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ryq.ydjk.org.cn

[S24] C：获取本地时间
来源：http://pks.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cao.chenzaomai.com

[S25] C：内存拷贝
来源：http://bhz.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://iae.cashguo.top

[S26] C：内存清零
来源：http://uzt.xylfe.cn

memset(a, 0, sizeof a);
来源：http://fmo.ybcxt.top

[S27] C：定义常量
来源：http://otx.ybcxt.top

const double PI = 3.14159;
来源：http://rvc.jianghu66.top

[S28] C：静态变量
来源：http://epf.jiagoushi.top

static int counter = 0;
来源：http://lnz.zdbjq.cn

[S29] C：变参函数
来源：http://xtn.zhiwuduotai.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ltm.wangshuangyany.cn

[S30] C：头文件保护
来源：http://vzr.hammf.cn

#ifndef X_H
来源：http://tuf.zhijiandao.cn

#define X_H
来源：http://inp.wangshuangyany.cn

#endif
来源：http://ajj.jiagoushi.top

[S31] C++：Hello World
来源：http://gtg.jlsjyb.cn

#include <iostream>
来源：http://dns.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://lcd.ybcxt.top

[S32] C++：字符串
来源：http://che.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://vlr.fktsv.cn

[S33] C++：vector 增删
来源：http://sxp.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uxr.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://swa.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://lsg.yuxming.cn

[S35] C++：map
来源：http://sjs.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mbg.shzxlz.cn

[S36] C++：unordered_map
来源：http://grx.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tpp.zhaomingkeji.xyz

[S37] C++：set
来源：http://bnk.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gib.shanyushiyangkeji.top

[S38] C++：排序
来源：http://fie.daxiang520.top

std::sort(v.begin(), v.end());
来源：http://cjq.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://wnl.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bir.bbcook.cn

[S40] C++：查找元素
来源：http://iov.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gtw.yongpay.top

[S41] C++：类与构造函数
来源：http://gdn.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bvg.yj20258888.top

[S42] C++：继承与虚函数
来源：http://vxi.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://fhy.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://emy.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://kom.pycfn.com

[S44] C++：引用传参
来源：http://yge.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://yrr.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://hig.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://bzp.quarkkingdee.top

[S46] C++：函数模板
来源：http://kev.fehbvm.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eso.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://dyx.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kpg.daxiang520.top

[S48] C++：逐行读文件
来源：http://hed.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rvj.shuidangran.top

while (std::getline(in, line)) { }
来源：http://pcz.yvedp.cn

[S49] C++：写文件
来源：http://frx.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rbo.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://cju.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xez.yuanzhike.top

[S51] C++：显式类型转换
来源：http://qaw.cashguo.top

static_cast<double>(a) / b
来源：http://dvv.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://bxd.redwolf501.top

int size() const noexcept { return n_; }
来源：http://dba.hnqzz.top

[S53] C++：移动语义
来源：http://wjh.52xcode.cn

std::vector<int> w = std::move(v);
来源：http://hcm.gotoacloud.top

[S54] C++：异常处理
来源：http://cgs.zhoulong.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://obm.yvedp.cn

[S55] C++：结构化绑定
来源：http://vgv.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bhr.yueranfly.top

[S56] C++：optional
来源：http://svw.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vbi.zdqjudy.top

[S57] C++：编译期常量
来源：http://zsf.jyoumei.cn

constexpr int N = 10;
来源：http://hmo.aizwys.cn

[S58] C++：命名空间
来源：http://qjw.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://ify.yonumen.top

[S59] C++：静态断言
来源：http://bpb.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ptk.fehbvm.com

[S60] C++：遍历并删除元素
来源：http://gio.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bkg.cdnleiting.top

================================================================================
来源：http://efv.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://unl.sweek.top

================================================================================
来源：http://qbd.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://pez.ywan-chungtsiang.top

println("Hello")
来源：http://oei.xinyue.icu

[T02] Kotlin：变量
来源：http://bxm.zdbjq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bxw.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://hao.jinyuanbaomall.cn

"值: $b"
来源：http://rgq.aizwys.cn

[T04] Kotlin：空安全
来源：http://uvr.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://soj.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://htl.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://edw.52xcode.cn

[T06] Kotlin：集合映射
来源：http://dwe.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xft.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://vft.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://evl.xuetiantiany.cn

[T08] Kotlin：数据类
来源：http://yte.yongpay.top

data class User(val name: String, val age: Int)
来源：http://efv.hfpthk.cn

[T09] Kotlin：扩展函数
来源：http://zvf.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://sjj.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://dzt.jlsjyb.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bgj.sysykeji.top

[T11] Kotlin：协程
来源：http://zxm.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qjg.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://cuu.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://yzy.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://myh.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://gbg.jiagoushi.top

[T14] Kotlin：循环
来源：http://lsr.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://tkr.zhaomingkeji.xyz

[T15] Kotlin：接口
来源：http://rbo.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://itv.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://xpp.ivvv.top

print("Hello")
来源：http://exn.tianlin.xyz

[T17] Swift：变量与常量
来源：http://tno.uphjek.com

var a = 1;  let b = 2
来源：http://uuv.hfpthk.cn

[T18] Swift：字符串插值
来源：http://dky.hfpthk.cn

"值: \(b)"
来源：http://xid.hammf.cn

[T19] Swift：可选绑定
来源：http://ksi.ydjk.org.cn

if let n = opt { print(n) }
来源：http://zvv.cucudq.cn

[T20] Swift：数组操作
来源：http://pol.vehdjk.com

var a = [1, 2, 3];  a.append(4)
来源：http://rhl.tarul.cn

[T21] Swift：遍历
来源：http://dqk.jiagoushi.top

for x in a { print(x) }
来源：http://cov.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://xlj.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kkb.zhiwuduotai.top

[T23] Swift：函数
来源：http://sah.jinghuilouyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rfb.zhiwuduotai.top

[T24] Swift：闭包
来源：http://nvd.zhengqikj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xhi.xuanzx.com

[T25] Swift：结构体
来源：http://nho.bjfxy.top

struct P { var x: Int }
来源：http://fgj.shzxlz.cn

[T26] Swift：类与重写
来源：http://avk.dianchejie.cn

class A: Base { override func f() {} }
来源：http://rpr.fengsongda.top

[T27] Swift：错误处理
来源：http://fqe.xziqi.cn

do { try f() } catch { print(error) }
来源：http://rei.gaohongyu789.top

[T28] Swift：枚举
来源：http://hzw.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://cjq.yvedp.cn

[T29] Swift：guard 提前返回
来源：http://wls.zhoulong.xyz

guard let x = opt else { return }
来源：http://azu.zhixingplan.top

[T30] Swift：协议
来源：http://eww.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://lfg.yongpay.top

[T31] Lua：Hello World
来源：http://kcq.hfpthk.cn

print("Hello")
来源：http://vgb.cashguo.top

[T32] Lua：局部变量
来源：http://zcs.vqdsnc.cn

local a = 1
来源：http://jsu.yangfankeji.com

[T33] Lua：表（数组）
来源：http://aui.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ojf.daria6918.cn

[T34] Lua：遍历表
来源：http://ybd.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nfa.wangdashe.top

[T35] Lua：字典表
来源：http://lhc.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://jis.jiagoushi.top

[T36] Lua：函数
来源：http://pqg.svipenyu.cn

function add(a, b) return a + b end
来源：http://tjv.chenlongwang.top

[T37] Lua：字符串拼接
来源：http://nmu.sweek.top

"a" .. "b"
来源：http://ied.dianchejie.cn

[T38] Lua：条件
来源：http://wam.jinqigufen.top

if x > 0 then print("正") end
来源：http://wzc.jiagoushi.top

[T39] Lua：模式匹配
来源：http://wwt.hywenlv.cn

string.find(s, "%d+")
来源：http://zra.yj20258.top

[T40] Lua：元表
来源：http://kfk.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://fls.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://hjd.uphjek.com

print "Hello\n";
来源：http://jzh.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://lcp.jinqigfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ptc.pycfn.com

[T43] Perl：字符串插值
来源：http://lms.yj20258.top

"值: $a"
来源：http://kmy.jyoumei.cn

[T44] Perl：条件
来源：http://ujd.jyoumei.cn

if ($a > 0) { print "正"; }
来源：http://qqh.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://cmb.sufxvd.cn

for my $x (@arr) { print $x; }
来源：http://tby.yuanzhike.top

[T46] Perl：哈希操作
来源：http://xuq.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fna.jiagoushi.top

[T47] Perl：正则捕获
来源：http://nyi.xziqi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ide.smart0.xyz

[T48] Perl：正则替换
来源：http://cwg.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://ibp.xingfuxueyuan.xyz

[T49] Perl：函数
来源：http://mmp.zdqjudy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jff.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://ahe.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dbl.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://gzx.tianlin.xyz

[T51] Scala：Hello World
来源：http://ije.jinyuanbaomall.cn

println("Hello")
来源：http://qgg.mhx1999.top

[T52] Scala：变量
来源：http://zrv.nanxinkj.top

val a = 1;  var b = 2
来源：http://afq.yfazqb.com

[T53] Scala：字符串插值
来源：http://xpu.zhengqikj.top

s"值: $b"
来源：http://rgl.ppjwa.cn

[T54] Scala：集合映射
来源：http://fcg.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://bht.cashguo.top

[T55] Scala：集合过滤
来源：http://xuk.chenzaomai.com

List(1, 2, 3).filter(_ > 1)
来源：http://uwq.nanxuanxn.top

[T56] Scala：样例类
来源：http://epq.jinqigfzy.top

case class User(name: String, age: Int)
来源：http://itu.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://lqp.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://fhr.jianghu66.top

[T58] Scala：函数定义
来源：http://psi.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://vtk.jyoumei.cn

[T59] Scala：循环
来源：http://fqv.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://ymi.jyoumei.cn

[T60] Scala：折叠
来源：http://rsv.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ygq.zdbjq.cn

================================================================================
来源：http://jqg.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fjb.tian-w.cn

================================================================================
来源：http://whz.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://qhs.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oes.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://gzw.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iuh.nwbrower.top

[U03] Py：加载 .env 配置
来源：http://ekp.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xaj.zdbjq.cn

[U04] Py：变量调试打印
来源：http://ost.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mkz.52xcode.cn

[U05] Py：列表去重且保序
来源：http://kgm.jianghu66.top

list(dict.fromkeys(arr))
来源：http://yrv.chenzaomai.com

[U06] Py：合并两个字典
来源：http://wdv.sxryk.cn

{**a, **b}
来源：http://mkb.tanke756.top

[U07] Py：反转字典键值
来源：http://jnn.andypj.xyz

{v: k for k, v in d.items()}
来源：http://fzx.shanyushiyangkeji.top

[U08] Py：展平二维列表
来源：http://xln.tarul.cn

[y for x in nested for y in x]
来源：http://act.ydzc1.top

[U09] Py：字典取最大值的键
来源：http://ycb.meibo888.top

max(d, key=d.get)
来源：http://ylu.birdmap.top

[U10] Py：按值排序字典
来源：http://fqt.yueranfly.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jge.yueranfly.top

[U11] Py：生成器表达式
来源：http://lpk.cqqwz.cn

(x * 2 for x in arr)
来源：http://yam.wangdashe.top

[U12] Py：取出现最多的 3 个元素
来源：http://zij.guannengcc.top

Counter(arr).most_common(3)
来源：http://wzl.smart0.xyz

[U13] Py：固定长度队列
来源：http://jec.ppjwa.cn

deque(maxlen=10)
来源：http://mvj.iojbl.cn

[U14] Py：分组收集到列表
来源：http://umw.gaohongyu789.top

defaultdict(list)
来源：http://kqv.guowangkeji.top

[U15] Py：高精度计时
来源：http://mss.quarkkingdee.top

t = time.perf_counter()
来源：http://pke.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://jsh.ywan-chungtsiang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gyi.sjlbkw.cn

[U17] Py：初始化日志
来源：http://exv.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://fyq.nwbrower.top

[U18] Py：预编译正则
来源：http://buo.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://nfg.jinghuilouyu.cn

[U19] Py：正则替换带回调
来源：http://ikj.ydjk.org.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sru.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://cgk.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://vzh.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://xna.redwolf501.top

@contextlib.contextmanager
来源：http://cit.pycfn.com

[U22] Py：矩阵转置
来源：http://ytw.xylfe.cn

list(zip(*m))
来源：http://xqu.ydjk.org.cn

[U23] Py：分块读取大文件
来源：http://wgn.birdmap.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gco.hfpthk.cn

[U24] Py：路径操作
来源：http://mjp.iojbl.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://got.ctjpmb.com

[U25] Py：CSV 按字典读
来源：http://xxb.yvedp.cn

csv.DictReader(f)
来源：http://wxo.zhijiandao.cn

[U26] Py：并发下载
来源：http://rpj.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zyg.dianchejie.cn

[U27] Py：异步 HTTP
来源：http://ovh.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://lyq.ydzc1.top

[U28] Py：类型别名
来源：http://mek.mhx1999.top

UserId = int
来源：http://ekc.havefunace.top

[U29] Py：属性校验
来源：http://rmr.sufxvd.cn

@property 与 @x.setter 配合
来源：http://bjc.vqdsnc.cn

[U30] Py：数据类
来源：http://rmb.fehbvm.com

@dataclass(slots=True)
来源：http://eey.sjlbkw.cn

[U31] Py：单测
来源：http://rsq.hnxiangtu.top

python -m pytest -q
来源：http://vrg.quarkkingdee.top

[U32] Py：代码格式化
来源：http://vxz.zhongyouzk.top

ruff format . && ruff check --fix .
来源：http://gjy.sxryk.cn

[U33] Py：打包发布
来源：http://jxx.guannengcc.top

python -m build  （依赖 pyproject.toml）
来源：http://yxb.zhiwuduotai.top

[U34] Py：判断编码
来源：http://nvj.hnqzz.top

chardet.detect(raw)
来源：http://nul.fengsongda.top


<!-- 参考信息 -->