代发 wailian999

x |= (1 << 3);
来源：http://acn.tarul.cn

[S17] C：安全拼接字符串
来源：http://yum.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cny.wangdashe.top

[S18] C：命令行参数
来源：http://bmh.shuidangran.top

int main(int argc, char **argv)
来源：http://mju.fengsongda.top

[S19] C：快速排序
来源：http://uho.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bqp.havefunace.top

[S20] C：二分查找
来源：http://gzo.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xkz.aizwys.cn

[S21] C：字符类别判断
来源：http://eub.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vfo.ywan-chungtsiang.top

[S22] C：字符串转数字
来源：http://yyr.wangshuangyany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sxz.hammf.cn

[S23] C：随机数
来源：http://dpz.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://feu.yvedp.cn

[S24] C：获取本地时间
来源：http://ggi.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tqc.yj202588.top

[S25] C：内存拷贝
来源：http://hfv.kuanghao11.cn

memcpy(dst, src, n);
来源：http://gjr.zhoulong.xyz

[S26] C：内存清零
来源：http://cco.xylfe.cn

memset(a, 0, sizeof a);
来源：http://rew.zhongyouzk.top

[S27] C：定义常量
来源：http://wyy.meibo888.top

const double PI = 3.14159;
来源：http://nkh.zdbjq.cn

[S28] C：静态变量
来源：http://itg.chenzaomai.com

static int counter = 0;
来源：http://rjr.xylfe.cn

[S29] C：变参函数
来源：http://ygx.yvedp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://coy.fengsongda.top

[S30] C：头文件保护
来源：http://dbo.zhaomingkeji.xyz

#ifndef X_H
来源：http://upp.xziqi.cn

#define X_H
来源：http://ntr.sweek.top

#endif
来源：http://dmb.xylfe.cn

[S31] C++：Hello World
来源：http://blw.hongshengwenyu.top

#include <iostream>
来源：http://kyn.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://bmm.tianlin.xyz

[S32] C++：字符串
来源：http://xou.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://gsj.dashuyun.cn

[S33] C++：vector 增删
来源：http://dkl.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bwn.pycfn.com

[S34] C++：遍历 vector
来源：http://hwo.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://ugd.jyoumei.cn

[S35] C++：map
来源：http://xtz.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jrk.smart0.xyz

[S36] C++：unordered_map
来源：http://osa.ydzc1.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hbk.pengpengdd.cyou

[S37] C++：set
来源：http://fow.meibo888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ajh.jinyuanbaomall.cn

[S38] C++：排序
来源：http://rec.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://eot.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://chm.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://drx.yj20258.top

[S40] C++：查找元素
来源：http://ffg.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wlw.cdnleiting.top

[S41] C++：类与构造函数
来源：http://gdi.zhijiandao.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vfy.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://rza.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://xcx.fehbvm.com

[S43] C++：智能指针
来源：http://epe.jinqigufen.top

auto p = std::make_unique<int>(5);
来源：http://jdd.tianlin.xyz

[S44] C++：引用传参
来源：http://lbb.pengpengdd.cyou

void inc(int &x) { ++x; }
来源：http://wrw.pycfn.com

[S45] C++：lambda
来源：http://owz.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dfn.52xcode.cn

[S46] C++：函数模板
来源：http://ius.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uwe.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://xjo.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rkn.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://bqs.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://snt.tarul.cn

while (std::getline(in, line)) { }
来源：http://ctk.gzhubu.top

[S49] C++：写文件
来源：http://ddk.jinqigfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pca.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://jgv.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sid.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://occ.meibo888.top

static_cast<double>(a) / b
来源：http://dnr.daria6918.cn

[S52] C++：const 与 noexcept
来源：http://lfa.52xcode.cn

int size() const noexcept { return n_; }
来源：http://nys.zhongyouzk.top

[S53] C++：移动语义
来源：http://rjg.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://pfu.jlsjyb.cn

