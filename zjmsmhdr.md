代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ktv.yuxming.cn

[S13] C：宏定义
来源：http://wba.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ael.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://fyd.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://qgi.sxryk.cn

[S15] C：类型转换
来源：http://vvi.sweek.top

(double) a / b
来源：http://ven.andypj.xyz

[S16] C：位操作置位
来源：http://vmt.cdnleiting.top

x |= (1 << 3);
来源：http://jel.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://dst.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zth.jinqigufen.top

[S18] C：命令行参数
来源：http://per.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://zkb.hammf.cn

[S19] C：快速排序
来源：http://msp.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://pfi.hnqzz.top

[S20] C：二分查找
来源：http://mwj.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fst.gaohongyu789.top

[S21] C：字符类别判断
来源：http://qtr.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zgn.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://lnl.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://htc.hysaishi.cn

[S23] C：随机数
来源：http://apn.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kta.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://mse.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wsx.jqgfzy.top

[S25] C：内存拷贝
来源：http://xfd.hywenlv.cn

memcpy(dst, src, n);
来源：http://die.316326.xyz

[S26] C：内存清零
来源：http://tvm.xinyue.icu

memset(a, 0, sizeof a);
来源：http://lsa.0kj1m.cn

[S27] C：定义常量
来源：http://yip.zhiwuduotai.top

const double PI = 3.14159;
来源：http://bka.ppjwa.cn

[S28] C：静态变量
来源：http://cbq.shzxlz.cn

static int counter = 0;
来源：http://cue.hfpthk.cn

[S29] C：变参函数
来源：http://njk.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jby.hesvh.cn

[S30] C：头文件保护
来源：http://aqc.jinghuilouyu.cn

#ifndef X_H
来源：http://zbx.chenzaomai.com

#define X_H
来源：http://ujd.nanxuanxn.top

#endif
来源：http://xmv.cucudq.cn

[S31] C++：Hello World
来源：http://liv.andypj.xyz

#include <iostream>
来源：http://kny.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://dzx.tian-w.cn

[S32] C++：字符串
来源：http://uup.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://vah.xinyue.icu

[S33] C++：vector 增删
来源：http://jtp.yongpay.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://obs.nwbrower.top

[S34] C++：遍历 vector
来源：http://xjl.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://olh.kuanghao11.cn

[S35] C++：map
来源：http://hxs.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ihc.chenlongwang.top

[S36] C++：unordered_map
来源：http://vqj.havefunace.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ptl.guannengcc.top

[S37] C++：set
来源：http://yel.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://byv.52xcode.cn

[S38] C++：排序
来源：http://iia.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://eat.cheryme.top

[S39] C++：自定义比较器排序
来源：http://xgu.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yqj.andypj.xyz

[S40] C++：查找元素
来源：http://mzl.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dbc.hnqzz.top

[S41] C++：类与构造函数
来源：http://ecb.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://juk.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://pyy.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://tah.jiagoushi.top

[S43] C++：智能指针
来源：http://xir.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://dox.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://ajp.epnwcf.com

void inc(int &x) { ++x; }
来源：http://psj.hongshengwenyu.top

[S45] C++：lambda
来源：http://zaz.redwolf501.top

auto add = [](int a, int b) { return a + b; };
来源：http://jzf.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://ahi.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gtr.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://ywh.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jxu.snrcjt.cn

[S48] C++：逐行读文件
来源：http://bus.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://iki.yj20258888.top

while (std::getline(in, line)) { }
来源：http://xxm.chenjidiqi.icu

[S49] C++：写文件
来源：http://ftj.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sgu.hnqzz.top

[S50] C++：格式化数字
来源：http://vom.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qze.yangfankeji.com

[S51] C++：显式类型转换
来源：http://cbp.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://mwn.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://jxw.shuidangran.top

int size() const noexcept { return n_; }
来源：http://brd.cdnleiting.top

[S53] C++：移动语义
来源：http://juz.cashguo.top

