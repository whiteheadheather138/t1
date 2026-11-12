代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://fsy.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tcq.sufxvd.cn

fclose(f);
来源：http://jld.vqdsnc.cn

[S12] C：写文件
来源：http://akd.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vot.redwolf501.top

[S13] C：宏定义
来源：http://mjs.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cgr.guowangkeji.top

[S14] C：枚举
来源：http://ezn.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://dam.hcnkem.com

[S15] C：类型转换
来源：http://fjr.meibo888.top

(double) a / b
来源：http://wjw.jlsjyb.cn

[S16] C：位操作置位
来源：http://uqu.epnwcf.com

x |= (1 << 3);
来源：http://nbq.jianghu66.top

[S17] C：安全拼接字符串
来源：http://gdw.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wql.ivvv.top

[S18] C：命令行参数
来源：http://izv.gaohongyu789.top

int main(int argc, char **argv)
来源：http://pxp.shzxlz.cn

[S19] C：快速排序
来源：http://szb.kuanghao11.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tfo.shuidangran.top

[S20] C：二分查找
来源：http://fkz.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qmo.xylfe.cn

[S21] C：字符类别判断
来源：http://uhx.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://flf.quarkkingdee.top

[S22] C：字符串转数字
来源：http://qcz.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qhi.jianghu66.top

[S23] C：随机数
来源：http://xfm.fehbvm.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ddd.xziqi.cn

[S24] C：获取本地时间
来源：http://gvu.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dzk.ehwqpu.com

[S25] C：内存拷贝
来源：http://vse.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://abr.guannengcc.top

[S26] C：内存清零
来源：http://vfc.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://yyy.gzhubu.top

[S27] C：定义常量
来源：http://fiw.fehbvm.com

const double PI = 3.14159;
来源：http://pzz.tarul.cn

[S28] C：静态变量
来源：http://gja.jinyuanbaomall.cn

static int counter = 0;
来源：http://dss.hfpthk.cn

[S29] C：变参函数
来源：http://rrh.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jap.xinyue.icu

[S30] C：头文件保护
来源：http://knj.shzxlz.cn

#ifndef X_H
来源：http://prl.shuidangran.top

#define X_H
来源：http://mec.gogol.net.cn

#endif
来源：http://pbk.zhoulong.xyz

[S31] C++：Hello World
来源：http://sdr.jianghu66.top

#include <iostream>
来源：http://rmr.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://vqc.smart0.xyz

[S32] C++：字符串
来源：http://luq.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://erc.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://hht.tianlin.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jry.zdbjq.cn

[S34] C++：遍历 vector
来源：http://ytj.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://vim.xinyue.icu

[S35] C++：map
来源：http://tpw.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rel.vehdjk.com

[S36] C++：unordered_map
来源：http://sbl.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pew.fengsongda.top

[S37] C++：set
来源：http://xzz.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gum.sjlbkw.cn

[S38] C++：排序
来源：http://gyv.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://ymh.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://sxa.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jyv.ydjk.org.cn

[S40] C++：查找元素
来源：http://eni.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://drk.ydzc1.top

[S41] C++：类与构造函数
来源：http://rdp.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bzp.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://aqd.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://qxo.52xcode.cn

[S43] C++：智能指针
来源：http://gqk.xingfuxueyuan.xyz

auto p = std::make_unique<int>(5);
来源：http://cai.yvedp.cn

[S44] C++：引用传参
来源：http://unq.aizwys.cn

void inc(int &x) { ++x; }
来源：http://lyt.zhijiandao.cn

[S45] C++：lambda
来源：http://vbu.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qtu.mhx1999.top

[S46] C++：函数模板
来源：http://wyd.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qgc.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://rdv.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wbm.andypj.xyz

[S48] C++：逐行读文件
来源：http://lbn.zhijiandao.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ckr.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://cls.yuxming.cn

[S49] C++：写文件
来源：http://hbi.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://acn.zycfv.cn