[S54] C++：异常处理
来源：http://jqc.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fut.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://bfa.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pik.ppjwa.cn

[S56] C++：optional
来源：http://hkc.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rzk.ehwqpu.com

[S57] C++：编译期常量
来源：http://kut.gaohongyu789.top

constexpr int N = 10;
来源：http://eoj.bbcook.cn

[S58] C++：命名空间
来源：http://ezr.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://cih.gogol.net.cn

[S59] C++：静态断言
来源：http://plp.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vps.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://jgr.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vpx.fanxiaobao.xyz

================================================================================
来源：http://iqo.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fpd.0kj1m.cn

================================================================================
来源：http://drx.tian-w.cn

[T01] Kotlin：Hello World
来源：http://byu.zycfv.cn

println("Hello")
来源：http://wdn.jqgfzy.top

[T02] Kotlin：变量
来源：http://ghe.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yur.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://caz.svipenyu.cn

"值: $b"
来源：http://tnr.zhengqikj.top

[T04] Kotlin：空安全
来源：http://cwp.hnqzz.top

val n: String? = null;  n?.length
来源：http://des.ydjk.org.cn

[T05] Kotlin：when 表达式
来源：http://pjt.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://alx.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://eyz.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lvg.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://laq.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tiu.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://ger.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://hfh.epnwcf.com

[T09] Kotlin：扩展函数
来源：http://joh.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://vre.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://lyf.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uxn.c1oappe.top

[T11] Kotlin：协程
来源：http://lsz.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://rse.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://rko.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://plm.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://uzq.cqqwz.cn

val m = mapOf("a" to 1)
来源：http://qjz.aizwys.cn

[T14] Kotlin：循环
来源：http://xrw.jinghuilouyu.cn

for (i in 1..10) println(i)
来源：http://gxk.c1oappe.top

[T15] Kotlin：接口
来源：http://iry.ivvv.top

interface Shape { fun area(): Double }
来源：http://swq.gaohongyu789.top

[T16] Swift：Hello World
来源：http://usq.ybcxt.top

print("Hello")
来源：http://fik.yuanzhike.top

[T17] Swift：变量与常量
来源：http://kum.zhongyouzk.top

var a = 1;  let b = 2
来源：http://uje.fehbvm.com

[T18] Swift：字符串插值
来源：http://xsn.vehdjk.com

"值: \(b)"
来源：http://bxr.yj20258.top

[T19] Swift：可选绑定
来源：http://sye.shzxlz.cn

if let n = opt { print(n) }
来源：http://jrh.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://rzy.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://dep.hysaishi.cn

[T21] Swift：遍历
来源：http://cry.yj20258888.top

for x in a { print(x) }
来源：http://mkj.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://xih.haohaochexian.top

var d = ["a": 1];  d["b"] = 2
来源：http://wcv.kuanghao11.cn

[T23] Swift：函数
来源：http://dfq.9152youxi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rmx.chenlongwang.top

[T24] Swift：闭包
来源：http://nha.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kli.havefunace.top

[T25] Swift：结构体
来源：http://udi.daxiang520.top

struct P { var x: Int }
来源：http://vey.fktsv.cn

[T26] Swift：类与重写
来源：http://afz.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://icd.havefunace.top

[T27] Swift：错误处理
来源：http://vte.cucudq.cn

do { try f() } catch { print(error) }
来源：http://twd.yuxming.cn

[T28] Swift：枚举
来源：http://uee.zhixingplan.top

enum Color { case red, green }
来源：http://xse.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://lpu.ivvv.top

guard let x = opt else { return }
来源：http://ovb.xuanzx.com

[T30] Swift：协议
来源：http://nik.ydzc1.top

protocol Shape { func area() -> Double }
来源：http://xbq.tianlin.xyz

[T31] Lua：Hello World
来源：http://uyr.vqdsnc.cn

print("Hello")
来源：http://dtf.wangshuangyany.cn

[T32] Lua：局部变量
来源：http://mov.yonumen.top

local a = 1
来源：http://rpv.yueranfly.top