std::vector<int> w = std::move(v);
来源：http://lmr.jlsjyb.cn

[S54] C++：异常处理
来源：http://qrm.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uoz.wangdashe.top

[S55] C++：结构化绑定
来源：http://llv.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pvx.vqdsnc.cn

[S56] C++：optional
来源：http://eou.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hqb.yuanzhike.top

[S57] C++：编译期常量
来源：http://tuk.daxiang520.top

constexpr int N = 10;
来源：http://dib.yonumen.top

[S58] C++：命名空间
来源：http://cao.uphjek.com

namespace ns { int f() { return 1; } }
来源：http://ifu.hfpthk.cn

[S59] C++：静态断言
来源：http://uwa.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qut.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://rxq.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hqn.andypj.xyz

================================================================================
来源：http://aal.chenjidiqi.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ctp.wangdashe.top

================================================================================
来源：http://ohq.andypj.xyz

[T01] Kotlin：Hello World
来源：http://dta.xziqi.cn

println("Hello")
来源：http://lyf.birdmap.top

[T02] Kotlin：变量
来源：http://xre.yj20258888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vpi.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://akq.316326.xyz

"值: $b"
来源：http://qlt.yj202588.top

[T04] Kotlin：空安全
来源：http://tjj.hfpthk.cn

val n: String? = null;  n?.length
来源：http://rkv.fanxiaobao.xyz

[T05] Kotlin：when 表达式
来源：http://dcx.hywenlv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tay.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://lzk.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://jnb.tanke756.top

[T07] Kotlin：集合过滤
来源：http://jme.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aza.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://htr.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://buy.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://dws.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://mdr.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://fip.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wmj.yongpay.top

[T11] Kotlin：协程
来源：http://wfk.kuanghao11.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sdr.kuanghao11.cn

[T12] Kotlin：解构声明
来源：http://naj.cashguo.top

val (a, b) = Pair(1, 2)
来源：http://zvh.pycfn.com

[T13] Kotlin：只读 Map
来源：http://xsb.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://reh.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://nsv.nanxinkj.top

for (i in 1..10) println(i)
来源：http://pdz.yvedp.cn

[T15] Kotlin：接口
来源：http://ayc.ywan-chungtsiang.top

interface Shape { fun area(): Double }
来源：http://gby.gogol.net.cn

[T16] Swift：Hello World
来源：http://tmm.yj20258.top

print("Hello")
来源：http://ntc.hammf.cn

[T17] Swift：变量与常量
来源：http://jeg.chenlongwang.top

var a = 1;  let b = 2
来源：http://fax.shanyushiyangkeji.top

[T18] Swift：字符串插值
来源：http://yid.316326.xyz

"值: \(b)"
来源：http://avz.0kj1m.cn

[T19] Swift：可选绑定
来源：http://xsl.ppjwa.cn

if let n = opt { print(n) }
来源：http://dkm.birdmap.top

[T20] Swift：数组操作
来源：http://fzt.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ajr.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://bsp.ivvv.top

for x in a { print(x) }
来源：http://lvv.iojbl.cn

[T22] Swift：字典
来源：http://mjl.chenzaomai.com

var d = ["a": 1];  d["b"] = 2
来源：http://gtt.hnxiangtu.top

[T23] Swift：函数
来源：http://maa.shangyingyoupin.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eii.pycfn.com

[T24] Swift：闭包
来源：http://hxk.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cxy.316326.xyz

[T25] Swift：结构体
来源：http://xat.dianchejie.cn

struct P { var x: Int }
来源：http://aqi.shzxlz.cn

[T26] Swift：类与重写
来源：http://ywm.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://rmg.yuanzhike.top

[T27] Swift：错误处理
来源：http://kgt.9152youxi.cn

do { try f() } catch { print(error) }
来源：http://ewq.jqgfzy.top

[T28] Swift：枚举
来源：http://qzg.tarul.cn