[S50] C++：格式化数字
来源：http://byp.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ohx.jyoumei.cn

[S51] C++：显式类型转换
来源：http://abb.iojbl.cn

static_cast<double>(a) / b
来源：http://esi.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://ipt.cucudq.cn

int size() const noexcept { return n_; }
来源：http://dwx.zhixingplan.top

[S53] C++：移动语义
来源：http://nhu.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://ddn.feifeiyinyue.top

[S54] C++：异常处理
来源：http://khq.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dyx.shuidangran.top

[S55] C++：结构化绑定
来源：http://czf.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://rom.tian-w.cn

[S56] C++：optional
来源：http://gns.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jic.cdnleiting.top

[S57] C++：编译期常量
来源：http://krg.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://vgq.hcnkem.com

[S58] C++：命名空间
来源：http://gzk.birdmap.top

namespace ns { int f() { return 1; } }
来源：http://tqv.daxiang520.top

[S59] C++：静态断言
来源：http://ita.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sit.zhaomingkeji.xyz

[S60] C++：遍历并删除元素
来源：http://lgj.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xrt.mhx1999.top

================================================================================
来源：http://ehz.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rxx.daxiang520.top

================================================================================
来源：http://oru.jianghu66.top

[T01] Kotlin：Hello World
来源：http://anu.yuxming.cn

println("Hello")
来源：http://fxv.nwbrower.top

[T02] Kotlin：变量
来源：http://znk.hywenlv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://chf.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://zxo.gotoacloud.top

"值: $b"
来源：http://eoh.epnwcf.com

[T04] Kotlin：空安全
来源：http://krr.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://gig.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://ebf.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://atn.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://xkw.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://hpo.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://iux.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dnm.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://qjj.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://zdy.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://svx.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://gys.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://vhw.dashuyun.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wdm.jinqigufen.top

[T11] Kotlin：协程
来源：http://bty.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zri.52xcode.cn

[T12] Kotlin：解构声明
来源：http://uid.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://zrd.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://xsd.shanyushiyangtech.top

val m = mapOf("a" to 1)
来源：http://cmm.ctjpmb.com

[T14] Kotlin：循环
来源：http://brn.jiagoushi.top

for (i in 1..10) println(i)
来源：http://ijt.yj202588.top

[T15] Kotlin：接口
来源：http://jyp.sweek.top

interface Shape { fun area(): Double }
来源：http://ipx.jinghuilouyu.cn

[T16] Swift：Hello World
来源：http://hbg.yonumen.top

print("Hello")
来源：http://ksh.yuxming.cn

[T17] Swift：变量与常量
来源：http://czx.dianchejie.cn

var a = 1;  let b = 2
来源：http://kqw.smart0.xyz

[T18] Swift：字符串插值
来源：http://pxg.sweek.top

"值: \(b)"
来源：http://klb.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://ujc.yuanzhike.top

if let n = opt { print(n) }
来源：http://cio.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://sjb.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://maj.jinghuilouyu.cn

[T21] Swift：遍历
来源：http://ggz.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://ysn.xylfe.cn

[T22] Swift：字典
来源：http://lyu.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://urb.gaohongyu789.top

[T23] Swift：函数
来源：http://ekp.tianlin.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://odx.shzxlz.cn

[T24] Swift：闭包
来源：http://cla.ydzc1.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zaj.quarkkingdee.top

[T25] Swift：结构体
来源：http://wub.svipenyu.cn

struct P { var x: Int }
来源：http://bfg.52xcode.cn

[T26] Swift：类与重写
来源：http://qam.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://vtc.quarkkingdee.top

[T27] Swift：错误处理
来源：http://msc.sxryk.cn

do { try f() } catch { print(error) }
来源：http://gwt.52xcode.cn

[T28] Swift：枚举
来源：http://xdy.birdmap.top

enum Color { case red, green }
来源：http://fev.vehdjk.com