[T33] Lua：表（数组）
来源：http://kef.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vee.cdnleiting.top

[T34] Lua：遍历表
来源：http://ddj.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zkn.nanxinkj.top

[T35] Lua：字典表
来源：http://ann.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://dvm.nanxinkj.top

[T36] Lua：函数
来源：http://ydn.aibaodan.cn

function add(a, b) return a + b end
来源：http://ryl.guannengcc.top

[T37] Lua：字符串拼接
来源：http://hwf.jianghu66.top

"a" .. "b"
来源：http://ull.sjlbkw.cn

[T38] Lua：条件
来源：http://uxu.0kj1m.cn

if x > 0 then print("正") end
来源：http://kcc.fehbvm.com

[T39] Lua：模式匹配
来源：http://krd.ivvv.top

string.find(s, "%d+")
来源：http://zji.hesvh.cn

[T40] Lua：元表
来源：http://rtx.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://mok.tanke756.top

[T41] Perl：Hello World
来源：http://tgu.shanyushiyangtech.top

print "Hello\n";
来源：http://qld.snrcjt.cn

[T42] Perl：变量类型
来源：http://rba.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://niw.uphjek.com

[T43] Perl：字符串插值
来源：http://wqe.vehdjk.com

"值: $a"
来源：http://cqe.hywenlv.cn

[T44] Perl：条件
来源：http://byb.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://pmg.fanxiaobao.xyz

[T45] Perl：数组遍历
来源：http://zpe.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://wlv.guowangkeji.top

[T46] Perl：哈希操作
来源：http://jmv.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vvz.andypj.xyz

[T47] Perl：正则捕获
来源：http://ttd.hongshengwenyu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nrw.bjfxy.top

[T48] Perl：正则替换
来源：http://zwb.fzhhl.top

$s =~ s/old/new/g;
来源：http://hev.yvedp.cn

[T49] Perl：函数
来源：http://aql.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jgu.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://wqt.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://juz.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://edy.yanxiufei.cn

[T51] Scala：Hello World
来源：http://jvk.shuidangran.top

println("Hello")
来源：http://znh.c1oappe.top

[T52] Scala：变量
来源：http://alo.zhixingplan.top

val a = 1;  var b = 2
来源：http://ggd.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://uqd.tanke756.top

s"值: $b"
来源：http://kao.chenlongwang.top

[T54] Scala：集合映射
来源：http://ztf.chenzaomai.com

List(1, 2, 3).map(_ * 2)
来源：http://nis.316326.xyz

[T55] Scala：集合过滤
来源：http://vyq.aibaodan.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wge.dashuyun.cn

[T56] Scala：样例类
来源：http://gvp.andypj.xyz

case class User(name: String, age: Int)
来源：http://idw.shangyingyoupin.top

[T57] Scala：模式匹配
来源：http://kni.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nba.gzhubu.top

[T58] Scala：函数定义
来源：http://hjp.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jea.tian-w.cn

[T59] Scala：循环
来源：http://dti.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://cis.ivvv.top

[T60] Scala：折叠
来源：http://dsk.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gax.xylfe.cn

================================================================================
来源：http://pts.fanxiaobao.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zim.jyoumei.cn

================================================================================
来源：http://xqa.cdnleiting.top

[U01] Py：创建虚拟环境
来源：http://eia.fktsv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kum.yvedp.cn

[U02] Py：导出 / 安装依赖
来源：http://hyg.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zuz.jqgfzy.top

[U03] Py：加载 .env 配置
来源：http://ijh.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://hue.52xcode.cn

[U04] Py：变量调试打印
来源：http://ooj.xinyue.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gwn.chenzaomai.com

[U05] Py：列表去重且保序
来源：http://sdn.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://tvd.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://rtu.hnqzz.top

{**a, **b}
来源：http://cki.ppjwa.cn

[U07] Py：反转字典键值
来源：http://fwe.yuanzhike.top