enum Color { case red, green }
来源：http://tep.nanxinkj.top

[T29] Swift：guard 提前返回
来源：http://azc.redwolf501.top

guard let x = opt else { return }
来源：http://los.yanxiufei.cn

[T30] Swift：协议
来源：http://wjw.chenzaomai.com

protocol Shape { func area() -> Double }
来源：http://bym.zhongyouzk.top

[T31] Lua：Hello World
来源：http://zxr.9152youxi.cn

print("Hello")
来源：http://zcu.yongpay.top

[T32] Lua：局部变量
来源：http://mbp.guannengcc.top

local a = 1
来源：http://cwr.sysykeji.top

[T33] Lua：表（数组）
来源：http://wcg.sxryk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vwf.cucudq.cn

[T34] Lua：遍历表
来源：http://qpj.andypj.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://jss.tian-w.cn

[T35] Lua：字典表
来源：http://fyd.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://szc.yuanzhike.top

[T36] Lua：函数
来源：http://aig.pycfn.com

function add(a, b) return a + b end
来源：http://arv.mhx1999.top

[T37] Lua：字符串拼接
来源：http://jgy.havefunace.top

"a" .. "b"
来源：http://ijw.jinqigufen.top

[T38] Lua：条件
来源：http://vff.yongpay.top

if x > 0 then print("正") end
来源：http://ywg.vqdsnc.cn

[T39] Lua：模式匹配
来源：http://rbw.daxiang520.top

string.find(s, "%d+")
来源：http://plg.dashuyun.cn

[T40] Lua：元表
来源：http://rjq.epnwcf.com

setmetatable({}, { __index = base })
来源：http://yge.kuanghao11.cn

[T41] Perl：Hello World
来源：http://jrc.zhaomingkeji.xyz

print "Hello\n";
来源：http://wuc.zdqjudy.top

[T42] Perl：变量类型
来源：http://qku.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tyd.xylfe.cn

[T43] Perl：字符串插值
来源：http://yqn.nanxinkj.top

"值: $a"
来源：http://kgl.tian-w.cn

[T44] Perl：条件
来源：http://bxl.ehwqpu.com

if ($a > 0) { print "正"; }
来源：http://kwe.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://tpz.meibo888.top

for my $x (@arr) { print $x; }
来源：http://bse.jyoumei.cn

[T46] Perl：哈希操作
来源：http://ayb.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ujg.ydzc1.top

[T47] Perl：正则捕获
来源：http://jyq.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://jsj.fehbvm.com

[T48] Perl：正则替换
来源：http://opr.0kj1m.cn

$s =~ s/old/new/g;
来源：http://hti.xuanzx.com

[T49] Perl：函数
来源：http://nxv.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vko.guannengcc.top

[T50] Perl：逐行读文件
来源：http://qcy.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kbk.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://kof.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://wub.cdnleiting.top

println("Hello")
来源：http://aoi.yj20258888.top

[T52] Scala：变量
来源：http://tlg.0kj1m.cn

val a = 1;  var b = 2
来源：http://wbt.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://wge.zhongyouzk.top

s"值: $b"
来源：http://jho.bjfxy.top

[T54] Scala：集合映射
来源：http://tzy.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://oqm.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://nmg.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://roq.epnwcf.com

[T56] Scala：样例类
来源：http://vrb.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://ppa.jyoumei.cn

[T57] Scala：模式匹配
来源：http://trg.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uar.sysykeji.top

[T58] Scala：函数定义
来源：http://pib.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dsc.smart0.xyz

[T59] Scala：循环
来源：http://xbq.smart0.xyz

for (i <- 1 to 10) println(i)
来源：http://kye.xuanzx.com

[T60] Scala：折叠
来源：http://usa.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sat.zhongyouzk.top

================================================================================
来源：http://rbt.shuidangran.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://unn.zhixingplan.top

================================================================================
来源：http://gsy.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://rgh.nanxinkj.top