[T29] Swift：guard 提前返回
来源：http://zsy.9152youxi.cn

guard let x = opt else { return }
来源：http://eeo.bjfxy.top

[T30] Swift：协议
来源：http://pkn.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://mfz.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://imn.pycfn.com

print("Hello")
来源：http://pts.hesvh.cn

[T32] Lua：局部变量
来源：http://ehq.zhengqikj.top

local a = 1
来源：http://ejk.sxryk.cn

[T33] Lua：表（数组）
来源：http://ytv.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ytv.hfpthk.cn

[T34] Lua：遍历表
来源：http://zgu.sufxvd.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://glh.52xcode.cn

[T35] Lua：字典表
来源：http://foc.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://itw.jqgfzy.top

[T36] Lua：函数
来源：http://wuo.yangfankeji.com

function add(a, b) return a + b end
来源：http://mwb.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://dzm.xuetiantiany.cn

"a" .. "b"
来源：http://jqe.dashuyun.cn

[T38] Lua：条件
来源：http://ecw.cqqwz.cn

if x > 0 then print("正") end
来源：http://pzg.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://vur.tarul.cn

string.find(s, "%d+")
来源：http://lik.316326.xyz

[T40] Lua：元表
来源：http://qhf.tanke756.top

setmetatable({}, { __index = base })
来源：http://cvr.52xcode.cn

[T41] Perl：Hello World
来源：http://wav.zhiwuduotai.top

print "Hello\n";
来源：http://zdy.mhx1999.top

[T42] Perl：变量类型
来源：http://pwa.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bxh.tanke756.top

[T43] Perl：字符串插值
来源：http://lbr.ctjpmb.com

"值: $a"
来源：http://dxl.jiagoushi.top

[T44] Perl：条件
来源：http://xsa.xuetiantiany.cn

if ($a > 0) { print "正"; }
来源：http://vwj.zdqjudy.top

[T45] Perl：数组遍历
来源：http://xtg.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://ogi.52xcode.cn

[T46] Perl：哈希操作
来源：http://owx.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jft.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://jxd.zdqjudy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bkq.shuidangran.top

[T48] Perl：正则替换
来源：http://iab.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://raj.cdnleiting.top

[T49] Perl：函数
来源：http://tfe.tianlin.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zco.fengsongda.top

[T50] Perl：逐行读文件
来源：http://pcg.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yea.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://vrm.cucudq.cn

[T51] Scala：Hello World
来源：http://tkp.redwolf501.top

println("Hello")
来源：http://rfr.chenzaomai.com

[T52] Scala：变量
来源：http://tgg.quarkkingdee.top

val a = 1;  var b = 2
来源：http://dxx.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://ihd.xinyue.icu

s"值: $b"
来源：http://prx.daria6918.cn

[T54] Scala：集合映射
来源：http://yep.316326.xyz

List(1, 2, 3).map(_ * 2)
来源：http://fmo.ybcxt.top

[T55] Scala：集合过滤
来源：http://hop.ivvv.top

List(1, 2, 3).filter(_ > 1)
来源：http://bnc.dianchejie.cn

[T56] Scala：样例类
来源：http://qpj.shanyushiyangkeji.top

case class User(name: String, age: Int)
来源：http://pyu.redwolf501.top

[T57] Scala：模式匹配
来源：http://xqw.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dtx.chenjidiqi.icu

[T58] Scala：函数定义
来源：http://rpz.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://nhd.yfazqb.com

[T59] Scala：循环
来源：http://own.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://umf.zycfv.cn

[T60] Scala：折叠
来源：http://muj.svipenyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zxj.ydjk.org.cn

================================================================================
来源：http://boc.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yac.ehwqpu.com

================================================================================
来源：http://fkp.c1oappe.top

[U01] Py：创建虚拟环境
来源：http://kft.bbcook.cn

python -m venv .venv && source .venv/bin/activate
来源：http://phc.cashguo.top