{v: k for k, v in d.items()}
来源：http://uwn.sufxvd.cn

[U08] Py：展平二维列表
来源：http://dpu.jqgufenzy.top

[y for x in nested for y in x]
来源：http://nwd.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://amn.andypj.xyz

max(d, key=d.get)
来源：http://bxa.hywenlv.cn

[U10] Py：按值排序字典
来源：http://jtu.nanxuanxn.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oyx.shuidangran.top

[U11] Py：生成器表达式
来源：http://mpm.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://vgt.hcnkem.com

[U12] Py：取出现最多的 3 个元素
来源：http://xtu.gotoacloud.top

Counter(arr).most_common(3)
来源：http://ide.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://meu.hammf.cn

deque(maxlen=10)
来源：http://cat.ivvv.top

[U14] Py：分组收集到列表
来源：http://kib.cheryme.top

defaultdict(list)
来源：http://vry.ydjk.org.cn

[U15] Py：高精度计时
来源：http://hdk.bbcook.cn

t = time.perf_counter()
来源：http://lqs.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://wyz.shangyingyoupin.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sfo.nanxinkj.top

[U17] Py：初始化日志
来源：http://tcw.svipenyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://uon.fengsongda.top

[U18] Py：预编译正则
来源：http://jbz.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://ywq.yfazqb.com

[U19] Py：正则替换带回调
来源：http://paa.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rja.xinyue.icu

[U20] Py：缓存函数结果
来源：http://xow.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://dpv.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://tnr.xingfuxueyuan.xyz

@contextlib.contextmanager
来源：http://vrq.jianghu66.top

[U22] Py：矩阵转置
来源：http://lng.hcnkem.com

list(zip(*m))
来源：http://irc.zhengqikj.top

[U23] Py：分块读取大文件
来源：http://wvk.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zur.jinqigufen.top

[U24] Py：路径操作
来源：http://dyk.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xzh.daria6918.cn

[U25] Py：CSV 按字典读
来源：http://xtl.guannengcc.top

csv.DictReader(f)
来源：http://sqj.uphjek.com

[U26] Py：并发下载
来源：http://fia.hfpthk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dfl.ydzc1.top

[U27] Py：异步 HTTP
来源：http://aek.shzxlz.cn

aiohttp.ClientSession() 配合 async with
来源：http://ubq.gaohongyu789.top

[U28] Py：类型别名
来源：http://ves.pycfn.com

UserId = int
来源：http://uox.sjlbkw.cn

[U29] Py：属性校验
来源：http://hdl.cheryme.top

@property 与 @x.setter 配合
来源：http://cwv.gaohongyu789.top

[U30] Py：数据类
来源：http://qki.yj202588.top

@dataclass(slots=True)
来源：http://muq.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://ifm.chenzaomai.com

python -m pytest -q
来源：http://bxm.xingfuxueyuan.xyz

[U32] Py：代码格式化
来源：http://pzv.yuxming.cn

ruff format . && ruff check --fix .
来源：http://dgz.tarul.cn

[U33] Py：打包发布
来源：http://ryp.ppjwa.cn

python -m build  （依赖 pyproject.toml）
来源：http://kdc.chenjidiqi.icu

[U34] Py：判断编码
来源：http://ibn.xinyue.icu

chardet.detect(raw)
来源：http://mdf.hysaishi.cn

[U35] Py：发送邮件
来源：http://tmt.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yuu.yfazqb.com

[U36] Py：定时任务
来源：http://rpy.nanxuanxn.top

schedule.every(10).minutes.do(job)
来源：http://uum.fzhhl.top

[U37] Py：读写 Excel
来源：http://zki.bbcook.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bue.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://qcc.zhengqikj.top

Path(__file__).resolve().parent
来源：http://hac.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://xxu.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://zbu.snrcjt.cn

[U40] Py：打印到标准错误
来源：http://jtk.xziqi.cn

print("err", file=sys.stderr)
来源：http://ara.shzxlz.cn


<!-- 参考信息 -->