python -m venv .venv && source .venv/bin/activate
来源：http://swp.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://lwh.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://irl.fanxiaobao.xyz

[U03] Py：加载 .env 配置
来源：http://msh.ybcxt.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dxz.yj202588.top

[U04] Py：变量调试打印
来源：http://zdh.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xcj.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://cxt.xingfuxueyuan.xyz

list(dict.fromkeys(arr))
来源：http://hoz.fehbvm.com

[U06] Py：合并两个字典
来源：http://mqf.chenjidiqi.icu

{**a, **b}
来源：http://nuv.zdqjudy.top

[U07] Py：反转字典键值
来源：http://wev.xinyue.icu

{v: k for k, v in d.items()}
来源：http://qvf.sxryk.cn

[U08] Py：展平二维列表
来源：http://yuh.cucudq.cn

[y for x in nested for y in x]
来源：http://tgu.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://die.yuanzhike.top

max(d, key=d.get)
来源：http://lcs.yfazqb.com

[U10] Py：按值排序字典
来源：http://czq.uphjek.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kvf.hcnkem.com

[U11] Py：生成器表达式
来源：http://hmm.hcnkem.com

(x * 2 for x in arr)
来源：http://ppc.tarul.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qeo.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://yth.nanxuanxn.top

[U13] Py：固定长度队列
来源：http://fsf.epnwcf.com

deque(maxlen=10)
来源：http://rbe.jqgufenzy.top

[U14] Py：分组收集到列表
来源：http://jpe.kuanghao11.cn

defaultdict(list)
来源：http://roe.zdqjudy.top

[U15] Py：高精度计时
来源：http://ktz.zhoulong.xyz

t = time.perf_counter()
来源：http://fus.cucudq.cn

[U16] Py：命令行参数解析
来源：http://lbv.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rqm.pycfn.com

[U17] Py：初始化日志
来源：http://qmh.nanxuanxn.top

logging.basicConfig(level=logging.INFO)
来源：http://pnw.yj20258888.top

[U18] Py：预编译正则
来源：http://kqg.xuetiantiany.cn

pat = re.compile(r"\d+")
来源：http://rqd.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://rxx.yj202588.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://juy.gzhubu.top

[U20] Py：缓存函数结果
来源：http://eub.nanxuanxn.top

@functools.lru_cache(maxsize=None)
来源：http://mvx.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://xse.nanxinkj.top

@contextlib.contextmanager
来源：http://lcl.bjfxy.top

[U22] Py：矩阵转置
来源：http://joa.epnwcf.com

list(zip(*m))
来源：http://lgx.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://vld.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ybw.shuidangran.top

[U24] Py：路径操作
来源：http://kxz.ehwqpu.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gpd.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://han.zhixingplan.top

csv.DictReader(f)
来源：http://qaf.bbcook.cn

[U26] Py：并发下载
来源：http://kdt.zhaomingkeji.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fyw.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://wob.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://enb.dashuyun.cn

[U28] Py：类型别名
来源：http://lvu.shangyingyoupin.top

UserId = int
来源：http://euf.tanke756.top

[U29] Py：属性校验
来源：http://xce.jinqigufen.top

@property 与 @x.setter 配合
来源：http://wtl.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://cee.quarkkingdee.top

@dataclass(slots=True)
来源：http://vje.nanxinkj.top

[U31] Py：单测
来源：http://med.hcnkem.com

python -m pytest -q
来源：http://xpc.birdmap.top

[U32] Py：代码格式化
来源：http://ljv.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://nog.gogol.net.cn

[U33] Py：打包发布
来源：http://pps.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://zyl.haohaochexian.top

[U34] Py：判断编码
来源：http://zfl.xziqi.cn

chardet.detect(raw)
来源：http://vlg.jqgfzy.top

[U35] Py：发送邮件
来源：http://vpx.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qfx.daxiang520.top

[U36] Py：定时任务
来源：http://ngi.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://qkr.daxiang520.top


<!-- 参考信息 -->