[U02] Py：导出 / 安装依赖
来源：http://nnx.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nfd.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://qnz.yuanzhike.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kix.daxiang520.top

[U04] Py：变量调试打印
来源：http://npk.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zdu.yonumen.top

[U05] Py：列表去重且保序
来源：http://dko.zycfv.cn

list(dict.fromkeys(arr))
来源：http://ovi.iojbl.cn

[U06] Py：合并两个字典
来源：http://zop.yj20258888.top

{**a, **b}
来源：http://eir.c1oappe.top

[U07] Py：反转字典键值
来源：http://nxg.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://jad.tian-w.cn

[U08] Py：展平二维列表
来源：http://yfi.kuanghao11.cn

[y for x in nested for y in x]
来源：http://rau.ivvv.top

[U09] Py：字典取最大值的键
来源：http://bmn.wangdashe.top

max(d, key=d.get)
来源：http://tmv.sufxvd.cn

[U10] Py：按值排序字典
来源：http://bjv.yfazqb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mro.xuanzx.com

[U11] Py：生成器表达式
来源：http://vmg.havefunace.top

(x * 2 for x in arr)
来源：http://hha.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://wwa.vehdjk.com

Counter(arr).most_common(3)
来源：http://chi.cdnleiting.top

[U13] Py：固定长度队列
来源：http://nsq.andypj.xyz

deque(maxlen=10)
来源：http://uoe.fehbvm.com

[U14] Py：分组收集到列表
来源：http://oob.52xcode.cn

defaultdict(list)
来源：http://ndz.xziqi.cn

[U15] Py：高精度计时
来源：http://pfn.hcnkem.com

t = time.perf_counter()
来源：http://qaq.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://qag.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://swj.zhaomingkeji.xyz

[U17] Py：初始化日志
来源：http://nyz.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://zde.cucudq.cn

[U18] Py：预编译正则
来源：http://fog.birdmap.top

pat = re.compile(r"\d+")
来源：http://nyg.yfazqb.com

[U19] Py：正则替换带回调
来源：http://wnm.yueranfly.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hkk.hammf.cn

[U20] Py：缓存函数结果
来源：http://isj.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://huk.fengsongda.top

[U21] Py：自定义上下文管理器
来源：http://yms.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://qnj.fehbvm.com

[U22] Py：矩阵转置
来源：http://xtl.gogol.net.cn

list(zip(*m))
来源：http://lei.ehwqpu.com

[U23] Py：分块读取大文件
来源：http://cra.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pqd.kuanghao11.cn

[U24] Py：路径操作
来源：http://oah.xinyue.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yiy.sjlbkw.cn

[U25] Py：CSV 按字典读
来源：http://wwo.jinqigufen.top

csv.DictReader(f)
来源：http://iot.yvedp.cn

[U26] Py：并发下载
来源：http://xfi.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nvk.hnqzz.top

[U27] Py：异步 HTTP
来源：http://gbu.snrcjt.cn

aiohttp.ClientSession() 配合 async with
来源：http://cjw.shanyushiyangtech.top

[U28] Py：类型别名
来源：http://afr.tanke756.top

UserId = int
来源：http://fgw.hysaishi.cn

[U29] Py：属性校验
来源：http://rdi.tarul.cn

@property 与 @x.setter 配合
来源：http://gtl.zhongyouzk.top

[U30] Py：数据类
来源：http://djd.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://xju.hywenlv.cn

[U31] Py：单测
来源：http://wod.jiagoushi.top

python -m pytest -q
来源：http://uel.yangfankeji.com

[U32] Py：代码格式化
来源：http://guu.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://vvj.bbcook.cn

[U33] Py：打包发布
来源：http://jee.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://ruo.wangshuangyany.cn

[U34] Py：判断编码
来源：http://icm.ivvv.top

chardet.detect(raw)
来源：http://ktx.kuanghao11.cn


<!-- 参考信息 -->